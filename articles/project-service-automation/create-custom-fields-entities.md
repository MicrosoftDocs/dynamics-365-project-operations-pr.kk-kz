---
title: Реттелетін өрістер мен нысандарды жасау
description: Бұл тақырыпта Power Apps платформасында өзіңіздің жеке шешіміңізде параметрлер жиыны мен нысандарды жасау жолы түсіндіріледі.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753131"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="65087-103">Реттелетін өрістер мен нысандарды жасау</span><span class="sxs-lookup"><span data-stu-id="65087-103">Create custom fields and entities</span></span> 

<span data-ttu-id="65087-104">Power Apps платформасында кез келген уақытта реттелетін параметрлер жиынын немесе нысанды жасау қажет болған кезде, келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="65087-105">Осы тақырыптағы процедуралар Project Service Automation (PSA) веб-интерфейсін пайдалану арқылы орындалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="65087-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="65087-106">Реттелетін баға белгілеу өлшемінің барлық өзгерістерін бөлек шешімде жасау ұсынылады.</span><span class="sxs-lookup"><span data-stu-id="65087-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="65087-107">Осы маңызды үздік тәжірибе болашақта өзгерістерді қажетінше жаңарту немесе жою икемділігін қамтамасыз етеді, жұмысты қайта пайдалануға көмектеседі және осы өзгерістерді басқа данаға тасымалдауды жеңілдетеді.</span><span class="sxs-lookup"><span data-stu-id="65087-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="65087-108">Барлық қажетті өзгерістерді енгізгеннен кейін, осы шешімді **Басқарылатын шешім** ретінде экспорттап, баға белгілеу орнатуын қайтадан пайдалану үшін оны басқа даналарға импорттаңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="65087-109">Баға белгілеу өлшемдеріне арналған реттелетін шешімді жасау</span><span class="sxs-lookup"><span data-stu-id="65087-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="65087-110">PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын басып, жаңа шешім жасау үшін **Жаңа** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-110">In PSA, click **Settings** > **Solutions**, and then click **New** to create a new solution.</span></span> 
2. <span data-ttu-id="65087-111">Шешімге ат қойып, **\<your organization name> баға белгілеу өлшемдері**, қалған қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then click **Save**.</span></span>

> ![Баға белгілеу өлшемдеріне арналған реттелетін шешімді жасау](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="65087-113">Баға белгілеу өлшемі шешімінде реттелетін өрістер мен параметрлер жиынын жасау</span><span class="sxs-lookup"><span data-stu-id="65087-113">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="65087-114">Баға белгілеу өлшемі параметрлер жиыны немесе нысан болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="65087-114">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="65087-115">Баға белгілеу шешімінде олардың екеуі де жасалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="65087-115">Both must be created in your pricing solution.</span></span> <span data-ttu-id="65087-116">Осы процедурадағы қадамдар нысанға негізделген өлшемдер мен параметрлер жиынына негізделген өлшемдерді жасау жолын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="65087-116">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="65087-117">Нысанға негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="65087-117">Entity-based dimensions</span></span>

1. <span data-ttu-id="65087-118">PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын басып, **\<your organization name> баға өлшемдері** тармағын екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-118">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="65087-119">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Нысандар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-119">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="65087-120">**Стандартты тақырып** деп аталатын жаңа нысанды жасау үшін **Жаңа** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-120">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="65087-121">Қалған қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-121">Enter the remaining required information, and then click **Save**.</span></span>

> ![Стандартты тақырып нысанының анықтамасы](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="65087-123">Параметрлер жиынына негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="65087-123">Option set-based dimensions</span></span> 
<span data-ttu-id="65087-124">Параметрлер жиынына негізделген екі өлшемді жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="65087-124">You can create two option set-based dimensions.</span></span> <span data-ttu-id="65087-125">**Үй** жұмыс орны мен **Оқиға орны** жұмысының бағасын бақылау үшін, **Ресурстың жұмыс орны** параметрін және жұмыс аяқталған кезде үстеме бағаны қосу үшін, **Тұрақты** and **Үстеме жұмыс** мәндері бар **Ресурстың жұмыс сағаттары** параметрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-125">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="65087-126">PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын басып, **\<your organization name> баға өлшемдері** тармағын екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-126">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="65087-127">Шешімдер жетекшісінде, сол жақ навигация тақтасында  **Параметрлер жиындары** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-127">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="65087-128">Жаңа параметрлер жиынын жасау үшін **Жаңа** опциясын басып, қалған қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-128">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="65087-129">Параметрлер жиынына негізделген баға белгілеу өлшемі "Ресурстың жұмыс орны" деп аталады</span><span class="sxs-lookup"><span data-stu-id="65087-129">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="65087-130">Параметрлер жиынына негізделген баға белгілеу өлшемі "Ресурстың жұмыс сағаттары" деп аталады</span><span class="sxs-lookup"><span data-stu-id="65087-130">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="65087-131">Нысанға негізделген өлшемдер үшін деректер жасау</span><span class="sxs-lookup"><span data-stu-id="65087-131">Create data for entity-based dimensions</span></span>

<span data-ttu-id="65087-132">Нысанға негізделген өлшемдер үшін деректерді қолмен немесе Microsoft Excel бағдарламасының импорттау мүмкіндігі немесе қызмет қоңыраулары арқылы жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="65087-132">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="65087-133">**Стандартты тақырып** нысанға негізделген өлшемінен екі стандартты **Жүйе инженері** және **Жүйенің аға инженері** тақырыптарын жасау үшін, осы процедурадағы қадамдарды пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-133">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="65087-134">Егер жасалатын деректер шағын болса, келесі мысалдағыдай стандартты пішінді пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="65087-134">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="65087-135">PSA жүйесінде **Кеңейтілген іздеу** опциясын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-135">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="65087-136">**Стандартты тақырып** нысанын таңдап, **Нәтижелер** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-136">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="65087-137">Осы кезде **Стандартты тақырып** нысанындағы барлық жолдар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="65087-137">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="65087-138">**Жаңа** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-138">Click **New**.</span></span> <span data-ttu-id="65087-139">**Атауы** өрісінде "Жүйе инженері" атауын енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-139">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="65087-140">Пішінді жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-140">Close the form.</span></span> 
4. <span data-ttu-id="65087-141">"Жүйенің аға инженері" үшін басқа стандартты тақырыпты жасау үшін 1-3 қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-141">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="65087-142">Стандартты тақырып нысанының үлгі деректері</span><span class="sxs-lookup"><span data-stu-id="65087-142">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="65087-143">Баға белгілеу өлшемі шешіміне барлық қажетті PSA нысандарын және оған қатысты компоненттерді қосыңыз</span><span class="sxs-lookup"><span data-stu-id="65087-143">Add all required PSA entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="65087-144">Баға белгілеу шешіміне Project Service бағдарламасының келесі нысандарын қосу керек болады.</span><span class="sxs-lookup"><span data-stu-id="65087-144">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="65087-145">Нысандар жаңа баға белгілеу өлшемдері туралы хабардар болуы үшін, схемаға кейбір маңызды өзгерістерді енгізу үшін осы процедурадағы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-145">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="65087-146">PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын басып, **\<your organization name> баға өлшемдері** тармағын екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-146">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="65087-147">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Бар нысанды қосу** > **Нысандар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-147">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="65087-148">**Шешім құрамдастары** диалогтік терезесінде келесі нысандарды таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="65087-148">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="65087-149">Нақты</span><span class="sxs-lookup"><span data-stu-id="65087-149">Actual</span></span>
- <span data-ttu-id="65087-150">Тапсырыс беруге болатын ресурс</span><span class="sxs-lookup"><span data-stu-id="65087-150">Bookable Resource</span></span>
- <span data-ttu-id="65087-151">Болжам жолы</span><span class="sxs-lookup"><span data-stu-id="65087-151">Estimate Line</span></span>
- <span data-ttu-id="65087-152">Есеп-шот жолы мәліметі</span><span class="sxs-lookup"><span data-stu-id="65087-152">Invoice Line Detail</span></span>
- <span data-ttu-id="65087-153">Журнал жолы</span><span class="sxs-lookup"><span data-stu-id="65087-153">Journal Line</span></span>
- <span data-ttu-id="65087-154">Жобалық келісім-шарт жолы мәліметі</span><span class="sxs-lookup"><span data-stu-id="65087-154">Project Contract Line Detail</span></span>
- <span data-ttu-id="65087-155">Жоба тобы мүшесі</span><span class="sxs-lookup"><span data-stu-id="65087-155">Project Team Member</span></span>
- <span data-ttu-id="65087-156">Баға ұсыну жолының мәліметтері</span><span class="sxs-lookup"><span data-stu-id="65087-156">Quote Line Detail</span></span>
- <span data-ttu-id="65087-157">Рөлдің үстеме бағасы</span><span class="sxs-lookup"><span data-stu-id="65087-157">Role Price Markup</span></span>
- <span data-ttu-id="65087-158">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="65087-158">Role Price</span></span> 
- <span data-ttu-id="65087-159">Уақыт жазбасы</span><span class="sxs-lookup"><span data-stu-id="65087-159">Time Entry</span></span> 

> ![Баға белгілеу өлшемі шешіміне бұрыннан бар нысандарды қосу](media/Existing-entities-to-PD-solution.png)

> ![Шешім құрамдастарын таңдау](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="65087-162">Таңдалған нысандардың әрқайсысына барлық пішіндер мен көріністерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-162">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="65087-163">Жоғарыда таңдалған нысандарға қандай да бір тәуелді нысандарды қосу сұралған кезде, **Жоқ** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="65087-163">When prompted to include any dependent entities for the entities selected above, click **No**.</span></span>

> ![Барлық қатысты құрамдастарды қоспаңыз](media/Do-not-include-required.png)


