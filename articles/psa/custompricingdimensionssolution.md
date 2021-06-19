---
title: Баға өлшемдеріне арналған реттелетін шешімдер жасау
description: Бұл бөлімде реттелетін баға өлшемдерін құру кезінде реттелетін шешімді құру жолы туралы түсіндіріледі.
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
ms.openlocfilehash: ae7f22b9cb092e956d0f1eaf1f1997c8e97392f4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012323"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="dd92a-103">Баға өлшемдеріне арналған реттелетін шешімдер жасау</span><span class="sxs-lookup"><span data-stu-id="dd92a-103">Create custom solutions for pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> <span data-ttu-id="dd92a-104">Реттелетін баға өлшемдерінің барлық өзгертулері бөлек шешімде болуы керек.</span><span class="sxs-lookup"><span data-stu-id="dd92a-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="dd92a-105">Осы маңызды үздік тәжірибе болашақта өзгерістерді қажетінше жаңарту немесе жою икемділігін қамтамасыз етеді, жұмысты қайта пайдалануға көмектеседі және осы өзгерістерді басқа данаға тасымалдауды жеңілдетеді.</span><span class="sxs-lookup"><span data-stu-id="dd92a-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="dd92a-106">Қажетті өзгерістерді жасағаннан кейін, осы шешімді **Басқарылатын шешім** ретінде экспорттап, баға белгілеу орнатуын қайтадан пайдалану үшін оны басқа даналарға импорттаңыз.</span><span class="sxs-lookup"><span data-stu-id="dd92a-106">After you make the required changes, export this solution as a **Managed solution**, and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="dd92a-107">**Параметрлер** > **Шешімдер** тармағын таңдап, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dd92a-107">Select **Settings** > **Solutions**, and then select **New**.</span></span> 
2. <span data-ttu-id="dd92a-108">Шешімді **\<your organization name> бағалау өлшемдері** деп атап, қалған қажет ақпаратты енгізіңіз, содан кейін **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dd92a-108">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>

> ![Баға белгілеу өлшемдеріне арналған реттелетін шешімді жасау](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="dd92a-110">Баға өлшемі шешіміне барлық қажет нысандар мен қатысты құрамдастарды қосу</span><span class="sxs-lookup"><span data-stu-id="dd92a-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="dd92a-111">Баға белгілеу шешіміне Project Service бағдарламасының келесі нысандарын қосу керек болады.</span><span class="sxs-lookup"><span data-stu-id="dd92a-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="dd92a-112">Нысандар жаңа баға белгілеу өлшемдері туралы хабардар болуы үшін, схемаға кейбір маңызды өзгерістерді енгізу үшін осы процедурадағы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="dd92a-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="dd92a-113">**Параметрлер** > **Шешімдер** тармағын таңдап, **\<your organization name> бағалау өлшемдері** түймешігін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="dd92a-113">Select **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="dd92a-114">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Бар нысанды қосу** > **Нысандар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dd92a-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="dd92a-115">**Шешім құрамдастары** диалогтік терезесінде келесі нысандарды таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="dd92a-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="dd92a-116">Нақты</span><span class="sxs-lookup"><span data-stu-id="dd92a-116">Actual</span></span>
- <span data-ttu-id="dd92a-117">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="dd92a-117">Bookable Resource</span></span>
- <span data-ttu-id="dd92a-118">Болжам жолы</span><span class="sxs-lookup"><span data-stu-id="dd92a-118">Estimate Line</span></span>
- <span data-ttu-id="dd92a-119">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="dd92a-119">Project Task</span></span>
- <span data-ttu-id="dd92a-120">Есеп-шот жолы мәліметі</span><span class="sxs-lookup"><span data-stu-id="dd92a-120">Invoice Line Detail</span></span>
- <span data-ttu-id="dd92a-121">Журнал жолы</span><span class="sxs-lookup"><span data-stu-id="dd92a-121">Journal Line</span></span>
- <span data-ttu-id="dd92a-122">Жобалық келісім-шарт жолы мәліметі</span><span class="sxs-lookup"><span data-stu-id="dd92a-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="dd92a-123">Жоба тобы мүшесі</span><span class="sxs-lookup"><span data-stu-id="dd92a-123">Project Team Member</span></span>
- <span data-ttu-id="dd92a-124">Баға ұсыну жолының мәліметтері</span><span class="sxs-lookup"><span data-stu-id="dd92a-124">Quote Line Detail</span></span>
- <span data-ttu-id="dd92a-125">Рөлдің үстеме бағасы</span><span class="sxs-lookup"><span data-stu-id="dd92a-125">Role Price Markup</span></span>
- <span data-ttu-id="dd92a-126">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="dd92a-126">Role Price</span></span> 
- <span data-ttu-id="dd92a-127">Уақыт жазбасы</span><span class="sxs-lookup"><span data-stu-id="dd92a-127">Time Entry</span></span> 

> ![Баға белгілеу өлшемі шешіміне бұрыннан бар нысандарды қосу](media/Existing-entities-to-PD-solution.png)

> ![Шешім құрамдастарын таңдау](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="dd92a-130">Таңдалған нысандардың әрқайсысына барлық пішіндер мен көріністерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="dd92a-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="dd92a-131">Таңдалған нысандарға қандай да бір тәуелді нысандарды қосу сұралған кезде, **Жоқ** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="dd92a-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![Барлық қатысты құрамдастарды қоспаңыз](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]