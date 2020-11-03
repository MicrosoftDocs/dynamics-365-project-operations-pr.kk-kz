---
title: Реттелетін өрістер мен нысандарды жасау
description: Бұл тақырыпта Power Apps платформасында өзіңіздің жеке шешіміңізде параметрлер жиыны мен нысандарды жасау жолы түсіндіріледі.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 442ff9cf2206bec307cea7ff30b9266502d8f77b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079729"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="74603-103">Реттелетін өрістер мен нысандарды жасау</span><span class="sxs-lookup"><span data-stu-id="74603-103">Create custom fields and entities</span></span> 

<span data-ttu-id="74603-104">Power Apps платформасында кез келген уақытта реттелетін параметрлер жиынын немесе нысанды жасау қажет болған кезде, келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="74603-105">Осы тақырыптағы процедуралар Project Service Automation (PSA) веб-интерфейсін пайдалану арқылы орындалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="74603-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="74603-106">Реттелетін баға белгілеу өлшемінің барлық өзгерістерін бөлек шешімде жасау ұсынылады.</span><span class="sxs-lookup"><span data-stu-id="74603-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="74603-107">Осы маңызды үздік тәжірибе болашақта өзгерістерді қажетінше жаңарту немесе жою икемділігін қамтамасыз етеді, жұмысты қайта пайдалануға көмектеседі және осы өзгерістерді басқа данаға тасымалдауды жеңілдетеді.</span><span class="sxs-lookup"><span data-stu-id="74603-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="74603-108">Барлық қажетті өзгерістерді енгізгеннен кейін, осы шешімді **Басқарылатын шешім** ретінде экспорттап, баға белгілеу орнатуын қайтадан пайдалану үшін оны басқа даналарға импорттаңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="74603-109">Баға белгілеу өлшемі шешімінде реттелетін өрістер мен параметрлер жиынын жасау</span><span class="sxs-lookup"><span data-stu-id="74603-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="74603-110">Баға белгілеу өлшемі параметрлер жиыны немесе нысан болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="74603-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="74603-111">Баға белгілеу шешімінде олардың екеуі де жасалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="74603-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="74603-112">Осы процедурадағы қадамдар нысанға негізделген өлшемдер мен параметрлер жиынына негізделген өлшемдерді жасау жолын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="74603-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="74603-113">Нысанға негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="74603-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="74603-114">PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын таңдап, содан кейін **\<your organization name> баға өлшемдері** пәрменін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-114">In PSA, click **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="74603-115">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Нысандар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="74603-116">**Стандартты тақырып** деп аталатын жаңа нысанды жасау үшін **Жаңа** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="74603-117">Қалған қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![Стандартты тақырып нысанының анықтамасы](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="74603-119">Параметрлер жиынына негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="74603-119">Option set-based dimensions</span></span> 
<span data-ttu-id="74603-120">Параметрлер жиынына негізделген екі өлшемді жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="74603-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="74603-121">**Үй** жұмыс орны мен **Оқиға орны** жұмысының бағасын бақылау үшін, **Ресурстың жұмыс орны** параметрін және жұмыс аяқталған кезде үстеме бағаны қосу үшін, **Тұрақты** and **Үстеме жұмыс** мәндері бар **Ресурстың жұмыс сағаттары** параметрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="74603-122">PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын басыңыз, содан кейін **\<your organization name> баға өлшемдері** параметрін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-122">In PSA, click **Settings** > **Solutions** , and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="74603-123">Шешімдер жетекшісінде, сол жақ навигация тақтасында  **Параметрлер жиындары** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="74603-124">Жаңа параметрлер жиынын жасау үшін **Жаңа** опциясын басып, қалған қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="74603-125">Параметрлер жиынына негізделген баға белгілеу өлшемі "Ресурстың жұмыс орны" деп аталады</span><span class="sxs-lookup"><span data-stu-id="74603-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="74603-126">Параметрлер жиынына негізделген баға белгілеу өлшемі "Ресурстың жұмыс сағаттары" деп аталады</span><span class="sxs-lookup"><span data-stu-id="74603-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="74603-127">Нысанға негізделген өлшемдер үшін деректер жасау</span><span class="sxs-lookup"><span data-stu-id="74603-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="74603-128">Нысанға негізделген өлшемдер үшін деректерді қолмен немесе Microsoft Excel бағдарламасының импорттау мүмкіндігі немесе қызмет қоңыраулары арқылы жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="74603-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="74603-129">**Стандартты тақырып** нысанға негізделген өлшемінен екі стандартты **Жүйе инженері** және **Жүйенің аға инженері** тақырыптарын жасау үшін, осы процедурадағы қадамдарды пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="74603-130">Егер жасалатын деректер шағын болса, келесі мысалдағыдай стандартты пішінді пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="74603-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="74603-131">PSA жүйесінде **Кеңейтілген іздеу** опциясын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="74603-132">**Стандартты тақырып** нысанын таңдап, **Нәтижелер** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="74603-133">Осы кезде **Стандартты тақырып** нысанындағы барлық жолдар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="74603-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="74603-134">**Жаңа** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-134">Click **New**.</span></span> <span data-ttu-id="74603-135">**Атауы** өрісінде "Жүйе инженері" атауын енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="74603-136">Пішінді жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-136">Close the form.</span></span> 
4. <span data-ttu-id="74603-137">"Жүйенің аға инженері" үшін басқа стандартты тақырыпты жасау үшін 1-3 қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="74603-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="74603-138">Стандартты тақырып нысанының үлгі деректері</span><span class="sxs-lookup"><span data-stu-id="74603-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)


