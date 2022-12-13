---
title: Project Operations Lite қолданбасын қолданыңыз
description: Бұл мақалада Project Operations жеңілдетілген нұсқасын мәміледен бастап проформа есеп-шотын ұсынуға дейін орналастыру бағдарламасын орнату жолы туралы ақпарат берілген.
author: stsporen
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 2c508f56b3018b6a86fea78bcf9ee4136e90f385
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/30/2022
ms.locfileid: "9810985"
---
# <a name="deploy-project-operations-lite"></a>Project Operations Lite қолданбасын қолданыңыз

_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_



Project Operations бірнеше орналастыру үлгілерін қолдайды. Орналастырудың ең үздік үлгісін анықтау үшін [Орналастыру үлгілері](determine-deployment-type.md) бөлімін қараңыз.


> [!IMPORTANT]
> Бұл жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі **тек Dataverse-арқылы Project Operations орналастыруға** әкеледі.

- [Project Operations бағдарламасын жаңа Dataverse ортасына орнату](#new)
- [Қолданыстағы Dataverse ортасына орнату](#existing)
- [Қос жазу құрамдастары бар Dataverse ортаға орнату](#existingdw)



## <a name="install-project-operations-lite-to-a-new-dataverse-environment"></a><a name="new"></a> Project Operations Lite бағдарламасын жаңа Dataverse ортаға орнатыңыз

1. Project Operations лицензиясы бар [глобалдық немесе Power Platform әкімшісі](/power-platform/admin/global-service-administrators-can-administer-without-license) ретінде [PowerPlatform басқару орталығы](https://admin.powerplatform.com) сайтында жаңа Dataverse ортасын жасаңыз. **Осы орта үшін дерекқор жасау** және **Dynamics 365 бағдарламалары** параметрлерінің қосулы екеніне көз жеткізіңіз. Қосымша ақпарат алу үшін [Орталарды Power Platform Басқару орталығында жасау және басқару](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center) бөлімін қараңыз.
1. Dynamics 365 бағдарламаларын орналастыру тізімінен **Microsoft Dynamics 365 Project Operations** опциясын таңдаңыз.


## <a name="install-project-operations-lite-to-an-existing-dataverse-environment"></a><a name="existing"></a> Project Operations Lite қолданбасын бар Dataverse ортасына орнатыңыз 
1. Project Operations лицензиясы бар [Басты немесе Power Platform әкімшісі](/power-platform/admin/global-service-administrators-can-administer-without-license) ретінде [PowerPlatform басқару орталығындағы](https://admin.powerplatform.com) Project Operations орнатқыңыз келетін жерге ортаны орналастырыңыз.
1. Dynamics 365 бағдарламаларын орналастыру тізімінен **Microsoft Dynamics 365 Project Operations** бағдарламасын орнатыңыз. Қосымша ақпарат алу үшін, [Dynamics 365 бағдарламаларын басқару](/power-platform/admin/manage-apps) бөлімін қараңыз.

## <a name="install-project-operations-lite-to-an-existing-dataverse-environment-where-dual-write-solutions-are-already-present"></a><a name="existingdw"></a> Project Operations Lite қолданбасын қос жазу шешімдері бұрыннан бар Dataverse ортасына орнатыңыз

Жоба операцияларын Lite Deployment режимінде іске қосуды жалғастырғыңыз келсе, мына қадамдарды орындауыңыз керек:

1. Project Operations лицензиясы бар [Басты немесе Power Platform әкімшісі](/power-platform/admin/global-service-administrators-can-administer-without-license) ретінде [PowerPlatform басқару орталығындағы](https://admin.powerplatform.com) Project Operations орнатқыңыз келетін жерге ортаны орналастырыңыз.
1. Dynamics 365 бағдарламаларын орналастыру тізімінен **Microsoft Dynamics 365 Project Operations** бағдарламасын орнатыңыз. Қосымша ақпарат алу үшін, [Dynamics 365 бағдарламаларын басқару](/power-platform/admin/manage-apps) бөлімін қараңыз.
1. Ортаңызда орнатылған қаржылық және операциялық қолданбаларды біріктіруге көмектесетін Қос жазу құрамдастары болғандықтан, Project Operations орнатуы жобаға қатысты деректерді қаржы және операциялық қолданбаларға біріктіру үшін қажетті мүмкіндіктер мен кеңейтімдерді де орнатады. Жоба операцияларын Lite орналастыруында іске қосқыңыз келгендіктен, бұл біріктіру құрамдастарын алып тастау керек, себебі олар Lite қолдану сценарийлері үшін шектеулер мен үстеме шығындар жасайды. Осы құрамдастарды жою үшін **Dynamics 365 Project Operations Dual Write** және **Dynamics 365 Project Operations Dual Write Entity Maps** шешімдерін қолмен жойыңыз.
1.  **Жоба операциялары -> Параметрлер -> Параметрлер**.  **Жоба параметрі** мәлімет бетін ашыңыз және **Шешімді жаңарту әрекеті** өрісін **Lite күйіне орнатыңыз. Тек**. Бұл жоба операцияларының кез келген кейінгі жаңартулары біріктіру құрамдастарын Жоба операцияларына қайтармайтынына кепілдік береді.  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
