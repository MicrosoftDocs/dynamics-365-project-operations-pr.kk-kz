---
title: Сәуір, 2022 ж. жаңалықтары - Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations
description: Бұл мақалада Microsoft корпорациясының 2022 жылғы сәуірдегі шығарылымында қолжетімді сапа жаңартулары туралы ақпарат берілген Dynamics 365 Project Operations ресурстарға/қорда жоқ сценарийлерге арналған.
author: sigitac
ms.date: 04/08/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 5ea1c96d64309990962f431b1c72ae47bf445bfa
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912385"
---
# <a name="whats-new-april-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Сәуір, 2022 ж. жаңалықтары - Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations

_**Қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Бұл мақала Microsoft корпорациясының келесі құрамдастары мен нұсқаларына қолданылады Dynamics 365 Project Operations:

- Жоба операциялары а Dataverse орта нұсқасы 4.41.0.45
- Dynamics 365 Finance ортасында жобаны басқару және есепке алу 10.0.26 нұсқасы

## <a name="features-included-in-this-release"></a>Осы шығарылымда қамтылған мүмкіндіктер

Сатып алу санаттары жобаның сатып алу тапсырыстарында және күтудегі жеткізушінің шот-фактураларында қолданылуы мүмкін. Қосымша ақпаратты қараңыз [Сатып алу санаттарын жобалық сатып алу тапсырыстарымен және күтудегі жеткізушінің шот-фактураларымен пайдаланыңыз](configure-procurement-categories.md).

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations қос жазу салыстыруларының жаңартулары

Келесі кестеде өзгертілген немесе 2022 жылдың наурыз айындағы Project Operations шығарылымында қосылған қос жазу карталары көрсетілген.

| Нысан картасы | Жаңартылған нұсқа | Комментарийлер |
| -------------- | ------------------- | ------------|
| Жоба операцияларын біріктіру жобасының жеткізушісі шот-фактура желісі экспорттау нысаны msdyn\_ проектвендорлық шот-фактуралар | 1.0.0.4 | Бұл карта сатып алу тапсырыстары мен күтудегі жеткізушінің шот-фактуралары бар сатып алу санаттарын пайдалануды қолдайды. |

Әрқашан ортаңызда картаның соңғы нұсқасын іске қосыңыз және жоба әрекеттерін жаңартқан кезде барлық қатысты кесте карталарын қосыңыз.Dataverse шешім және қаржылық шешім нұсқасы. Картаның соңғы нұсқасы іске қосылмаған болса, кейбір мүмкіндіктер мен мүмкіндіктер дұрыс жұмыс істемеуі мүмкін. Картаның белсенді нұсқасын **Қос жазу** бетіндегі **Нұсқа** бағанында қарауға болады. **Кесте картасының нұсқалары** параметрін, соңғы нұсқаны таңдап, содан кейін таңдалған нұсқаны сақтау арқылы картаның жаңа нұсқасын белсендіруге болады. Егер сіз қораптан тыс кесте картасын теңшеген болсаңыз, өзгертулерді қайта қолданыңыз. Қосымша ақпарат алу үшін [Шешімнің жарамдылық кезеңін басқару](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management) бөлімін қараңыз.

Картаны бастаған кезде мәселеге тап болсаңыз, бөліміндегі нұсқауларды орындаңыз [Карталарда кесте бағандары жоқ](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Қосарлы жазу ақауларын жою нұсқаулығы бөлімі.

## <a name="quality-updates"></a>Сапа жаңартулары

### <a name="project-operations-on-dataverse"></a>Dataverse ортасындағы Project Operations бағдарламасы

| Мүмкіндік аумағы | Сілтемелік нөмір | Сапа жаңартуы |
| ------------ | ---------------- | -------------- |
| Уақыт және шығыс | 2573900 | The **Заманауи бекіту** мүмкіндік әдепкі бойынша қосулы болуы керек. |
| Есеп-шот ұсыну және баға белгілеу | 2603313 | Өнімі бар тырнақша мен келісім-шарт жолдарын қосуға жол бермейтін қайталанатын жазба қатесі түзетілді. |
| Орналастыру және конфигурациялау | 2611368 | Тұтынушылар заманауи қолданба дизайнерін пайдалану арқылы шешімге бес теңшелетін нысанды қоса алуы керек. |
| Уақыт және шығыс | 2628285 | Уақытты енгізу импорты кезінде дұрыс ресурс санатын орнату мүмкіндігіне әсер еткен мәселе түзетілді. |
| Мүмкіндік басқармасы| 2628815 | Тақырып 100 таңбадан ұзақ болатын тапсырмалар үшін импорт сәтті болуы үшін тапсырма тақырыбының таңба шегіне сәйкестендіру үшін дәйексөз жолының егжей-тегжейлі сипаттамасының таңба шегін жаңартыңыз. |
| Уақыт және шығыс| 2629547 | The **Жіберген** жобаны мақұлдау өрісі жазбаны жіберген пайдаланушыны көрсетуі керек. |
| Уақыт және шығыс| 2629865 | The **Санатты көшіру** жобаларды көшіру кезінде тапсырмалар өрісі. |
| Уақыт және шығыс| 2636463 | Заманауи бекіту пішіндеріндегі мақұлдауларға сүзгілер түзетілді. |
| Жобаны жоспарлау және бақылау | 2648300 | Жоба иесін өзгертуге кедергі келтіретін мәселе түзетілді. |
| Есеп-шот ұсыну және баға белгілеу | 2563000 | Валюта келісім-шарт валютасынан ерекшеленетін шотсыз сатуға арналған журнал жолдарына рұқсат етілмеуі керек. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Dynamics 365 Finance жүйесінде жобаны басқару және есепке алу

Осы жаңартуға енгізілген қателерді түзету туралы ақпарат алу үшін жүйеге кіріңіз Microsoft Dynamics Lifecycle Services (LCS) және қараңыз [KB мақаласы](https://fix.lcs.dynamics.com/Issue/Details?bugId=662864).