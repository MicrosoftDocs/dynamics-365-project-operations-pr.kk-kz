---
title: Реттелетін өрістер мен нысандарды баға өлшемдері ретінде жасау
description: Осы тақырып реттелетін параметр жиындарын немесе нысандарды жасау әдісі туралы ақпаратты ұсынады.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2000f7e710267560fe2bd52b0e33024617d108ea
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898268"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="f1572-103">Реттелетін өрістер мен нысандарды баға өлшемдері ретінде жасау</span><span class="sxs-lookup"><span data-stu-id="f1572-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="f1572-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="f1572-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f1572-105">Реттелетін параметр жиынын немесе нысан жасау қажет болған кез келген уақытта келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-105">Complete the following steps any time that you want to create a custom option set or entity.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f1572-106">Реттелетін баға белгілеу өлшемінің барлық өзгерістерін бөлек шешімде жасау ұсынылады.</span><span class="sxs-lookup"><span data-stu-id="f1572-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="f1572-107">Осы маңызды үздік тәжірибе болашақта өзгерістерді қажетінше жаңарту немесе жою икемділігін қамтамасыз етеді, жұмысты қайта пайдалануға көмектеседі және осы өзгерістерді басқа данаға тасымалдауды жеңілдетеді.</span><span class="sxs-lookup"><span data-stu-id="f1572-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="f1572-108">Барлық қажетті өзгерістерді енгізгеннен кейін, осы шешімді **Басқарылатын шешім** ретінде экспорттап, баға белгілеу орнатуын қайтадан пайдалану үшін оны басқа даналарға импорттаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="f1572-109">Баға белгілеу өлшемдеріне арналған реттелетін шешімді жасау</span><span class="sxs-lookup"><span data-stu-id="f1572-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="f1572-110">Жаңа шешім жасау үшін **Параметрлер** > **Шешімдер** тармағын, содан кейін **Жаңа** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-110">Go to **Settings** > **Solutions**, and then select **New** to create a new solution.</span></span> 
2. <span data-ttu-id="f1572-111">Шешімді **\<your organization name> бағалау өлшемдері** деп атап, қалған қажет ақпаратты енгізіңіз, содан кейін **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="f1572-112">Баға белгілеу өлшемі шешімінде реттелетін өрістер мен параметрлер жиынын жасау</span><span class="sxs-lookup"><span data-stu-id="f1572-112">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="f1572-113">Баға белгілеу өлшемі параметрлер жиыны немесе нысан болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f1572-113">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="f1572-114">Баға белгілеу шешімінде олардың екеуі де жасалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="f1572-114">Both must be created in your pricing solution.</span></span> <span data-ttu-id="f1572-115">Осы процедурадағы қадамдар нысанға негізделген өлшемдер мен параметрлер жиынына негізделген өлшемдерді жасау жолын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="f1572-115">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="f1572-116">Нысанға негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="f1572-116">Entity-based dimensions</span></span>

1. <span data-ttu-id="f1572-117">**Параметрлер** > **Шешімдер** тармағы бойынша өтіп, **\<your organization name> бағалау өлшемдері** түймешігін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-117">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="f1572-118">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Нысандар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-118">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="f1572-119">**Жаңа** түймешігін **Стандартты тақырып** деп аталатын жаңа нысан жасау үшін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-119">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="f1572-120">Қалған қажет ақпаратты енгізіп, **Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-120">Enter the remaining required information, and then select **Save**.</span></span>


### <a name="option-set-based-dimensions"></a><span data-ttu-id="f1572-121">Параметрлер жиынына негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="f1572-121">Option set-based dimensions</span></span> 
<span data-ttu-id="f1572-122">Параметрлер жиынына негізделген екі өлшемді жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="f1572-122">You can create two option set-based dimensions.</span></span> <span data-ttu-id="f1572-123">**Үй** жұмыс орны мен **Оқиға орны** жұмысының бағасын бақылау үшін, **Ресурстың жұмыс орны** параметрін және жұмыс аяқталған кезде үстеме бағаны қосу үшін, **Тұрақты** and **Үстеме жұмыс** мәндері бар **Ресурстың жұмыс сағаттары** параметрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="f1572-124">**Параметрлер** > **Шешімдер** тармағы бойынша өтіп, **\<your organization name> бағалау өлшемдері** түймешігін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-124">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="f1572-125">Шешімдер жетекшісінде, сол жақ навигация тақтасында  **Параметрлер жиындары** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-125">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="f1572-126">Жаңа параметр жиынын жасау үшін **Жаңа** түймешігін таңдаңыз, қалған қажет ақпаратты енгізіңіз, содан кейін **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-126">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="f1572-127">Нысанға негізделген өлшемдер үшін деректер жасау</span><span class="sxs-lookup"><span data-stu-id="f1572-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="f1572-128">Нысанға негізделген өлшемдер үшін деректерді қолмен немесе Microsoft Excel бағдарламасының импорттау мүмкіндігі немесе қызмет қоңыраулары арқылы жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="f1572-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="f1572-129">**Стандартты тақырып** нысанға негізделген өлшемінен екі стандартты **Жүйе инженері** және **Жүйенің аға инженері** тақырыптарын жасау үшін, осы процедурадағы қадамдарды пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="f1572-130">Егер жасалатын деректер шағын болса, келесі мысалдағыдай стандартты пішінді пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="f1572-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="f1572-131">**Кеңейтілген іздеу** опциясын, **Стандартты тақырып** нысанын, содан кейін **Нәтижелер** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-131">Select **Advanced Find**, select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="f1572-132">Осы кезде **Стандартты тақырып** нысанындағы барлық жолдар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="f1572-132">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="f1572-133">**Жаңа** түймешігін таңдап, **Аты** өрісінде "Жүйелер инженері" деп енгізіп, **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-133">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
3. <span data-ttu-id="f1572-134">Пішінді жабу.</span><span class="sxs-lookup"><span data-stu-id="f1572-134">Close the form.</span></span> 
4. <span data-ttu-id="f1572-135">"Жүйенің аға инженері" үшін басқа стандартты тақырыпты жасау үшін 1-3 қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-135">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="f1572-136">Бағалау өлшемі шешіміне барлық қажет нысандар мен қатысты құрамдастарды қосу</span><span class="sxs-lookup"><span data-stu-id="f1572-136">Add all required entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="f1572-137">Бағалау шешіміне келесі нысандарды қосу қажет болады.</span><span class="sxs-lookup"><span data-stu-id="f1572-137">You will need to add the following entities to your pricing solution.</span></span> <span data-ttu-id="f1572-138">Нысандар жаңа баға белгілеу өлшемдері туралы хабардар болуы үшін, схемаға кейбір маңызды өзгерістерді енгізу үшін осы процедурадағы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-138">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="f1572-139">**Параметрлер** > **Шешімдер** тармағын таңдап, **\<your organization name> бағалау өлшемдері** түймешігін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-139">Select **Settings** > **Solutions**, and double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="f1572-140">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Бар нысанды қосу** > **Нысандар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-140">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="f1572-141">**Шешім құрамдастары** диалогтік терезесінде келесі нысандарды таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="f1572-141">In the **Solution Components** dialog box, select the following entities:</span></span>

  - <span data-ttu-id="f1572-142">Нақты</span><span class="sxs-lookup"><span data-stu-id="f1572-142">Actual</span></span>
  - <span data-ttu-id="f1572-143">Тапсырыс беруге болатын ресурс</span><span class="sxs-lookup"><span data-stu-id="f1572-143">Bookable Resource</span></span>
  - <span data-ttu-id="f1572-144">Болжам жолы</span><span class="sxs-lookup"><span data-stu-id="f1572-144">Estimate Line</span></span>
  - <span data-ttu-id="f1572-145">Есеп-шот жолы мәліметі</span><span class="sxs-lookup"><span data-stu-id="f1572-145">Invoice Line Detail</span></span>
  - <span data-ttu-id="f1572-146">Журнал жолы</span><span class="sxs-lookup"><span data-stu-id="f1572-146">Journal Line</span></span>
  - <span data-ttu-id="f1572-147">Жобалық келісім-шарт жолы мәліметі</span><span class="sxs-lookup"><span data-stu-id="f1572-147">Project Contract Line Detail</span></span>
  - <span data-ttu-id="f1572-148">Жоба тобы мүшесі</span><span class="sxs-lookup"><span data-stu-id="f1572-148">Project Team Member</span></span>
  - <span data-ttu-id="f1572-149">Баға ұсыну жолының мәліметтері</span><span class="sxs-lookup"><span data-stu-id="f1572-149">Quote Line Detail</span></span>
  - <span data-ttu-id="f1572-150">Рөлдің үстеме бағасы</span><span class="sxs-lookup"><span data-stu-id="f1572-150">Role Price Markup</span></span>
  - <span data-ttu-id="f1572-151">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="f1572-151">Role Price</span></span> 
  - <span data-ttu-id="f1572-152">Уақыт нысаны</span><span class="sxs-lookup"><span data-stu-id="f1572-152">Time Entry</span></span> 


> [!NOTE]
> <span data-ttu-id="f1572-153">Таңдалған нысандардың әрқайсысына барлық пішіндер мен көріністерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-153">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="f1572-154">Жоғарыда таңдалған нысандар үшін қандай да бір тәуелді нысанды кірістіру туралы сұралса, **Жоқ** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f1572-154">When prompted to include any dependent entities for the entities selected above, select **No**.</span></span>

