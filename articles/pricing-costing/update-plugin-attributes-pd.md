---
title: Жаңа баға өлшемдерін қосылатын модуль төлсипаттарын жаңарту
description: Бұл тақырыпта бағалар өлшемдеріне арналған қосылатын модуль төлсипаттарын жаңарту жолдары туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 11/18/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 9b0cf48318d0b9e94c4be0d3775b54e83832c1b7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643225"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a><span data-ttu-id="bacfd-103">Жаңа баға өлшемдерін қосылатын модуль төлсипаттарын жаңарту</span><span class="sxs-lookup"><span data-stu-id="bacfd-103">Update plug-in attributes with new pricing dimensions</span></span>

<span data-ttu-id="bacfd-104">Бұл тақырыпта бағалар өлшемдеріне арналған қосылатын модуль төлсипаттарын жаңарту жолдары туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="bacfd-104">This topic provides information about how to update plug-in attributes for pricing dimensions.</span></span>

> [!NOTE]
> <span data-ttu-id="bacfd-105">Бұл тақырып Dynamics 365 Project Operations жүйесіндегі тек баға ұсыну мен келісім-шарт мүмкіндіктеріне қолданылады.</span><span class="sxs-lookup"><span data-stu-id="bacfd-105">This topic is only applicable to the quote and contract features in Dynamics 365 Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bacfd-106">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="bacfd-106">Prerequisites</span></span>
<span data-ttu-id="bacfd-107">Осы тақырыптағы қадамдарды орындамас бұрын, келесі тақырыптардағы процедураларды аяқтау қажет:</span><span class="sxs-lookup"><span data-stu-id="bacfd-107">Before you complete the steps in this topic, you must have completed the procedures in the following topics:</span></span>

  - [<span data-ttu-id="bacfd-108">Реттелетін өрістер мен нысандар жасау</span><span class="sxs-lookup"><span data-stu-id="bacfd-108">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md) 
  - [<span data-ttu-id="bacfd-109">Баға параметрлері мен транзакциялық нысандарға реттелетін өрістерді қосу </span><span class="sxs-lookup"><span data-stu-id="bacfd-109">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
  - <span data-ttu-id="bacfd-110">[Реттелетін өрістерді баға өлшемдері ретінде орнату](set-up-custom-fields-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="bacfd-110">[Set up custom fields as pricing dimensions](set-up-custom-fields-pricing-dimensions.md).</span></span> 
  
<span data-ttu-id="bacfd-111">Егер сіз бұл процедураларды орындамасаңыз, оларды орындап, содан кейін осы тақырыпқа оралыңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-111">If you haven't completed those procedures, complete them and then return to this topic.</span></span>

## <a name="register-a-plug-in"></a><span data-ttu-id="bacfd-112">Қосылатын модульді тіркеңіз</span><span class="sxs-lookup"><span data-stu-id="bacfd-112">Register a plug-in</span></span>
<span data-ttu-id="bacfd-113">Жобалық баға ұсыну жолы үшін **Баға ұсыну жолы** бетінде баға ұсыну жолы мәліметтері жасалғанда жүйе екі болжам жолын жасайды.</span><span class="sxs-lookup"><span data-stu-id="bacfd-113">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines.</span></span> <span data-ttu-id="bacfd-114">Бір жол болжамның құн тарапына, ал екінші жол сатылым тарапына арналған.</span><span class="sxs-lookup"><span data-stu-id="bacfd-114">One line is for the cost side of the estimate and the other line is for sales the side.</span></span> <span data-ttu-id="bacfd-115">Бұл жобаның келісім-шарт жолдары үшін бірдей.</span><span class="sxs-lookup"><span data-stu-id="bacfd-115">This is the same  for project contract lines.</span></span>

<span data-ttu-id="bacfd-116">Құн тарапындағы санға немесе өріске өзгеріс енгізген кезде, бұл өзгеріс сатылым тарапында да жасалады.</span><span class="sxs-lookup"><span data-stu-id="bacfd-116">When you make a change to the quantity or a field on the cost side, that change is also made on the sales side.</span></span> <span data-ttu-id="bacfd-117">Бұл мүмкін, себебі Quotelinedetail және келісімшарт жолының егжей-тегжейлі нысандарындағы PreOperation қосылатын модульдері шығындар тарапындағы нақты төлсипаттарды транзакцияның сатылым тарапына қосады.</span><span class="sxs-lookup"><span data-stu-id="bacfd-117">This is possible because the PreOperation plug-ins on Quotelinedetail and contractline detail entities connect specific attributes on the cost side to the sales side of the transaction.</span></span> <span data-ttu-id="bacfd-118">Егер сізге сатылым жағында баға өлшемдерінің мәндеріне өзгертулер енгізу қажет болса, сонымен қатар шығындар жағында жасалуы керек, баға өлшеміне өзгертулер енгізілгеннен кейін келесі қосылатын модульдер қайта тіркелуі керек.</span><span class="sxs-lookup"><span data-stu-id="bacfd-118">If you need changes made to the pricing dimension values on the sales side to also be made on the cost side, the following plug-ins must be re-registered after making changes to a pricing dimension.</span></span>

<span data-ttu-id="bacfd-119">Жаңартуға және қайта тіркеуге арналған қосылатын модульдер:</span><span class="sxs-lookup"><span data-stu-id="bacfd-119">These are the plug-ins to update and re-register:</span></span>

- <span data-ttu-id="bacfd-120">PreOperationContractLineDetailUpdate - **msdyn_orderlinetransaction жаңарту**</span><span class="sxs-lookup"><span data-stu-id="bacfd-120">PreOperationContractLineDetailUpdate - **Update msdyn_orderlinetransaction**</span></span>
- <span data-ttu-id="bacfd-121">PreOperationQuoteLineDetailUpdate - **msdyn_quotelinetransaction жаңартулары**</span><span class="sxs-lookup"><span data-stu-id="bacfd-121">PreOperationQuoteLineDetailUpdate - **Updates msdyn_quotelinetransaction**</span></span>

<span data-ttu-id="bacfd-122">Қосылатын модульдерді жаңарту және қайта тіркеу үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-122">Complete the following steps to update and re-register the plug-ins.</span></span>

1. <span data-ttu-id="bacfd-123">**PluginRegistrationTool** құралын ашып, Project Operations Dataverse ортасына қосылыңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-123">Open **PluginRegistrationTool** and connect to your Project Operations Dataverse environment.</span></span>
2. <span data-ttu-id="bacfd-124">**Іздеу** түймесін таңдап, жаңартылатын қосылатын модульдің алғашқы әріптерін теріңіз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-124">Select **Search**, and type in the first few letters of the plug-in to be updated.</span></span>
3. <span data-ttu-id="bacfd-125">Қосылатын модуль табылғаннан кейін оны таңдаңыз да, **Негізгі формада таңдау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-125">After the plug-in is found, select it, and then select **Select on Main Form**.</span></span>
4. <span data-ttu-id="bacfd-126">**msdyn_orderlinetransaction жаңарту** қадамын таңдаңыз да, тінтуірдің оң жақ түймешігімен басып, **Жаңарту** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-126">Select the **Update msdyn_orderlinetransaction** step, right-click, and then select **Update**.</span></span>
5. <span data-ttu-id="bacfd-127">**Жаңарту** диалогтік бетінде сүзгі төлсипаттарындағы көп нүктені (**…**) басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-127">In the **Update** dialog page, select the ellipsis (**...**) in the filtering attributes.</span></span>
6. <span data-ttu-id="bacfd-128">Төлсипаттардың сүзгі терезесі ашылады және ұйымдағы барлық төлсипаттар тізімін және баға өлшемдерін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="bacfd-128">The filtering attributes window opens and provides a list of all attributes in the entity and the pricing dimensions.</span></span> <span data-ttu-id="bacfd-129">Баға өлшемінің төлсипаттары үшін құсбелгілерді қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-129">Select the check boxes for the pricing dimension attributes.</span></span>
7. <span data-ttu-id="bacfd-130">Бетті жабу үшін **OK** түймешігін, содан кейін **Қадамды жаңарту** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-130">Select **OK** to close the page, and then select **Update Step**.</span></span>
8. <span data-ttu-id="bacfd-131">**PreOperationQuoteLineDetail** екінші қосылатын модуль үшін 2-7 қадамдарын қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-131">Repeat steps 2-7 for the second plug-in, **PreOperationQuoteLineDetail**.</span></span> <span data-ttu-id="bacfd-132">Осы қосылатын модуль үшін **msdyn_quotelinetransaction төлсипатын жаңарту** қадамын жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-132">For this plug-in, you need to update the **Update of msdyn_quotelinetransaction** step.</span></span>
9. <span data-ttu-id="bacfd-133">**PluginRegistrationTool** құралын жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="bacfd-133">Close **PluginRegistrationTool**.</span></span>
