---
title: Баға өлшемдеріне арналған реттелетін шешімдер жасау
description: Бұл бөлімде реттелетін баға өлшемдерін құру кезінде реттелетін шешімді құру жолы туралы түсіндіріледі.
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
ms.openlocfilehash: 1d8117d6f6bcedc97264401fc941470f34efb1ae
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284995"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="12e6c-103">Баға өлшемдеріне арналған реттелетін шешімдер жасау</span><span class="sxs-lookup"><span data-stu-id="12e6c-103">Create custom solutions for pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> <span data-ttu-id="12e6c-104">Реттелетін баға өлшемдерінің барлық өзгертулері бөлек шешімде болуы керек.</span><span class="sxs-lookup"><span data-stu-id="12e6c-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="12e6c-105">Осы маңызды үздік тәжірибе болашақта өзгерістерді қажетінше жаңарту немесе жою икемділігін қамтамасыз етеді, жұмысты қайта пайдалануға көмектеседі және осы өзгерістерді басқа данаға тасымалдауды жеңілдетеді.</span><span class="sxs-lookup"><span data-stu-id="12e6c-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="12e6c-106">Қажетті өзгерістерді жасағаннан кейін, осы шешімді **Басқарылатын шешім** ретінде экспорттап, баға белгілеу орнатуын қайтадан пайдалану үшін оны басқа даналарға импорттаңыз.</span><span class="sxs-lookup"><span data-stu-id="12e6c-106">After you make the required changes, export this solution as a **Managed solution**, and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="12e6c-107">**Параметрлер** > **Шешімдер** тармағын таңдап, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="12e6c-107">Select **Settings** > **Solutions**, and then select **New**.</span></span> 
2. <span data-ttu-id="12e6c-108">Шешімді **\<your organization name> бағалау өлшемдері** деп атап, қалған қажет ақпаратты енгізіңіз, содан кейін **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="12e6c-108">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>

> ![Баға белгілеу өлшемдеріне арналған реттелетін шешімді жасау](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="12e6c-110">Баға өлшемі шешіміне барлық қажет нысандар мен қатысты құрамдастарды қосу</span><span class="sxs-lookup"><span data-stu-id="12e6c-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="12e6c-111">Баға белгілеу шешіміне Project Service бағдарламасының келесі нысандарын қосу керек болады.</span><span class="sxs-lookup"><span data-stu-id="12e6c-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="12e6c-112">Нысандар жаңа баға белгілеу өлшемдері туралы хабардар болуы үшін, схемаға кейбір маңызды өзгерістерді енгізу үшін осы процедурадағы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="12e6c-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="12e6c-113">**Параметрлер** > **Шешімдер** тармағын таңдап, **\<your organization name> бағалау өлшемдері** түймешігін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="12e6c-113">Select **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="12e6c-114">Шешімдер жетекшісінде, сол жақ навигация тақтасында **Бар нысанды қосу** > **Нысандар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="12e6c-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="12e6c-115">**Шешім құрамдастары** диалогтік терезесінде келесі нысандарды таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="12e6c-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="12e6c-116">Нақты</span><span class="sxs-lookup"><span data-stu-id="12e6c-116">Actual</span></span>
- <span data-ttu-id="12e6c-117">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="12e6c-117">Bookable Resource</span></span>
- <span data-ttu-id="12e6c-118">Болжам жолы</span><span class="sxs-lookup"><span data-stu-id="12e6c-118">Estimate Line</span></span>
- <span data-ttu-id="12e6c-119">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="12e6c-119">Project Task</span></span>
- <span data-ttu-id="12e6c-120">Есеп-шот жолы мәліметі</span><span class="sxs-lookup"><span data-stu-id="12e6c-120">Invoice Line Detail</span></span>
- <span data-ttu-id="12e6c-121">Журнал жолы</span><span class="sxs-lookup"><span data-stu-id="12e6c-121">Journal Line</span></span>
- <span data-ttu-id="12e6c-122">Жобалық келісім-шарт жолы мәліметі</span><span class="sxs-lookup"><span data-stu-id="12e6c-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="12e6c-123">Жоба тобы мүшесі</span><span class="sxs-lookup"><span data-stu-id="12e6c-123">Project Team Member</span></span>
- <span data-ttu-id="12e6c-124">Баға ұсыну жолының мәліметтері</span><span class="sxs-lookup"><span data-stu-id="12e6c-124">Quote Line Detail</span></span>
- <span data-ttu-id="12e6c-125">Рөлдің үстеме бағасы</span><span class="sxs-lookup"><span data-stu-id="12e6c-125">Role Price Markup</span></span>
- <span data-ttu-id="12e6c-126">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="12e6c-126">Role Price</span></span> 
- <span data-ttu-id="12e6c-127">Уақыт жазбасы</span><span class="sxs-lookup"><span data-stu-id="12e6c-127">Time Entry</span></span> 

> ![Баға белгілеу өлшемі шешіміне бұрыннан бар нысандарды қосу](media/Existing-entities-to-PD-solution.png)

> ![Шешім құрамдастарын таңдау](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="12e6c-130">Таңдалған нысандардың әрқайсысына барлық пішіндер мен көріністерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="12e6c-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="12e6c-131">Таңдалған нысандарға қандай да бір тәуелді нысандарды қосу сұралған кезде, **Жоқ** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="12e6c-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![Барлық қатысты құрамдастарды қоспаңыз](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]