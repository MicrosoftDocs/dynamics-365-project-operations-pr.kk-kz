---
title: Жобаға негізделген келісім-шарт жолдарына шолу
description: Бұл тақырыпта жобаға негізделген келісім-шарт жолдарымен жұмыс істеу туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 824fdd54d7b513b49afd1a6d76d3387df81418e2
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858165"
---
# <a name="project-based-contract-lines-overview"></a>Жобаға негізделген келісім-шарт жолдарына шолу

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

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
| **Project** | Бұл өрісті осы келісім бойынша жұмысты орындау үшін пайдаланылатын жобаны анықтау үшін пайдаланыңыз. | Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жазбаны бағалау үшін **Қосылған тапсырмалар** және **Қосылған транзакциялар санаттары** опцияларымен бірге пайдаланылады. |
| **Қосылған тапсырмалар** | Осы келісім-шарт жолына таңдалған жоба бойынша барлық жоба тапсырмалары немесе тапсырмалар жиыны ғана қосылғанын көрсетеді. Бұл келесі мүмкін мәндерге ие параметрлер жиыны болып табылады:</br>- **Барлық жоба тапсырмалары**</br>- **Тек таңдалған жоба тапсырмалары**. Бұл өрістегі бос мән **Барлық жоба тапсырмалары** таңдауына тең. | Егер **Тек таңдалған тапсырмалар** таңдалған болса, сіз нақты тапсырмаларды таңдап, оларды **Жоба** бетіндегі **Тапсырма шотын ұсынуды реттеу** қойыншасындағы келісім-шарт жолымен байланыстыра аласыз. Бұл мән келісім-шарттың нақты немесе болжамды жол жазбасына сілтеме жасау үшін **Жоба** және **Қамтылған транзакция** кластарымен бірге пайдаланылады. |
| **Уақытпен қоса** | **Иә**/**Жоқ** мәні таңдалған жобадағы уақыт транзакцияларының немесе еңбек шығындарының осы келісім-шарт жолына кіретінін не кірмейтінін көрсетеді. **Жоқ** мәні уақыт транзакциялары немесе еңбек құны осы келісім-шарт жолына қосылмайтынын көрсетеді. **Иә** мәні олардың қосылатынын көрсетеді. | Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жол жазбасын бағалау үшін жобамен бірге пайдаланылады. |
| **Шығыспен қоса** | **Иә**/**Жоқ** мәні таңдалған жобадағы шығындардың осы келісім-шарт жолына кіретінін не кірмейтінін көрсетеді. **Жоқ** мәні шығыс құны осы келісім-шарт жолына қосылмайтынын көрсетеді. **Иә** мәні қосылатынын көрсетеді. | Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жол жазбасын бағалау үшін жобамен бірге пайдаланылады. |
| **Материалдармен қоса** | **Иә**/**Жоқ** мәні таңдалған жобадағы материалдың осы келісім-шарт жолына кіретінін не кірмейтінін көрсетеді. **Жоқ** мәні материал шығындарының осы келісім-шарт жолына кірмейтінін көрсетеді. **Иә** мәні қосылатынын көрсетеді. | Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жол жазбасын бағалау үшін жобамен бірге пайдаланылады. |
| **Ақымен қоса** | **Иә**/**Жоқ** мәні таңдалған жобадағы ақылардың осы келісім-шарт жолына кіретінін не кірмейтінін көрсетеді. **Жоқ** мәні ақы осы келісім-шарт жолына қосылмайтынын көрсетеді. **Иә** мәні олардың қосылатынын көрсетеді. | Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жол жазбасын бағалау үшін жобамен бірге пайдаланылады. |
| **Келісім-шарт сомасы** | Белгіленген баға келісім-шарты жолы бойынша, бұл сома тұтынушыға осы келісім-шарт жолымен байланысты барлық жұмыс құрамдастары үшін есеп-шот ұсынылатын келісілген мән болып табылады. Уақыт және материал бойынша келісім-шарт жолы бойынша, бұл сома тұтынушыға осы келісім-шарт жолымен байланысты барлық жұмыс құрамдастары үшін есеп-шот ұсынылатын болжалды мән болып табылады. Баға ұсынудан жасалған жоба келісім-шарты бойынша, бұл мән баға ұсыну жолындағы сәйкес өрістен көшірілген. Жобаға негізделген келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл өріс өңдеу үшін құлыпталады және келісім-шарт жолы туралы мәліметтердегі сомадан жинақталады. | Келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл мәнді жол туралы мәліметтердегі сомаларды өзгерту арқылы өзгертуге болады. Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді шот ұсыну кезеңдеріне салық алдында соманы құру үшін пайдаланылады. |
| **Болжалды салық** | Пайдаланушы бұл өрісті келісім-шарт жолына болжалды салық сомасын енгізу үшін өңдей алады. Жобаға негізделген келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл өріс өңдеу үшін құлыпталады және келісім-шарт жолы туралы мәліметтердегі салық сомасынан жинақталады. | Келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл мәнді жол туралы мәліметтердегі салық сомаларын өзгерту арқылы өзгертуге болады. Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді төлем жасау кезеңдеріне салық салу үшін пайдаланылады. |
| **Салықтан кейінгі келісім-шарт сомасы** | Салықтан кейінгі келісім-шарт жолының сомасы. Бұл өріс тек оқуға арналған және **Келісім-шарт сомасы + салық** ретінде есептеледі. | Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді төлем жасау кезеңдерін құру үшін пайдаланылады. |
| **Асырмау шегі** | Пайдаланушы бұл өрісті өңдей алады және ол тек шот ұсыну әдісін уақыт пен материал ретінде орнатқан жобаға негізделген келісім-шарт жолдарында қолжетімді. | Пайдаланушы бұл өрісті өңдей алады. Уақыт пен материалға арналған нақты көрсеткіштер осы келісім-шарт жолына уақыт пен материал үшін сілтеме жасаған кезде, нақты сома осы келісім-шарт жолындағы асырмау шегімен бағаланады. Бұл бағалау жұмсалған және жасалған сомалар есепке алынғаннан кейін аяқталады. |
| **Тұтынушы бюджеті** | Бұл өрісті өңдеуге болады және келісім-шарт баға ұсынудан жасалған болса, баға ұсыну жолындағы сәйкес өрістен көшіріледі. | Бұл өріс тек ақпарат алу үшін пайдаланылады және бұл өрісте ағынның маңыздылығы жоқ. |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a>Жобаға негізделген келісім-шарт жолдарының Жалпы қойыншасындағы опцияларға арналған тексеру ережелері

1-ереже: **Қосылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** опциясына орнатылса, жобаның барлық тапсырмалары келісім-шарт жолына қосылады.

2-ереже: **Қосылған тапсырмалар** өрісі бос болған кезде немесе нақты **Барлық жоба тапсырмалары** опциясына орнатылған кезде, жоба мен белгілі бір транзакция класын тек келісім-шарттың бір жобаға негізделген келісім-шарт жолына қосуға болады.

3-ереже: **Қосылған тапсырмалар** өрісі **Тек таңдалған жоба тапсырмалары** опциясына орнатылған кезде, жоба мен белгілі бір транзакция класын тек келісім-шарттың бірнеше жобаға негізделген келісім-шарт жолдарына қосуға болады.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p>
                    <strong>Келісімшарт</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Келісім-шарт жолы</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="67" valign="top">
                <p>
                    <strong>Қамтылған тапсырмалар</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Уақытпен қоса</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Шығыспен қоса</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Материалдармен қоса</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Қамту</strong>
                </p>
                <p>
                    <strong>Құн</strong>
                </p>
            </td>
            <td width="53" valign="top">
                <p>
                    <strong>Жарамды/ Жарамсыз</strong>
                </p>
            </td>
            <td width="250" valign="top">
                <p>
                    <strong>Себеп</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Жарамсыз </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
№2 ережені бұзу. Р1 жобасындағы уақыт, шығын , материалдар және төлемдер CL1 және CL2 келісім-шарт жолдарына бірдей енгізілген.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Жарамсыз </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
№2 ережені бұзу. Р1 жобасындағы уақыт, материалдар және төлемдер CL1 және CL2 келісім-шарт жолдарына бірдей енгізілген.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Жарамды </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
Р1 жобасындағы уақыт, материалдар және төлемдер CL1 баға ұсыну жолына бірдей енгізілген.
                </p>
                <ul>
                    <li>
P1 жобасындағы шығыс CL2 баға ұсыну жолына енгізілген.
                    </li>
                </ul>
                <p>
Әрбір келісім-шарт жолына кіретін ешнәрсе қабаттаспайды, сондықтан жарамды болып табылады.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
No </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Тек таңдалған тапсырмалар </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Жарамсыз </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
№2 ережені бұзу </p>
                <p>
C1 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығындағы уақытты, материалдарды, шығындар мен ақыларды қамтиды.
                </p>
                <p>
CL2 жолына бүкіл P1 жобасы үшін уақыт, материалдар, шығын және төлем қосылған, сондықтан C1 жолында қамтылғанмен қабаттасады.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Тек таңдалған тапсырмалар </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Жарамды </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
№3 ережеге сәйкес </p>
                <p>
C1 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығындағы уақытты, шығындарды, материалдар мен төлемдерді қамтиды.
                </p>
                <p>
CL2 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығы үшін уақытты, материалдарды, шығындар мен төлемдерді қамтиды.
                </p>
                <p>
Жалғыз қосымша тексеру CL1 бойынша тапсырмалар жиынтығының айналасында болады, бұл CL2 бойынша тапсырмалар жиынтығынан ерекшеленеді, осылайша қабаттасудың болмауын қамтамасыз етеді. Бұл тапсырмалар байланыстырылған кезде жүйе тарапынан жасалады.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Тек таңдалған тапсырмалар </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]