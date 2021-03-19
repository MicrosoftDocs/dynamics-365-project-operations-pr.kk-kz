---
title: Бірлік топтары және бірліктер
description: Бұл тақырыпта бірлік топтары мен бірліктер туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 45e4a95b429cd9d1f174653bd28cf567f690676d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291626"
---
# <a name="unit-groups-and-units"></a><span data-ttu-id="ee1bc-103">Бірлік топтары және бірліктер</span><span class="sxs-lookup"><span data-stu-id="ee1bc-103">Unit groups and units</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ee1bc-104">Бірлік топтары мен бірліктер Microsoft Dynamics 365 бағдарламасының негізгі нысандары болып табылады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-104">Unit groups and units are basic entities in Microsoft Dynamics 365.</span></span> <span data-ttu-id="ee1bc-105">Бірлік — бұл өлшемнің бір бірлігі, ал бірнеше бірлікті бірлік топтарға топтастыруға болады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-105">A unit is a single unit of measure, and multiple units can be grouped into unit groups.</span></span> <span data-ttu-id="ee1bc-106">Бірлік тобы Dynamics 365 пайдаланушы интерфейсінде (UI) кейде бірлік кестесі деп те аталады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-106">A unit group is sometimes referred to as a unit schedule in the Dynamics 365 user interface (UI).</span></span> 

<span data-ttu-id="ee1bc-107">Бірліктер мен бірлік топтарының бірнеше мысалы:</span><span class="sxs-lookup"><span data-stu-id="ee1bc-107">Here are some examples of units and unit groups:</span></span>
 
- <span data-ttu-id="ee1bc-108">**Бірлік тобы**: Қашықтық</span><span class="sxs-lookup"><span data-stu-id="ee1bc-108">**Unit group**: Distance</span></span> 
    - <span data-ttu-id="ee1bc-109">**Бірліктер**: Миля, километр және т.б.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-109">**Units**: Mile, Kilometer, and so on.</span></span>
- <span data-ttu-id="ee1bc-110">**Бірлік тобы**: Уақыт</span><span class="sxs-lookup"><span data-stu-id="ee1bc-110">**Unit group**: Time</span></span>
    - <span data-ttu-id="ee1bc-111">**Бірліктер**: Сағат, күн, апта және т.б.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-111">**Units**: Hour, day, week, and so on.</span></span> 

<span data-ttu-id="ee1bc-112">Бірлік тобына бірнеше бірлікті орнатқан кезде, бірлік тобына әдепкі немесе бастапқы бірлік ретінде орнатылған бірінші бірлікті тағайындау арқылы олардың арасындағы түрлендіру коэффициентін де орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-112">When you set up multiple units in a unit group, you must also set up a conversion factor between them by designating the first unit that you set up as the default or primary unit for the unit group.</span></span> 

<span data-ttu-id="ee1bc-113">Мысалы, **Уақыт** бірлік тобында **Сағат** бірлігін бірінші бірлік ретінде орнатсаңыз, жүйе **Сағат** бірлігін әдепкі бірлік ретінде тағайындайды.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-113">For example, in a **Time** unit group, if you set up **Hour** as the first unit, the system designates **Hour** as the default unit.</span></span> <span data-ttu-id="ee1bc-114">Егер келесі орнатылатын бірлік **Күн** бірлігі болса, **Күн** бірлігінен **Сағат** бірлігіне арналған түрлендіру коэффициентін орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-114">If the next unit that you set up is **Day**, you must set up a conversion factor for **Day** to **Hour**.</span></span> <span data-ttu-id="ee1bc-115">Содан кейін **Апта** бірлігі үшінші бірлік ретінде қосылса, **Апта** бірлігі үшін **Күн** немесе **Сағат** бірлігіне сәйкес түрлендіру коэффициентін орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-115">If you then add **Week** as a third unit, you must set up a conversion factor for **Week** in terms of **Day** or **Hour**.</span></span> 

<span data-ttu-id="ee1bc-116">Төмендегі кескінде **Күн** бірлігі үшін орнату мысалы көрсетіледі, бұл бірлікте **Саны** өрісі бір күндегі сағат санын көрсетсе, ал **Апта** бірлігінде **Саны** өрісі бір аптадағы күндер санын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-116">The following image shows an example setup for the **Day** unit, where the **Quantity** field shows the number of hours that are in a day, and **Week**, where the **Quantity** field show the number of days that are in a week.</span></span>

> ![Бөлім тобы: Ақпараттық бет](media/advanced-2.png)

## <a name="using-units-and-unit-groups"></a><span data-ttu-id="ee1bc-118">Бірліктер мен бірлік топтарын пайдалану</span><span class="sxs-lookup"><span data-stu-id="ee1bc-118">Using units and unit groups</span></span>

<span data-ttu-id="ee1bc-119">Dynamics 365 Project Service Automation бағдарламасы шығыстар мен уақыт бойынша болжамдар мен жазбаларды өңдеу үшін бірліктер мен бірлік топтарын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-119">Dynamics 365 Project Service Automation uses units and unit groups to process estimates and entries for both expenses and time.</span></span> 

<span data-ttu-id="ee1bc-120">Шығыстар бойынша әр шығыс санатында әдепкі бірлік тобы және бірлігі болады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-120">For expenses, each expense category has a default unit group and unit.</span></span> <span data-ttu-id="ee1bc-121">Бұл мәндер шығыс санаттарына арналған бағатізбе жазбасында әдепкі мәндер ретінде енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-121">These values are entered as default values on price list entries for expense categories.</span></span> 

<span data-ttu-id="ee1bc-122">Мысалы, сізде **Жүріп өткен қашықтық** деп аталатын шығыс санаты бар.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-122">For example, you have an expense category that is named **Mileage**.</span></span> <span data-ttu-id="ee1bc-123">Онда **Қашықтық** деп аталатын бірлік тобы және **Миля** деп аталатын әдепкі бірлік бар.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-123">It has a unit group that is named **Distance** and a default unit that is named **Mile**.</span></span> <span data-ttu-id="ee1bc-124">Егер **Қашықтық** бірлік тобы екі бірліктен (**Миля** және **Километр**) тұратындай етіп орнатылса, **Жүріп өткен қашықтық** санаты үшін бір бағатізбеге екі бағаны орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-124">If you set up the **Distance** unit group so that it has two units (**Mile** and **Kilometer**), you can set two prices for the **Mileage** category on one price list: price per mile and price per kilometer.</span></span>

| <span data-ttu-id="ee1bc-125">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="ee1bc-125">Expense category</span></span>  | <span data-ttu-id="ee1bc-126">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-126">Unit group</span></span>  | <span data-ttu-id="ee1bc-127">Бірлік</span><span class="sxs-lookup"><span data-stu-id="ee1bc-127">Unit</span></span>      | <span data-ttu-id="ee1bc-128">Баға белгілеу әдісі</span><span class="sxs-lookup"><span data-stu-id="ee1bc-128">Pricing method</span></span>  | <span data-ttu-id="ee1bc-129">Бірлік бағасы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-129">Price per unit</span></span>  |
|-------------------|---------------|-----------|-------------------|-------------------|
| <span data-ttu-id="ee1bc-130">Жүріп өткен қашықтық</span><span class="sxs-lookup"><span data-stu-id="ee1bc-130">Mileage</span></span>           | <span data-ttu-id="ee1bc-131">Қашықтық</span><span class="sxs-lookup"><span data-stu-id="ee1bc-131">Distance</span></span>      | <span data-ttu-id="ee1bc-132">Миля</span><span class="sxs-lookup"><span data-stu-id="ee1bc-132">Mile</span></span>      | <span data-ttu-id="ee1bc-133">Бірлік бағасы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-133">Price per unit</span></span>    | <span data-ttu-id="ee1bc-134">10 USD</span><span class="sxs-lookup"><span data-stu-id="ee1bc-134">10 USD</span></span>            |
| <span data-ttu-id="ee1bc-135">Жүріп өткен қашықтық</span><span class="sxs-lookup"><span data-stu-id="ee1bc-135">Mileage</span></span>           | <span data-ttu-id="ee1bc-136">Қашықтық</span><span class="sxs-lookup"><span data-stu-id="ee1bc-136">Distance</span></span>      | <span data-ttu-id="ee1bc-137">Километр</span><span class="sxs-lookup"><span data-stu-id="ee1bc-137">Kilometer</span></span> | <span data-ttu-id="ee1bc-138">Бірлік бағасы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-138">Price per unit</span></span>    |  <span data-ttu-id="ee1bc-139">6 USD</span><span class="sxs-lookup"><span data-stu-id="ee1bc-139">6 USD</span></span>            |

<span data-ttu-id="ee1bc-140">Жобада шығысты енгізген кезде, жүйе бағаны санат пен шығыстағы бірлікті біріктіру арқылы анықтайды.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-140">When you enter an expense on a project, the system determines the price through the combination of the category and the unit on the expense.</span></span> 

| <span data-ttu-id="ee1bc-141">Шығыс сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-141">Expense description</span></span>        | <span data-ttu-id="ee1bc-142">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="ee1bc-142">Expense category</span></span>  | <span data-ttu-id="ee1bc-143">Бірлік</span><span class="sxs-lookup"><span data-stu-id="ee1bc-143">Unit</span></span>  | <span data-ttu-id="ee1bc-144">Саны</span><span class="sxs-lookup"><span data-stu-id="ee1bc-144">Quantity</span></span>  | <span data-ttu-id="ee1bc-145">Бірлік бағасы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-145">Unit price</span></span>   |
|----------------------------|---------------------|-------|-----------|----------------|
| <span data-ttu-id="ee1bc-146">Клиентке жеткізу</span><span class="sxs-lookup"><span data-stu-id="ee1bc-146">Drive to client location</span></span> | <span data-ttu-id="ee1bc-147">Жүріп өткен қашықтық</span><span class="sxs-lookup"><span data-stu-id="ee1bc-147">Mileage</span></span>             | <span data-ttu-id="ee1bc-148">Миля</span><span class="sxs-lookup"><span data-stu-id="ee1bc-148">Mile</span></span>  | <span data-ttu-id="ee1bc-149">10</span><span class="sxs-lookup"><span data-stu-id="ee1bc-149">10</span></span>        | <span data-ttu-id="ee1bc-150">10 USD</span><span class="sxs-lookup"><span data-stu-id="ee1bc-150">10 USD</span></span>         |

<span data-ttu-id="ee1bc-151">Уақыт өте келе, әр бағатізбенің жоғарғы деректемесінде **Әдепкі уақыт бірлігі** өрісі болады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-151">For time, each price list header has a **Default Time Unit** field.</span></span> <span data-ttu-id="ee1bc-152">Бағатізбенің жоғарғы деректемесін жасаған кезде мән орнатылады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-152">The value is set when you create the price list header.</span></span> <span data-ttu-id="ee1bc-153">Содан кейін бұл бірлік барлық рөлге негізделген бағаларды орнату үшін сол бағатізбеде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-153">This unit is then used to set all role-based prices on that price list.</span></span>

<span data-ttu-id="ee1bc-154">**Баға ұсыну уақыты** өрісіне арналған болжам жолдарын уақыттың кез келген бірлігінде көрсетуге болады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-154">Estimate lines for the **Time on Quote** field can be expressed in any unit of time.</span></span> <span data-ttu-id="ee1bc-155">Алайда, жобалардағы болжам жолдары мен жобаларға арналған уақыт жазбалары тек **Сағат** уақыт бірлігін қолдана алады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-155">However, estimate lines on projects and time entries for projects can use only the **Hour** unit of time.</span></span> <span data-ttu-id="ee1bc-156">Егер уақыт жазбасындағы немесе болжам жолындағы бірлік сол рөлге арналған бағатізбедегі бірлікке сәйкес келмесе, жүйе бағаны жоба болжамында немесе жобаның нақты транзакциясында анықталған бірліктерге түрлендіреді.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-156">If the unit on the time entry or estimate line doesn't match the unit on the price list line for that role, the system converts the price to the units that are defined in the project estimate or the project actual transaction.</span></span>

<span data-ttu-id="ee1bc-157">Төмендегі мысалда PSA жүйесінің бірлік тобын, бірліктерді және түрлендіру коэффициенттерін қалай пайдаланатыны көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-157">The following example shows how PSA uses the unit group, units, and conversion factors.</span></span>
- <span data-ttu-id="ee1bc-158">Бірліктер</span><span class="sxs-lookup"><span data-stu-id="ee1bc-158">Units</span></span>

   - <span data-ttu-id="ee1bc-159">**Бірлік тобы**: Уақыт</span><span class="sxs-lookup"><span data-stu-id="ee1bc-159">**Unit group**: Time</span></span> 
   - <span data-ttu-id="ee1bc-160">**Бірліктер**: Сағат</span><span class="sxs-lookup"><span data-stu-id="ee1bc-160">**Units**: Hour</span></span> 
    
    - <span data-ttu-id="ee1bc-161">**Күн** - Түрлендіру коэффициенті: 8 сағат</span><span class="sxs-lookup"><span data-stu-id="ee1bc-161">**Day** - Conversion factor: 8 hours</span></span>       
    - <span data-ttu-id="ee1bc-162">**Апта** - Түрлендіру коэффициенті: 40 сағат</span><span class="sxs-lookup"><span data-stu-id="ee1bc-162">**Week** - Conversion factor: 40 hours</span></span>  
        
- <span data-ttu-id="ee1bc-163">А жобасындағы бағатізбе орнатылымы:</span><span class="sxs-lookup"><span data-stu-id="ee1bc-163">Price list setup on Project A:</span></span>

    - <span data-ttu-id="ee1bc-164">**Атауы**: Ұлыбританиядағы сатылым бағалары 2016</span><span class="sxs-lookup"><span data-stu-id="ee1bc-164">**Name**: UK sales prices 2016</span></span> 
    - <span data-ttu-id="ee1bc-165">**Әдепкі уақыт бірлігі**: Күн</span><span class="sxs-lookup"><span data-stu-id="ee1bc-165">**Default time unit**: Day</span></span> 
    - <span data-ttu-id="ee1bc-166">**Валюта**: GBP</span><span class="sxs-lookup"><span data-stu-id="ee1bc-166">**Currency**: GBP</span></span>

| <span data-ttu-id="ee1bc-167">Рөл</span><span class="sxs-lookup"><span data-stu-id="ee1bc-167">Role</span></span>      | <span data-ttu-id="ee1bc-168">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-168">Unit group</span></span> | <span data-ttu-id="ee1bc-169">Бірлік</span><span class="sxs-lookup"><span data-stu-id="ee1bc-169">Unit</span></span> | <span data-ttu-id="ee1bc-170">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="ee1bc-170">Organizational unit</span></span> | <span data-ttu-id="ee1bc-171">Баға</span><span class="sxs-lookup"><span data-stu-id="ee1bc-171">Price</span></span>   |
|-----------|------------|------|---------------------|---------|
| <span data-ttu-id="ee1bc-172">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="ee1bc-172">Developer</span></span> | <span data-ttu-id="ee1bc-173">Time</span><span class="sxs-lookup"><span data-stu-id="ee1bc-173">Time</span></span>       | <span data-ttu-id="ee1bc-174">Day</span><span class="sxs-lookup"><span data-stu-id="ee1bc-174">Day</span></span>  | <span data-ttu-id="ee1bc-175">Contoso UK</span><span class="sxs-lookup"><span data-stu-id="ee1bc-175">Contoso UK</span></span>          | <span data-ttu-id="ee1bc-176">800 GBP</span><span class="sxs-lookup"><span data-stu-id="ee1bc-176">800 GBP</span></span> |

### <a name="time-entry"></a><span data-ttu-id="ee1bc-177">Уақыт жазбасы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-177">Time entry</span></span>

<span data-ttu-id="ee1bc-178">Төмендегі кестеде PSA жүйесінің үш сағаттық жоба үшін жасаған нәтижелі сатылымдар бүйірлік транзакциясы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-178">The following table shows the resulting sales-side transaction created by PSA for a three hour project.</span></span>


| <span data-ttu-id="ee1bc-179">Жоба</span><span class="sxs-lookup"><span data-stu-id="ee1bc-179">Project</span></span>   | <span data-ttu-id="ee1bc-180">Тапсырма</span><span class="sxs-lookup"><span data-stu-id="ee1bc-180">Task</span></span>    | <span data-ttu-id="ee1bc-181">Рөл</span><span class="sxs-lookup"><span data-stu-id="ee1bc-181">Role</span></span>      | <span data-ttu-id="ee1bc-182">Саны</span><span class="sxs-lookup"><span data-stu-id="ee1bc-182">Quantity</span></span> | <span data-ttu-id="ee1bc-183">Бірлік</span><span class="sxs-lookup"><span data-stu-id="ee1bc-183">Unit</span></span>  | <span data-ttu-id="ee1bc-184">Бірлік бағасы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-184">Unit price</span></span> | <span data-ttu-id="ee1bc-185">Шот ұсынылмаған сатылым көлемі</span><span class="sxs-lookup"><span data-stu-id="ee1bc-185">Unbilled sales amount</span></span> |
|-----------|---------|-----------|----------|-------|------------|-----------------------|
| <span data-ttu-id="ee1bc-186">А жобасы</span><span class="sxs-lookup"><span data-stu-id="ee1bc-186">Project A</span></span> | <span data-ttu-id="ee1bc-187">Құрастыру</span><span class="sxs-lookup"><span data-stu-id="ee1bc-187">Design</span></span>  | <span data-ttu-id="ee1bc-188">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="ee1bc-188">Developer</span></span> | <span data-ttu-id="ee1bc-189">3</span><span class="sxs-lookup"><span data-stu-id="ee1bc-189">3</span></span>        | <span data-ttu-id="ee1bc-190">Hour</span><span class="sxs-lookup"><span data-stu-id="ee1bc-190">Hour</span></span>  | <span data-ttu-id="ee1bc-191">100 GBP</span><span class="sxs-lookup"><span data-stu-id="ee1bc-191">100 GBP</span></span>    | <span data-ttu-id="ee1bc-192">300 GBP</span><span class="sxs-lookup"><span data-stu-id="ee1bc-192">300 GBP</span></span>               |

## <a name="time-unit-faq"></a><span data-ttu-id="ee1bc-193">Уақыт бірлігі туралы ЖҚС</span><span class="sxs-lookup"><span data-stu-id="ee1bc-193">Time unit FAQ</span></span>

### <a name="does-psa-convert-to-different-units-in-the-case-of-expenses"></a><span data-ttu-id="ee1bc-194">Шығыстар туындаған жағдайда PSA жүйесі әртүрлі бірліктерге түрлендіреді ме?</span><span class="sxs-lookup"><span data-stu-id="ee1bc-194">Does PSA convert to different units in the case of expenses?</span></span>
<span data-ttu-id="ee1bc-195">Жоқ.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-195">No.</span></span> <span data-ttu-id="ee1bc-196">Бірлікті түрлендіру әрекеті тек уақытқа ғана жүзеге асады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-196">Unit conversion works only for time.</span></span> <span data-ttu-id="ee1bc-197">Шығыстар үшін, егер жүйе шығыс санаты мен бірліктің бірігу бағасын таба алмаса, онда баға әдепкі бойынша 0.00-ге орнатылады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-197">For expenses, if the system can't find a price for the combination of the expense category and unit, the price is set to 0.00 by default.</span></span>

### <a name="why-does-psa-convert-time-units"></a><span data-ttu-id="ee1bc-198">Неліктен PSA жүйесі уақыт бірліктерін түрлендіреді?</span><span class="sxs-lookup"><span data-stu-id="ee1bc-198">Why does PSA convert time units?</span></span>
<span data-ttu-id="ee1bc-199">Кейбір елдерде немесе аймақтарда пайыздық мөлшерлеменің күндер бойынша орнатылуы жөніндегі заң талабы бар.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-199">In some countries or regions, there is a legal requirement that bill rates be set up in days.</span></span> <span data-ttu-id="ee1bc-200">Баға ұсыну циклі кезіндегі баға келісімі және шегерімі әрбір ақы төленетін рөл үшін тәуліктік мөлшерлемелерді қолдану арқылы жүзеге асырылады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-200">Price negotiation and discounting during the quote cycle is done by using day rates for each billable role.</span></span> <span data-ttu-id="ee1bc-201">Болжам кестесі және уақыт жазбасы сағатпен жүргізіледі.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-201">Schedule estimation and time entry are done in hours.</span></span> <span data-ttu-id="ee1bc-202">Уақыт бірліктеріндегі осы айырмашылықты қолдау үшін, PSA жүйесі уақыт бірліктерін түрлендіреді.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-202">To support this difference in time units, PSA converts time units.</span></span>

### <a name="can-time-units-be-changed-on-project-estimates"></a><span data-ttu-id="ee1bc-203">Жоба болжамдарында уақыт бірліктерін өзгертуге бола ма?</span><span class="sxs-lookup"><span data-stu-id="ee1bc-203">Can time units be changed on project estimates?</span></span>
<span data-ttu-id="ee1bc-204">Жоқ.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-204">No.</span></span> <span data-ttu-id="ee1bc-205">Қазіргі уақытта болжам кестесі сағатпен шектелген және оны өзгерту мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-205">Schedule estimation is currently restricted to hours and can’t be changed.</span></span>

### <a name="can-units-and-unit-groups-be-edited-deleted-and-added"></a><span data-ttu-id="ee1bc-206">Бірліктер мен бірлік топтарын өзгертуге, жоюға және қосуға бола ма?</span><span class="sxs-lookup"><span data-stu-id="ee1bc-206">Can units and unit groups be edited, deleted, and added?</span></span>
<span data-ttu-id="ee1bc-207">Иә.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-207">Yes.</span></span> <span data-ttu-id="ee1bc-208">**Уақыт** бірлік тобы мен **Сағат** бірлігін қоспағанда, барлық бірліктерді жоюға немесе өңдеуге болады және жаңа бірліктерді қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-208">With exception of the **Time** unit group and the **Hour** unit, all units can be deleted or edited, and new units can be added.</span></span> <span data-ttu-id="ee1bc-209">PSA жүйесінде **Уақыт** бірлік тобы мен **Сағат** бірлігін жою мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-209">In PSA, the **Time** unit group and the **Hour** unit can't be deleted.</span></span> <span data-ttu-id="ee1bc-210">Алайда, оларды **Атауы** өрісінің аударылған мәтінімен жаңартуға болады.</span><span class="sxs-lookup"><span data-stu-id="ee1bc-210">However, they can be updated with a translated text for the **Name** field.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]