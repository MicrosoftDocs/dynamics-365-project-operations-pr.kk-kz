---
title: Project Service Automation бағдарламасының 42-жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл мақалада Microsoft Dynamics 365 Project Service Automation 42, V3 жаңарту шығарылымындағы қолжетімді мүмкіндіктер мен түзетулердің тізімі берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/05/2022
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
ms.openlocfilehash: e9911531e4acbd78db416f554c8d85c4f1fee1cf
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912722"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>Project Service Automation бағдарламасының 42-жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер

[!include [banner](../includes/psa-now-project-operations.md)]

Біз Microsoft Dynamics 365 Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз. Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды. Бұл Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді. Осы шығарылымға жаңарту үшін Dynamics 365 онлайн шешімдері бетінің әкімші орталығына кіріп, жаңартуды орнатыңыз. Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.

Бұл мақалада жаңа немесе Project Service Automation 42, V3 жаңарту шығарылымы үшін өзгертілген мүмкіндіктер мен түзетулердің тізімі берілген. Бұл нұсқа V3.10.73.61 жиынтық нөміріне ие және әдетте өзін-өзі жаңарту арқылы 2022 жылдың сәуірінде қолжетімді.

## <a name="update-release-42"></a>42-жаңарту шығарылымы

### <a name="bug-fixes"></a>Қателерді түзету

Келесі мәселелер түзетілді.

**Уақыт және шығыс**

- Уақыт кестесі қабылданбаған кезде, оны қабылдамаған пайдаланушы **Жүйе** қате ретінде анықталады.
- Уақыт жазбалары импортталған кезде, **Ресурс санаты** мәні болмайды.
- Жобаны бекітушілердің рұқсаттары **Бекіте алады** мәніне арнайы орнатылмаған кезде, олар жіберілген жобаларды бекіте алады.

**Сатылым**

- Нақты мәндер түбірлік емес деңгейдегі тапсырмаларға тіркелгенде, нақты шығындар дұрыс жинақталмайды.
