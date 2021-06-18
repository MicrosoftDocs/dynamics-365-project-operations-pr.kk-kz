---
title: Project Service Automation бағдарламасына шолу
description: Бұл тақырыпта Dynamics 365 Project Service Automation бағдарламасын Dynamics 365 Finance бағдарламасына біріктіру шешімі туралы ақпарат көрсетілген.
author: ruhercul
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5ca459b99881b612e4656be112c8a2e420b4196e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005888"
---
# <a name="project-service-automation-overview"></a><span data-ttu-id="26348-103">Project Service Automation бағдарламасына шолу</span><span class="sxs-lookup"><span data-stu-id="26348-103">Project Service Automation overview</span></span>

[!include[banner](../includes/banner.md)]
[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="26348-104">Project Service Automation және Finance біріктіру шешімі Common Data Service арқылы Dynamics 365 Finance және Dynamics 365 Project Service Automation даналары бойынша деректерді синхрондау үшін деректерді біріктіру мүмкіндігін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="26348-104">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Dynamics 365 Finance and Dynamics 365 Project Service Automation via Common Data Service.</span></span> <span data-ttu-id="26348-105">Деректерді біріктіру мүмкіндігімен бірге қолжетімді біріктіру үлгілері Project Service Automation бағдарламасынан Finance бағдарламасына жоба, жоба келісім-шарттары, жоба келісім-шарты жолдары, жоба келісім-шарты жолының кезеңдері, жоба тапсырмалары, шығыс транзакция санаттары, сағаттық болжамдар және шығын болжамдары ағынына мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="26348-105">The integration templates that are available with the Data integration feature enable the flow of projects, project contracts, project contract lines, project contract line milestones, project tasks, expense transaction categories, hour estimates, and expense estimates from Project Service Automation to Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="26348-106">Егер 7.3.0 нұсқасын пайдалансаңыз, 4074835 білім қорын орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="26348-106">If you're using version 7.3.0, you must install KB 4074835.</span></span> <span data-ttu-id="26348-107">Содан кейін белгіленген баға жобаларын біріктіре аласыз.</span><span class="sxs-lookup"><span data-stu-id="26348-107">You will then be able to integrate fixed price projects.</span></span>
> - <span data-ttu-id="26348-108">Егер 7.3.0 нұсқасын пайдалансаңыз және төлем транзакцияларын Project Service Automation бағдарламасынан алып тастасаңыз, онда ол төлемдерді жоба есеп-шотына қосу үшін 4345320 білім қорын орындау қажет.</span><span class="sxs-lookup"><span data-stu-id="26348-108">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="26348-109">8.0 нұсқасын пайдалансаңыз, жоба тапсырмаларын біріктіру, шығындар транзакциясының санаттары, сағаттық болжамдар, шығын болжамдары және функционалды құлыптау мүмкіндіктерін пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="26348-109">If you're using version 8.0, you will be able to use project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking.</span></span>
> - <span data-ttu-id="26348-110">8.0.1 немесе одан кейінгі нұсқаны пайдалансаңыз, нақты көрсеткіштерді синхрондау мүмкіндігіне ие боласыз.</span><span class="sxs-lookup"><span data-stu-id="26348-110">If you're using version 8.0.1 or later, you will be able to synchronize actuals.</span></span>

<span data-ttu-id="26348-111">Project Service Automation Finance бағдарламасын біріктірмес бұрын, Project Service Automation біріктіру параметрлерін конфигурациялау қажет.</span><span class="sxs-lookup"><span data-stu-id="26348-111">Before you can integrate Project Service Automation Finance, you must configure the Project Service Automation integration parameters.</span></span> <span data-ttu-id="26348-112">Қосымша ақпаратты [Project Service Automation біріктіру параметрлері](PSA-parameters.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-112">For more information, see [Project Service Automation integration parameters](PSA-parameters.md).</span></span>

<span data-ttu-id="26348-113">Бұл біріктіру шешімі келесі сценарийлерде тікелей синхрондауға мүмкіндік береді:</span><span class="sxs-lookup"><span data-stu-id="26348-113">This integration solution enables direct synchronization in the following scenarios:</span></span>

- <span data-ttu-id="26348-114">Project Service Automation бағдарламасында жоба келісім-шарттарын орындаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-114">Maintain project contracts in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="26348-115">Project Service Automation бағдарламасында жобалар жасаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-115">Create projects in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="26348-116">Project Service Automation бағдарламасында жоба келісім-шарты жолдарын сақтаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-116">Maintain project contract lines in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="26348-117">Project Service Automation бағдарламасында жоба келісім-шарты жолының кезеңдерін сақтаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-117">Maintain project contract line milestones in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="26348-118">Project Service Automation бағдарламасында жоба тапсырмаларын орындаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-118">Maintain project tasks in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="26348-119">Finance бағдарламасында шығыс транзакция санаттарын сақтаңыз және оларды Finance бағдарламасынан Project Service Automation бағдарламасына тікелей синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-119">Maintain expense transaction categories in Finance, and synchronize them directly from Finance to Project Service Automation.</span></span>
- <span data-ttu-id="26348-120">Project Service Automation бағдарламасында жобаның сағаттық болжамдарын жасаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-120">Create project hour estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="26348-121">Project Service Automation бағдарламасында жобаның шығын болжамдарын жасаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-121">Create project expense estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="26348-122">Project Service Automation бағдарламасында жоба уақыты, шығын және төлемнің нақты көрсеткіштерін жасаңыз және оларды Finance бағдарламасында жариялай алу үшін Project Service Automation біріктіру журналында жоба транзакцияларын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-122">Create project time, expense, and fee actuals in Project Service Automation, and create project transactions in the Project Service Automation integration journal so that they can be posted in Finance.</span></span>

## <a name="data-synchronization"></a><span data-ttu-id="26348-123">Деректерді синхрондау</span><span class="sxs-lookup"><span data-stu-id="26348-123">Data synchronization</span></span>

<span data-ttu-id="26348-124">Келесі суретте деректердің Project Service Automation және Finance арасында біріктіру бөлігі ретінде синхрондалу жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="26348-124">The following illustration shows how data is synchronized as part of the integration between Project Service Automation and Finance.</span></span>

> [!NOTE]
> <span data-ttu-id="26348-125">Ағымдағы уақытта барлық үлгілер қолжетімді емес.</span><span class="sxs-lookup"><span data-stu-id="26348-125">Not all templates are currently available.</span></span> <span data-ttu-id="26348-126">Үлгілер аяқталғаннан кейін шығарылады.</span><span class="sxs-lookup"><span data-stu-id="26348-126">Templates will be released as they are completed.</span></span>

<span data-ttu-id="26348-127">[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіру](./media/PSA-integration.png)](./media/PSA-integration.png)</span><span class="sxs-lookup"><span data-stu-id="26348-127">[![Project Service Automation integration with Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span></span>

## <a name="system-requirements-for-finance"></a><span data-ttu-id="26348-128">Finance бағдарламасына қойылатын жүйе талаптары</span><span class="sxs-lookup"><span data-stu-id="26348-128">System requirements for Finance</span></span>

<span data-ttu-id="26348-129">Project Service Automation және Finance біріктіру шешімін пайдалану үшін Platform 12 немесе одан кейінгі жаңартуы бар Enterprise Edition 7.3 нұсқасын орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="26348-129">To use the Project Service Automation to Finance integration solution, you must install Enterprise edition 7.3 with Platform update 12 or later.</span></span>

## <a name="system-requirements-for-project-service-automation"></a><span data-ttu-id="26348-130">Project Service Automation бағдарламасы үшін қойылатын жүйе талаптары</span><span class="sxs-lookup"><span data-stu-id="26348-130">System requirements for Project Service Automation</span></span>

<span data-ttu-id="26348-131">Project Service Automation және Finance біріктіру шешімін пайдалану үшін келесі компоненттерді орнату қажет:</span><span class="sxs-lookup"><span data-stu-id="26348-131">To use the Project Service Automation to Finance integration solution, you must install the following components:</span></span>

- <span data-ttu-id="26348-132">Dynamics 365 Project Service Automation 9.0.0.0 нұсқасы не одан жоғары</span><span class="sxs-lookup"><span data-stu-id="26348-132">Dynamics 365 Project Service Automation version 9.0.0.0 or later</span></span>
- <span data-ttu-id="26348-133">Dynamics 365 Sales, 1.14.0.0 (v14) нұсқасы немесе одан кейінгі нұсқасына арналған қаражат шешімінің әлеуетті тұтынушысы</span><span class="sxs-lookup"><span data-stu-id="26348-133">Prospect to cash solution for Dynamics 365 Sales, version 1.14.0.0 (v14) or later</span></span>
- <span data-ttu-id="26348-134">Dynamics 365 Project Service Automation 1.0.0.0 нұсқасы немесе одан кейінгі нұсқасына арналған Project Service Automation және Finance шешімі</span><span class="sxs-lookup"><span data-stu-id="26348-134">Project Service Automation to Finance solution for Dynamics 365 Project Service Automation version 1.0.0.0 or later</span></span>

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a><span data-ttu-id="26348-135">Project Service Automation данасында Project Service Automation және Finance біріктіру шешімін орнатыңыз</span><span class="sxs-lookup"><span data-stu-id="26348-135">Install the Project Service Automation to Finance integration solution in your Project Service Automation instance</span></span>

<span data-ttu-id="26348-136">[Microsoft жүктеу орталығынан](https://www.microsoft.com/download/details.aspx?id=57016) Project Service Automation және Finance біріктіру шешімін жүктеп алыңыз және шешіммен бірге берілген нұсқауларды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="26348-136">Download the Project Service Automation to Finance integration solution from [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016), and follow the instructions that are included with the solution.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]