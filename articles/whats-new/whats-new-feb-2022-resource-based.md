---
title: 2022 жылғы ақпандағы жаңалық - ресурс/биржадан тыс негіздегі сценарийлерді орналастыруға арналған Project Operations
description: Бұл мақала 2022 жылдың ақпан айындағы Project Operations шығарылымында ресурс/қорда жоқ негізделген сценарийлер үшін қол жетімді сапа жаңартулары туралы ақпарат береді.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: b036c0a3c39c52cb15277293679ef88906cae2c4
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8932993"
---
# <a name="whats-new-february-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>2022 жылғы ақпандағы жаңалық - ресурс/биржадан тыс негіздегі сценарийлерді орналастыруға арналған Project Operations

*Қолданылады: ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations*

Бұл мақала Microsoft корпорациясының келесі құрамдастары мен нұсқаларына қолданылады Dynamics 365 Project Operations:

- Жоба операциялары а Dataverse орта нұсқасы 4.28.0.120
- Dynamics 365 Finance ортасында жобаны басқару және есепке алу 10.0.24 нұсқасы

## <a name="features-included-in-this-release"></a>Осы шығарылымда қамтылған мүмкіндіктер

- Осы шығарылымнан бастап бір жобаға 300-ге дейін топ мүшелерін қосуға болады. Бұған дейін команда мүшелерінің санына шектеу 150 болатын. Қосымша ақпаратты қараңыз [Жоба шектеулері](../project-management/create-wbs.md#project-limitations).

## <a name="project-operations-dual-write-map-updates"></a>Project Operations қос жазу картасының жаңартулары

Келесі тізім 2022 жылдың ақпан айындағы Project Operations шығарылымында өзгертілген немесе қосылған қос жазу карталарын көрсетеді.

| Нысан картасы | Жаңартылған нұсқа | Комментарийлер |
| --- | --- | --- |
| Жоба операцияларын біріктіру жоба шығыстары экспорттық ұйым (msdyn\_ шығындар) | 1.0.0.3 | Жоба әрекетін синхрондау үшін кеңейтілген Dataverse. |

Project Operations қос жазу карталарының ағымдағы тізімі мен нұсқаларын көру үшін қараңыз [Project Operations қосарлы жазу картасының нұсқалары](../environment/resource-dual-write-maps.md).

Әрқашан ортаңызда картаның соңғы нұсқасын іске қосыңыз және жоба әрекеттерін жаңартқан кезде барлық қатысты кесте карталарын қосыңыз.Dataverse шешім және қаржылық шешім нұсқасы. Картаның соңғы нұсқасы іске қосылмаған болса, кейбір мүмкіндіктер мен мүмкіндіктер дұрыс жұмыс істемеуі мүмкін. Картаның белсенді нұсқасын **Қос жазу** бетіндегі **Нұсқа** бағанында қарауға болады. **Кесте картасының нұсқалары** параметрін, соңғы нұсқаны таңдап, содан кейін таңдалған нұсқаны сақтау арқылы картаның жаңа нұсқасын белсендіруге болады. Егер сіз қораптан тыс кесте картасын теңшеген болсаңыз, өзгертулерді қайта қолданыңыз. Қосымша ақпарат алу үшін [Шешімнің жарамдылық кезеңін басқару](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management) бөлімін қараңыз.

Картаны бастаған кезде мәселеге тап болсаңыз, бөліміндегі нұсқауларды орындаңыз [Карталарда кесте бағандары жоқ](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Dual Write ақауларын жою нұсқаулығы бөлімі.

## <a name="quality-updates"></a>Сапа жаңартулары

### <a name="project-operations-on-dataverse"></a>Dataverse ортасындағы Project Operations бағдарламасы

| Мүмкіндік аумағы | Сілтемелік нөмір | Сапа жаңартуы |
| --- | --- | --- |
| Есеп-шот ұсыну және баға белгілеу | 2415109 | ішіндегі әдепкі мән **Операцияларды төлеу шарттары** өріс жоба келісімшартының тұтынушы жазбасы және проформа шот-фактура жазбасы болуы керек. |
| Есеп-шот ұсыну және баға белгілеу | 2497369 | Материалды түзету файлдағы күн мәніне сәйкес болуы керек **Түзету** параметрлері. |
| Есеп-шот ұсыну және баға белгілеу | 2498697 | үшін қауіпсіздік конфигурациясын жақсартты **Уақытты енгізуді еске түсіру**. |
| Есеп-шот ұсыну және баға белгілеу | 2513824 | Ресурсқа негізделген сценарийлер үшін транзакция санатының идентификаторы Жоба операцияларында 28 таңбадан аспауы керек. |
| Есеп-шот ұсыну және баға белгілеу | 2517455 | The **Шот-фактура транзакцияларын жаңарту** әрекетті бір шот-фактура үшін бір уақытта бірнеше рет іске қосуға рұқсат етілмеуі керек. |
| Есеп-шот ұсыну және баға белгілеу | 2517465 | The **Шот-фактура желісінің мәліметтерін өшіру** әрекет бұғатталған, себебі оған қолдау көрсетілмейді. |
| Есеп-шот ұсыну және баға белгілеу | 2556660 | Жоба параметрлері жазбасына тіркелген бағалар тізімінде орындалатын күн тиімділігін тексеру бекітілді. |
| Мүмкіндік басқармасы | 2369202 | Бір жоба келісімшартына қайталанатын әрекет ету мерзімі бар баға тізімдерін тіркейтінін тексеретін бизнес логикасы түзетілді. |
| Мүмкіндік басқармасы | 2385965 | бойынша мінез-құлық түзетілді **Тұтынушылар** қойындысы **Жоба шарты** таңдаған кезде бет **Сақтау және жабу**. |
| Уақыт және шығыс | 2538503 | Жоба тапсырмасы файлда қолжетімді болуы керек **Жобаның нақты деректері** шығындар туралы есеп жарияланғаннан кейін ұйым. |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Dynamics 365 Finance сайтында жобаны басқару және есепке алу

| Мүмкіндік аумағы | Сілтемелік нөмір | Сапа жаңартуы |
| --- | --- | --- |
| Жобаларды басқару және есеп | [615496](https://fix.lcs.dynamics.com/Issue/Details/?bugId=615496) | Жеткізушінің несиелік жазбаларын импорттау кезінде қате орын алады. Қате туралы хабарда "Сақтау сомасы қалған таза сомадан артық болуы мүмкін емес" делінген. |
| Жобаларды басқару және есеп | [619391](https://fix.lcs.dynamics.com/Issue/Details/?bugId=619391) | Егер шот-фактура ұсынысында шот-фактура көрсетілмеген сатулар болып табылатын нөлдік сомадағы комиссиялық транзакциялар болса, шот-фактура жасау мүмкін емес. |
| Жобаларды басқару және есеп | [624423](https://fix.lcs.dynamics.com/Issue/Details/?bugId=624423) | Сатып алу бағасы жаңартылғаннан кейін жарияланған құн дұрыс емес және **Өзгерістерді басқаруды іске қосыңыз** қосылған.|
| Жобаларды басқару және есеп | [628386](https://fix.lcs.dynamics.com/Issue/Details/?bugId=628386) | Бекітілген баға жобасының жариялау сметасы, тіпті егер баға белгіленбесе де, сметалық ваучердегі қате валюта мен соманы пайдаланады.**Сметалық есептеу үшін жоба келісімшартының валютасын қосыңыз** мүмкіндігі қосылған. |
| Жобаларды басқару және есеп | [629239](https://fix.lcs.dynamics.com/Issue/Details/?bugId=629239) | **ProjDMFDataPopulation\_ Кеңейтім** қосылмаған конфигурация кілттері бар нысандар үшін ерекше жағдайларды ұстамай, өзгерістерді бақылауды қосу үшін қоңырау шалмауы керек. |
| Жобаларды басқару және есеп | [623818](https://fix.lcs.dynamics.com/Issue/Details/?bugId=623818) | Пакеттік тапсырма бірнеше жетілдірілген журналдар жарияланғанда және қате орын алған кезде бекітіледі. |
| Сапар және шығыс | [616805](https://fix.lcs.dynamics.com/Issue/Details/?bugId=616805) | Шығындар туралы есептер бойынша ақшалай аванстармен байланысты есеп айырысу мәселесіне байланысты салық сомасы ақшалай аванс бөлігі ретінде жабылмайды. |
| Сапар және шығыс | [616959](https://fix.lcs.dynamics.com/Issue/Details/?bugId=616959) | Сату салығы туралы ақпарат қамтылмаған **Шығындар - жарияланған транзакциялар** есеп беру. |
| Сапар және шығыс | [618943](https://fix.lcs.dynamics.com/Issue/Details/?bugId=618943) | The **Түбіртектер қажет** шығыс саясатының бұзылуы шығыс есептері бойынша ескертуді қате көрсетеді. |
| Сапар және шығыс | [633470](https://fix.lcs.dynamics.com/Issue/Details/?bugId=633470) | Егер транзакция жүгіріс шығынының нәтижесі болса, жоба транзакциясы жалпы сату сомасына өтелмейтін сату салығын қамтымайды. |
| Сапар және шығыс | [642979](https://fix.lcs.dynamics.com/Issue/Details/?bugId=642979) | Бөлшектелген жолда салық болса, бөлшектеу жолының күнін өзгерте алмайсыз және бастапқы құжат күйінің қатесі орын алады. |

## <a name="removed-and-deprecated-features"></a>Жойылған және ескірген мүмкіндіктер

The [Жоба операцияларындағы жойылған немесе ескірген мүмкіндіктер](removed-depreciated-features-project.md) мақалада жойылған немесе ескірген мүмкіндіктер сипатталған Dynamics 365 Project Operations.

- Жойылған мүмкіндік өнім ішінде бұдан былай қолжетімді емес.
- Ескірген мүмкіндік белсенді әзірленуде емес және болашақ жаңартуда жойылуы мүмкін.

Ескерту туралы хабарландыру бетінде пайда болады [Жоба операцияларындағы жойылған немесе ескірген мүмкіндіктер](removed-depreciated-features-project.md) өнімнен кез келген мүмкіндік жойылғанға дейін 12 ай бұрын.

Тек құрастыру уақытына әсер ететін, бірақ құм жәшігімен және өндіріс ортасымен екілік үйлесімді өзгерістерді бұзу үшін ескіру уақыты 12 айдан аз болады. Әдетте, бұл өзгерістер компиляторға жасалуы керек функционалды жаңартулар болып табылады.