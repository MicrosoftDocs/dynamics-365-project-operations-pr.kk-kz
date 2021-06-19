---
title: Жобаны көшіру
description: Бұл тақырыпта Dynamics 365 Project Operations бағдарламасында жобаларды көшіру туралы ақпарат берілген.
author: ruhercul
ms.date: 05/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c3055ab5b8c07faa2bc9167956d283e2a66029dd
ms.sourcegitcommit: 173f2b1f4e063c440a5f78d76d456c62aadbd89e
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/24/2021
ms.locfileid: "6091261"
---
# <a name="copy-a-project"></a><span data-ttu-id="102dd-103">Жобаны көшіру</span><span class="sxs-lookup"><span data-stu-id="102dd-103">Copy a project</span></span>

<span data-ttu-id="102dd-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="102dd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="102dd-105">Dynamics 365 Project Operations көмегімен **Жобалар** пішінінде **Жобаны көшіру** параметрін таңдау арқылы жаңа жобаларды жылдам құруға болады.</span><span class="sxs-lookup"><span data-stu-id="102dd-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="102dd-106">Жобаны көшіру үшін көшіру керек жобаны ашып, **Жобаны көшіру** әрекетін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="102dd-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="102dd-107">Әрекет келесілерді көшіреді:</span><span class="sxs-lookup"><span data-stu-id="102dd-107">The action will copy the following:</span></span>

- <span data-ttu-id="102dd-108">Жоба сипаттары</span><span class="sxs-lookup"><span data-stu-id="102dd-108">Project properties</span></span> 
- <span data-ttu-id="102dd-109">Жұмыс декомпозициясының құрылымы</span><span class="sxs-lookup"><span data-stu-id="102dd-109">Work breakdown structure</span></span>
- <span data-ttu-id="102dd-110">Жоба тобының мүшелері</span><span class="sxs-lookup"><span data-stu-id="102dd-110">Project team members</span></span>
- <span data-ttu-id="102dd-111">Жоба болжамдары</span><span class="sxs-lookup"><span data-stu-id="102dd-111">Project estimates</span></span>
- <span data-ttu-id="102dd-112">Жобаның шығыс болжамдары</span><span class="sxs-lookup"><span data-stu-id="102dd-112">Project expense estimates</span></span>
- <span data-ttu-id="102dd-113">Жобаның материал болжамдары</span><span class="sxs-lookup"><span data-stu-id="102dd-113">Project material estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="102dd-114">Жоба сипаттары</span><span class="sxs-lookup"><span data-stu-id="102dd-114">Project properties</span></span>

<span data-ttu-id="102dd-115">Жоба көшірілген кезде, келесі өрістердегі мәндер көшіріледі:</span><span class="sxs-lookup"><span data-stu-id="102dd-115">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="102dd-116">Атауы</span><span class="sxs-lookup"><span data-stu-id="102dd-116">Name</span></span>
- <span data-ttu-id="102dd-117">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="102dd-117">Description</span></span>
- <span data-ttu-id="102dd-118">Тұтынушы</span><span class="sxs-lookup"><span data-stu-id="102dd-118">Customer</span></span>
- <span data-ttu-id="102dd-119">Күнтізбе үлгісі</span><span class="sxs-lookup"><span data-stu-id="102dd-119">Calendar Template</span></span>
- <span data-ttu-id="102dd-120">Валюта</span><span class="sxs-lookup"><span data-stu-id="102dd-120">Currency</span></span>
- <span data-ttu-id="102dd-121">Келісім-шарт бірлігі</span><span class="sxs-lookup"><span data-stu-id="102dd-121">Contracting Unit</span></span>
- <span data-ttu-id="102dd-122">Жоба менеджері</span><span class="sxs-lookup"><span data-stu-id="102dd-122">Project Manager</span></span>
- <span data-ttu-id="102dd-123">Күй</span><span class="sxs-lookup"><span data-stu-id="102dd-123">Status</span></span>
- <span data-ttu-id="102dd-124">Жалпы жоба күйі</span><span class="sxs-lookup"><span data-stu-id="102dd-124">Overall Project Status</span></span>
- <span data-ttu-id="102dd-125">Аңғартпалар</span><span class="sxs-lookup"><span data-stu-id="102dd-125">Comments</span></span>
- <span data-ttu-id="102dd-126">Болжамдар</span><span class="sxs-lookup"><span data-stu-id="102dd-126">Estimates</span></span>
- <span data-ttu-id="102dd-127">Болжалды басталу күні: бұл жоба көшірмеден жасалған күн.</span><span class="sxs-lookup"><span data-stu-id="102dd-127">Estimated Start Date: This is the date that the project is created from the copy.</span></span>
- <span data-ttu-id="102dd-128">Болжалды аяқталу күні: бұл күн көшірмеден жасалған жаңа жобаның басталу күніне байланысты реттеледі.</span><span class="sxs-lookup"><span data-stu-id="102dd-128">Estimated Finish Date: This date is adjusted based on the start date of the new project that was made from the copy.</span></span>
- <span data-ttu-id="102dd-129">Талпыныс (сағаттар)</span><span class="sxs-lookup"><span data-stu-id="102dd-129">Effort (Hours)</span></span>
- <span data-ttu-id="102dd-130">Болжалды еңбек құны</span><span class="sxs-lookup"><span data-stu-id="102dd-130">Estimated Labor Cost</span></span>
- <span data-ttu-id="102dd-131">Болжалды шығыс құны</span><span class="sxs-lookup"><span data-stu-id="102dd-131">Estimated Expense Cost</span></span>
- <span data-ttu-id="102dd-132">Болжалды материал құны</span><span class="sxs-lookup"><span data-stu-id="102dd-132">Estimated Material Cost</span></span>

> [!NOTE]
> <span data-ttu-id="102dd-133">Жобаны көшіру ұзақ уақытқа созылатын жұмыс.</span><span class="sxs-lookup"><span data-stu-id="102dd-133">Copy project is a long running operation.</span></span> <span data-ttu-id="102dd-134">Жоба жазбалары, олардың тиісті төлсипаттары және көптеген байланысты нысандар да көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="102dd-134">Project records, their relevant attributes, and many related entities are also copied.</span></span> <span data-ttu-id="102dd-135">Операция ұзаққа созылғандықтан, көшіру басталғаннан кейін мақсатты жоба беті көшіру әрекеті аяқталғанша өңдеу үшін бұғатталады.</span><span class="sxs-lookup"><span data-stu-id="102dd-135">Because of the long running nature of the operation, after the copy starts, the target project page is locked for editing until the copy operation is complete.</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="102dd-136">Жұмыс декомпозициясының құрылымы</span><span class="sxs-lookup"><span data-stu-id="102dd-136">Work breakdown structure</span></span>

<span data-ttu-id="102dd-137">Жоба көшірілген кезде, ресурсы жүктелген жұмыс декомпозициясының құрылымы көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="102dd-137">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="102dd-138">Аталған ресурстар жалпы ресурстармен алмастырылады.</span><span class="sxs-lookup"><span data-stu-id="102dd-138">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="102dd-139">Егер аталған ресурстар жалпы жұмыс сағатымен бірдей болмаса, кесте қайта есептеледі және тапсырманың ұзақтығы өзгеруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="102dd-139">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="102dd-140">Жоба тобы мүшелері</span><span class="sxs-lookup"><span data-stu-id="102dd-140">Project team members</span></span>

<span data-ttu-id="102dd-141">Жоба тобы бастапқы жобадан көшірілген кезде жалпы ресурстар көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="102dd-141">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="102dd-142">Әмбебап ресурс тағайындаулары да бастапқы жобадағы күйде сақталады.</span><span class="sxs-lookup"><span data-stu-id="102dd-142">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="102dd-143">Аталған ресурстар жалпы топ мүшелеріне айналады.</span><span class="sxs-lookup"><span data-stu-id="102dd-143">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="102dd-144">Болжамдар</span><span class="sxs-lookup"><span data-stu-id="102dd-144">Estimates</span></span>

<span data-ttu-id="102dd-145">Жоба көшірілген кезде ресурстар, шығындар және материал болжамы жолдары бастапқы жобадан көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="102dd-145">When the project is copied, resource, expense and material estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="102dd-146">Copy Project бағдарламасына бағдарламалы түрде қатынасу жолы туралы ақпаратты [ Copy Project көмегімен жоба үлгілерін жасау](dev-copy-project.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="102dd-146">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
