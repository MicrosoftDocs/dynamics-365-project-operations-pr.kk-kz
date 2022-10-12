---
title: Project Service Automation бағдарламасының 30-жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл мақалада Project Service Automation Update Release 30, V3 нұсқасында қолжетімді мүмкіндіктер мен түзетулер тізімі берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: ad00b126a13e18a5de47df335aea06b9690efa13
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925081"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a>Project Service Automation бағдарламасының 30-жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер

[!include [banner](../includes/psa-now-project-operations.md)]

Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз. Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды. Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді. Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз. Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.

Бұл мақалада Project Service Automation V3, Жаңарту шығарылымы 30 үшін жаңа немесе өзгертілген мүмкіндіктер мен түзетулер тізімі берілген. Бұл нұсқа V3.10.51.61 жиынтық нөміріне ие және әдетте өзін-өзі жаңарту арқылы 2021 жылдың сәуірінде қолжетімді.

## <a name="update-release-30"></a>30-жаңарту шығарылымы

### <a name="bug-fixes"></a>Қателерді түзету

**Уақыт және шығыс**

Келесі мәселелер түзетілді:

- **Рөл** өрісі жойылған болса, **Жылдам жасау** бетіндегі уақыт жазбасын жасағанда және сақтағанда қате пайда болады.
- "Уақыт жазбасы" сүзгісі қате сүзгі операторын қолданады.
- Уақыт жазбасы басқару элементіндегі **Аптаны көшіру** опциясын таңдаған кезде көшірілген уақыт кестелері автоматты түрде көрсетілмейді.

**Ресурсты басқару**

Келесі мәселелер түзетілді:

- Тапсырысты ұзартқанда, қатты көшірмелеуге тағайындалған брондау күйі дұрыс емес. Брондауды ұзарту брондауды орнату метадеректерінде **Бекітілген** ретінде анықталған күйге сәйкес келеді.
- Брондаудың жарамды күйі көрсетілмеген кезде, қате туралы хабарлама дұрыс локализацияланбаған.

**Жоба басқармасы**

Келесі мәселелер түзетілді:

- Жобаларды бір валютада жасау мүмкін емес және оған басқа валютада тиісті тапсырмалар кіреді.

**Сатылым**

Келесі мәселелер түзетілді:

- Бағатізбе көшірілген кезде бағалар жаңартылмайды.
- Баға мәліметтерінің шыққан жеріне сәйкес мәні болса, баға ұсыныстарын "ұтқан" ретінде жабу сәтсіз аяқталды.
- **Жоба тапсырмасы** нысанында **Болжалды құны** атауы **Жоспарланған құны (негізгі)** атауына өзгертілді.
- Жарамсыз сілтеме ерекшеліктері шот-фактуралар жасалған немесе жойылған кезде жасалады.