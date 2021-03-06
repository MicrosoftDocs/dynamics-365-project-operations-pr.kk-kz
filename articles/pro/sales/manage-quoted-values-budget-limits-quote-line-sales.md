---
title: Жобаға негізделген баға ұсыну жолдары (Pro)
description: Бұл тақырыпта Project Operations бағдарламасындағы жоба жұмысына арналған жобаға негізделген баға ұсыну жолын пайдалану туралы ақпарат берілген. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908321"
---
# <a name="project-based-quote-lines-pro"></a>Жобаға негізделген баға ұсыну жолдары (Pro)

_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_

Жобаға негізделген баға ұсыну жолдары жоба жұмысын бағалауға көмектесуге арналған. Жобаға негізделген баға ұсыну жолының құрылымы жоба болжамдары үшін келесі тұжырымдамалармен кеңейтілген:

- Есепшот ұсыну әдісі
- Жоба мен тапсырманы салыстыру
- Қамтылған транзакция кластары
- Асырмау шегі
- Төлем қабілеттілігін орнату
- Баға ұсыну жолының мәліметтері көмегімен бағалау
- Баға ұсыну жолының тұтынушылары

Келесі кестеде жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасындағы өрістері туралы ақпарат берілген. Бұл өрістер жоба жұмысын егжей-тегжейлі, алдын ала болжам негізін орнатуға көмектеседі.

| **Өріс** | **Маңыздылық, мақсаты және нұсқаулығы** | **Төменгі әсер** |
| --- | --- | --- |
| Атауы | Бағаланатын баға ұсынудың жеке компонентін анықтауға көмектесетін баға ұсыну жолының атауы. | Баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Есепшот ұсыну әдісі | Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолының сәйкес өрісінен көшіріледі. Бұл өрісте Dynamics 365 Project Operations тарапынан қолдау көрсетілетін екі негізгі келісілген үлгілер қамтылған:</br>- Бекітілген баға</br>- Уақыт және материал.| Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Project | Осы қосымша өрісті осы келісім бойынша жұмысты орындау мақсатында пайдаланылатын жобаны анықтау үшін пайдаланыңыз. Жоба баға ұсыну жолымен байланыстырылған кезде, ақылы тапсырмаларды орнатуға, сондай-ақ баға ұсыну жолын баға ұсыну жолының мәліметтері ретінде жоба негізінде болжауға көмектеседі. Жоба жобаға негізделген баға ұсыну жолымен салыстырылмаған кезде, баға әр баға ұсыну жолының мәліметтерін құру арқылы қолмен жасалуы керек. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.|
| Қосылған тапсырмалар | Осы баға ұсыну жолының таңдалған жобаға арналған барлық немесе кейбір жоба тапсырмалары үшін пайдаланылатынын көрсетеді. Бұл өріс келесі мүмкін мәндерге ие:</br>- Барлық жоба тапсырмалары</br>- Тек таңдалған жоба тапсырмалары</br>Осы өрістегі бос мән **Барлық жоба тапсырмалары** опциясына балама болып табылады. | Жоба бетінде **Тек таңдалған жоба тапсырмалары** таңдалған кезде, **Тапсырма төлемін орнату** қойыншасы арнайы тапсырмаларды баға ұсыну жолымен байланыстыру үшін оларды таңдауға мүмкіндік береді. Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Уақытпен қоса | Таңдалған жобадағы уақыт транзакциялары немесе еңбек құны осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі. Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі. Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылатын жағдайда, **Иә** мәні көрсетіледі. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Шығыспен қоса | Таңдалған жобадағы шығыс құны осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі. Баға ұсыну жолындағы болжамға шығыс құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі. Баға ұсыну жолындағы болжамға шығыс құны қосылатын жағдайда, **Иә** мәні көрсетіледі. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Ақымен қоса | Таңдалған жобадағы төлемдер осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі. Баға ұсыну жолындағы болжамға төлемдер қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі. Баға ұсыну жолындағы болжамға төлемдер қосылатын жағдайда, **Иә** мәні көрсетіледі. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Баға ұсынылған көлем | Бұл тұтынушыға осы жобаға негізделген баға ұсыну жолы бойынша болжамдалған барлық жұмыстар үшін ұсынылатын сома. Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолындағы **Тұтынушы бюджеті** өрісінен көшіріледі. Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі мөлшерден жинақталады. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Болжалды салық | Бұл пайдаланушыға баға ұсыну жолына салықтың есептелген мөлшерін қосатын өңделетін өріс. Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі салық мөлшерінен жинақталады. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Салықтан кейінгі баға ұсыну сомасы | Бұл өріс салықтан кейінгі баға ұсыну жолының сомасы болып табылады және тек оқуға арналған. Бұл өрістегі сома *Ұсынылған сома + Салық* ретінде есептеледі. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Асырмау шегі | Бұл өрісті өңдеуге болады және тек **Уақыт және материал** төлем әдісіне ие жобаға негізделген баға ұсыну жолдарында қолжетімді. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |
| Тұтынушы бюджеті | Бұл өрісті өңдеуге болады және мүмкіндіктен баға ұсынуы жасалған жағдайда, мүмкіндік жолындағы сәйкес өрісінен көшіріледі. | Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>Жобаға негізделген баға ұсыну жолдарының Жалпы қойыншасындағы өрістерді тексеру ережелері

**1-ереже**: Егер **Қамтылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** өрісіне орнатылған болса, жоба баға ұсыну жолына енгізіледі.

**2-ереже**: Егер **Қаматылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** өрісіне орнатылған болса, жоба мен белгілі бір транзакция класын баға ұсыныстарының жобаға негізделген баға ұсыну жолына енгізуге болады.

**3-ереже**: Егер **Қаматылған тапсырмалар** өрісі **Тек таңдалған жоба тапсырмалары** өрісіне орнатылған болса, жоба мен белгілі бір транзакция класын баға ұсыныстарының бірнеше жобаға негізделген баға ұсыну жолдарына енгізуге болады.

**4-ереже**: Егер мүмкіндікте бірнеше баға ұсыныстары болса, онда барлығы бірдей жобаға сілтеме жасайтын және бір транзакция класын қамтитын әртүрлі баға ұсыныстарында баға ұсыну жолдары болуы мүмкін.

**5-ереже**: Егер баға ұсыныстары бірдей мүмкіндікке тиесілі болмаса, олар бірдей жоба мен транзакция класын қамтуы мүмкін емес.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p>
                    <strong>Мүмкіндік</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Баға ұсынысы</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Баға ұсыну жолы</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="90" valign="top">
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
                    <strong>Қамту</strong>
                </p>
                <p>
                    <strong>Құн</strong>
                </p>
            </td>
            <td width="54" valign="top">
                <p>
                    <strong>Жарамды/ Жарамсыз</strong>
                </p>
            </td>
            <td width="308" valign="top">
                <p>
                    <strong>Себеп</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
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
            <td width="54" rowspan="2" valign="top">
                <p>
Жарамсыз </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
№2 ережені бұзу. Р1 жобасындағы уақыт, шығыс және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
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
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
№ </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Жарамсыз </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
№2 ережені бұзу. Р1 жобасындағы уақыт және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
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
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="48" valign="top">
                <p>
№ </p>
            </td>
            <td width="42" valign="top">
                <p>
Иә </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Жарамды </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
P1 жобасындағы уақыт және төлемдер QL1 баға ұсыну жолына енгізілген.
P1 жобасындағы шығыс QL2 баға ұсыну жолына енгізілген.
Әр баға ұсыну жолына енгізілгенде қабаттасу жоқ және ол жарамды.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Бос </p>
            </td>
            <td width="48" valign="top">
                <p>
№ </p>
            </td>
            <td width="48" valign="top">
                <p>
Иә </p>
            </td>
            <td width="42" valign="top">
                <p>
№ </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
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
            <td width="54" rowspan="2" valign="top">
                <p>
Жарамсыз </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Жоғарыдағы №2 ережені бұзу </p>
                <p>
Q1 Р1 жобасында тапсырмалар жиынындағы уақыт, шығыс және төлемдерді қамтиды.
                </p>
                <p>
QL2 бүкіл P1 жобасына арналған уақыт, шығыстар және төлемдерді қамтиды және Q1 баға ұсыну жолына енгізілгендермен қабаттасады.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
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
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
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
            <td width="54" rowspan="2" valign="top">
                <p>
Жарамды </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Жоғарыдағы №3 ережеге сәйкес, </p>
                <p>
Q1 Р1 жобасында тапсырмалар жиынындағы уақыт, шығыс және төлемдерді қамтиды.
                </p>
                <p>
QL2 Р1 жобасында тапсырмалар жиынындағы уақыт, шығыс және төлемдерді қамтиды.
                </p>
                <p>
Жалғыз қосымша тексеру QL2 тапсырмаларының жиынынан ерекшеленетін QL1 тапсырмаларының жиыны шеңберінде болады. Бұл қабаттасудың болмауын қамтамасыз етеді. Бұл тапсырмалар байланыстырылған кезде жүйе тарапынан жасалады.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
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
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Барлық жоба тапсырмалары немесе бос </p>
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
            <td width="54" valign="top">
                <p>
Жарамды </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
№5 ереже негізінде, Q1 және Q2 - бір мүмкіндіктегі екі баға ұсыну жолы, сондықтан екеуі де жобаның бірдей компоненттерін бағалай алады.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Q2 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Барлық жоба тапсырмалары немесе бос </p>
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
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Барлық жоба тапсырмалары немесе бос </p>
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
            <td width="54" valign="top">
                <p>
Жарамды </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
№4 ереже негізінде, Q1 және Q2 - әртүрлі мүмкіндіктегі екі баға ұсыну жолы, сондықтан екеуі де бірдей жобаның бірдей компоненттерін бағалай алмайды.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O2 </p>
            </td>
            <td width="41" valign="top">
                <p>
Т1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Барлық жоба тапсырмалары немесе бос </p>
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
            <td width="54" valign="top">
                <p>
Жарамсыз </p>
            </td>
        </tr>
    </tbody>
</table>

