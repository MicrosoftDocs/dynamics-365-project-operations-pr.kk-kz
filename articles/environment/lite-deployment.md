---
title: Project Operations бағдарламасын орналастыру - жеңілдетілген
description: Бұл тақырыпта Project Operations жеңілдетілген орналастыру бағдарламасын орнату амалы туралы ақпарат берілген - проформа-шотын ұсыну мәмілесі.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: e33506504665f2e7ef7ad48469082f9f64a2a44b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580739"
---
# <a name="deploy-project-operations---lite"></a>Project Operations бағдарламасын орналастыру - жеңілдетілген

_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_



Project Operations бірнеше орналастыру үлгілерін қолдайды. Орналастырудың ең үздік үлгісін анықтау үшін [Орналастыру үлгілері](determine-deployment-type.md) бөлімін қараңыз.


> [!IMPORTANT]
> Бұл жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі **тек Dataverse-арқылы Project Operations орналастыруға** әкеледі.

- [Жоба операцияларын жаңасына орнатыңыз Dataverse қоршаған орта](#new)
- [Барға орнату Dataverse қоршаған орта](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a> Жоба операцияларын жаңасына орнатыңыз Dataverse қоршаған орта

1. ретінде [Ғаламдық немесе Power Platform Әкімші](/power-platform/admin/global-service-administrators-can-administer-without-license) Project Operations лицензиясымен жаңасын жасаңыз Dataverse ішіндегі орта [PowerPlatform басқару орталығы](https://admin.powerplatform.com). Бұған көз жеткізіңіз **Осы орта үшін дерекқор жасаңыз** және **Dynamics 365 қолданбалары** қосылған. Қосымша ақпарат алу үшін [Орталарды Power Platform Басқару орталығында жасау және басқару](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center) бөлімін қараңыз.
2. Dynamics 365 бағдарламаларын орналастыру тізімінен **Microsoft Dynamics 365 Project Operations** опциясын таңдаңыз.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a> Жоба операцияларын барға орнатыңыз Dataverse қоршаған орта
1. Ортаның конфигурацияланбағанына көз жеткізіңіз [қосарлы жазу](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) өйткені орнату содан кейін орнатылады [Ресурс/қорда жоқ негізделген сценарийлер үшін жоба операциялары](project-operations-integrated-deployment-overview.md) мүмкіндіктері.
2. Project Operations лицензиясы бар [Басты немесе Power Platform әкімшісі](/power-platform/admin/global-service-administrators-can-administer-without-license) ретінде [PowerPlatform басқару орталығындағы](https://admin.powerplatform.com) Project Operations орнатқыңыз келетін жерге ортаны орналастырыңыз.
3. Dynamics 365 бағдарламаларын орналастыру тізімінен **Microsoft Dynamics 365 Project Operations** бағдарламасын орнатыңыз. Қосымша ақпарат алу үшін, [Dynamics 365 бағдарламаларын басқару](/power-platform/admin/manage-apps) бөлімін қараңыз.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
