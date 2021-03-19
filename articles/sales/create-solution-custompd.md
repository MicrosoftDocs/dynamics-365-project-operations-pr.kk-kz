---
title: Реттелетін баға өлшемдері үшін шешім жасау
description: Бұл тақырыпта реттелетін бағалар өлшемдеріне арналған шешімдерді жасау жолдары туралы ақпарат берілген.
author: Rumant
manager: tfehr
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3e3f688b0147974ef252a0ee00be20c4669d7165
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278425"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="48764-103">Реттелетін баға өлшемдері үшін шешім жасау</span><span class="sxs-lookup"><span data-stu-id="48764-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="48764-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="48764-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="48764-105">Реттелетін баға өлшемдерінің барлық өзгертулері бөлек шешімде болуы керек.</span><span class="sxs-lookup"><span data-stu-id="48764-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="48764-106">Осы маңызды үздік тәжірибе болашақта өзгерістерді қажетінше жаңарту немесе жою икемділігіне мүмкіндік береді, жұмысты қайта пайдалануға көмектеседі және осы өзгерістерді басқа даналарға тасымалдауды жеңілдетеді.</span><span class="sxs-lookup"><span data-stu-id="48764-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="48764-107">Барлық қажетті өзгерістерді енгізгеннен кейін, осы шешімді **Басқарылған** шешім ретінде экспорттап, содан кейін қайтадан пайдалану үшін оны басқа даналарға импорттаңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="48764-108">Реттелетін баға өлшемдері үшін шешім жасау</span><span class="sxs-lookup"><span data-stu-id="48764-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="48764-109">**Параметрлер** > **Шешімдер** тармағын таңдап, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="48764-110">Шешімді атаңыз, *<your organization name> баға өлшемдері*.</span><span class="sxs-lookup"><span data-stu-id="48764-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="48764-111">Қалған қажет ақпаратты енгізіп, **Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![Реттелетін баға өлшемдерінің шешімін жасау](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="48764-113">Баға өлшемі шешіміне барлық қажет нысандар мен қатысты құрамдастарды қосу</span><span class="sxs-lookup"><span data-stu-id="48764-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="48764-114">Баға шешіміне маңызды схемалық өзгертулерді енгізу үшін бағалық шешімге келесі Project Service нысандарын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="48764-115">Бұл процедураны аяқтағаннан кейін, нысандар бағалардың жаңа өлшемдерін таниды.</span><span class="sxs-lookup"><span data-stu-id="48764-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="48764-116">**Параметрлер** > **Шешімдер** тармағын басыңыз, содан кейін **<*your organization name*> баға өлшемдері** опциясын екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="48764-117">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Бар нысанды қосу** > **Нысандар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="48764-118">**Шешім құрамдастары** диалогтік терезесінде келесі нысандарды таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="48764-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="48764-119">**Нақты**</span><span class="sxs-lookup"><span data-stu-id="48764-119">**Actual**</span></span>
   - <span data-ttu-id="48764-120">**Резервтелетін ресурс**</span><span class="sxs-lookup"><span data-stu-id="48764-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="48764-121">**Болжам жолы**</span><span class="sxs-lookup"><span data-stu-id="48764-121">**Estimate Line**</span></span>
   - <span data-ttu-id="48764-122">**Жоба тапсырмасы**</span><span class="sxs-lookup"><span data-stu-id="48764-122">**Project Task**</span></span>
   - <span data-ttu-id="48764-123">**Есеп-шот жолы мәліметі**</span><span class="sxs-lookup"><span data-stu-id="48764-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="48764-124">**Журнал жолы**</span><span class="sxs-lookup"><span data-stu-id="48764-124">**Journal Line**</span></span>
   - <span data-ttu-id="48764-125">**Жобалық келісім-шарт жолы мәліметі**</span><span class="sxs-lookup"><span data-stu-id="48764-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="48764-126">**Жоба тобы мүшесі**</span><span class="sxs-lookup"><span data-stu-id="48764-126">**Project Team Member**</span></span>
   - <span data-ttu-id="48764-127">**Баға ұсыну жолының мәліметтері**</span><span class="sxs-lookup"><span data-stu-id="48764-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="48764-128">**Рөлдің үстеме бағасы**</span><span class="sxs-lookup"><span data-stu-id="48764-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="48764-129">**Рөл бағасы**</span><span class="sxs-lookup"><span data-stu-id="48764-129">**Role Price**</span></span>
   - <span data-ttu-id="48764-130">**Уақыт нысаны**</span><span class="sxs-lookup"><span data-stu-id="48764-130">**Time Entry**</span></span>
 
   ![Реттелетін баға белгілеу өлшемі шешіміне бұрыннан бар нысандарды қосу](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="48764-132">Әрбір нысан үшін қосылатын құрамдастарды және әрбір нысан үшін нысан активтерінің соңғы тізімін қарап шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="48764-133">Таңдалған нысандардың әрқайсысына барлық пішіндер мен көріністерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-133">Include all forms and views for each of the selected entities.</span></span>

  ![Қосылған нысандар](./media/solution-component-selection.png)


5.  <span data-ttu-id="48764-135">Таңдалған нысандар үшін кез келген тәуелді нысандарды қосу ұсынылған кезде, **Жоқ, қажетті құрамдастарды қоспау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="48764-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![Тәуелді нысандарды қосу](./media/Do-not-include-required.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]