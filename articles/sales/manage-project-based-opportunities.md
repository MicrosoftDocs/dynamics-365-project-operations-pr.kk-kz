---
title: Жобаға негізделген мүмкіндіктерді басқару
description: Бұл тақырыпта жобаларға қатысты мүмкіндіктермен жұмыс істеу туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5ce9ad1458d338d63469c3d6fddb98b9cbbced31
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948427"
---
# <a name="manage-project-based-opportunities"></a><span data-ttu-id="e5924-103">Жобаға негізделген мүмкіндіктерді басқару</span><span class="sxs-lookup"><span data-stu-id="e5924-103">Manage project-based opportunities</span></span>

<span data-ttu-id="e5924-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="e5924-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e5924-105">Жобаға негізделген компаниялар, әдетте, жеткізу операцияларын көптеген елдер мен географиялық аймақтарға таратады.</span><span class="sxs-lookup"><span data-stu-id="e5924-105">Project-based companies typically have their operations for delivery spread across multiple countries and geographies.</span></span> <span data-ttu-id="e5924-106">Жобаны орындау және жеткізу құны географиялық аймақтың немесе бөлімнің жеткізуді басқаруына байланысты әртүрлі болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e5924-106">The cost of the project execution and delivery can vary  based on which geography or division manages the delivery.</span></span> <span data-ttu-id="e5924-107">Өз кезегінде, бұл мәміленің маржасына әсер етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e5924-107">In turn, this can impact the margins of the deal.</span></span> <span data-ttu-id="e5924-108">Жобаға негізделген қызметтерді жеткізу, әдетте, адам ресурстарына көп уақытты, іссапар шығындарын, материалдық шығындарды және басқа шығындарды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="e5924-108">Delivery of project-based services typically involves large quantities of human resource time, considerable expenses for travel, material costs, and other expenses.</span></span>

<span data-ttu-id="e5924-109">Dynamics 365 Project Operations бағдарламасындағы жобаға негізделген мүмкіндіктер Dynamics 365 Sales кеңейтімдерімен жасалған.</span><span class="sxs-lookup"><span data-stu-id="e5924-109">Project-based opportunities in Dynamics 365 Project Operations are designed with extensions to Dynamics 365 Sales.</span></span> <span data-ttu-id="e5924-110">Тақырыпта жобаға негізделген компаниялар жобаға негізделген мүмкіндіктерді басқаруды талап ететін қосымша функцияға енгізілген әртүрлі өрістер мен бизнес-логика туралы мәліметтер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="e5924-110">The topic provides details about the different fields and business logic included in the additional functionality that is required by project-based companies to manage project-based opportunities.</span></span>

## <a name="view-all-project-based-opportunities"></a><span data-ttu-id="e5924-111">Жобаға негізделген барлық мүмкіндіктерді қарау</span><span class="sxs-lookup"><span data-stu-id="e5924-111">View all project-based opportunities</span></span>

<span data-ttu-id="e5924-112">Жобаға негізделген барлық мүмкіндіктердің тізімін **Мүмкіндік** тізім бетінен көруге болады.</span><span class="sxs-lookup"><span data-stu-id="e5924-112">A list of all the project-based opportunities can be seen from the **Opportunity** list page.</span></span> 

1. <span data-ttu-id="e5924-113">**Сатылым** > **Мүмкіндіктер** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="e5924-113">Go to **Sales** > **Opportunities**.</span></span>
2. <span data-ttu-id="e5924-114">Мүмкіндіктердің басқа сүзгіленген көріністерін таңдау үшін **Көрініс ауыстыру құралы** параметрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-114">Use the **View switcher** to select other filtered views of the opportunities.</span></span> <span data-ttu-id="e5924-115">Осы көріністер мен навигация параметрлерін конфигурациялау үшін реттелетін сүзгі шарттарымен өз көріністеріңізді жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-115">You can create your own views with custom filter criteria to configure these views and navigation options.</span></span>

<span data-ttu-id="e5924-116">Жоба мүмкіндіктерін осы тізім бетінен немесе мәліметтер бетінен жасауға немесе жоюға болады.</span><span class="sxs-lookup"><span data-stu-id="e5924-116">Project Opportunities can be created or deleted from this list page or the detail page.</span></span>

## <a name="business-process-flow-for-project-based-deals"></a><span data-ttu-id="e5924-117">Жобаға негізделген мәмілелерге арналған бизнес процесінің ағыны</span><span class="sxs-lookup"><span data-stu-id="e5924-117">Business process flow for project-based deals</span></span>

<span data-ttu-id="e5924-118">Келесі бизнес процесінің ағындарына Project Operations ішіндегі жобаға негізделген мәмілелер үшін қолдау көрсетіледі:</span><span class="sxs-lookup"><span data-stu-id="e5924-118">The following business process flows are supported for project-based deals in Project Operations:</span></span>

- <span data-ttu-id="e5924-119">Ықтимал тұтынушы бизнес процесі</span><span class="sxs-lookup"><span data-stu-id="e5924-119">Lead to Opportunity business process</span></span>
- <span data-ttu-id="e5924-120">Мүмкіндік сатылымдар процесі</span><span class="sxs-lookup"><span data-stu-id="e5924-120">Opportunity sales process</span></span>

### <a name="lead-to-opportunity-business-process"></a><span data-ttu-id="e5924-121">Ықтимал тұтынушы - мүмкіндік бизнес процесі</span><span class="sxs-lookup"><span data-stu-id="e5924-121">Lead to opportunity business process</span></span> 
<span data-ttu-id="e5924-122">Ықтимал тұтынушы - мүмкіндік бизнес-процесі келесі кезеңдерді қолдайды:</span><span class="sxs-lookup"><span data-stu-id="e5924-122">The lead to opportunity business process supports the following stages:</span></span>

| <span data-ttu-id="e5924-123">Кезең</span><span class="sxs-lookup"><span data-stu-id="e5924-123">Stage</span></span> | <span data-ttu-id="e5924-124">Салыстырылған нысан</span><span class="sxs-lookup"><span data-stu-id="e5924-124">Mapped entity</span></span> | <span data-ttu-id="e5924-125">Функционалдылық</span><span class="sxs-lookup"><span data-stu-id="e5924-125">Functionality</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e5924-126">Сапа</span><span class="sxs-lookup"><span data-stu-id="e5924-126">Qualify</span></span> | <span data-ttu-id="e5924-127">Ықтимал тұтынушы</span><span class="sxs-lookup"><span data-stu-id="e5924-127">Lead</span></span> | <span data-ttu-id="e5924-128">Тіркелгіні, контактіні және мүмкіндікті жасау үшін ықтимал тұтынушыны нақтылаңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-128">Qualify the lead to create an account, contact, and an opportunity.</span></span> |
| <span data-ttu-id="e5924-129">Жақсарту</span><span class="sxs-lookup"><span data-stu-id="e5924-129">Develop</span></span> | <span data-ttu-id="e5924-130">Мүмкіндік</span><span class="sxs-lookup"><span data-stu-id="e5924-130">Opportunity</span></span> | <span data-ttu-id="e5924-131">Істелген жұмыс, негізгі пай иелері және бәсекелестік туралы қосымша ақпарат қосу мүмкіндігін әзірлеу.</span><span class="sxs-lookup"><span data-stu-id="e5924-131">Develop the opportunity to add more information on the work involved, key stakeholders, and competition.</span></span> |
| <span data-ttu-id="e5924-132">Ұсыну</span><span class="sxs-lookup"><span data-stu-id="e5924-132">Propose</span></span> | <span data-ttu-id="e5924-133">Мүмкіндік</span><span class="sxs-lookup"><span data-stu-id="e5924-133">Opportunity</span></span> | <span data-ttu-id="e5924-134">Ұсыныс әзірлеп, ішкі сараптау тобынан растау алыңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-134">Develop the proposal and get approval from the internal review team.</span></span> |
| <span data-ttu-id="e5924-135">Жабу</span><span class="sxs-lookup"><span data-stu-id="e5924-135">Close</span></span> | <span data-ttu-id="e5924-136">Мүмкіндік</span><span class="sxs-lookup"><span data-stu-id="e5924-136">Opportunity</span></span> | <span data-ttu-id="e5924-137">Мәмілені жабу үшін мүмкіндікті ұтыңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-137">Win the opportunity to close the deal.</span></span> |

### <a name="opportunity-sales-process"></a><span data-ttu-id="e5924-138">Мүмкіндік сатылымдар процесі</span><span class="sxs-lookup"><span data-stu-id="e5924-138">Opportunity sales process</span></span>
<span data-ttu-id="e5924-139">Project Operations бағдарламасындағы мүмкіндікті сату процесі - бұл Сатылымдар бағдарламасындағы Мүмкіндіктерді сату процесінің бизнес ағынының кеңеюі.</span><span class="sxs-lookup"><span data-stu-id="e5924-139">The Opportunity sales process in Project Operations is an extension to the Opportunity sales process business flow in the Sales application.</span></span> <span data-ttu-id="e5924-140">Бұл бизнес-процес жобаға негізделген мүмкіндіктің келесі кезеңдерін қолдауға арналған.</span><span class="sxs-lookup"><span data-stu-id="e5924-140">This business process is designed out-of-the-box to support the following stages in a project-based opportunity.</span></span>

| <span data-ttu-id="e5924-141">Кезең</span><span class="sxs-lookup"><span data-stu-id="e5924-141">Stage</span></span> | <span data-ttu-id="e5924-142">Салыстырылған нысан</span><span class="sxs-lookup"><span data-stu-id="e5924-142">Mapped entity</span></span> | <span data-ttu-id="e5924-143">Функционалдылық</span><span class="sxs-lookup"><span data-stu-id="e5924-143">Functionality</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e5924-144">Сапа</span><span class="sxs-lookup"><span data-stu-id="e5924-144">Qualify</span></span> | <span data-ttu-id="e5924-145">Мүмкіндік</span><span class="sxs-lookup"><span data-stu-id="e5924-145">Opportunity</span></span> | <span data-ttu-id="e5924-146">Тіркелгіні, контактіні және мүмкіндікті жасау үшін ықтимал тұтынушыны нақтылаңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-146">Qualify the lead to create an account, contact, and an opportunity.</span></span> |
| <span data-ttu-id="e5924-147">Ұсыну</span><span class="sxs-lookup"><span data-stu-id="e5924-147">Propose</span></span> | <span data-ttu-id="e5924-148">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="e5924-148">Quote</span></span> | <span data-ttu-id="e5924-149">Жобаның баға ұсынысы арқылы ұсыныс әзірлеп, ішкі сараптау тобынан растау алыңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-149">Develop the proposal using project quotes and get approval from the internal review team.</span></span> |
| <span data-ttu-id="e5924-150">Келісім-шарт</span><span class="sxs-lookup"><span data-stu-id="e5924-150">Contract</span></span> | <span data-ttu-id="e5924-151">Жоба келісім-шарты</span><span class="sxs-lookup"><span data-stu-id="e5924-151">Project Contract</span></span> | <span data-ttu-id="e5924-152">Келісім-шартты құру үшін баға ұсынысын ұтып алып, жобаны орындауды және жеткізуді бастаңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-152">Win the quote to create the contract and begin execution and delivery on the project.</span></span> |
| <span data-ttu-id="e5924-153">Жабу</span><span class="sxs-lookup"><span data-stu-id="e5924-153">Close</span></span> | <span data-ttu-id="e5924-154">Жоба келісім-шарты</span><span class="sxs-lookup"><span data-stu-id="e5924-154">Project Contract</span></span> | <span data-ttu-id="e5924-155">Жұмысты сәтті аяқтаңыз және жоба келісім-шартын жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-155">Finish the work successfully and close the project contract.</span></span> |

> [!NOTE]
> <span data-ttu-id="e5924-156">Жобаға негізделген мәміле ықтимал тұтынушыдан басталса, ықтимал тұтынушы - мүмкіндік бизнес-процесі басым болады.</span><span class="sxs-lookup"><span data-stu-id="e5924-156">If your project-based deal started with a Lead, the Lead to Opportunity business process takes precedence.</span></span>
>
> <span data-ttu-id="e5924-157">Жобаға негізделген мәміле мүмкіндіктен басталса, мүмкіндік сатылымдары бизнес-процесі басым болады.</span><span class="sxs-lookup"><span data-stu-id="e5924-157">If your project-based deal started with an Opportunity, the Opportunity sales process takes precedence.</span></span>

<span data-ttu-id="e5924-158">Өнімнің бизнес процесінің ағынын өңдей аласыз немесе қажет болған жағдайда сатылым процесін қадағалау үшін өз бизнес процесіңіздің ағындарын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-158">You can edit the product business process flow or create your own business process flows to track your sales process as needed.</span></span> <span data-ttu-id="e5924-159">Бизнес процесінің ағындары туралы қосымша ақпаратты [Бизнес процесінің ағындарына шолу](/dynamics365/customerengagement/on-premises/customize/business-process-flows-overview) бөлімінде қараңыз.</span><span class="sxs-lookup"><span data-stu-id="e5924-159">For more information about the business process flow, see [Business process flows overview](/dynamics365/customerengagement/on-premises/customize/business-process-flows-overview).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]