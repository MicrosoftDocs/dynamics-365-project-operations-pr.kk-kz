---
title: Жобаға негізделген келісім-шарт жолдарымен жұмыс істеу - жеңілдетілген
description: Бұл тақырыпта жобаға негізделген келісім-шарт жолдарымен жұмыс істеу туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7ec8973df1def3f707603019cdd45147423c1ae3
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180649"
---
# <a name="work-with-projectbased-contract-lines---lite"></a>Жобаға негізделген келісім-шарт жолдарымен жұмыс істеу - жеңілдетілген

_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_

Dynamics 365 Project Operations бағдарламасындағы жобаға негізделген келісім-шарт жолдары келісім бойынша жоба жұмысының нақты құрамдастары үшін болжам және төлем келісімдерін сақтауға арналған. Жобаға негізделген келісім-шарт жолының құрылымы жобаның болжам және төлем сценарийлері үшін келесі тұжырымдамалармен кеңейтілген:

- Төлем әдісі
- Жоба мен тапсырманы салыстыру
- Қамтылған транзакция кластары
- Асырмау шегі
- Төлем қабілеттілігін орнату
- Келісім-шарт жолдары туралы мәліметтерді пайдаланатын болжамдар
- Келісім-шарт жолы тұтынушылары

Келесі кестеде жобаға негізделген жұмыстардың толық, негізгі болжам және төлем реттеулері үшін негізді орнатуға көмектесетін жобаға негізделген келісім-шарт жолдарының **Жалпы мәліметтер** қойыншасындағы өрістер қамтылған.

| Өріс | Сипаттамасы | Төменгі әсер |
| --- | --- | --- |
| **Атауы** | Келісім-шарт жолының атауы. Бұл бағаланатын келісім-шарттың дискретті құрамдасын анықтайды. Баға ұсынудан жасалған жоба келісім-шарты үшін бұл мән жобаға негізделген баға ұсыну жолының сәйкес мәнінен көшіріледі. | Атауы есеп-шот жасалған кезде осы келісім-шарт жолынан жасалған жоба есеп-шоты жолына көшіріледі. |
| **Есепшот ұсыну әдісі** | Баға ұсынудан жасалған жоба келісім-шартында бұл мән баға ұсыну жолындағы сәйкес өрістен көшіріледі. Бұл Project Operations қолдайтын екі негізгі келісім-шарттық үлгілерді ұсынатын параметрлер жиыны:</br>- **Бекітілген баға**</br>- **Уақыт және материал** | Сілтеме жасалған келісім-шарт жолының төлем әдісі негізінде нақты транзакция өңделеді. Егер нақты мән арқылы сілтеме жасалған келісім-шарт жолында уақыт пен материалдық есеп-шот ұсыну әдісі болса, құн мен төлем жасалмаған сатылымның нақты жазбалары жасалады. Егер нақты мән арқылы сілтеме жасалған келісім-шарт жолында белгіленген баға бойынша есеп-шот ұсыну әдісі болса, тек нақты өзіндік құн жасалады. |
| **Project** | Бұл өрісті осы келісім бойынша жұмысты орындау үшін пайдаланылатын жобаны анықтау үшін пайдаланыңыз. | Бұл мән келісім-шарттың нақты немесе болжамды жол жазбасына сілтеме жасау үшін **Қамтылған тапсырмалар** және **Қамтылған транзакция кластары** өрістерімен бірге пайдаланылады. |
| **Қосылған тапсырмалар** | Осы келісім-шарт жолына таңдалған жоба бойынша барлық жоба тапсырмалары немесе тапсырмалар жиыны ғана қосылғанын көрсетеді. Бұл келесі мүмкін мәндерге ие параметрлер жиыны болып табылады:</br>- **Барлық жоба тапсырмалары**</br>- **Тек таңдалған жоба тапсырмалары**. Бұл өрістегі бос мән **Барлық жоба тапсырмалары** таңдауына тең. | Егер **Тек таңдалған тапсырмалар** таңдалған болса, сіз нақты тапсырмаларды таңдап, оларды **Жоба** бетіндегі **Тапсырма шотын ұсынуды реттеу** қойыншасындағы келісім-шарт жолымен байланыстыра аласыз. Бұл мән келісім-шарттың нақты немесе болжамды жол жазбасына сілтеме жасау үшін **Жоба** және **Қамтылған транзакция** кластарымен бірге пайдаланылады. |
| **Уақытпен қоса** | Жалауша таңдалған жобадағы уақыт транзакциялары немесе еңбек құны осы келісім-шарт жолына қосылатынын көрсетеді. **Жоқ** мәні уақыт транзакциялары немесе еңбек құны осы келісім-шарт жолына қосылмайтынын көрсетеді. **Иә** мәні олардың қосылатынын көрсетеді. | Бұл мән нақты немесе болжамды жол жазбасындағы келісім-шарт жолына сілтеме жасау үшін жобамен бірге пайдаланылады. |
| **Шығыспен қоса** | Жалауша таңдалған жобадағы шығыс құны осы келісім-шарт жолына қосылатынын көрсетеді. **Жоқ** мәні шығыс құны осы келісім-шарт жолына қосылмайтынын көрсетеді. **Иә** мәні қосылатынын көрсетеді. | Бұл мән нақты немесе болжамды жол жазбасындағы келісім-шарт жолына сілтеме жасау үшін жобамен бірге пайдаланылады. |
| **Ақымен қоса** | Жалауша таңдалған жобадағы ақы осы келісім-шарт жолына қосылатынын көрсетеді. **Жоқ** мәні ақы осы келісім-шарт жолына қосылмайтынын көрсетеді. **Иә** мәні олардың қосылатынын көрсетеді. | Бұл мән нақты немесе болжамды жол жазбасындағы келісім-шарт жолына сілтеме жасау үшін жобамен бірге пайдаланылады. |
| **Келісім-шарт сомасы** | Белгіленген баға келісім-шарты жолы бойынша, бұл сома тұтынушыға осы келісім-шарт жолымен байланысты барлық жұмыс құрамдастары үшін есеп-шот ұсынылатын келісілген мән болып табылады. Уақыт және материал бойынша келісім-шарт жолы бойынша, бұл сома тұтынушыға осы келісім-шарт жолымен байланысты барлық жұмыс құрамдастары үшін есеп-шот ұсынылатын болжалды мән болып табылады. Баға ұсынудан жасалған жоба келісім-шарты бойынша, бұл мән баға ұсыну жолындағы сәйкес өрістен көшірілген. Жобаға негізделген келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл өріс өңдеу үшін құлыпталады және келісім-шарт жолы туралы мәліметтердегі сомадан жинақталады. | Келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл мәнді жол туралы мәліметтердегі сомаларды өзгерту арқылы өзгертуге болады. Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді шот ұсыну кезеңдеріне салық алдында соманы құру үшін пайдаланылады. |
| **Болжалды салық** | Пайдаланушы бұл өрісті келісім-шарт жолына болжалды салық сомасын енгізу үшін өңдей алады. Жобаға негізделген келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл өріс өңдеу үшін құлыпталады және келісім-шарт жолы туралы мәліметтердегі салық сомасынан жинақталады. | Келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл мәнді жол туралы мәліметтердегі салық сомаларын өзгерту арқылы өзгертуге болады. Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді төлем жасау кезеңдеріне салық салу үшін пайдаланылады. |
| **Салықтан кейінгі келісім-шарт сомасы** | Салықтан кейінгі келісім-шарт жолының сомасы. Бұл өріс тек оқуға арналған және **Келісім-шарт сомасы + салық** ретінде есептеледі. | Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді төлем жасау кезеңдерін құру үшін пайдаланылады. |
| **Асырмау шегі** | Пайдаланушы бұл өрісті өңдей алады және ол тек шот ұсыну әдісін уақыт пен материал ретінде орнатқан жобаға негізделген келісім-шарт жолдарында қолжетімді. | Пайдаланушы бұл өрісті өңдей алады. Уақыт пен материалға арналған нақты көрсеткіштер осы келісім-шарт жолына уақыт пен материал үшін сілтеме жасаған кезде, нақты сома осы келісім-шарт жолындағы асырмау шегімен бағаланады. Бұл бағалау жұмсалған және жасалған сомалар есепке алынғаннан кейін аяқталады. |
| **Тұтынушы бюджеті** | Бұл өрісті өңдеуге болады және келісім-шарт баға ұсынудан жасалған болса, баға ұсыну жолындағы сәйкес өрістен көшіріледі. | Бұл өріс тек ақпарат алу үшін пайдаланылады және бұл өрісте ағынның маңыздылығы жоқ. |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a>Жобаға негізделген келісім-шарт жолдарының Жалпы қойыншасындағы опцияларға арналған тексеру ережелері

1-ереже: **Қосылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** опциясына орнатылса, жобаның барлық тапсырмалары келісім-шарт жолына қосылады.

2-ереже: **Қосылған тапсырмалар** өрісі бос болған кезде немесе нақты **Барлық жоба тапсырмалары** опциясына орнатылған кезде, жоба мен белгілі бір транзакция класын тек келісім-шарттың бір жобаға негізделген келісім-шарт жолына қосуға болады.

3-ереже: **Қосылған тапсырмалар** өрісі **Тек таңдалған жоба тапсырмалары** опциясына орнатылған кезде, жоба мен белгілі бір транзакция класын тек келісім-шарттың бірнеше жобаға негізделген келісім-шарт жолдарына қосуға болады.

| Келісім-шарт | Келісім-шарт жолы | Project | Қосылған тапсырмалар      | Уақытпен қоса | Шығыспен қоса | Ақымен қоса | Жарамды/жарамсыз | Себеп                                                                                                                                                                                                                                                                                                                                                                                                                         |
|----------|---------------|---------|---------------------|--------------|-----------------|-------------|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| C1       | CL1           | P1      | Бос               | Иә          | Иә             | Иә         | Жарамсыз       | №2 ережені бұзу. Р1 жобасы бойынша уақыт, шығыс пен ақы CL1 және CL2 келісім-шарттарының екі жолына да қосылған.                                                                                                                                                                                                                                                                                                              |
| C1       | CL2           | P1      | Бос               | Иә          | Иә             | Иә         | Жарамсыз       | №2 ережені бұзу. Р1 жобасы бойынша уақыт, шығыс пен ақы CL1 және CL2 келісім-шарттарының екі жолына да қосылған.                                                                                                                                                                                                                                                                                                              |
| C1       | CL1           | P1      | Бос               | Иә          | №              | Иә         | Жарамсыз       | №2 ережені бұзу. Р1 жобасы бойынша уақыт пен ақы CL1 және CL2 келісім-шарттарының екі жолына да қосылған.                                                                                                                                                                                                                                                                                                                          |
| C1       | CL2           | P1      | Бос               | Иә          | Иә             | Иә         | Жарамсыз       | №2 ережені бұзу. Р1 жобасы бойынша уақыт пен ақы CL1 және CL2 келісім-шарттарының екі жолына да қосылған.                                                                                                                                                                                                                                                                                                                          |
| C1       | CL1           | P1      | Бос               | Иә          | №              | Иә         | Жарамды           | Р1 жобасы бойынша уақыт пен ақы CL1 жолына қосылған. P1 жобасындағы шығыс CL2 жолына қосылған. </br>   Әрбір келісім-шарт жолына қосылатын жерде ешқандай қабаттасу жоқ, сондықтан ол жарамды болып табылады.                                                                                                                                                                                                                         |
| C1       | CL2           | P1      | Бос               | №           | Иә             | №          | Жарамды           | Р1 жобасы бойынша уақыт пен ақы CL1 жолына қосылған. P1 жобасындағы шығыс CL2 жолына қосылған. </br>   Әрбір келісім-шарт жолына қосылатын жерде ешқандай қабаттасу жоқ, сондықтан ол жарамды болып табылады.                                                                                                                                                                                                                         |
| C1       | CL1           | P1      | Тек таңдалған тапсырмалар | Иә          | Иә             | Иә         | Жарамсыз       | №2 ережені бұзу.   </br>- C1 жолына Р1 жобасы бойынша тапсырмалар жиынындағы уақыт, шығыс және ақы қосылған. </br>- CL2 жолына бүкіл P1 жобасы үшін уақыт, шығыс және ақы қосылған, сондықтан C1 жолында қамтылғанмен қабаттасады.                                                                                                                                                                                          |
| C1       | CL2           | P1      | Бос               | Иә          | Иә             | Иә         | Жарамсыз       | №2 ережені бұзу.   </br>- C1 жолына Р1 жобасы бойынша тапсырмалар жиынындағы уақыт, шығыс және ақы қосылған. </br>- CL2 жолына бүкіл P1 жобасы үшін уақыт, шығыс және ақы қосылған, сондықтан C1 жолында қамтылғанмен қабаттасады.                                                                                                                                                                                          |
| C1       | CL1           | P1      | Тек таңдалған тапсырмалар | Иә          | Иә             | Иә         | Жарамды           | №3 ережеге сәйкес</br>-  C1 жолына Р1 жобасы бойынша тапсырмалар жиынындағы уақыт, шығыс және ақы қосылған. </br> - CL2 жолына Р1 жобасы бойынша тапсырмалар жиыны үшін уақыт, шығыс және ақы қосылған. </br> Жалғыз қосымша тексеру — CL1 жолындағы тапсырмалар жиынында, бұл қабаттасулардың болмауын қамтамасыз ететін CL2 жолындағы тапсырмалар жиынынан өзгеше. Бұл тексеру жүйемен тапсырмалар байланысты болған кезде аяқталады. |
| C1       | CL2           | P1      | Тек таңдалған тапсырмалар | Иә          | Иә             | Иә         | Жарамды           | №3 ережеге сәйкес</br>-  C1 жолына Р1 жобасы бойынша тапсырмалар жиынындағы уақыт, шығыс және ақы қосылған. </br> - CL2 жолына Р1 жобасы бойынша тапсырмалар жиыны үшін уақыт, шығыс және ақы қосылған. </br> Жалғыз қосымша тексеру — CL1 жолындағы тапсырмалар жиынында, бұл қабаттасулардың болмауын қамтамасыз ететін CL2 жолындағы тапсырмалар жиынынан өзгеше. Бұл тексеру жүйемен тапсырмалар байланысты болған кезде аяқталады. |