---
title: Project Service Automation бағдарламасының 27-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 27-жаңарту шығарылымының 3-нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
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
ms.openlocfilehash: ee7bbe888a982e3554ba524c67442437c9be9183a5ee0940ccc3261b4a4992e7
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "6985058"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-27-v3"></a>Project Service Automation бағдарламасының 27-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер

[!include [banner](../includes/psa-now-project-operations.md)]

Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз. Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды. Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді. Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз. Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.

Бұл бөлімде Project Service Automation бағдарламасының 27-жаңарту шығарылымының 3-нұсқасындағы мүмкіндіктер мен түзетулер берілген. Бұл нұсқа V3.10.45.98 құрылым нөміріне ие және әдетте 2021 жылдың қаңтар айында шыққан өзін-өзі жаңарту мүмкіндігі арқылы қолжетімді.

## <a name="update-release-27"></a>27-жаңарту шығарылымы

### <a name="bug-fixes"></a>Қателерді түзету

**Жалпы**

Келесі мәселелер түзетілді:

- Project Service Automation бағдарламасындағы қосылатын модульдер арқылы жасалған журналдар автоматты түрде жойылатын күйге орнатылмаған.
- Автоматты жаңарту сәтсіз аяқталды, себебі Project Service Automation шешімінде бұрынғы нөлдік NavBarArea және тақырып элементі бар.

**Уақыт және шығыс**

Келесі мәселелер түзетілді:

- **Уақыт жазбасы** торы **Тәуелсіз уақыт белдеуі** күн тәртібі үшін дұрыс емес деректерді көрсетеді.
- **Уақыт жазбасы** торы **Тәуелсіз уақыт белдеуі** күн тәртібі үшін дұрыс емес уақыт жасайды.
- Тапсырманы іздеу **Уақыт жазбасын өңдеу** бетіндегі таңдалған жобаға шектелмейді.
- Жобадан тыс уақыт жазбаларына арналған уақыт растауы бұғатталған, себебі жүйе жобаны растаушыны іздейді.
- Уақыт мәндердегі дұрыс жазбалар дұрыс емес қате туралы хабарды көрсетеді.
- Тапсырмада нақты өзіндік құны үшін нөлдік мәні болып, жоба қорытындылары жаңартылған кезде келесі қате пайда болады: "Берілген кілт сөздікте жоқ".
- Нақты жағдайларда **Жоба болжамы** қойыншасындағы **Топтау әдісі** сүзгілері шығыс болжамдарын көрсетпейді.
- **Күндізгі уақыт** аралығы уақыт жазбалары үшін дұрыс емес.

**Жоба басқармасы**

Келесі мәселелер түзетілді:

- **Жоба** бетін жүктеуге қатысты өнімділікті арттыратын кэштеу жақсартулары.
- Жобалық тапсырмаларды орындауға мүмкіндік бермейтін ескірген бизнес ережесі.
- Microsoft Project қондырмаларының контуры қондырманың күнтізбесіне сәйкес келмейді, нәтижесінде ресурстардың дұрыс емес талаптарына алып келеді.
- Үлгілерден жобаларды жасау тағайындау күндерін дұрыс белгілемейді және ресурстар талаптарын құруға жол бермейді.
- Пайдаланушы пернетақта арқылы **Санат**, **Сипаттама**, **Күй** опцияларына кіре алмайды.
- Жобаның нақты сатылым мәндері ақы мен материалдардың сатылым мәндерін ескермейді.
- Нақты сатылымдар мен нақты шығындардың жиынтығы әр түрлі бағамдармен қате жүреді.
- **Әдепкі жұмыс уақыты үлгісі** бөліміндегі сипаттама жарамсыз.
- Тапсырма шегінісі пайдаланушы интерфейсінде жаңартылғанға дейін **Санат** өрісін жоймайды.
- Жобаның аяқталу мерзімінен тыс жылжуын қамтамасыз ететін тексеруді жіберіп алуға жол берілмейді.

**Sales**

Келесі мәселелер түзетілді:

- Жобалық баға ұсынысында бос сілтеме ерекшелігі жасалады, себебі жоба таңдалмағанда **Жоба болжамынан импорттау** мүмкіндігі көрінеді.
- Баға ұсынысын **Ұтқан** ретінде жапқанда келесі қате пайда болады: "Нысан сілтемесі нысан данасына орнатылмаған".
- Жобаны келісім-шарт жолынан ажыратқанда реттеу күйі нақты кері бағыттау кезінде орнатылмаған.
- Dynamics 365 Field Service және Project Service Automation бағдарламаларының екеуі де орнатылғанда **Бағаны бекітуді бұғаттау** және **Ағымдағы бағаны бекітуді пайдалану** опциялары **Есеп-шот** бетінде бір уақытта көрсетілмейді.
- Жапон тілі үшін басқа күнтізбелік беттермен сәйкес келмейтін аударма бар.
- **Іске қосу** және **Өшіру** мүмкіндіктері Project Service Automation бағдарламасындағы **Бағатізбе байланысы** нысандарынан жойылды.


[!INCLUDE[footer-include](../includes/footer-banner.md)]