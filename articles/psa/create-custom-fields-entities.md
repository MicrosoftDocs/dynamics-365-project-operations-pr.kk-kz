---
title: Реттелетін өрістер мен нысандарды жасау
description: Бұл тақырыпта Power Apps платформасында өзіңіздің жеке шешіміңізде параметрлер жиыны мен нысандарды жасау жолы түсіндіріледі.
author: Rumant
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 3d838bde8a3d7cbc15e06fb3289924468c284a8a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998958"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="69b21-103">Реттелетін өрістер мен нысандарды жасау</span><span class="sxs-lookup"><span data-stu-id="69b21-103">Create custom fields and entities</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="69b21-104">Power Apps платформасында кез келген уақытта реттелетін параметрлер жиынын немесе нысанды жасау қажет болған кезде, келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="69b21-105">Осы тақырыптағы процедуралар Project Service Automation (PSA) веб-интерфейсін пайдалану арқылы орындалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="69b21-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="69b21-106">Реттелетін баға белгілеу өлшемінің барлық өзгерістерін бөлек шешімде жасау ұсынылады.</span><span class="sxs-lookup"><span data-stu-id="69b21-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="69b21-107">Осы маңызды үздік тәжірибе болашақта өзгерістерді қажетінше жаңарту немесе жою икемділігін қамтамасыз етеді, жұмысты қайта пайдалануға көмектеседі және осы өзгерістерді басқа данаға тасымалдауды жеңілдетеді.</span><span class="sxs-lookup"><span data-stu-id="69b21-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="69b21-108">Барлық қажетті өзгерістерді енгізгеннен кейін, осы шешімді **Басқарылатын шешім** ретінде экспорттап, баға белгілеу орнатуын қайтадан пайдалану үшін оны басқа даналарға импорттаңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="69b21-109">Баға белгілеу өлшемі шешімінде реттелетін өрістер мен параметрлер жиынын жасау</span><span class="sxs-lookup"><span data-stu-id="69b21-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="69b21-110">Баға белгілеу өлшемі параметрлер жиыны немесе нысан болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="69b21-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="69b21-111">Баға белгілеу шешімінде олардың екеуі де жасалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="69b21-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="69b21-112">Осы процедурадағы қадамдар нысанға негізделген өлшемдер мен параметрлер жиынына негізделген өлшемдерді жасау жолын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="69b21-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="69b21-113">Нысанға негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="69b21-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="69b21-114">PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын таңдап, содан кейін **\<your organization name> баға өлшемдері** пәрменін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-114">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="69b21-115">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Нысандар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="69b21-116">**Стандартты тақырып** деп аталатын жаңа нысанды жасау үшін **Жаңа** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="69b21-117">Қалған қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![Стандартты тақырып нысанының анықтамасы](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="69b21-119">Параметрлер жиынына негізделген өлшемдер</span><span class="sxs-lookup"><span data-stu-id="69b21-119">Option set-based dimensions</span></span> 
<span data-ttu-id="69b21-120">Параметрлер жиынына негізделген екі өлшемді жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="69b21-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="69b21-121">**Үй** жұмыс орны мен **Оқиға орны** жұмысының бағасын бақылау үшін, **Ресурстың жұмыс орны** параметрін және жұмыс аяқталған кезде үстеме бағаны қосу үшін, **Тұрақты** and **Үстеме жұмыс** мәндері бар **Ресурстың жұмыс сағаттары** параметрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="69b21-122">PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын басыңыз, содан кейін **\<your organization name> баға өлшемдері** параметрін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-122">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="69b21-123">Шешімдер жетекшісінде, сол жақ навигация тақтасында  **Параметрлер жиындары** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="69b21-124">Жаңа параметрлер жиынын жасау үшін **Жаңа** опциясын басып, қалған қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="69b21-125">Параметрлер жиынына негізделген баға белгілеу өлшемі "Ресурстың жұмыс орны" деп аталады</span><span class="sxs-lookup"><span data-stu-id="69b21-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="69b21-126">Параметрлер жиынына негізделген баға белгілеу өлшемі "Ресурстың жұмыс сағаттары" деп аталады</span><span class="sxs-lookup"><span data-stu-id="69b21-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="69b21-127">Нысанға негізделген өлшемдер үшін деректер жасау</span><span class="sxs-lookup"><span data-stu-id="69b21-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="69b21-128">Нысанға негізделген өлшемдер үшін деректерді қолмен немесе Microsoft Excel бағдарламасының импорттау мүмкіндігі немесе қызмет қоңыраулары арқылы жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="69b21-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="69b21-129">**Стандартты тақырып** нысанға негізделген өлшемінен екі стандартты **Жүйе инженері** және **Жүйенің аға инженері** тақырыптарын жасау үшін, осы процедурадағы қадамдарды пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="69b21-130">Егер жасалатын деректер шағын болса, келесі мысалдағыдай стандартты пішінді пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="69b21-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="69b21-131">PSA жүйесінде **Кеңейтілген іздеу** опциясын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="69b21-132">**Стандартты тақырып** нысанын таңдап, **Нәтижелер** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="69b21-133">Осы кезде **Стандартты тақырып** нысанындағы барлық жолдар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="69b21-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="69b21-134">**Жаңа** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-134">Click **New**.</span></span> <span data-ttu-id="69b21-135">**Атауы** өрісінде "Жүйе инженері" атауын енгізіп, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="69b21-136">Пішінді жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-136">Close the form.</span></span> 
4. <span data-ttu-id="69b21-137">"Жүйенің аға инженері" үшін басқа стандартты тақырыпты жасау үшін 1-3 қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="69b21-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="69b21-138">Стандартты тақырып нысанының үлгі деректері</span><span class="sxs-lookup"><span data-stu-id="69b21-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]