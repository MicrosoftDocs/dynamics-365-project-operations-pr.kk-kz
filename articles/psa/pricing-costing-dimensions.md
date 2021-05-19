---
title: Бағалар және шығын өлшемдерінің басты бет
description: Бұл тақырыпта бағалау өлшемдері туралы жалпы мәліметтер беріледі.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 137fee27dd2302d47ae12faccde1682cff43db93
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284140"
---
# <a name="pricing-and-costing-dimensions-home-page"></a>Бағалар және шығын өлшемдерінің басты бет

[!include [banner](../includes/psa-now-project-operations.md)]

Жобаға негізделген ұйымдарда еңбекақы бағасын және өзіндік құнын белгілеу үшін қолданылатын өлшемдерге келесі төлсипаттар әсер етеді:

- Адамдар өздерінің тәжірибесіне, рөліне немесе географиясына ұқсас жұмыс істейді
- Оның күрделілігіне немесе тәулік уақытына ұқсас орындалатын жұмыс

Жұмыстың осы төлсипаттарының және жұмысты орындауға қажетті адамдардың типтік сипатына сәйкес, Project Service Automation бағдарламасында баға өлшемі мәндерінің екі түрі бар: 

- **Параметрлер жиындары** - мәндер жиынтығы үшін бекітілген тізімдер болып табылатын төлсипаттар.
- **Нысанға негізделген мәндер** - шектеулі, бірақ уақыт өте өзгеруі мүмкін әртүрлі мәндер жиынына ие болатын төлсипаттар.

## <a name="pricing-dimensions"></a>Бағалар өлшемдері

PSA бағдарламасы әдепкі бағалар өлшемдерінің жиынтығымен жеткізіледі. Мұны **Project Service** > **Параметрлер** тармағына өту арқылы көре аласыз. Параметр жазбасындағы **Сомаға негізделген бағалар өлшемдері** қойыншасында рөлді тексеріңіз, **msdyn_resourcecategory** және ресурстық бөлімше, **msdyn_organizationalunit** параметрінің **Иә** мәніне орнатылған бар **Сатуға қолданылады** және **Құны үшін қолданылады** өрістері бар. Бұл әр рөл мен бірлік тіркесімінің бағасы мен құнын белгілеуге мүмкіндік береді.

!["Сатылымға қолданбалы" параметрі бөлектелген Project Service параметрлерінің скриншоты](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> Егер сіз PSA 3 нұсқасына дейін бағалар өлшемдері ретінде рөл мен ұйымдық бөлімшенің дайын өрістерін қолданған болсаңыз, елеулі өзгерістер болмайды. Project Service қызметін әдеттегідей пайдалануды жалғастыра аласыз. 

Егер қосымша атрибуттарды қолдана отырып, ресурстарыңыздың бағасын немесе құнын анықтау қажет болса, реттелген өрістерді, нысандарды және өлшемдерді жасай аласыз. Қосымша ақпарат алу үшін, келесі тақырыптарды қараңыз, бірақ процедураларды төменде көрсетілген ретпен орындау керектігін ескеріңіз:

- [Реттелетін өрістер мен нысандарды жасау](create-custom-fields-entities.md)
- [Баға орнатуы және транзакциялық нысандарға реттелетін өрістер қосу](field-references.md)
- [Реттелетін өрістерді баға өлшемдері ретінде орнату ](set-up-pricing-dimensions.md)
- [Жаңа бағалар өлшемдерін қосу үшін қосылатын модуль атрибуттарын жаңарту](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a>Кадрлық ресурс уақытының құнын белгілеу
Ұйымның кадрлық ресурс уақытының құнын белгілеу жолы көбінесе ұйымның табыстылығына тікелей әсер ететін маңызды стратегиялық фактор болып табылады. Ұйымыңыз кадрлық ресурс уақытына арналған пайыздық мөлшерлеме мен құн мөлшерлемесін реттеу жолын анықтауға дайын болған кезде, қаржылық топтармен және тәжірибе жетекшілерімен жұмыс жасаңыз.

Баға белгілеуге қатысты ұсыныстар қазіргі уақытта бағалар өлшемдері болып табылмайтын, бірақ ұйымыңыз үшін бағалар өлшемі ретінде қолданылатын өрістерді немесе нысандарды қайта пайдалану қажеттігін қамтиды. **Транзакция санаты** (**msdyn_transactioncategory**) және **Резервтеу үшін қолжетімді ресурс** (**bookableresource**) өрістері кандидат өлшемдерінің мысалдары болып табылады. 

Бағалау өлшемі кесте немесе параметр жинағы болуы керек екенін қарастырыңыз. Егер сіз 10 немесе 12-ден асатын өлшем мәндерінің өзгерістерін болжасаңыз және осы мәндерге қосымша төлсипаттар қажет болса, параметрлер жиынын емес, нысанды жасаңыз. Мәндерді қосу немесе жою сияқты параметрлер жиынын сақтау үшін әкімші немесе әзірлеуші қажет, ал кестеге жаңа жолдар қосу әрекетін көптеген іскери пайдаланушылар орындай алады.

Төмендегі мысалда ресурстар тиесілі рөл мен ресурстық бөлімше негізінде құрылған пайыздық мөлшерлемелер көрсетілген. Құн мөлшерлемелері, әдетте, қызметкердің жалақы деңгейіне және құрамына кіретін бөлімшеге негізделеді. Бұл мысалда вексель мен құн мөлшерлемесі кестелері келесідей болады.

**Үлгілі вексель мөлшерлемелері**

| Рөл        | Ұйымдық бөлімше    |Бірлік      |Баға      |Валюта  |
| ------------|-------------|----------|----------:|----------|
| Әзірлеуші   | Contoso АҚШ  |Hour | 200|USD     |
| Әзірлеуші   | Contoso India |Hour|   112|USD     |


**Үлгілі құн мөлшерлемелері**

| Жалақы деңгейі     | Ұйымдық бөлімше    |Бірлік      |Баға      |Валюта  |
| ----------------|-------------|----------|----------:|----------|
| My company_Band1 | Contoso АҚШ  |Hour | 145|USD     |
| My company_Band2 | Contoso India |Hour|   67|USD     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]