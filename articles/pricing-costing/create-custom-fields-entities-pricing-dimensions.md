---
title: Реттелетін өрістер мен нысандарды баға өлшемдері ретінде жасау
description: Осы тақырып реттелетін параметр жиындарын немесе нысандарды жасау әдісі туралы ақпаратты ұсынады.
author: rumant
manager: AnnBe
ms.date: 11/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: 089481cd3e7c0f8f1d1aa880d64cb79e8d677c2d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5275635"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="2839a-103">Реттелетін өрістер мен нысандарды баға өлшемдері ретінде жасау</span><span class="sxs-lookup"><span data-stu-id="2839a-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="2839a-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="2839a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2839a-105">Реттелетін параметрлер жиынын немесе нысанды бағалау өлшемі ретінде пайдалану үшін жасау керек болғанда, келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-105">Complete the following steps when you want to create a custom option set or entity for using it as a pricing dimension.</span></span> <span data-ttu-id="2839a-106">Қосымша ақпарат алу үшін [Бағалау өлшемдерін шолу](pricing-dimensions-overview.md) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-106">For more information, see [Pricing dimensions overview](pricing-dimensions-overview.md).</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="2839a-107">Реттелетін баға белгілеу өлшемінің барлық өзгерістерін бөлек шешімде жасау ұсынылады.</span><span class="sxs-lookup"><span data-stu-id="2839a-107">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="2839a-108">Бұл маңызды озық тәжірибе болашақта қажетінше өзгерістерді жаңарту немесе жою үшін икемділікті қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="2839a-108">This important best practice provides flexibility in the future to update or remove changes as needed.</span></span> <span data-ttu-id="2839a-109">Сондай-ақ бұл сіздің жұмысыңызды қайта пайдалануға көмектеседі және бұл өзгерістерді басқа данаға ауыстыруды жеңілдетеді. Барлық қажетті өзгертулерді жасағаннан кейін, бұл шешімді **Басқарылатын шешім** ретінде экспорттаңыз және баға параметрлерін қайта пайдалану үшін оны басқа даналарға импорттаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-109">This will also help with re-use of your work and make it easier to port these changes to another instance After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="2839a-110">Баға белгілеу өлшемі шешімінде реттелетін өрістер мен параметрлер жиынын жасау</span><span class="sxs-lookup"><span data-stu-id="2839a-110">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="2839a-111">Баға белгілеу өлшемі параметрлер жиыны немесе нысан болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="2839a-111">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="2839a-112">Баға белгілеу шешімінде олардың екеуі де жасалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="2839a-112">Both must be created in your pricing solution.</span></span> <span data-ttu-id="2839a-113">Осы процедурадағы қадамдар нысанға негізделген өлшемдер мен параметрлер жиынына негізделген өлшемдерді жасау жолын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="2839a-113">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="2839a-114">Нысанға негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="2839a-114">Entity-based dimensions</span></span>
<span data-ttu-id="2839a-115">Нысанға негізделген өлшемдерді жасау үшін келесі қадамдарды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="2839a-115">To create entity-based dimensions, follow these steps:</span></span>

1. <span data-ttu-id="2839a-116">**Параметрлер** > **Шешімдер** тармағы бойынша өтіп, **\<your organization name> бағалау өлшемдері** түймешігін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-116">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="2839a-117">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Нысандар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-117">In Solution Explorer, in the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="2839a-118">**Жаңа** түймешігін **Стандартты тақырып** деп аталатын жаңа нысан жасау үшін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-118">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="2839a-119">Қалған қажет ақпаратты енгізіп, **Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-119">Enter the remaining required information, and then select **Save**.</span></span>

> ![Стандартты тақырып нысанының анықтамасы](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a><span data-ttu-id="2839a-121">Параметрлер жиынына негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="2839a-121">Option set-based dimensions</span></span> 
<span data-ttu-id="2839a-122">Параметрлер жиынына негізделген екі өлшемді жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="2839a-122">You can create two option set-based dimensions.</span></span> 

- <span data-ttu-id="2839a-123">**Басты** орналасу жұмысы және **Жергілікті** жұмысының бағасын бақылау үшін **Ресурстық жұмыс орны** параметрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work.</span></span> 
- <span data-ttu-id="2839a-124">Жұмыс аяқталғаннан кейін үстеме бағаны қолдану үшін **Ресурстың жұмыс сағаттары** параметрін **Тұрақты** және **Үстеме жұмыс** мәндерімен пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-124">Use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when the work is complete.</span></span>

<span data-ttu-id="2839a-125">Келесі графикада **Ресурстың жұмыс орны** өлшемінің көрінісі берілген.</span><span class="sxs-lookup"><span data-stu-id="2839a-125">The following graphic provides a view of the **Resource Work Location** dimension.</span></span> 

> ![Параметрлер жиынына негізделген баға белгілеу өлшемі "Ресурстың жұмыс орны" деп аталады](media/Option-set-PD-called-Resource-Work-Location.png)

<span data-ttu-id="2839a-127">Келесі графикада **Ресурстың жұмыс сағаттары** өлшемінің көрінісі берілген.</span><span class="sxs-lookup"><span data-stu-id="2839a-127">The following graphic provides a view of the **Resource Work Hours** dimension.</span></span> 

> ![Параметрлер жиынына негізделген баға белгілеу өлшемі "Ресурстың жұмыс сағаттары" деп аталады](media/Option-set-PD-called-Resource-Work-Hours.png)

1. <span data-ttu-id="2839a-129">**Параметрлер** > **Шешімдер** тармағы бойынша өтіп, **\<your organization name> бағалау өлшемдері** түймешігін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-129">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="2839a-130">Шешімдер жетекшісінде, сол жақ навигация тақтасында  **Параметрлер жиындары** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-130">In Solution Explorer, in the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="2839a-131">Жаңа параметр жиынын жасау үшін **Жаңа** түймешігін таңдаңыз, қалған қажет ақпаратты енгізіңіз, содан кейін **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-131">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="2839a-132">Нысанға негізделген өлшемдер үшін деректер жасау</span><span class="sxs-lookup"><span data-stu-id="2839a-132">Create data for entity-based dimensions</span></span>

<span data-ttu-id="2839a-133">Нысанға негізделген өлшемдер үшін деректерді қолмен немесе Microsoft Excel бағдарламасының импорттау мүмкіндігі немесе қызмет қоңыраулары арқылы жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="2839a-133">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="2839a-134">**Стандартты тақырып** нысанға негізделген өлшемінен екі стандартты **Жүйе инженері** және **Жүйенің аға инженері** тақырыптарын жасау үшін, осы процедурадағы қадамдарды пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-134">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="2839a-135">Егер жасалатын деректер шағын болса, келесі мысалдағыдай стандартты пішінді пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="2839a-135">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="2839a-136">**Кеңейтілген іздеу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-136">Select **Advanced Find**.</span></span>
2. <span data-ttu-id="2839a-137">**Стандартты тақырып** нысанын таңдап, содан кейін **Нәтижелер** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-137">Select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="2839a-138">Осы кезде **Стандартты тақырып** нысанындағы барлық жолдар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="2839a-138">All of the rows in the **Standard Title** entity will be shown.</span></span>
3. <span data-ttu-id="2839a-139">**Жаңа** түймешігін таңдап, **Аты** өрісінде "Жүйелер инженері" деп енгізіп, **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-139">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
4. <span data-ttu-id="2839a-140">Бетті жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-140">Close the page.</span></span> 
5. <span data-ttu-id="2839a-141">"Жүйенің аға инженері" үшін басқа стандартты тақырыпты жасау үшін 1-3 қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="2839a-141">Repeat steps 1-3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![Стандартты тақырып нысанының үлгі деректері](media/ST-data.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]