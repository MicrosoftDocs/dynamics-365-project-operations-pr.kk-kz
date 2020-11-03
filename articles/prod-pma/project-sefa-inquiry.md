---
title: Федералдық марапаттарға сұраныс беру шығындарының кестесі
description: Бұл тақырыпта Федералдық марапаттарға сұраныс беру шығындарының кестесі туралы ақпарат берілген.
author: velofog
manager: Ann Beebe
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: eaf523ab147cbe974fed6e7eab21967404583fe6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079644"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="f80f8-103">Федералдық марапаттарға сұраныс беру шығындарының кестесі</span><span class="sxs-lookup"><span data-stu-id="f80f8-103">Schedule of Expenditures of Federal Awards inquiry</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="f80f8-104">Басқарма және A-133 бюджет айналымына сәйкес федералды қаражат алатын мекемелер тексеру талаптарына тәуелді, ол бірыңғай тексерулер деп те аталады.</span><span class="sxs-lookup"><span data-stu-id="f80f8-104">According to Office of Management and Budget Circular A-133, agencies that receive federal funds are subject to audit requirements, which are also known as single audits.</span></span> <span data-ttu-id="f80f8-105">Тексеру процесі федералды гранттардың кірістері мен шығыстары туралы есеп беру үшін қайталанатын негізде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="f80f8-105">The audit process is used to report on the revenues and expenditures of federal grants on a recurring basis.</span></span> <span data-ttu-id="f80f8-106">Бірыңғай тексеру есебінің бір бөлігі Федералды марапаттардың шығындар кестесін (SEFA) қамтиды.</span><span class="sxs-lookup"><span data-stu-id="f80f8-106">Part of the single audit report includes the Schedule of Expenditures of Federal Awards (SEFA).</span></span>

<span data-ttu-id="f80f8-107">Федералдық марапаттарға сұраныс беру шығындарының кестесіне Федералдық ішкі көмек каталогы (CFDA) атауы мен нөмірі, грант нөмірі, грант берілген жыл, қаражат беретін федералдық агенттіктің атауы және транзиттік нысанның атауы кіреді.</span><span class="sxs-lookup"><span data-stu-id="f80f8-107">The Schedule of Expenditures of Federal Awards inquiry includes the Catalog of Federal Domestic Assistance (CFDA) title and number, the grant number, the year of the grant, the name of the federal agency that provides the funds, and the name of the pass-through entity.</span></span> <span data-ttu-id="f80f8-108">Сұраныс белгілі бір мерзімге арналған.</span><span class="sxs-lookup"><span data-stu-id="f80f8-108">The inquiry is for a specific period.</span></span> <span data-ttu-id="f80f8-109">Әдетте, бұл кезең қаржы жылы болып табылатын қаржылық есептілік кезеңімен бірдей.</span><span class="sxs-lookup"><span data-stu-id="f80f8-109">Typically, that period is the same as the financial statement period, which is a fiscal year.</span></span>

<span data-ttu-id="f80f8-110">Сұраныс таңдалған күндер аралығында жобалау күндеріне ие гранттарды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="f80f8-110">The inquiry includes grants that have projection dates in the selected date range.</span></span> <span data-ttu-id="f80f8-111">Сұраныстың **Грант беруші агенттік** бағанында грант тұтынушысы немесе транзиттік грант үшін грант беруші агенттік көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="f80f8-111">The **Grantor agency** column of the inquiry shows the grant customer or, for a pass-through grant, the grantor agency.</span></span> <span data-ttu-id="f80f8-112">Транзиттік грант үшін **Транзиттік агенттік** бағанында грант тұтынушысы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="f80f8-112">For a pass-through grant, the **Pass-through agency** column shows the grant customer.</span></span> <span data-ttu-id="f80f8-113">Грант транзиттік грант болмаса, **Транзиттік агенттік** бағаны бос болады.</span><span class="sxs-lookup"><span data-stu-id="f80f8-113">If the grant isn't a pass-through grant, the **Pass-through agency** column is blank.</span></span>

## <a name="set-up-the-cfda-clusters"></a><span data-ttu-id="f80f8-114">CFDA кластерлерін орнату</span><span class="sxs-lookup"><span data-stu-id="f80f8-114">Set up the CFDA clusters</span></span>

<span data-ttu-id="f80f8-115">Федералдық марапаттарға сұраныс беру шығындарының кестесінде CFDA нөмірлерімен байланыстыруға болатын CFDA кластерлерін құру керек.</span><span class="sxs-lookup"><span data-stu-id="f80f8-115">You must set up the CFDA clusters that can be associated with CFDA numbers in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="f80f8-116">**Жобаларды басқару және есепке алу \> Орнату \> Гранттар \> Федералдық ішкі көмек каталогының кластерлері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-116">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance clusters**.</span></span>
2. <span data-ttu-id="f80f8-117">CFDA кластерін жасау үшін **Жаңа** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-117">Select **New** to create a CFDA cluster.</span></span>
3. <span data-ttu-id="f80f8-118">Кластер атауын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-118">Enter the cluster name.</span></span>
4. <span data-ttu-id="f80f8-119">Өзгерістерді сақтау үшін **Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-119">Select **Save** to save your changes.</span></span>

## <a name="set-up-cfda-numbers"></a><span data-ttu-id="f80f8-120">CFDA нөмірлерін орнату</span><span class="sxs-lookup"><span data-stu-id="f80f8-120">Set up CFDA numbers</span></span>

<span data-ttu-id="f80f8-121">Гранттарға және Федералдық марапаттарға сұраныс беру шығындарының кестесіне қосуға болатын CFDA нөмірлерін құру керек.</span><span class="sxs-lookup"><span data-stu-id="f80f8-121">You must set up CFDA numbers that can be added to grants and included in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="f80f8-122">**Жобаларды басқару және есепке алу \> Орнату \> Гранттар \> Федералдық ішкі көмек каталогының нөмірлері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-122">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance numbers**.</span></span>
2. <span data-ttu-id="f80f8-123">CFDA нөмірін жасау үшін **Жаңа** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-123">Select **New** to create a CFDA number.</span></span>
3. <span data-ttu-id="f80f8-124">**Сан** бағанында CFDA нөмірін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-124">In the **Number** column, enter the CFDA number.</span></span>
4. <span data-ttu-id="f80f8-125">**Tab** пернесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-125">Press the **Tab** key.</span></span>
5. <span data-ttu-id="f80f8-126">**Сипаттама** бағанында CFDA тақырыбын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-126">In the **Description** column, enter the CFDA title.</span></span>
6. <span data-ttu-id="f80f8-127">**Tab** пернесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-127">Press the **Tab** key.</span></span>
7. <span data-ttu-id="f80f8-128">Қосымша: **Бағдарлама кластері** өрісіне тиісті CFDA кластерін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-128">Optional: In the **Program cluster** field, add the appropriate CFDA cluster.</span></span>
8. <span data-ttu-id="f80f8-129">Өзгерістерді сақтау үшін **Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-129">Select **Save** to save your changes.</span></span>

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="f80f8-130">Федералдық марапаттарға сұраныс беру шығындарының кестесіне есеп беру үшін гранттар құру</span><span class="sxs-lookup"><span data-stu-id="f80f8-130">Set up grants to report for the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="f80f8-131">**Жобаларды басқару және есепке алу \> Гранттар \> Гранттар** тармағына өтіп, бұрыннан бар грантты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-131">Go to **Project management and accounting \> Grants \> Grants** , and select an existing grant.</span></span>
2. <span data-ttu-id="f80f8-132">**Орнату** FastTab қойыншасындағы **Федералды ішкі көмек каталогы** өрісіне CFDA нөмірін тағайындаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-132">On the **Setup** FastTab, in the  **Catalog of Federal Domestic Assistance** field, assign the CFDA number.</span></span> <span data-ttu-id="f80f8-133">Гранттағы CFDA нөмірі есеп беруге арналған CFDA кластерін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="f80f8-133">The CFDA number on the grant determines the CFDA cluster for reporting.</span></span>
3. <span data-ttu-id="f80f8-134">**Байланыс ақпараты** FastTab қойыншасында грант беруші туралы ақпаратты мына қадамдарды орындау арқылы енгізіңіз:</span><span class="sxs-lookup"><span data-stu-id="f80f8-134">On **Contact information** FastTab, enter the grantor information by following these steps:</span></span>

    1. <span data-ttu-id="f80f8-135">**Грант тұтынушысы** өрісіне грант үшін жауапты тұтынушыны енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-135">In the **Grant customer** field, enter the customer who is responsible for the grant.</span></span> <span data-ttu-id="f80f8-136">Бұрыннан бар грант үшін бұл ақпарат енгізілген болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f80f8-136">For an existing grant, this information might already be entered.</span></span>
    2. <span data-ttu-id="f80f8-137">Грант тұтынушысы қаржыландырушы болып табылатынын көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-137">Indicate whether the grant customer is the funder.</span></span> <span data-ttu-id="f80f8-138">Егер грант тұтынушысы қаржыландырушы болса, **Транзиттік** ұяшығын бос қалдырыңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-138">If the grant customer is the funder, leave the **Pass-through** check box cleared.</span></span> <span data-ttu-id="f80f8-139">Егер басқа тұтынушы қаржыландырушы болса, ал грант тұтынушысы ақшаны жұмсауға және қадағалауға жауапты болса, **Транзиттік** ұяшығына құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-139">If another customer is the funder, and the grant customer is responsible for spending and tracking the money, select the **Pass-through** check box.</span></span>

4. <span data-ttu-id="f80f8-140">Алдыңғы қадамда **Транзиттік** ұяшығына құсбелгі қойсаңыз, **Грант беруші агенттік** өрісіне грант ұсынған тұтынушыны енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-140">If you selected the **Pass-through** check box in the previous step, in the **Grantor agency** field, enter the customer who provided the grant.</span></span> <span data-ttu-id="f80f8-141">Грант беруші агенттік пен грант тұтынушысы бірдей тұтынушы бола алмайды.</span><span class="sxs-lookup"><span data-stu-id="f80f8-141">The grantor agency and the grant customer can't be the same customer.</span></span>

<span data-ttu-id="f80f8-142">Өтетін гранттың мысалы:</span><span class="sxs-lookup"><span data-stu-id="f80f8-142">Here is an example of a pass-through grant:</span></span>

<span data-ttu-id="f80f8-143">Федералдық үкімет мемлекеттің инфрақұрылымдық жобасын қаржыландырды.</span><span class="sxs-lookup"><span data-stu-id="f80f8-143">The federal government funded an infrastructure project for a state.</span></span> <span data-ttu-id="f80f8-144">Федералдық үкімет ақшаны мемлекетке жұмсауға берді.</span><span class="sxs-lookup"><span data-stu-id="f80f8-144">The federal government gave the money to the state to spend.</span></span> <span data-ttu-id="f80f8-145">Бұл жағдайда, федералдық үкімет – грант беруші агенттік, ал мемлекет – грант тұтынушысы.</span><span class="sxs-lookup"><span data-stu-id="f80f8-145">In this case, the federal government is the grantor agency, and the state is the grant customer.</span></span>

> [!NOTE] 
> <span data-ttu-id="f80f8-146">Мүмкіндікті алғаш қосқан кезде бастапқы CFDA нөмірлері гранттардағы бұрыннан бар нөмірлер көмегімен енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="f80f8-146">When you first turn on the feature, initial CFDA numbers will be entered by using the existing numbers on grants.</span></span>

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a><span data-ttu-id="f80f8-147">Грант түріне негізделген SEFA есептілігінен гранттарды шығару</span><span class="sxs-lookup"><span data-stu-id="f80f8-147">Exclude grants from SEFA reporting based on the grant type</span></span>

1. <span data-ttu-id="f80f8-148"> **Жобаны басқару және есепке алу \> Орнату \> Гранттар \> Грант түрлері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-148">Go to **Project management and accounting \> Setup \> Grants \> Grant types**.</span></span>
2. <span data-ttu-id="f80f8-149"> **Әдепкі ақпарат** FastTab қойыншасында **Федералдық марапаттардың шығындар кестесінен шығару** құсбелгісін қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-149">On the **Default information** FastTab, select the **Exclude from Schedule of Expenditures of Federal Awards** check box.</span></span>
3. <span data-ttu-id="f80f8-150">Өзгерістерді сақтау үшін **Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-150">Select **Save** to save your changes.</span></span>

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="f80f8-151">Федералдық марапаттарға сұраныс беру шығындарының кестесін жүргізу</span><span class="sxs-lookup"><span data-stu-id="f80f8-151">Run the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="f80f8-152">**Жобаларды басқару және есепке алу \> Сұраулар мен есептер \> Грантқа сұраныс беру \> Федералдық марапаттарға сұраныс беру кестесі** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-152">Go to **Project management and accounting \> Inquiries and reports \> Grant inquiry \> Schedule of Expenditures of Federal Awards**.</span></span>
2. <span data-ttu-id="f80f8-153">**Параметрлер** бөлімінде мына қадамдарды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="f80f8-153">In the **Parameters** section, follow these steps:</span></span>

    1. <span data-ttu-id="f80f8-154">**Күн аралығы** өрісінде күн аралығы үшін кодты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-154">In the **Date interval** field, select the code for the date interval.</span></span> <span data-ttu-id="f80f8-155">Сонымен қатар, **Басталу күні** және **Аяқталу күні** өрістерінде күн аралығын анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-155">Alternatively, in the **From date** and **To date** fields, define the date interval.</span></span>
    2. <span data-ttu-id="f80f8-156">Қосымша: сұранысқа табыс ретінде тек шот ұсынылған транзакцияларды қосу үшін **Шот ұсынылған табыстарды ғана қосу** опциясын **Иә** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="f80f8-156">Optional: To include only billed transactions as revenue in the inquiry, set the **Include only billed revenues** option to **Yes**.</span></span>

## <a name="columns"></a><span data-ttu-id="f80f8-157">Бағандар</span><span class="sxs-lookup"><span data-stu-id="f80f8-157">Columns</span></span>

<span data-ttu-id="f80f8-158">Федералдық марапаттарға сұраныс беру кестесіне келесі бағандар кіреді:</span><span class="sxs-lookup"><span data-stu-id="f80f8-158">The Schedule of Expenditures of Federal Awards inquiry includes the following columns:</span></span>

- <span data-ttu-id="f80f8-159">Федералдық ішкі көмек каталогы кластерінің атауы</span><span class="sxs-lookup"><span data-stu-id="f80f8-159">Catalog of Federal Domestic Assistance cluster name</span></span>
- <span data-ttu-id="f80f8-160">Грант беруші агенттік</span><span class="sxs-lookup"><span data-stu-id="f80f8-160">Grantor agency</span></span>
- <span data-ttu-id="f80f8-161">Транзиттік агенттік</span><span class="sxs-lookup"><span data-stu-id="f80f8-161">Pass-through agency</span></span>
- <span data-ttu-id="f80f8-162">Грант атауы</span><span class="sxs-lookup"><span data-stu-id="f80f8-162">Grant name</span></span>
- <span data-ttu-id="f80f8-163">Грант идентификаторы</span><span class="sxs-lookup"><span data-stu-id="f80f8-163">Grant ID</span></span>
- <span data-ttu-id="f80f8-164">Грант өтінімінің идентификаторы</span><span class="sxs-lookup"><span data-stu-id="f80f8-164">Grant application ID</span></span>
- <span data-ttu-id="f80f8-165">Федералдық ішкі көмек каталогы</span><span class="sxs-lookup"><span data-stu-id="f80f8-165">Catalog of Federal Domestic Assistance</span></span>
- <span data-ttu-id="f80f8-166">Түсімдер</span><span class="sxs-lookup"><span data-stu-id="f80f8-166">Receipts</span></span>
- <span data-ttu-id="f80f8-167">Шығындар</span><span class="sxs-lookup"><span data-stu-id="f80f8-167">Expenditures</span></span>
