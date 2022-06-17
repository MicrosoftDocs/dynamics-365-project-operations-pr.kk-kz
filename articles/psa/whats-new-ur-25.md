---
title: Project Service Automation бағдарламасының 25-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл мақалада Project Service Automation Update Release 25, V3 нұсқасында қолжетімді мүмкіндіктер мен түзетулер тізімі берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 2330c7dc5d2dfb148d5c7fb9a5ce643fded84dde
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922551"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a>Project Service Automation бағдарламасының 25-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер

[!include [banner](../includes/psa-now-project-operations.md)]

Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз. Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды. Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді. Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз. Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.

Бұл мақалада Project Service Automation V3, Жаңарту шығарылымы 25 үшін жаңа немесе өзгертілген мүмкіндіктер мен түзетулер тізімі берілген. Бұл нұсқада V 3.10.43.76 құрастыру нөмірі бар және әдетте 2020 жылдың қазан айында өзін-өзі жаңарту арқылы қол жетімді.

## <a name="update-release-25"></a>25-жаңарту шығарылымы

### <a name="bug-fixes"></a>Қателерді түзету

**Уақыт және шығыс**

Келесі мәселе түзетілді:

- Тым үлкен аралыққа негізделген қосымша деректерді көрсететін уақыт жазбасы шығарылды.

**Ресурсты басқару**

Келесі мәселе түзетілді:

- Universal Resource Scheduling түзетуінің импортын, жоғары нұсқалы түзету бұрыннан бар болса, өткізіп жіберу үшін Package deployer құралының коды қосылды.

**Жоба басқармасы**

Келесі мәселелер түзетілді:

- Жобаны бақылау торында дұрыс емес жоспарлы құнға әкелетін айырбас бағамының дөңгелектенуі мен сәйкессіздіктері түзетілді.
- **Жоба** пішінінде екі немесе одан да көп реакция торларын көрсету мүмкіндігіне қолдау көрсетілді.
- Тапсырманы күнтізбелік аяқталу күнінен бұрын тағайындау мүмкіндігін шешу үшін тексеру ұсынылды, бұл ресурстың сәтсіз тағайындалуына әкеледі.
- Төменде келтірілгеннен құрылған Null Reference Exception мүмкіндігін шешу үшін қателерді өңдеу жақсартылды:

    - **PreValidateProjectTeamMemberCreate** қосылатын модулі
    - **PreValidateProjectTaskCreate** жоба тапсырмасы байланысты жобасыз жасалған кезде
    - **PreProjectTeamMemberCreate** қосылатын модулі
    - **PostProjectTeamMemberDelete** қосылатын модулі
    - **PreValidateProjectTaskDelete** қосылатын модулі

**Sales**

Келесі мәселелер түзетілді:

- **Жобаны көшіру: HelperResource болжамдарын басқару** мүмкіндігінен құрылған Null Reference Exception мүмкіндігін шешу үшін қателерді өңдеу жақсартылды.
- **Уақыт және материалдық шоттың орындалмаған әрекеттері** тармағындағы **Есеп-шот ұсынуға дайын емес** төлем күйін өшірмейді.
- **Рөл бағасы** және **Каталог элементтері** қойыншасындағы қате белгіленген **Бағалар** түймешігі түзетілді.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
