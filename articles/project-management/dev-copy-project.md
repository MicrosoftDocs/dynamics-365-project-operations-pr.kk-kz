---
title: Copy Project көмегімен жоба үлгілерін жасау
description: Бұл тақырыпта Copy Project реттелетін әрекеті көмегімен жоба үлгілерін жасау жолы туралы ақпарат берілген.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0100c29873be6346614e958ef6ea0c77da2c9590
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131620"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="82844-103">Copy Project көмегімен жоба үлгілерін жасау</span><span class="sxs-lookup"><span data-stu-id="82844-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="82844-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="82844-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="82844-105">Dynamics 365 Project Operations жобаны көшіру және кез-келген тапсырманы рөлді көрсететін жалпы ресурстарға қайтару мүмкіндігін қолдайды.</span><span class="sxs-lookup"><span data-stu-id="82844-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="82844-106">Тұтынушылар бұл функцияны жобаның негізгі үлгілерін құру үшін пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="82844-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="82844-107">**Copy Project** таңдалған кезде, мақсатты жобаның күйі жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="82844-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="82844-108">Көшіру әрекеті қашан аяқталғанын анықтау **Күй себебі** пәрменін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="82844-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="82844-109">**Copy Project** таңдау мақсатты жоба нысанында ешқандай мақсатты күн анықталмаса, жобаның басталу күнін ағымдағы басталу күніне дейін жаңартады.</span><span class="sxs-lookup"><span data-stu-id="82844-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="82844-110">Copy Project реттелетін әрекеті</span><span class="sxs-lookup"><span data-stu-id="82844-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="82844-111">Атауы</span><span class="sxs-lookup"><span data-stu-id="82844-111">Name</span></span> 

<span data-ttu-id="82844-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="82844-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="82844-113">Кіріс параметрлер</span><span class="sxs-lookup"><span data-stu-id="82844-113">Input parameters</span></span>
<span data-ttu-id="82844-114">Үш кіріс параметрі берілген:</span><span class="sxs-lookup"><span data-stu-id="82844-114">There are three input parameters:</span></span>

| <span data-ttu-id="82844-115">Параметр</span><span class="sxs-lookup"><span data-stu-id="82844-115">Parameter</span></span>          | <span data-ttu-id="82844-116">Түр</span><span class="sxs-lookup"><span data-stu-id="82844-116">Type</span></span>   | <span data-ttu-id="82844-117">Мәндер</span><span class="sxs-lookup"><span data-stu-id="82844-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="82844-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="82844-118">ProjectCopyOption</span></span>  | <span data-ttu-id="82844-119">String</span><span class="sxs-lookup"><span data-stu-id="82844-119">String</span></span> | <span data-ttu-id="82844-120">**{"removeNamedResources":true}** немесе **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="82844-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="82844-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="82844-121">SourceProject</span></span>      | <span data-ttu-id="82844-122">Нысан анықтамасы</span><span class="sxs-lookup"><span data-stu-id="82844-122">Entity Reference</span></span> | <span data-ttu-id="82844-123">Бастапқы жоба</span><span class="sxs-lookup"><span data-stu-id="82844-123">Source Project</span></span> |
| <span data-ttu-id="82844-124">Мақсатты мән</span><span class="sxs-lookup"><span data-stu-id="82844-124">Target</span></span>             | <span data-ttu-id="82844-125">Нысан анықтамасы</span><span class="sxs-lookup"><span data-stu-id="82844-125">Entity Reference</span></span> | <span data-ttu-id="82844-126">Мақсатты жоба</span><span class="sxs-lookup"><span data-stu-id="82844-126">Target Project</span></span> |


- <span data-ttu-id="82844-127">**{"clearTeamsAndAssignments":true}**: интернетке арналған жобаның әдепкі әрекеті және барлық тапсырмалар мен топ мүшелерін жояды.</span><span class="sxs-lookup"><span data-stu-id="82844-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="82844-128">**{"removeNamedResources":true}** Project Operation бағдарламасына арналған әдепкі әрекет және тағайындауларды жалпы ресурстарға қайтарады.</span><span class="sxs-lookup"><span data-stu-id="82844-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="82844-129">Әрекеттердегі әдепкі параметрлер туралы ақпарат алу үшін [Веб API әрекеттерін пайдалану](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions) бөлімін қараңыз</span><span class="sxs-lookup"><span data-stu-id="82844-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="82844-130">Көшіру үшін өрістерді көрсетіңіз</span><span class="sxs-lookup"><span data-stu-id="82844-130">Specify fields to copy</span></span> 
<span data-ttu-id="82844-131">Әрекет шақырылған кезде, **Copy Project** жоба көшірілгенде қандай өрістер көшірілетінін анықтау үшін **Жоба бағандарын көшіру** жоба көрінісін қарастырады.</span><span class="sxs-lookup"><span data-stu-id="82844-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>
