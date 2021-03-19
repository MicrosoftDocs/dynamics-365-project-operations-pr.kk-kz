---
title: Жобаны көшіру
description: Бұл тақырыпта Dynamics 365 Project Operations бағдарламасында жобаларды көшіру туралы ақпарат берілген.
author: ruhercul
manager: AnnBe
ms.date: 02/22/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: af1942e81691d9e13fdcbbf68599c1a8a4004582
ms.sourcegitcommit: 24528bb9c0ef8898077cb3bc672daa211c0e73aa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "5479526"
---
# <a name="copy-a-project"></a><span data-ttu-id="f260b-103">Жобаны көшіру</span><span class="sxs-lookup"><span data-stu-id="f260b-103">Copy a project</span></span>

<span data-ttu-id="f260b-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="f260b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f260b-105">Dynamics 365 Project Operations көмегімен **Жобалар** пішінінде **Жобаны көшіру** параметрін таңдау арқылы жаңа жобаларды жылдам құруға болады.</span><span class="sxs-lookup"><span data-stu-id="f260b-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="f260b-106">Жобаны көшіру үшін көшіру керек жобаны ашып, **Жобаны көшіру** әрекетін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f260b-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="f260b-107">Әрекет келесіні көшіреді:</span><span class="sxs-lookup"><span data-stu-id="f260b-107">The action will copy:</span></span>

- <span data-ttu-id="f260b-108">Жоба сипаттары (болжамды басталу күні бастапқы жобадан көшіріледі)</span><span class="sxs-lookup"><span data-stu-id="f260b-108">Project properties (The estimated start date is copied from the source project)</span></span>
- <span data-ttu-id="f260b-109">Жұмыс декомпозициясының құрылымы</span><span class="sxs-lookup"><span data-stu-id="f260b-109">The Work breakdown structure</span></span>
- <span data-ttu-id="f260b-110">Жоба тобының мүшелері</span><span class="sxs-lookup"><span data-stu-id="f260b-110">Project team members</span></span>
- <span data-ttu-id="f260b-111">Жоба болжамдары</span><span class="sxs-lookup"><span data-stu-id="f260b-111">Project estimates</span></span>
- <span data-ttu-id="f260b-112">Жобаның шығыс болжамдары</span><span class="sxs-lookup"><span data-stu-id="f260b-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="f260b-113">Жоба сипаттары</span><span class="sxs-lookup"><span data-stu-id="f260b-113">Project properties</span></span>

<span data-ttu-id="f260b-114">Жоба көшірілген кезде, келесі өрістердегі мәндер көшіріледі:</span><span class="sxs-lookup"><span data-stu-id="f260b-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="f260b-115">Атауы</span><span class="sxs-lookup"><span data-stu-id="f260b-115">Name</span></span>
- <span data-ttu-id="f260b-116">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="f260b-116">Description</span></span>
- <span data-ttu-id="f260b-117">Тұтынушы</span><span class="sxs-lookup"><span data-stu-id="f260b-117">Customer</span></span>
- <span data-ttu-id="f260b-118">Күнтізбе үлгісі</span><span class="sxs-lookup"><span data-stu-id="f260b-118">Calendar Template</span></span>
- <span data-ttu-id="f260b-119">Валюта</span><span class="sxs-lookup"><span data-stu-id="f260b-119">Currency</span></span>
- <span data-ttu-id="f260b-120">Келісім-шарт бірлігі</span><span class="sxs-lookup"><span data-stu-id="f260b-120">Contracting Unit</span></span>
- <span data-ttu-id="f260b-121">Жоба менеджері</span><span class="sxs-lookup"><span data-stu-id="f260b-121">Project Manager</span></span>
- <span data-ttu-id="f260b-122">Күй</span><span class="sxs-lookup"><span data-stu-id="f260b-122">Status</span></span>
- <span data-ttu-id="f260b-123">Жалпы жоба күйі</span><span class="sxs-lookup"><span data-stu-id="f260b-123">Overall Project Status</span></span>
- <span data-ttu-id="f260b-124">Комментарийлер</span><span class="sxs-lookup"><span data-stu-id="f260b-124">Comments</span></span>
- <span data-ttu-id="f260b-125">Болжамдар</span><span class="sxs-lookup"><span data-stu-id="f260b-125">Estimates</span></span>
- <span data-ttu-id="f260b-126">Болжалды басталу күні</span><span class="sxs-lookup"><span data-stu-id="f260b-126">Estimated Start Date</span></span>
- <span data-ttu-id="f260b-127">Аяқталу күні</span><span class="sxs-lookup"><span data-stu-id="f260b-127">Finish Date</span></span>
- <span data-ttu-id="f260b-128">Талпыныс (сағаттар)</span><span class="sxs-lookup"><span data-stu-id="f260b-128">Effort (Hours)</span></span>
- <span data-ttu-id="f260b-129">Болжалды еңбек құны</span><span class="sxs-lookup"><span data-stu-id="f260b-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="f260b-130">Болжалды шығын</span><span class="sxs-lookup"><span data-stu-id="f260b-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="f260b-131">Жұмыс декомпозициясының құрылымы</span><span class="sxs-lookup"><span data-stu-id="f260b-131">Work breakdown structure</span></span>

<span data-ttu-id="f260b-132">Жоба көшірілген кезде, ресурсы жүктелген жұмыс декомпозициясының құрылымы көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="f260b-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="f260b-133">Аталған ресурстар жалпы ресурстармен алмастырылады.</span><span class="sxs-lookup"><span data-stu-id="f260b-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="f260b-134">Егер аталған ресурстар жалпы жұмыс сағатымен бірдей болмаса, кесте қайта есептеледі және тапсырманың ұзақтығы өзгеруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f260b-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="f260b-135">Жоба тобы мүшелері</span><span class="sxs-lookup"><span data-stu-id="f260b-135">Project team members</span></span>

<span data-ttu-id="f260b-136">Жоба тобы бастапқы жобадан көшірілген кезде жалпы ресурстар көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="f260b-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="f260b-137">Әмбебап ресурс тағайындаулары да бастапқы жобадағы күйде сақталады.</span><span class="sxs-lookup"><span data-stu-id="f260b-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="f260b-138">Аталған ресурстар жалпы топ мүшелеріне айналады.</span><span class="sxs-lookup"><span data-stu-id="f260b-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="f260b-139">Болжамдар</span><span class="sxs-lookup"><span data-stu-id="f260b-139">Estimates</span></span>

<span data-ttu-id="f260b-140">Жоба көшірілген кезде, ресурстар мен шығыстар болжамының жолдары бастапқы жобадан көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="f260b-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="f260b-141">Copy Project бағдарламасына бағдарламалы түрде қатынасу жолы туралы ақпаратты [ Copy Project көмегімен жоба үлгілерін жасау](dev-copy-project.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="f260b-141">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
