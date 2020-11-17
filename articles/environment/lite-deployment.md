---
title: Project Operations бағдарламасын орналастыру - жеңілдетілген
description: Бұл тақырыпта Project Operations жеңілдетілген орналастыру бағдарламасын орнату амалы туралы ақпарат берілген - проформа-шотын ұсыну мәмілесі.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0633585fcef91d9218d6140764addb7cf96ab31d
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175673"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="94068-103">Project Operations бағдарламасын орналастыру - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="94068-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="94068-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="94068-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="94068-105">Project Operations бірнеше орналастыру үлгілерін қолдайды.</span><span class="sxs-lookup"><span data-stu-id="94068-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="94068-106">Орналастырудың ең үздік үлгісін анықтау үшін [Орналастыру үлгілері](determine-deployment-type.md) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="94068-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="94068-107">Бұл жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі **тек Common Data Service-арқылы Project Operations орналастыруға** әкеледі.</span><span class="sxs-lookup"><span data-stu-id="94068-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="94068-108">Project Operations бағдарламасын жаңа CDS ортасына орнату</span><span class="sxs-lookup"><span data-stu-id="94068-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="94068-109">Қолданыстағы CDS ортасына орнату</span><span class="sxs-lookup"><span data-stu-id="94068-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="94068-110">Project Operations бағдарламасын жаңа CDS ортасына орнату</span><span class="sxs-lookup"><span data-stu-id="94068-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="94068-111">Project Operations лицензиясы бар [Басты немесе Power Platform әкімшісі](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) ретінде [PowerPlatform басқару орталығында](https://admin.powerplatform.com) жаңа CDS ортасын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="94068-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="94068-112">**CDS дерекқоры** және **Dynamics 365 бағдарламалары** іске қосылғанына көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="94068-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="94068-113">Қосымша ақпарат алу үшін [Орталарды Power Platform Басқару орталығында жасау және басқару](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="94068-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="94068-114">Dynamics 365 бағдарламаларының орналастырулар тізімінен **Microsoft Dynamics 365 Project Operations** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="94068-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="94068-115">Project Operations бағдарламасын қолданыстағы CDS ортасына орнату</span><span class="sxs-lookup"><span data-stu-id="94068-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="94068-116">Project Operations лицензиясы бар [Басты немесе Power Platform әкімшісі](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) ретінде [PowerPlatform басқару орталығындағы](https://admin.powerplatform.com) Project Operations орнатқыңыз келетін жерге ортаны орналастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="94068-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="94068-117">Dynamics 365 бағдарламаларының орналастырулар тізімінен **Microsoft Dynamics 365 Project Operations** тармағын орнатып алыңыз.</span><span class="sxs-lookup"><span data-stu-id="94068-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="94068-118">Қосымша ақпарат алу үшін, [Dynamics 365 бағдарламаларын басқару](https://docs.microsoft.com/power-platform/admin/manage-apps) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="94068-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>


