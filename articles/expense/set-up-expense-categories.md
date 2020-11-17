---
title: Шығыс санаттарын орнату
description: Бұл тақырып шығыстар санаттарын және шығындар туралы есептер үшін ортақ санаттарды жасау жолдары туралы ақпарат береді.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 13e72e4b852fd0edac5ad35d5162e74b016bce33
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123790"
---
# <a name="set-up-expense-categories"></a><span data-ttu-id="be0de-103">Шығыс санаттарын орнату</span><span class="sxs-lookup"><span data-stu-id="be0de-103">Set up expense categories</span></span>

<span data-ttu-id="be0de-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="be0de-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="be0de-105">Қызметкерлер шығындар туралы есептер жасаған кезде, олар жазған әрбір шығын шығындар санатымен байланысты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="be0de-105">When employees create expense reports, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="be0de-106">Шығыстар санаттары ұйымыңыздағы нысандармен ортақ пайдалануға болатын ортақ санаттардан алынады.</span><span class="sxs-lookup"><span data-stu-id="be0de-106">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="be0de-107">Ұйымыңыздың анықталу жолына байланысты, бұл шығындар санаттарын басқа салаларда да ортақ пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="be0de-107">Depending on how your organization is defined, these expense categories can also be shared in other areas.</span></span> <span data-ttu-id="be0de-108">Ұйымыңыздың анықтамасы мен іске асыру тобының басшылығына сүйене отырып, сіз шығыстарды басқаруда пайдаланылатын санаттар тек шығыстарды басқаруда пайдаланылатындығын немесе басқа салаларда ортақ пайдалануға болатындығын анықтауы керек.</span><span class="sxs-lookup"><span data-stu-id="be0de-108">Based on the definition of your organization and guidance from the implementation team, you must determine whether the categories that are used in Expense management will be used only in Expense management or should be shared in other areas.</span></span>

> [!NOTE]
> <span data-ttu-id="be0de-109">Бұл санаттар жобаны басқару және бухгалтерлік есеп пен шығыстарды басқару арасында немесе жобаны басқару мен есеп және өндіріс арасында ортақ пайдаланылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="be0de-109">These categories can be shared between Project management and accounting and Expense management, or between Project management and accounting and Production.</span></span> <span data-ttu-id="be0de-110">Алайда, оларды шығыстарды басқару және өндіріс арасында ортақ пайдалану мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="be0de-110">However, they can't be shared between Expense management and Production.</span></span>

<span data-ttu-id="be0de-111">Орнату процесін бастамас бұрын, шығындардың әр санаты үшін келесі шешімдер қабылдануы керек:</span><span class="sxs-lookup"><span data-stu-id="be0de-111">Before you can begin the setup process, the following decisions must be made for each expense category:</span></span>

- <span data-ttu-id="be0de-112">Шығыс санаты дегеніміз не?</span><span class="sxs-lookup"><span data-stu-id="be0de-112">What is the expense category?</span></span> <span data-ttu-id="be0de-113">Мысал ретінде рейстерге, қонақ үйге немесе жүгіруге арналған санаттарды алуға болады.</span><span class="sxs-lookup"><span data-stu-id="be0de-113">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="be0de-114">Шығындар санатын жобаны басқару және есепке алу кезінде де пайдалануға бола ма?</span><span class="sxs-lookup"><span data-stu-id="be0de-114">Can the expense category also be used in Project management and accounting?</span></span> <span data-ttu-id="be0de-115">Егер болса, сонымен қатар мына шешімдерді жасауыңыз керек:</span><span class="sxs-lookup"><span data-stu-id="be0de-115">If it can, you must also make the following decisions:</span></span>

    - <span data-ttu-id="be0de-116">Келесі шығындар үшін қандай шығындар есептері пайдаланылады?</span><span class="sxs-lookup"><span data-stu-id="be0de-116">Which cost accounts will be used for the following expenses?</span></span>

        - <span data-ttu-id="be0de-117">Құны</span><span class="sxs-lookup"><span data-stu-id="be0de-117">Cost</span></span>
        - <span data-ttu-id="be0de-118">Жалақы бөлу</span><span class="sxs-lookup"><span data-stu-id="be0de-118">Payroll allocation</span></span>
        - <span data-ttu-id="be0de-119">WIP-шығын мәні</span><span class="sxs-lookup"><span data-stu-id="be0de-119">WIP-cost value</span></span>
        - <span data-ttu-id="be0de-120">Шығындар-элемент</span><span class="sxs-lookup"><span data-stu-id="be0de-120">Cost-item</span></span>
        - <span data-ttu-id="be0de-121">WIP-шығын құнының элементі</span><span class="sxs-lookup"><span data-stu-id="be0de-121">WIP-cost value-item</span></span>
        - <span data-ttu-id="be0de-122">Есептелген шығын</span><span class="sxs-lookup"><span data-stu-id="be0de-122">Accrued loss</span></span>
        - <span data-ttu-id="be0de-123">WIP-есептелген шығын</span><span class="sxs-lookup"><span data-stu-id="be0de-123">WIP-accrued loss</span></span>

    - <span data-ttu-id="be0de-124">Келесі кіріс көздері үшін қандай кірістер есептері пайдаланылады?</span><span class="sxs-lookup"><span data-stu-id="be0de-124">Which revenue accounts will be used for the following sources of revenue?</span></span>

        - <span data-ttu-id="be0de-125">Шот-фактура бойынша табыс</span><span class="sxs-lookup"><span data-stu-id="be0de-125">Invoiced revenue</span></span>
        - <span data-ttu-id="be0de-126">Есептелген табыс-сатылым құны</span><span class="sxs-lookup"><span data-stu-id="be0de-126">Accrued revenue-sales value</span></span>
        - <span data-ttu-id="be0de-127">WIP-сату құны</span><span class="sxs-lookup"><span data-stu-id="be0de-127">WIP-sales value</span></span>
        - <span data-ttu-id="be0de-128">Есептелген кіріс-өндіріс</span><span class="sxs-lookup"><span data-stu-id="be0de-128">Accrued revenue-production</span></span>
        - <span data-ttu-id="be0de-129">WIP-өндіріс</span><span class="sxs-lookup"><span data-stu-id="be0de-129">WIP-production</span></span>
        - <span data-ttu-id="be0de-130">Есептелген кіріс-пайда</span><span class="sxs-lookup"><span data-stu-id="be0de-130">Accrued revenue-profit</span></span>
        - <span data-ttu-id="be0de-131">WIP-пайда</span><span class="sxs-lookup"><span data-stu-id="be0de-131">WIP-profit</span></span>
        - <span data-ttu-id="be0de-132">Есептелген кіріс-жазылым</span><span class="sxs-lookup"><span data-stu-id="be0de-132">Accrued revenue-subscription</span></span>
        - <span data-ttu-id="be0de-133">WIP-жазылым</span><span class="sxs-lookup"><span data-stu-id="be0de-133">WIP-subscription</span></span>

- <span data-ttu-id="be0de-134">Шығыс түрі дегеніміз не?</span><span class="sxs-lookup"><span data-stu-id="be0de-134">What is the expense type?</span></span>
- <span data-ttu-id="be0de-135">Шығындар санаты үшін төлеудің әдепкі әдісі қандай?</span><span class="sxs-lookup"><span data-stu-id="be0de-135">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="be0de-136">Шығындар санатындағы шығындарды бөлу керек пе?</span><span class="sxs-lookup"><span data-stu-id="be0de-136">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="be0de-137">Шығындар санаты үшін негізгі әдепкі есеп қандай?</span><span class="sxs-lookup"><span data-stu-id="be0de-137">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="be0de-138">Шығындар санаты бойынша сатудан алынатын салық тобы қандай болады?</span><span class="sxs-lookup"><span data-stu-id="be0de-138">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="be0de-139">Шығындар санаты үшін қосымша төлем әдістеріне жол беріле ме?</span><span class="sxs-lookup"><span data-stu-id="be0de-139">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="be0de-140">Егер солай болса, олар қандай?</span><span class="sxs-lookup"><span data-stu-id="be0de-140">If so, what are they?</span></span>
- <span data-ttu-id="be0de-141">Бұл шығыстар санатында ішкі санаттар бар ма?</span><span class="sxs-lookup"><span data-stu-id="be0de-141">Are there subcategories in this expense category?</span></span> <span data-ttu-id="be0de-142">Егер ішкі санаттар болса, сонымен қатар мына шешімдерді жасауыңыз керек:</span><span class="sxs-lookup"><span data-stu-id="be0de-142">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="be0de-143">Ішкі санаттардың біреуі салықты қалпына келтіруден шығарылған ба?</span><span class="sxs-lookup"><span data-stu-id="be0de-143">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="be0de-144">Ішкі санаттардың сатылым салығының тобы қандай?</span><span class="sxs-lookup"><span data-stu-id="be0de-144">What is the item sales tax group of the subcategories?</span></span>
