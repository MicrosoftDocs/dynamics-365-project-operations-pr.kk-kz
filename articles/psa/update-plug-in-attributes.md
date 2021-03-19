---
title: Жаңа бағалар өлшемдерін қосу үшін қосылатын модуль атрибуттарын жаңарту
description: Бұл тақырыпта бағалар өлшемдеріне арналған қосылатын модуль атрибуттарын жаңарту туралы ақпарат берілген.
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: project-operations
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 958646c9e06a15e265bc0caa8b0f3eb9f79fc347
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281800"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a><span data-ttu-id="8d8a3-103">Жаңа бағалар өлшемдерін қосу үшін қосылатын модуль атрибуттарын жаңарту</span><span class="sxs-lookup"><span data-stu-id="8d8a3-103">Update plug-in attributes to include new pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!NOTE]
> <span data-ttu-id="8d8a3-104">Егер Project Service Automation (PSA) баға ұсыну және келісім-шарт мүмкіндіктерін пайдаланбасаңыз, осы тақырыпты өткізіп жіберуге болады.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-104">If you are not using the Project Service Automation (PSA) Quoting and Contracting features, you can skip this topic.</span></span>

<span data-ttu-id="8d8a3-105">Бұл тақырыпта [Реттелетін өрістер мен нысандарды жасау](create-custom-fields-entities.md), [Бағаны орнату және транзакциялық нысандарға реттелетін өрістер қосу](field-references.md) және [Реттелетін өрістерді бағалар өлшемдері ретінде орнату](set-up-pricing-dimensions.md) тақырыптарындағы процедуралар орындалды деп саналады.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-105">This topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md), [Add custom fields to price setup and transactional entities](field-references.md), and [Set up custom fields as pricing dimensions](set-up-pricing-dimensions.md).</span></span> <span data-ttu-id="8d8a3-106">Егер сіз бұл процедураларды орындамасаңыз, кері қайтып, оларды орындаңыз, содан кейін осы тақырыпқа оралыңыз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span>

<span data-ttu-id="8d8a3-107">Жобаның баға ұсыну жолына арналған **Баға ұсыну жолы** бетінде баға ұсыну жолының мәліметі жасалған кезде, жүйе фондық режимде екі болжам жолын жасайды - біреуі болжамның құн тарапы үшін, ал екіншісі сатылым тарапы үшін.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-107">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines in the background -- one line for the cost side of the estimate and one for sales side.</span></span> <span data-ttu-id="8d8a3-108">Бұл жобаның келісім-шарт жолдары үшін бірдей.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-108">This is the same  for project contract lines.</span></span>

<span data-ttu-id="8d8a3-109">Құн тарапындағы санға немесе өріске өзгеріс енгізген кезде, бұл өзгеріс сатылып тарапына таратылады.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-109">When you make a change to the quantity or a field on the cost side, that change is propagated to the sales side.</span></span> <span data-ttu-id="8d8a3-110">Бағалар өлшемдеріне өзгеріс енгізілгеннен кейін қайта тіркелуі қажет келесі қосылатын модульдер себеп болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-110">This is possible because of the following plug-ins that must be re-registered after a change to pricing dimensions.</span></span>

- <span data-ttu-id="8d8a3-111">PreOperationContractLineDetailUpdate - жаңартулар **msdyn_orderlinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span></span>
- <span data-ttu-id="8d8a3-112">PreOperationQuoteLineDetailUpdate - Жаңартулар **msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span></span>

<span data-ttu-id="8d8a3-113">Келесі қадамдар сізге қосылатын модульдерді тіркеу процесін түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-113">The following steps walk you through the process of registering the plug-ins.</span></span>

1. <span data-ttu-id="8d8a3-114">**PluginRegistrationTool** құралын ашып, онлайн данаға қосылыңыз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-114">Open the **PluginRegistrationTool** and connect to your online instance.</span></span>
2. <span data-ttu-id="8d8a3-115">**Іздеу** түймешігін басып, жаңарту қажет қосылатын модульді іздеңіз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-115">Click **Search** and search for the plug-in to be updated.</span></span>

 ![Іздеу тармағының скриншоты](media/PRT-1.png)

3. <span data-ttu-id="8d8a3-117">Қосылатын модуль табылғаннан кейін оны таңдаңыз да, **Негізгі формада таңдау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-117">After the plug-in is found, select it and then click **Select on Main Form**.</span></span>

4. <span data-ttu-id="8d8a3-118">Жаңарту қажет қосылатын модульдің қадамын таңдап, тінтуірдің оң жақ түймешігімен басып, **Жаңарту** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-118">Select the step of the plug-in to be updated, right-click, and then select **Update**.</span></span>

 ![Жаңарту қажет қосылатын модульдің скриншоты](media/PRT-2.png)
 
5. <span data-ttu-id="8d8a3-120">Жаңарту терезесінде сүзгі атрибуттарындағы көп нүктені ( **...**) басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-120">In the update window, click the ellipsis (**...**) in the filtering attributes.</span></span>

 ![Қадам конфигурациясы туралы ақпаратты жаңарту скриншоты](media/PRT-3.png)
 
6. <span data-ttu-id="8d8a3-122">Баға атрибутының ұяшықтарына құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-122">Select the pricing attribute check boxes.</span></span>

 ![Баға атрибуттарына арналған құсбелгі таңдауы көрсетілген скриншот](media/PRT-4.png)

7. <span data-ttu-id="8d8a3-124">Бетті жабу үшін **OK** түймешігін, содан кейін **Қадамды жаңарту** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-124">Click **OK** to close the page and then select **Update Step**.</span></span>

 !["Жаңарту қадамы" түймешігі көрсетілген скриншот](media/PRT-5.png)
 
8. <span data-ttu-id="8d8a3-126">Бұл процесті екінші қосылатын модуль үшін қайталаңыз, **PreOperationQuoteLineDetail - msdyn_quotelinetransaction жаңартуы**.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-126">Repeat this process for the second plug-in, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span></span>

9. <span data-ttu-id="8d8a3-127">Plug-in Registration Tool құралын жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="8d8a3-127">Close the plug-in registration tool.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]