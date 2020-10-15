---
title: Жобаны көшіру
description: Бұл тақырыпта Dynamics 365 Project Operations жобаларын көшіру туралы ақпарат берілген.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: e35dc725e7938e9f59f7151dd1b37500fabf77a4
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908319"
---
# <a name="copy-a-project"></a><span data-ttu-id="f64cb-103">Жобаны көшіру</span><span class="sxs-lookup"><span data-stu-id="f64cb-103">Copy a project</span></span>

<span data-ttu-id="f64cb-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="f64cb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f64cb-105">Dynamics 365 Project Operations көмегімен **Жобалар** пішініндегі **Жобаны көшіру** әрекетін пайдалану арқылы жаңа жобалар жылдам жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="f64cb-105">With Dynamics 365 Project Operations, you can quickly build new projects by using the **Copy Project** action on the **Projects** from.</span></span> <span data-ttu-id="f64cb-106">Жобаны көшіру үшін жобаны таңдап, **Көшіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f64cb-106">To copy a project, select a project, and then select **Copy**.</span></span> <span data-ttu-id="f64cb-107">Әрекет келесіні көшіреді:</span><span class="sxs-lookup"><span data-stu-id="f64cb-107">The action will copy:</span></span>

- <span data-ttu-id="f64cb-108">Жоба сипаттары</span><span class="sxs-lookup"><span data-stu-id="f64cb-108">Project properties</span></span>
- <span data-ttu-id="f64cb-109">Жұмыс декомпозициясының құрылымы</span><span class="sxs-lookup"><span data-stu-id="f64cb-109">The Work breakdown structure</span></span>
- <span data-ttu-id="f64cb-110">Жоба тобы мүшелері</span><span class="sxs-lookup"><span data-stu-id="f64cb-110">Project team members</span></span>
- <span data-ttu-id="f64cb-111">Жоба болжамдары</span><span class="sxs-lookup"><span data-stu-id="f64cb-111">Project estimates</span></span>
- <span data-ttu-id="f64cb-112">Жобаның шығыс болжамдары</span><span class="sxs-lookup"><span data-stu-id="f64cb-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="f64cb-113">Жоба сипаттары</span><span class="sxs-lookup"><span data-stu-id="f64cb-113">Project properties</span></span>

<span data-ttu-id="f64cb-114">Жоба көшірілген кезде, келесі өрістердегі мәндер көшіріледі:</span><span class="sxs-lookup"><span data-stu-id="f64cb-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="f64cb-115">Атауы</span><span class="sxs-lookup"><span data-stu-id="f64cb-115">Name</span></span>
- <span data-ttu-id="f64cb-116">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="f64cb-116">Description</span></span>
- <span data-ttu-id="f64cb-117">Тұтынушы</span><span class="sxs-lookup"><span data-stu-id="f64cb-117">Customer</span></span>
- <span data-ttu-id="f64cb-118">Күнтізбе үлгісі</span><span class="sxs-lookup"><span data-stu-id="f64cb-118">Calendar Template</span></span>
- <span data-ttu-id="f64cb-119">Валюта</span><span class="sxs-lookup"><span data-stu-id="f64cb-119">Currency</span></span>
- <span data-ttu-id="f64cb-120">Келісім-шарт бірлігі</span><span class="sxs-lookup"><span data-stu-id="f64cb-120">Contracting Unit</span></span>
- <span data-ttu-id="f64cb-121">Жоба менеджері</span><span class="sxs-lookup"><span data-stu-id="f64cb-121">Project Manager</span></span>
- <span data-ttu-id="f64cb-122">Күй</span><span class="sxs-lookup"><span data-stu-id="f64cb-122">Status</span></span>
- <span data-ttu-id="f64cb-123">Жалпы жоба күйі</span><span class="sxs-lookup"><span data-stu-id="f64cb-123">Overall Project Status</span></span>
- <span data-ttu-id="f64cb-124">Комментарийлер</span><span class="sxs-lookup"><span data-stu-id="f64cb-124">Comments</span></span>
- <span data-ttu-id="f64cb-125">Болжамдар</span><span class="sxs-lookup"><span data-stu-id="f64cb-125">Estimates</span></span>
- <span data-ttu-id="f64cb-126">Болжалды басталу күні</span><span class="sxs-lookup"><span data-stu-id="f64cb-126">Estimated Start Date</span></span>
- <span data-ttu-id="f64cb-127">Аяқталу күні</span><span class="sxs-lookup"><span data-stu-id="f64cb-127">Finish Date</span></span>
- <span data-ttu-id="f64cb-128">Талпыныс (сағаттар)</span><span class="sxs-lookup"><span data-stu-id="f64cb-128">Effort (Hours)</span></span>
- <span data-ttu-id="f64cb-129">Болжалды еңбек құны</span><span class="sxs-lookup"><span data-stu-id="f64cb-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="f64cb-130">Болжалды шығын</span><span class="sxs-lookup"><span data-stu-id="f64cb-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="f64cb-131">Жұмыс декомпозициясының құрылымы</span><span class="sxs-lookup"><span data-stu-id="f64cb-131">Work breakdown structure</span></span>

<span data-ttu-id="f64cb-132">Жоба көшірілген кезде, ресурсы жүктелген жұмыс декомпозициясының құрылымы көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="f64cb-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="f64cb-133">Аталған ресурстар жалпы ресурстармен алмастырылады.</span><span class="sxs-lookup"><span data-stu-id="f64cb-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="f64cb-134">Егер аталған ресурстар жалпы жұмыс сағатымен бірдей болмаса, кесте қайта есептеледі және тапсырманың ұзақтығы өзгеруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f64cb-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="f64cb-135">Жоба тобы мүшелері</span><span class="sxs-lookup"><span data-stu-id="f64cb-135">Project team members</span></span>

<span data-ttu-id="f64cb-136">Жоба тобы бастапқы жобадан көшірілген кезде жалпы ресурстар көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="f64cb-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="f64cb-137">Әмбебап ресурс тағайындаулары да бастапқы жобадағы күйде сақталады.</span><span class="sxs-lookup"><span data-stu-id="f64cb-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="f64cb-138">Аталған ресурстар жалпы топ мүшелеріне айналады.</span><span class="sxs-lookup"><span data-stu-id="f64cb-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="f64cb-139">Болжамдар</span><span class="sxs-lookup"><span data-stu-id="f64cb-139">Estimates</span></span>

<span data-ttu-id="f64cb-140">Жоба көшірілген кезде, ресурстар мен шығыстар болжамының жолдары бастапқы жобадан көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="f64cb-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span>