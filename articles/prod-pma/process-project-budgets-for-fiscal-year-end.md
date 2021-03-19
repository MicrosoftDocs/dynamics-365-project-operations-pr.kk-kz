---
title: Жоба бюджеттерін қаржы жылының соңына тасымалдау
description: Бұл мақалада қалған бюджеттік сомаларды алдағы жылдарға қалай ауыстыру және бюджет регистрі туралы мәліметтерді жасау туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 03/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 1f601be072e84fc04246cd55a260c8004f6fb3e5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289736"
---
# <a name="transfer-project-budgets-at-fiscal-year-end"></a><span data-ttu-id="8eba8-103">Жоба бюджеттерін қаржы жылының соңына тасымалдау</span><span class="sxs-lookup"><span data-stu-id="8eba8-103">Transfer project budgets at fiscal year end</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="8eba8-104">Көп жылдық жобамен жұмыс істеген кезде сізде қаржы жылының соңына дейін бюджет қалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8eba8-104">When working on a multi-year project, you might have remaining budget at the end of the fiscal year.</span></span> <span data-ttu-id="8eba8-105">Бюджеттің қалған сомаларын келесі жылға ауыстыруға және бас кітаптың байланысқан шоттарындағы сомалар үшін бюджетті тіркеу туралы ақпарат жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="8eba8-105">You can transfer the remaining budget amounts to a future year, and create budget register details for the amounts in the associated general ledger accounts.</span></span> <span data-ttu-id="8eba8-106">Қалған сомаларды жібермес бұрын, бюджеттің қалған сомаларын қарап шығыңыз және талдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-106">Before you carry forward the remaining amounts, review and analyze the remaining budget amounts.</span></span>

## <a name="review-and-analyze-remaining-budget-amounts"></a><span data-ttu-id="8eba8-107">Бюджеттің қалған сомаларын қарастырыңыз және талдаңыз</span><span class="sxs-lookup"><span data-stu-id="8eba8-107">Review and analyze remaining budget amounts</span></span>

<span data-ttu-id="8eba8-108">Жобалар үшін жылдың соңындағы бюджет сомасын қарау үшін келесі қадамдарды орындаңыз, бірақ оларды аудармаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-108">Complete the following steps to review the year-end budget amounts for projects, but not carry the amounts forward.</span></span>

1. <span data-ttu-id="8eba8-109">**Жобаларды басқару және бухгалтерлік есеп** > **Мерзімді** > **Бюджеттер** > **Бюджеттерді аудару** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-109">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="8eba8-110">**Жоба бюджетін басқа бетке ауыстыру процесі** бетінде **Жыл соңындағы опциялар** қойыншасында **Жоба бюджетінің қалған сомаларын аудару** параметрінің қосылмағанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-110">On the **Project budget carry-forward process** page, on the **Year-end options** tab, verify that **Carry forward remaining project budget amounts** is not enabled.</span></span>
3. <span data-ttu-id="8eba8-111">**Параметрлер** қойыншасындағы **Жобаның бюджеттік жылы** өрісінде бюджеттің қалған сомасын көргіңіз келетін қаржы жылын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-111">On the **Parameters** tab, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
4. <span data-ttu-id="8eba8-112">**Ашылатын қаржы жылы** өрісінде бюджеттің қалған сомасын көргіңіз келетін қаржы жылын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-112">In the **Opening fiscal year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
5. <span data-ttu-id="8eba8-113">**Болжау үлгісінен** өрісінде **Қалған бюджет** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-113">In the **From forecast model** field, select **Remaining budget**.</span></span> 
6. <span data-ttu-id="8eba8-114">Таңдалған шарттарға сәйкес келетін және қалған бюджеті жоқ жобаларды қосу үшін **Нөлдік қалған соманы көрсету** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-114">To include projects that meet your selected criteria and have no remaining budget, select **Show zero remaining**.</span></span>  
7. <span data-ttu-id="8eba8-115">**Бюджеттерді таңдау** қойыншасында таңдалған шарттарға сәйкес келетін барлық бюджеттерді жүктеу үшін **Барлық бюджеттерді алу** параметрін таңдап, содан соң **Өңдеу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-115">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match your selected criteria, and then select **Process**.</span></span> 
8. <span data-ttu-id="8eba8-116">Белгілі бір бюджеттер жиынтығын панельге жүктейтін дерекқор сұрауын жасау үшін **Таңдалған бюджеттерді алу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-116">To design a database query that loads a specific set of budgets into the pane, select **Retrieve selected budgets**.</span></span>

<span data-ttu-id="8eba8-117">Тақтадағы белгілі бір жол туралы қосымша ақпарат алу үшін жолды таңдап, **Бюджет мәліметтерін қарау** немесе **Шоттарды қарау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-117">For more information about a specific line in the pane, select the line, and then select **View budget details** or **View accounts**.</span></span>

## <a name="carry-forward-remaining-budget-amounts"></a><span data-ttu-id="8eba8-118">Бюджеттің қалған сомаларын аударыңыз</span><span class="sxs-lookup"><span data-stu-id="8eba8-118">Carry forward remaining budget amounts</span></span> 

<span data-ttu-id="8eba8-119">Бюджеттің қалған сомаларын өңдеген кезде сіз бас кітапта өзіңіз жүргізетін сомалар бойынша операциялар жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-119">When you process remaining budget amounts, you can create transactions in the general ledger for the amounts that you are carrying forward.</span></span> <span data-ttu-id="8eba8-120">Бас кітап операцияларын жасау үшін [Бюджеттік сомаларды аудару және бас кітап операцияларын жасау](#carry-forward) бөліміндегі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-120">To create general ledger transactions, complete the steps in the section, [Carry forward budget amounts and create general ledger transactions](#carry-forward).</span></span> 

> [!NOTE]
> <span data-ttu-id="8eba8-121">Аударылған бюджеттік сомалар аударуды болжау үлгісі ретінде **Болжамды үлгілер** бетінде таңдалған болжамды үлгіге көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8eba8-121">Budget amounts that are carried forward are transferred to the forecast model that is selected in the **Forecast models** page as the carry-forward forecast model.</span></span>  

## <a name="carry-forward-budget-amounts-and-create-general-ledger-transactions"></a><a name="carry-forward"></a><span data-ttu-id="8eba8-122">Бюджет сомаларын аударыңыз және бас кітап операцияларын жасаңыз</span><span class="sxs-lookup"><span data-stu-id="8eba8-122">Carry forward budget amounts and create general ledger transactions</span></span>

1.  <span data-ttu-id="8eba8-123">**Жобаларды басқару және бухгалтерлік есеп** > **Мерзімді** > **Бюджеттер** > **Бюджеттерді аудару** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-123">Select **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="8eba8-124">**Жоба бюджетін аудару процесі** бетіде **Жыл соңы** параметрін таңдап, содан кейін **Жоба бюджетінің қалған сомаларын аудару** және **Бас кітаптағы бюджеттік тіркелім жазбаларын жасау** өрістерін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-124">On the **Project budget carry-forward process** page, select **Year-end**, and then enable **Carry forward remaining project budget amounts** and **Create budget register entries in general ledger**.</span></span> 
3. <span data-ttu-id="8eba8-125">**Параметрлер** қойыншасында, **Жоба параметрлері** өріс тобына келесілерді таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="8eba8-125">On the **Parameters** tab, in the **Project parameters** field group, select the following:</span></span>

   - <span data-ttu-id="8eba8-126">**Жобаның бюджеттік жылы**: Бюджеттің қалған сомаларын көргіңіз келетін қаржы жылының басын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-126">**Project budget year**: Select the beginning of the fiscal year for which you want to view the remaining budget amounts.</span></span> 
   - <span data-ttu-id="8eba8-127">**Пайда және шығын**: Бас кітапта пайда мен шығын операцияларын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-127">**Profit and loss**: Create profit and loss transactions in the general ledger.</span></span> 
   -  <span data-ttu-id="8eba8-128">**WIP**: Бас кітапта аяқталмаған жұмыс (WIP) операцияларын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-128">**WIP**: Create Work in Progress (WIP) transactions in the general ledger.</span></span>
   -  <span data-ttu-id="8eba8-129">**Жалақы**: Бас кітапта жалақы бөлу операцияларын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-129">**Payroll**: Create payroll allocation transactions in the general ledger.</span></span> 

5. <span data-ttu-id="8eba8-130">**Бас кітап** өріс тобында келесі ақпаратты қамтамасыз етіңіз:</span><span class="sxs-lookup"><span data-stu-id="8eba8-130">In the **General ledger** field group, provide the following information:</span></span> 

   - <span data-ttu-id="8eba8-131">**Ашылатын қаржы жылы** өрісінде бюджеттің қалған сомаларын жобаларға тасымалдағыңыз келетін қаржы жылын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-131">In the **Opening fiscal year** field, select the fiscal year that you want to transfer remaining budget amounts to for the projects.</span></span> <span data-ttu-id="8eba8-132">Әдепкі мәні - **Жобаның бюджеттік жылы** өрісіндегі мәннен бір жылдан кейін.</span><span class="sxs-lookup"><span data-stu-id="8eba8-132">The default value is one year after the value in the **Project budget year** field.</span></span>
   -  <span data-ttu-id="8eba8-133">**Аудару кезеңі** өрісінде бас кітапта бюджеттік тіркелім туралы мәліметтер жасағыңыз келетін кезеңді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-133">In the **Carry-forward period** field, select the period that you want to create the budget register details for in the general ledger.</span></span> <span data-ttu-id="8eba8-134">Әдетте бұл – ашылатын қаржы жылындағы алғашқы кезең.</span><span class="sxs-lookup"><span data-stu-id="8eba8-134">This is typically the first period in the opening fiscal year.</span></span>

6. <span data-ttu-id="8eba8-135">**Өрістен/өріске көшіру** өріс тобында келесі ақпаратты қамтамасыз етіңіз:</span><span class="sxs-lookup"><span data-stu-id="8eba8-135">In the **Copy from/to** field group, provide the following information:</span></span>

   - <span data-ttu-id="8eba8-136">**Болжау үлгісінен** өрісінде жобалар үшін аударғыңыз келетін бюджеттің қалған сомаларымен байланысты жоба бюджетін болжау үлгісін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-136">In the **From forecast model** field, select the project budget forecast model associated with the remaining budget amounts you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="8eba8-137">**Болжау үлгісінен** өрісінде бас кітапқа тасымалдағыңыз келетін бюджеттік сомалармен байланысты бас кітап бюджетінің үлгісін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-137">In the **To ledger budget model** field, select the ledger budget model associated with the budget amounts you want to transfer to the general ledger.</span></span> 
   -  <span data-ttu-id="8eba8-138">Жобаның бюджет сомасын аударған кезде жасалатын бас кітап операциялары үшін жобаның сатылым валютасын пайдалану үшін **Сатылым валютасын ауыстыру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-138">Select **Transfer sales currency** to use the project's sales currency for the general ledger transactions that are created when you transfer the budget amounts for the projects.</span></span> <span data-ttu-id="8eba8-139">Опцион таңдалмаған кезде, операциялар есеп валютасын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="8eba8-139">When the option is not selected, the transactions use the accounting currency.</span></span> 
   -  <span data-ttu-id="8eba8-140">Бюджеттің қалған сомасы жоқ, бірақ төменгі бөлікте көрсетілген жобаларда сіз таңдаған басқа шарттарға сәйкес келетін жобаларды қосу үшін **Нөлдік қалған соманы көрсету** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-140">Select **Show zero remaining** to include projects that have no remaining budget amounts, but meet the other criteria that you select in the projects displayed in the bottom pane.</span></span>

7. <span data-ttu-id="8eba8-141">**Бюджеттерді таңдау** қойыншасында таңдалған шарттарға сәйкес келетін барлық бюджеттерді жүктеу үшін **Барлық бюджеттерді алу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-141">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match the criteria you selected.</span></span> <span data-ttu-id="8eba8-142">Белгілі бір жобалық бюджеттер жиынтығын панельге жүктейтін дерекқор сұрауын жасағыңыз келсе, **Таңдалған бюджеттерді алу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-142">If you prefer to design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>
8. <span data-ttu-id="8eba8-143">Өңдегіңіз келетін әр жоба үшін жоба үшін жолдың басындағы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-143">For each project that you want to process, select the option at the beginning of the line for the project.</span></span>

    > [!TIP]
    > <span data-ttu-id="8eba8-144">Жобалардың барлығын немесе көпшілігін таңдау үшін жоғарғы сол жақ бұрыштағы құсбелгіні таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-144">To select all or most of the projects, select the check mark in the top upper-left corner.</span></span> <span data-ttu-id="8eba8-145">Кез келген жобаны өңдеуді болдырмау үшін, сол жобадан құсбелгіні алып тастаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-145">To exclude processing any project, clear the check mark for that project.</span></span>

9. <span data-ttu-id="8eba8-146">Таңдалған жобалар бойынша бюджеттің қалған сомаларын таңдалған қаржы жылына аудару және бас кітапта бюджеттік тіркелімнің мәліметтерін жасау үшін таңдаңыз **Өңдеу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-146">To transfer the remaining budget amounts for the selected projects to the selected fiscal year and create budget register details in the general ledger, select **Process**.</span></span>

## <a name="carry-forward-budget-amounts-without-creating-general-ledger-transactions"></a><span data-ttu-id="8eba8-147">Бас кітап операцияларын жасамай тұрып бюджеттік сомаларды аударыңыз</span><span class="sxs-lookup"><span data-stu-id="8eba8-147">Carry forward budget amounts without creating general ledger transactions</span></span>

1. <span data-ttu-id="8eba8-148">**Жобаларды басқару және бухгалтерлік есеп** > **Мерзімді** > **Бюджеттер** > **Бюджеттерді аудару** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-148">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span>
2. <span data-ttu-id="8eba8-149">**Жоба бюджетін басқа бетке ауыстыру процесі** бетінде **Жыл соңындағы опциялар** өрісінде **Жоба бюджетінің қалған сомаларын аудару** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-149">On the **Project budget carry-forward process** page, in the **Year-end options** field, select **Carry forward remaining project budget amounts**.</span></span>
3. <span data-ttu-id="8eba8-150">**Параметрлер** тобында, **Жобаның бюджеттік жылы** өрісінде бюджеттің қалған сомаларын көргіңіз келетін қаржы жылын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-150">In the **Parameters** group, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amounts.</span></span>
4. <span data-ttu-id="8eba8-151">**Өрістен/өріске көшіру** тобында келесі ақпаратты қамтамасыз етіңіз:</span><span class="sxs-lookup"><span data-stu-id="8eba8-151">In the **Copy from/to** group, provide the following information:</span></span>

   - <span data-ttu-id="8eba8-152">**Болжау үлгісінен** өрісінде жобалар үшін аударғыңыз келетін бюджеттің қалған сомаларымен байланысты жоба бюджетін болжау үлгісін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-152">In the **From forecast model** field, select the project budget forecast model that is associated with the remaining budget amounts that you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="8eba8-153">Қалған бюджеті жоқ, бірақ таңдалған шарттарға сәйкес келетін жобаларды қосу үшін **Нөлдік қалған соманы көрсету** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-153">Select **Show zero remaining** to include projects that have no remaining budget amounts, but that meet the other criteria you selected.</span></span>
   - <span data-ttu-id="8eba8-154">**Бюджеттерді таңдау** тобында таңдалған шарттарға сәйкес келетін барлық бюджеттерді жүктеу үшін **Барлық бюджеттерді алу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-154">In the **Select Budgets** group, select **Retrieve all budgets** to load all budgets that match the criteria that you selected.</span></span> <span data-ttu-id="8eba8-155">Белгілі бір жобалық бюджеттер жиынтығын панельге жүктейтін дерекқор сұрауын жасау үшін **Таңдалған бюджеттерді алу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-155">To design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>

5. <span data-ttu-id="8eba8-156">Өңдегіңіз келетін әр жоба үшін жоба үшін жолдың басындағы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-156">For each project that you want to process, select the option at the beginning of the line for the project.</span></span> 
6. <span data-ttu-id="8eba8-157">Таңдалған жобалар бойынша бюджеттің қалған сомаларын таңдалған қаржы жылына аудару үшін **Өңдеу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8eba8-157">Select **Process** to transfer the remaining budget amounts for the selected projects to the selected fiscal year.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]