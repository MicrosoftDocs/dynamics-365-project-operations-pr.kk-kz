---
title: Project Service Automation бағдарламасының 45-жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл мақалада Microsoft Dynamics 365 Project Service Automation 45, V3 жаңарту шығарылымындағы қолжетімді мүмкіндіктер мен түзетулердің тізімі берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 07/14/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 98f7c973917d7d6334e6e0aeb15214c538b33143
ms.sourcegitcommit: 36fda4f45ddeb0f81d30bd1e22852727df644754
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/16/2022
ms.locfileid: "9169181"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-45-v3"></a>Project Service Automation бағдарламасының 45-жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер

[!include [banner](../includes/psa-now-project-operations.md)]

Біз Microsoft Dynamics 365 Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз. Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды. Бұл Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді. Осы шығарылымға жаңарту үшін Dynamics 365 онлайн шешімдері бетінің әкімші орталығына кіріп, жаңартуды орнатыңыз. Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.

Бұл мақалада жаңа немесе Project Service Automation 45, V3 жаңарту шығарылымы үшін өзгертілген мүмкіндіктер мен түзетулердің тізімі берілген. Бұл нұсқада V3.10.76.168 құрастыру нөмірі бар және әдетте 2022 жылдың шілде айындағы өзін-өзі жаңарту арқылы қолжетімді.

## <a name="update-release-45"></a>45-жаңарту шығарылымы

### <a name="bug-fixes"></a>Қателерді түзету

Келесі мәселелер түзетілді.

**Сатылым**

- Егер пайдаланушылар беттің бірдей данасын қарап жатса және оны жаңартпаса, пайдаланушылар шот-фактураны шот ұсынылмаған сатылымсыз жасауға әрекеттенгеннен кейін сәтті жасай алмайды.

**Уақыт және шығыс**

- Заманауи мақұлдаулар қосылғанда және қайта шақырылған жобаны мақұлдау бекітілгенде, жазба кезеңі **Қайта шақыру сұрауы мақұлданды** күйіне қателікпен жаңартылады.
- Заманауи мақұлдаулар қосылғанда және бұлттық ағындар белсенді емес болғанда, мақұлдау процесі сәтті болмайды және жіберуші немесе мақұлдаушы пайдаланушылар хабардар етілмейді.
