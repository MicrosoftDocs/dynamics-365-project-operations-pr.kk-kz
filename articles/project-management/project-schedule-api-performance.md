---
title: Жоба кестесінің API өнімділігі
description: Бұл тақырыпта Жоба кестесі API интерфейстерінің өнімділік көрсеткіштері туралы ақпарат берілген және оңтайлы пайдалану үшін ең жақсы тәжірибелер анықталған.
author: ruhercul
ms.date: 11/03/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a1abadbae044ccbd40077c6937262f0f17387bad
ms.sourcegitcommit: 5c536cf05e2cbfc1d15982e4695d726064a074da
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/04/2021
ms.locfileid: "7750609"
---
# <a name="project-schedule-api-performance"></a>Жоба кестесінің API өнімділігі

_**Келесіге қолданылады:** ресурсқа/биржадан тыс негізделген сценарийлерге арналған Project Operations, жеңілдетілген орналастыру - проформа есеп‑шотын ұсыну мәмілесі, Project for the Web_

Бұл тақырыпта Жоба кестесі бағдарламасын бағдарламалау интерфейстерінің (APIs) өнімділік көрсеткіштері туралы ақпарат берілген және оңтайландырылған пайдалану үшін ең жақсы тәжірибелер анықталған.

## <a name="project-scheduling-service"></a>Жобаны жоспарлау қызметі
Жобаны жоспарлау қызметі — Microsoft Azure бағдарламасында іске қосылатын бірнеше қатысушыдан тұратын қызмет. Ол пайдаланушылар жобаларда жұмыс істегенде жылдам және бірқалыпты тәжірибені қамтамасыз ету арқылы өзара әрекеттесуді жақсартуға арналған. Бұл жақсартуға өзгерту сұрауларын қабылдау, оларды өңдеу және нәтижені бірден қайтару арқылы қол жеткізіледі. Қызмет асинхронды түрде Dataverse қызметіне сақталады және пайдаланушылардың басқа әрекеттерді орындауына тыйым салмайды.

Жоба кестесі API интерфейстері осы тақырыптың кейінгі бөлімдерінде толығырақ сипатталған сұрауларды орындау үшін Жобаны жоспарлау қызметіне сүйенеді.

Жоба кестесінің API интерфейстері келесі жұмыс декомпозициясының құрылымы (WBS) нысандарымен жұмыс істеуге арналған:

  - Project
  - Жоба тапсырмасы
  - Жоба тапсырмасы тәуелділігі
  - Жоба тобы мүшесі
  - Ресурс тағайындауы
  
Кірістірілген өрістерге де, реттелетін өрістерге де қолдау көрсетіледі. Басқаша айтылмаса, жасау, жаңарту және жою секілді барлық жалпы әрекеттерге қолдау көрсетіледі. Қосымша ақпаратты [Әрекеттерді және жоспарлау нысандарын орындау үшін жоба кестесі API интерфейстерін пайдалану](schedule-api-preview.md) бөлімін қараңыз.

Жоба кестесі API интерфейстерінің бөлігі ретінде жұмыс бірлігі үлгісі қосылды. Бұл үлгі OperationSet ретінде белгілі және оны бір транзакцияда бірнеше сұрауды өңдеу қажет болғанда пайдалануға болады.

Келесі сурет осы мүмкіндікті пайдаланған кезде серіктеске кездесетін ағынды көрсетеді.

![Dataverse және жобаны жоспарлау қызметінің ағыны.](./media/dataverse-project-scheduling-service-flow.png)

**1-қадам**: клиент OperationSet жинағын жасау үшін Dataverse қызметінде ашық деректер протоколының (OData) соңғы нүктесіне API қоңырауын жасайды.

**2-қадам**: жаңа OperationSet жасалғаннан кейін, **OperationSetId** мәні қайтарылады.

**3-қадам**: клиент басқа жоба кестесі API сұрауын жасау үшін **OperationSetId** мәнін пайдаланады. Нәтиже жоспарлау нысанында сұрауды жасау, жаңарту немесе жою болып табылады. Бұл сұрау жасалғанда, метадеректерді тексеру орындалады. Тексеру сәтсіз болса, сұрау тоқтатылады және қате қайтарылады.

**4a–4c қадамдары**: бұл қадамдар ҚАБЫЛДАУ кезеңін білдіреді. Клиент барлық өзгерістерді бір топтамада жобаны жоспарлау қызметіне жіберетін **ExecuteOperationSetV1** API интерфейсін шақырады. Жобаны жоспарлау қызметі топтамадағы сұраулар бойынша өз тексерулерін жүргізеді. Кез келген тексеру қателері топтаманы болдырмайды және шақырушыға ерекше жағдайды қайтарады. Топтама жобаны жоспарлау қызметі арқылы сәтті қабылданса, OperationSet күйі OperationSet жобаны жоспарлау қызметі арқылы өңделетінін көрсету үшін жаңартылады.

**5-қадам**: бұл қадам PERSIST кезеңін білдіреді. Жобаны жоспарлау қызметі топтаманы транзакцияда Dataverse қызметіне асинхронды түрде жазады. Жазу әрекеті сәтті болса, OperationSet **Аяқталды** ретінде белгіленеді. Кез келген қателер транзакция мен топтаманы кері қайтарады және OperationSet **Сәтсіз** ретінде белгіленеді.

## <a name="performance-methodology"></a>Өнімділік әдістемесі
Орындау уақыты жобаны жоспарлау уақыты Dataverse қызметіне жазуды аяқтағанға дейін қоңыраудан **ExecuteOperationSetV1** API интерфейсіне дейінгі уақыт ретінде анықталады. Барлық операциялар біріктірілген 2200 рет орындалады және P99 орындалу уақытының өлшемдері хабарланады. Бір жазба және көлемді операциялар өлшенеді.

Бір жазба әрекеті үшін OperationSet бір сұрауды қамтиды. Жаппай операцияларда ол 20, 50 немесе 100 сұраудан тұрады. Әрбір жаппай өлшем бөлек хабарланады.

Бұл операциялар Солтүстік Америкада UR 15 Project Operations Lite орналастыруында орындалады.

## <a name="results"></a>Нәтижелер
### <a name="create-operations"></a>Операциялар жасау
#### <a name="single-record-create-operations"></a>Бір жазбаны жасау операциялары
Төмендегі кестеде бір жазбаны жасау үшін орындалу уақыттары көрсетілген. Уақыттар секундтармен берілген.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">Жазба&nbsp;&nbsp;&nbsp;түрі</th>
    <th class="tg-0lax" colspan="2">Уақыт</th>
  </tr>
  <tr>
    <th class="tg-0lax">Талап етілетін өрісте</th>
    <th class="tg-0lax">Барлық қолдау көрсетілетін өрістер</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Project</td>
    <td class="tg-0lax">2.5</td>
    <td class="tg-0lax">3.78</td>
  </tr>
  <tr>
    <td class="tg-0lax">Тапсырма</td>
    <td class="tg-0lax">8.82</td>
    <td class="tg-0lax">9.34</td>
  </tr>
  <tr>
    <td class="tg-0lax">Тағайындау</td>
    <td class="tg-0lax">9.19</td>
    <td class="tg-0lax">9.19</td>
  </tr>
  <tr>
    <td class="tg-0lax">Топ мүшесі</td>
    <td class="tg-0lax">0.84</td>
    <td class="tg-0lax">4.2</td>
  </tr>
  <tr>
    <td class="tg-0lax">Тәуелділік</td>
    <td class="tg-0lax">8.84</td>
    <td class="tg-0lax">8.84</td>
  </tr>
</tbody>
</table>

#### <a name="bulk-create-operations"></a>Жаппай жасау операциялары
Төмендегі кестеде бірнеше жазбаны жасау үшін орындалу уақыттары көрсетілген. Атап айтқанда, Microsoft бір OperationSet ішінде 20, 50 және 100 жазбаны жасау үшін орындалу уақыттарын өлшеген. Уақыттар секундтармен берілген.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="3">Жазба&nbsp;&nbsp;&nbsp;түрі</th>
    <th class="tg-0lax" colspan="6">Уақыт</th>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2">20 жазба</th>
    <th class="tg-0lax" colspan="2">50 жазба</th>
    <th class="tg-0lax" colspan="2">100 жазба</th>
  </tr>
  <tr>
    <th class="tg-0lax">Талап етілетін өрісте</th>
    <th class="tg-0lax">Барлық қолдау көрсетілетін өрістер</th>
    <th class="tg-0lax">Талап етілетін өрісте</th>
    <th class="tg-0lax">Барлық қолдау көрсетілетін өрістер</th>
    <th class="tg-0lax">Талап етілетін өрісте</th>
    <th class="tg-0lax">Барлық қолдау көрсетілетін өрістер</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Тапсырма</td>
    <td class="tg-0lax">19.92</td>
    <td class="tg-0lax">38.35</td>
    <td class="tg-0lax">36.67</td>
    <td class="tg-0lax">99.13</td>
    <td class="tg-0lax">116.77</td>
    <td class="tg-0lax">174.06</td>
  </tr>
  <tr>
    <td class="tg-0lax">Тағайындау</td>
    <td class="tg-0lax">13.94</td>
    <td class="tg-0lax">13.94</td>
    <td class="tg-0lax">43.95</td>
    <td class="tg-0lax">43.95</td>
    <td class="tg-0lax">69.38</td>
    <td class="tg-0lax">69.38</td>
  </tr>
  <tr>
    <td class="tg-0lax">Тәуелділік</td>
    <td class="tg-0lax">30.04</td>
    <td class="tg-0lax">30.04</td>
    <td class="tg-0lax">77.82</td>
    <td class="tg-0lax">77.82</td>
    <td class="tg-0lax">176.89</td>
    <td class="tg-0lax">176.89</td>
  </tr>
</tbody>
</table>

> [!NOTE] 
> **Жоба** және **Топ мүшесі** нысандары бойынша жаппай операциялар жасау бұл кестеге қосылмаған, себебі сол әрекеттердің орындалу уақыты жалғыз жазба жасауға арналған API бірнеше рет шақырылған кездегі орындалу уақытына ұқсас болады. Бұл API интерфейстері дереу Dataverse қызметінде іске қосылады.

Келесі суретте 20, 50 және 100 жазба жасалғанда және барлық қолдау көрсетілетін өрістер пайдаланылғанда **Тапсырма**, **Тағайындау** және **Тәуелділік** нысандарына арналған орындалу уақыттарының сызбасы көрсетіледі.

![Жазбаның орындалу уақытының графигін жасаңыз.](./media/create-record-execution-time.png)

### <a name="update-operations"></a>Операцияларды жаңарту
#### <a name="single-record-update-operations"></a>Бір жазбаны жаңарту операциялары
Төмендегі кестеде бір жазбаны жаңарту үшін орындалу уақыттары көрсетілген. Уақыттар секундтармен берілген.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">Жазба&nbsp;&nbsp;&nbsp;түрі</th>
    <th class="tg-0lax" colspan="2">Уақыт</th>
  </tr>
  <tr>
    <th class="tg-0lax">Талап етілетін өрісте </th>
    <th class="tg-0lax">Барлық қолдау көрсетілетін өрістер</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Project</td>
    <td class="tg-0lax">9.53</td>
    <td class="tg-0lax">13.91</td>
  </tr>
  <tr>
    <td class="tg-0lax">Тапсырма</td>
    <td class="tg-0lax">8.82</td>
    <td class="tg-0lax">9.91</td>
  </tr>
  <tr>
    <td class="tg-0lax">Топ мүшесі</td>
    <td class="tg-0lax">9</td>
    <td class="tg-0lax">8.96</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> **Ресурстарды тағайындау** және **Жоба тапсырмасына тәуелділігі** нысандарында операцияларды жаңартуға қолдау көрсетілмейді.

#### <a name="bulk-update-operations"></a>Жаппай жаңарту операциялары
Төмендегі кестеде бірнеше жазбаны жаңарту үшін орындалу уақыттары көрсетілген. Атап айтқанда, Microsoft бір OperationSet ішінде 20, 50 және 100 жазбаны жаңарту үшін орындалу уақыттарын өлшеген. Уақыттар секундтармен берілген.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="3">Жазба&nbsp;&nbsp;&nbsp;түрі</th>
    <th class="tg-0lax" colspan="6">Уақыт</th>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2">20 жазба</th>
    <th class="tg-0lax" colspan="2">50 жазба</th>
    <th class="tg-0lax" colspan="2">100 жазба</th>
  </tr>
  <tr>
    <th class="tg-0lax">Талап етілетін өрісте</th>
    <th class="tg-0lax">Барлық қолдау көрсетілетін өрістер</th>
    <th class="tg-0lax">Талап етілетін өрісте</th>
    <th class="tg-0lax">Барлық қолдау көрсетілетін өрістер</th>
    <th class="tg-0lax">Талап етілетін өрісте</th>
    <th class="tg-0lax">Барлық қолдау көрсетілетін өрістер</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Тапсырма</td>
    <td class="tg-0lax">8.91</td>
    <td class="tg-0lax">38.71</td>
    <td class="tg-0lax">20.92</td>
    <td class="tg-0lax">87.13</td>
    <td class="tg-0lax">36.68</td>
    <td class="tg-0lax">190.34</td>
  </tr>
  <tr>
    <td class="tg-0lax">Топ мүшесі</td>
    <td class="tg-0lax">20.52</td>
    <td class="tg-0lax">26.06</td>
    <td class="tg-0lax">41.93</td>
    <td class="tg-0lax">44.51</td>
    <td class="tg-0lax">38.63</td>
    <td class="tg-0lax">66.53</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> **Ресурстарды тағайындау** және **Жоба тапсырмасына тәуелділігі** нысандарында операцияларды жаңартуға қолдау көрсетілмейді.

Келесі суретте 20, 50 және 100 жазба жаңартылғанда және барлық қолдау көрсетілетін өрістер пайдаланылғанда тапсырма және топ мүшесі нысандарына арналған орындалу уақыттарының сызбасы көрсетіледі.

![Жазбаның орындалу уақытының графигін жаңартыңыз.](./media/update-record-execution-time.png)

### <a name="delete-operations"></a>Жою операциялары
#### <a name="single-record-delete-operations"></a>Бір жазбаны жою операциялары
Төмендегі кестеде бір жазбаны жою үшін орындалу уақыттары көрсетілген. Уақыттар секундтармен берілген.

| Жазба түрі | Уақыт  |
|-------------|-------|
| Тапсырма        | 20.12 |
| Тағайындау  | 10.86 |
| Топ мүшесі | 12.52 |
| Тәуелділік  | 20.89 |

> [!NOTE]
> **Жоба** нысаны бойынша жою операцияларына қолдау көрсетілмейді.

#### <a name="bulk-delete-operations"></a>Жаппай жою амалдары
Төмендегі кестеде бірнеше жазбаны жою үшін орындалу уақыттары көрсетілген. Атап айтқанда, Microsoft бір OperationSet ішінде 20, 50 және 100 жазбаны жою үшін орындалу уақыттарын өлшеген. Уақыттар секундтармен берілген.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">Жазба&nbsp;&nbsp;&nbsp;түрі</th>
    <th class="tg-0lax" colspan="3">Уақыт</th>
  </tr>
  <tr>
    <th class="tg-0lax">20 жазба</th>
    <th class="tg-0lax">50 жазба</th>
    <th class="tg-0lax">100 жазба</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Тапсырма</td>
    <td class="tg-0lax">20.91</td>
    <td class="tg-0lax">67.43</td>
    <td class="tg-0lax">71.96</td>
  </tr>
  <tr>
    <td class="tg-0lax">Тағайындау</td>
    <td class="tg-0lax">11.75</td>
    <td class="tg-0lax">25.79</td>
    <td class="tg-0lax">47.66</td>
  </tr>
  <tr>
    <td class="tg-0lax">Топ мүшесі</td>
    <td class="tg-0lax">9.78</td>
    <td class="tg-0lax">39.73</td>
    <td class="tg-0lax">24.33</td>
  </tr>
  <tr>
    <td class="tg-0lax">Тәуелділік</td>
    <td class="tg-0lax">24.61</td>
    <td class="tg-0lax">54.9</td>
    <td class="tg-0lax">109.16</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> **Жоба** нысаны бойынша жою операцияларына қолдау көрсетілмейді.

Келесі суретте 20, 50 және 100 жазба жойылғанда **Тапсырма**, **Тағайындау**, **Топ мүшесі** және **Тәуелділік** нысандарына арналған орындалу уақыттарының сызбасы көрсетіледі.

![Жазбаның орындалу уақытының графигін жойыңыз.](./media/delete-record-execution-time.png)

## <a name="observations"></a>Бақылаулар
Әрбір жазба операциясында **ExecuteOperationSet** API жобаны жоспарлау қызметіне сұрау жіберу үшін шамамен 800 миллисекундты алады. Содан кейін жобаны жоспарлау қызметі жүктемені өңдеуге және Dataverse қызметіне қоңырау шалу үшін шамамен бес секундты алады. Қалған орындалу уақыты бизнес логикасын орындауға және Dataverse қызметінде дерекқорға деректерді жазуға жұмсалады.

100 жазба жасалғанда, жаңартылғанда немесе жойылғанда, **ExecuteOperationSet** API сұрауды Жобаны жоспарлау қызметіне жіберу үшін шамамен үш секундты алады. Содан кейін жобаны жоспарлау қызметі сұрауларды өңдеуге және Dataverse қызметіне қоңырау шалу үшін шамамен бес секундты алады. Жаппай операциялар **Жобаны жоспарлау қызметі салығын** OperationSet ішіндегі барлық жазбалар үшін бір рет төлеуі тиіс. Демек, жаппай операциялардың орташа орындалу уақыты бір жазба операцияларына қарағанда айтарлықтай төмен.

## <a name="scenarios"></a>Сценарийлер
Келесі кесте нақты сценарийлерді орындау үшін Жоба кестесі API интерфейстері пайдаланылған орындалу уақыттарын көрсетеді. Уақыттар секундтармен берілген.

| Сценарий                                                                   | Уақыт  |
|----------------------------------------------------------------------------|-------|
| 40 тапсырмасы бар жоба жасаңыз.                                      | 36.01 |
| 40 тапсырмасы және 20 тәуелділігі бар жоба жасаңыз.                  | 38.11 |
| 40 тапсырмасы және 30 тағайындауы бар жоба жасаңыз.                   | 60.17 |
| 40 тапсырмасы және 20 тәуелділігі және 30 тағайындауы бар жоба жасаңыз. | 60.27 |

## <a name="best-practices"></a>Үздік тәжірибелер
Алдыңғы сценарий нәтижелеріне негізделген API келесі жағдайларда жақсырақ жұмыс істейді:

  - Мүмкіндігінше көп операцияларды біріктіріңіз. Жаппай операциялардың орташа орындалу уақыты бір жазбалы операциялардың орташа орындалу уақытынан жақсы. Қолданылатын OperationSets саны неғұрлым аз болса, орташа орындау уақыты соғұрлым жылдамырақ болады.
  - Сценарийді орындау үшін қажетті минималды төлсипаттарды ғана орнатыңыз. OperationSet сұрауында қамтылған талап етілмейтін өрістердің түрлерін таңдап алыңыз. Басқа кілттерді немесе жиынтық өрістерді қамтитын өрістер өнімділікке теріс әсер етеді.