---
title: Бағатізбе жасау
description: Project Service жүйесінде бағатізбе жасау жолы
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: bdd05aea-27a3-431d-9a80-2e220fb25e53
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 756af2fe3bc73d478b0355493aae6f0e49ac5835
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753155"
---
# <a name="create-a-price-list-project-service"></a><span data-ttu-id="8686c-103">Бағатізбе жасау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="8686c-103">Create a price list (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="8686c-104">Бағатізбелер баға ұсынулар мен жобалар жасауға тіркелгі менеджерлері пайдаланатын және жоба шығындарын анықтауға арналған үлгіні береді.</span><span class="sxs-lookup"><span data-stu-id="8686c-104">Price lists provide a template your account managers can use for creating quotes and projects, and for establishing the costs of a project.</span></span> <span data-ttu-id="8686c-105">Олар әркімнен алынатын рөлдер, шығыстар және баға жолы элементі тізімін береді.</span><span class="sxs-lookup"><span data-stu-id="8686c-105">They provide a line item list of roles and expenses, and the price you will charge for each.</span></span> <span data-ttu-id="8686c-106">Әр түрлі өнімдерді сату аудандары немесе сауда арналары үшін бөлек баға құрылымдарын пайдалану мақсатында бірнеше бағатізбе жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="8686c-106">You can create multiple price lists so that you can maintain separate price structures for different regions you sell your products in or for different sales channels.</span></span> <span data-ttu-id="8686c-107">Тұтынушыларға шот ұсыну жоспарланған әрбір валюта үшін кемінде бір бағатізбе жасау керек.</span><span class="sxs-lookup"><span data-stu-id="8686c-107">It’s a good idea to create at least one price list for every currency you plan to bill your customers in.</span></span>  
  
<span data-ttu-id="8686c-108">Көрсетілетін жұмыс үшін қаржылық болжамдар жасау үшін әрбір жобада қалдық құн және сатылым бағатізбесі бар-жоғын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="8686c-108">To create financial estimates for the work to be delivered, make sure every project has a backing cost and sales price list.</span></span> <span data-ttu-id="8686c-109">Ұйымда жасалған барлық жобаларға қолданылатын әдепкі құн және сатылым бағатізбесін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-109">Set up a default cost and sales pricelist that applies to all projects created in your organization.</span></span>  
  
<span data-ttu-id="8686c-110">Бағатізбелер рөлдер мен шығыс санаттарына бөлінеді, сол себепті бағатізбе жасау алдында пайдаланылуы керек рөлдер мен шығыс санаттары әлдеқашан теңшелуі керек.</span><span class="sxs-lookup"><span data-stu-id="8686c-110">Price lists rely on roles and expense categories, so before you create a price list, make sure you’ve already configured the roles and expense categories you want to use while creating the price list.</span></span>  
  
1.  <span data-ttu-id="8686c-111">**Project Service > Бағатізбелер** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="8686c-111">Go to **Project Service > Price Lists**.</span></span>  
  
2.  <span data-ttu-id="8686c-112">**Жаңа** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-112">Click **New**.</span></span>  
  
3.  <span data-ttu-id="8686c-113">**Мәтінмән** ішінен **Құн**, **Сатып алу** немесе **Сатылым** бағатізбесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-113">In **Context**, select whether this price list is for **Cost**, **Purchase**, or **Sales**.</span></span>  
  
4.  <span data-ttu-id="8686c-114">**Ат** ішіне бағатізбе атын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="8686c-114">In **Name**, enter a name for the price list.</span></span>  
  
5.  <span data-ttu-id="8686c-115">**Валюта** өрісінен шот ұсынуға немесе шығынға пайдаланылатын валютаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-115">In **Currency**, select the currency you’re going to use for billing or costing.</span></span>  
  
6.  <span data-ttu-id="8686c-116">**Уақыт бірлігі** өрісінде күн немесе сағат сияқты баға қолданылатын уақыт кезеңін көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="8686c-116">In **Time Unit**, specify the period of time the price applies to, such as day or hour.</span></span>  
  
7.  <span data-ttu-id="8686c-117">**Басталу күні**, **Аяқталу күні** және **Сипаттама** өрістерін қажетінше толтырыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-117">Fill in the **Start Date**, **End Date**, and **Description** as needed.</span></span>  
  
8.  <span data-ttu-id="8686c-118">Өңдеуді жалғастыра алу үшін жазбаны жасауға **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-118">Click **Save** to create the record so you can continue editing it.</span></span>  
  
9. <span data-ttu-id="8686c-119">Бағатізбеге рөл бағасын қосу үшін **+** түймешігін **Рөл бағалары** астынан басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-119">To add a role price to the price list, click **+** under **Role prices**.</span></span>  
  
10. <span data-ttu-id="8686c-120">**Рөл бағасы** тақтасында мәліметтерді толтырып, **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-120">In the **Role Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="8686c-121">Рөл бағаларын қосуды қажетінше жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-121">Continue adding role prices as necessary.</span></span> <span data-ttu-id="8686c-122">Орындалған кезде экранның төменгі оң жақ бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-122">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
11. <span data-ttu-id="8686c-123">Бағатізбеге шығыс санатының бағасын қосу үшін **+** түймешігін **Санат бағалары** астынан басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-123">To add an expense category price to the price list, click **+** under **Category prices**.</span></span>  
  
12. <span data-ttu-id="8686c-124">**Транзакция санаты бағасы** тақтасында мәліметтерді толтырып, **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-124">In the **Transaction Category Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="8686c-125">Санат бағаларын қосуды қажетінше жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-125">Continue adding category prices as necessary.</span></span> <span data-ttu-id="8686c-126">Орындалған кезде экранның төменгі оң жақ бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-126">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
13. <span data-ttu-id="8686c-127">Бағатізбеге бағатізбе элементтерін қосу үшін **+** түймешігін **Бағатізбе элементтері** астынан басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-127">To add price list items to the price list, click **+** under **Price List Items**.</span></span>  
  
14. <span data-ttu-id="8686c-128">**Бағатізбе элементі** тақтасында мәліметтерді толтырып, **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-128">In the **Price List Item** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="8686c-129">Бағатізбе элементтерін қосуды қажетінше жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-129">Continue adding price list items as necessary.</span></span> <span data-ttu-id="8686c-130">Орындалған кезде экранның төменгі оң жақ бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-130">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
15. <span data-ttu-id="8686c-131">Бағатізбеге аумақ қатынастарын қосу үшін **+** түймешігін **Аумақ қатынастары** астынан басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-131">To add territory relationships to the price list, click **+** under **Territory Relationships**.</span></span>  
  
16. <span data-ttu-id="8686c-132">**Жаңа байланыс** терезесінде мәліметтерді толтырып, **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-132">In the **New Connection** window, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="8686c-133">Аумақ қатынастарын қажетінше қосуды жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-133">Continue adding territory relationships as necessary.</span></span> <span data-ttu-id="8686c-134">Орындалған кезде экранның төменгі оң жақ бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8686c-134">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="8686c-135">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="8686c-135">See Also</span></span>  
 [<span data-ttu-id="8686c-136">Project Service Automation бағдарламасын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="8686c-136">Configure Project Service Automation</span></span>](../project-service/configure.md)
