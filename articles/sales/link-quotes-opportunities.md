---
title: Мүмкіндіктерден жоба баға ұсыныстарын жасау
description: Бұл тақырыпта мүмкіндіктен жобалық баға ұсынысын жасау жөнінде ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 606098473db479d0015e3a7a3c01a3d3b6de9db1
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898539"
---
# <a name="create-project-quotes-from-opportunities"></a><span data-ttu-id="6bf41-103">Мүмкіндіктерден жоба баға ұсыныстарын жасау</span><span class="sxs-lookup"><span data-stu-id="6bf41-103">Create project quotes from opportunities</span></span>

<span data-ttu-id="6bf41-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="6bf41-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6bf41-105">Баға ұсыныстарын жоба мүмкіндіктерінен келесі жолдармен жасауға болады:</span><span class="sxs-lookup"><span data-stu-id="6bf41-105">Quotes can be created from project opportunities in the following ways:</span></span>

- <span data-ttu-id="6bf41-106">**Жоба мүмкіндігі** бетіндегі **Баға ұсыныстары** қойыншасынан</span><span class="sxs-lookup"><span data-stu-id="6bf41-106">From the **Quotes** tab on the **Project Opportunity** page</span></span>
- <span data-ttu-id="6bf41-107">Мүмкіндік сатылымының процестік ағынан</span><span class="sxs-lookup"><span data-stu-id="6bf41-107">From the Opportunity sales process flow</span></span>
- <span data-ttu-id="6bf41-108">Қолданыстағы баға ұсынысы бойынша мүмкіндік анықтамасын жаңарту арқылы</span><span class="sxs-lookup"><span data-stu-id="6bf41-108">By updating the opportunity reference on an existing quote</span></span>

## <a name="from-the-quotes-tab-of-the-project-opportunity-page"></a><span data-ttu-id="6bf41-109">Жоба мүмкіндігі бетінің Баға ұсыныстары қойыншасынан</span><span class="sxs-lookup"><span data-stu-id="6bf41-109">From the Quotes tab of the Project Opportunity page</span></span>

<span data-ttu-id="6bf41-110">Мүмкіндіктен жоба ұсынысын жасау үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-110">To create a project quote from an opportunity, complete the following steps.</span></span>

1. <span data-ttu-id="6bf41-111">**Жоба мүмкіндігі** бетін ашып, **Баға ұсыныстары** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-111">Open the **Project Opportunity** page and select the **Quotes** tab.</span></span> 
2. <span data-ttu-id="6bf41-112">**Баға ұсыныстары** ішкі торында мүмкіндікке негізделген жаңа жоба баға ұсынысын жасау үшін **+** таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-112">On the **Quotes** sub-grid, select the **+** to create a new project quote based on the opportunity.</span></span> <span data-ttu-id="6bf41-113">Барлық мүмкіндік жолдары мен байланысты жобаның бағатізбелері мүмкіндіктің жаңа баға ұсынысына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="6bf41-113">All of the opportunity lines and related Project price lists are copied to the new quote from the opportunity.</span></span>

## <a name="from-the-opportunity-sales-process-flow"></a><span data-ttu-id="6bf41-114">Мүмкіндік сатылымының процестік ағынан</span><span class="sxs-lookup"><span data-stu-id="6bf41-114">From the Opportunity sales process flow</span></span>

<span data-ttu-id="6bf41-115">Мүмкіндік сатылымының процестік ағынынан баға ұсынысын жасау үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-115">To create a quote from the Opportunity sales process flow, complete the following steps.</span></span>

1. <span data-ttu-id="6bf41-116">Мүмкіндік сатылымының процестік ағынынан мүмкіндікті ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-116">From the Opportunity sales process flow, open the Opportunity.</span></span>
2. <span data-ttu-id="6bf41-117">**Нақтылау** кезеңін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-117">Select the **Qualify** stage.</span></span> 
3. <span data-ttu-id="6bf41-118">Жаңа баға ұсынысын жасау үшін **Келесі**, содан соң **+ Жасау** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-118">Select **Next** and then select **+ Create** to create a new quote.</span></span> <span data-ttu-id="6bf41-119">Осы жаңа баға ұсынысының **Жиынтық** қойыншасындағы ақпараттың бөлігі әдепкі бойынша мүмкіндіктен жойылады.</span><span class="sxs-lookup"><span data-stu-id="6bf41-119">Most of the information on the **Summary** tab for this new quote will have defaulted from the opportunity.</span></span> 
4. <span data-ttu-id="6bf41-120">Қолданыста жоқ кез-келген қажетті ақпаратты енгізіңіз немесе **Жиынтық** қойыншасында қажетінше әдепкі мәндерді жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-120">Enter in any required information that is missing, or update defaulted values as necessary on the **Summary** tab,</span></span>
5. <span data-ttu-id="6bf41-121">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-121">Select **Save**.</span></span> <span data-ttu-id="6bf41-122">Жаға баға ұсынысы жасалып, мүмкіндікке байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="6bf41-122">The new quote is created and associated to the opportunity.</span></span> <span data-ttu-id="6bf41-123">**Мүмкіндік** бетінің **Баға ұсыныстары** қойыншасында баға ұсынысы ақпаратын қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="6bf41-123">You can now view the quote information on the **Quotes** tab of the **Opportunity** page.</span></span> 

   <span data-ttu-id="6bf41-124">Мүмкіндік сатылымы процесі **Ұсына** келесі кезеңіне өтеді.</span><span class="sxs-lookup"><span data-stu-id="6bf41-124">The Opportunity sales process moves to the next stage, **Propose**.</span></span>


## <a name="by-updating-the-opportunity-reference-on-an-existing-quote"></a><span data-ttu-id="6bf41-125">Қолданыстағы баға ұсынысы бойынша мүмкіндік анықтамасын жаңарту арқылы</span><span class="sxs-lookup"><span data-stu-id="6bf41-125">By updating the opportunity reference on an existing quote</span></span>

<span data-ttu-id="6bf41-126">Қолданыстағы баға ұсынысын мүмкіндікпен байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="6bf41-126">An existing quote can be linked to an Opportunity.</span></span> <span data-ttu-id="6bf41-127">Қолданыстағы баға ұсынысында мүмкіндік ақпаратын жаңарту үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-127">Complete the following steps to update the Opportunity information on an existing quote.</span></span>

1. <span data-ttu-id="6bf41-128">**Баға ұсынысы** бетін ашып, **Жиынтық** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-128">Open the **Quote** page and select the **Summary** tab.</span></span>
2. <span data-ttu-id="6bf41-129">**Мүмкіндік** өрісінде баға ұсынысын байланыстыру қажет мүмкіндікті таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-129">In the **Opportunity** field, select the opportunity that you want to link to the quote.</span></span> <span data-ttu-id="6bf41-130">Баға ұсынысын мүмкіндіктің **Баға ұсыныстары** торында қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="6bf41-130">You can see the quote in the **Quotes** grid of the Opportunity.</span></span> 
3. <span data-ttu-id="6bf41-131">Мүмкіндік сатылымы процесі арқылы мүмкіндікті келесі **Ұсыну** кезеңіне ауыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="6bf41-131">Using the Opportunity sales process, the opportunity can be moved to the next stage, **Propose**.</span></span> 

   <span data-ttu-id="6bf41-132">Мүмкіндікті осы кезеңге ауыстырған кезде, сіз осы баға ұсынысын осы мүмкіндікке байланысты баға ұсыныстары тізімінен таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-132">When you move an opportunity to this stage, you can select this quote from a list of quotes associated with this opportunity.</span></span> <span data-ttu-id="6bf41-133">Бұл баға ұсынысын таңдау сіз онымен ілгері жылжитыныңызды білдіреді.</span><span class="sxs-lookup"><span data-stu-id="6bf41-133">Selecting this quote indicates that you're moving forward with it.</span></span>

   <span data-ttu-id="6bf41-134">Мүмкіндікке қатысты барлық басқа сілтемелер олардың біреуі жеңіске жеткенше қолжетімді және белсенді болады.</span><span class="sxs-lookup"><span data-stu-id="6bf41-134">All the other quotes associated with the Opportunity will still be available and active until one of them is won.</span></span> <span data-ttu-id="6bf41-135">Сіз сату процесін алдыңғы **Нақтылау** кезеңіне ауыстыра аласыз және алға жылжу үшін тағы бір баға ұсынысын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6bf41-135">You can move the sales process back to the previous stage **Qualify**, and pick another quote to move forward with.</span></span>
