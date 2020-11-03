---
title: Жұмыс декомпозициясының құрылымы бойынша пікірлерді жаңарту
description: Бұл тақырыпта Project Service Automation 2.x және 3.x аралығындағы нұсқадағы жұмыс декомпозициясының құрылымын жаңарту туралы ақпарат берілген.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 169dc24f0d1ae151ea5927123fb738221de88250
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079742"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="6114a-103">Жұмыс декомпозициясының құрылымы бойынша пікірлерді жаңарту</span><span class="sxs-lookup"><span data-stu-id="6114a-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="6114a-104">Бұл тақырыпта Project Service Automation 2.x және 3.x аралығындағы нұсқадағы жұмыс декомпозициясының құрылымын жаңарту туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="6114a-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="6114a-105">Бұл тақырыпта сәтті жаңарту үшін қажет Project Service Automation (PSA) жобасындағы дұрыс күйді анықтайды.</span><span class="sxs-lookup"><span data-stu-id="6114a-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="6114a-106">Сондай-ақ жаңартудың сәтсіз болуына әкелетін блоктаудың жалпы шарттары туралы ақпарат бар.</span><span class="sxs-lookup"><span data-stu-id="6114a-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="6114a-107">Жоба кестесінде жоба тапсырмалары мен функцияларын анықтау туралы қосымша ақпаратты [Жоба кестелері](project-creating.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="6114a-108">Негізгі нысандар</span><span class="sxs-lookup"><span data-stu-id="6114a-108">Key entities</span></span>
<span data-ttu-id="6114a-109">Ресурстармен жүктеліп қойған жұмыс декомпозициясының нақты құрылымы үшін келесі нысандар қажет:</span><span class="sxs-lookup"><span data-stu-id="6114a-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="6114a-110">Жоба</span><span class="sxs-lookup"><span data-stu-id="6114a-110">Project</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [<span data-ttu-id="6114a-111">Жоба тобы</span><span class="sxs-lookup"><span data-stu-id="6114a-111">Project Team</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [<span data-ttu-id="6114a-112">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="6114a-112">Project Task</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [<span data-ttu-id="6114a-113">Ресурс тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="6114a-113">Resource Assignments</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [<span data-ttu-id="6114a-114">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="6114a-114">Project Task Dependency</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [<span data-ttu-id="6114a-115">Тапсырыс беруге болатын ресурстар</span><span class="sxs-lookup"><span data-stu-id="6114a-115">Bookable Resources</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

<span data-ttu-id="6114a-116">Жұмыс декомпозициясының құрылымын жүктеген ресурсты анықтау үшін келесі қадамдарды орындау керек:</span><span class="sxs-lookup"><span data-stu-id="6114a-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="6114a-117">Жаңа жоба жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-117">Create a new project.</span></span> <span data-ttu-id="6114a-118">Жаңа жоба жасау жолы туралы ақпарат алу үшін [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-118">For more information about how to create a new project, see [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span></span>
2. <span data-ttu-id="6114a-119">Бір немесе бірнеше тапсырма жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-119">Create one or more tasks.</span></span> <span data-ttu-id="6114a-120">Тапсырма жасау жолы туралы ақпарат алу үшін [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-120">For more information about how to create a task, see [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span></span>
3. <span data-ttu-id="6114a-121">Тапсырма тәуелділіктерін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-121">Define the task dependencies.</span></span> <span data-ttu-id="6114a-122">Қосымша ақпарат алу үшін [Жоба тапсырмасы тәуелділігі](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-122">For more information, see [Project Task Dependency](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span></span>
4. <span data-ttu-id="6114a-123">Жобаға жоба тобының мүшелерін тағайындаңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-123">Assign project team members to the project.</span></span> <span data-ttu-id="6114a-124">Қосымша ақпарат алу үшін [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-124">For more information, see [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span></span>
5. <span data-ttu-id="6114a-125">Тапсырмаларға жоба тобының мүшелерін тағайындаңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="6114a-126">Қосымша ақпарат алу үшін [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-126">For more information, see [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="6114a-127">Жоба тобының қатынастары</span><span class="sxs-lookup"><span data-stu-id="6114a-127">Project team relationships</span></span>

<span data-ttu-id="6114a-128">Жаңартуды сәтті орындау үшін келесі қатынастарды дұрыс сақтау керек:</span><span class="sxs-lookup"><span data-stu-id="6114a-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="6114a-129">Жоба тобының барлық мүшелері тапсырыс беруге болатын ресурспен байланыстырылуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="6114a-130">Жоба тобының барлық мүшелері бірдей жобамен байланыстырылуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="6114a-131">Жоба тапсырмасының қатынастары</span><span class="sxs-lookup"><span data-stu-id="6114a-131">Project task relationships</span></span>
<span data-ttu-id="6114a-132">Жаңартуды сәтті орындау үшін келесі қатынастарды дұрыс сақтау керек:</span><span class="sxs-lookup"><span data-stu-id="6114a-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="6114a-133">Кез келген қатысты тапсырмалар бір жобамен байланысты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="6114a-134">Әр жол тапсырмасында негізгі тапсырма болуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="6114a-135">Әр тапсырмада негізгі жоба болуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="6114a-136">Жарамды шарттар</span><span class="sxs-lookup"><span data-stu-id="6114a-136">Valid conditions</span></span>

- <span data-ttu-id="6114a-137">Барлық тапсырма ұзақтықтары бір сағаттан үлкен немесе оған тең болуы (> =) және 1 800 000 минуттан (1250 күн) аспауы керек.\*</span><span class="sxs-lookup"><span data-stu-id="6114a-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="6114a-138">Барлық тапсырмалардың басталу күні 2000/01/01 күнінен кейін болуы керек.\*</span><span class="sxs-lookup"><span data-stu-id="6114a-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="6114a-139">Барлық тапсырмалардың басталу күні осы күннен бастап ең көбі 17 жыл бұрын болуы керек.\*</span><span class="sxs-lookup"><span data-stu-id="6114a-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="6114a-140">Барлық тапсырмалардың басталу күні аяқталу күнінен ертерек немесе оған тең болуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="6114a-141">Классификациялар бойынша транзакцияның барлық түрлерінде (шығыс, материал, салық және уақыт) **Әдепкі бірлік** және **Бірлік тобы** мәндері болуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="6114a-142">Күн пішімдерінде әріптер болмауы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="6114a-143">Ықтимал жеңілдету қадамдары</span><span class="sxs-lookup"><span data-stu-id="6114a-143">Potential mitigation steps</span></span>
- <span data-ttu-id="6114a-144">Жоба идентификаторы жоқ жоба тапсырмаларын анықтау үшін "Кеңейтілген іздеу" құралын қолданыңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="6114a-145">Жоспарланған ұзақтығы> 1,800,000-ден үлкен жоба тапсырмаларын анықтау үшін "Кеңейтілген іздеу" құралын қолданыңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="6114a-146">Деректерді өзгертуден бұрын, деректердің нашар күйге келуіне әкелуі мүмкін кез келген реттеулерді зерттеуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="6114a-147">Бұл реттеулер деректерге қатысты жаңартуларды жасамас бұрын қарастырылуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="6114a-148">Жоғып кеткен анықталған тапсырмалар үшін, егер олар қажет болмаса немесе дұрыс негізгі жобамен байланысты болуы керек болса, оларды жою туралы ойланыңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="6114a-149">Ұзақтығы 1250 күннен асатын кез келген тапсырмалар үшін, егер мүмкін болса, жалпы ұзақтығын көрсететін бірнеше тапсырма қосуды ойлаңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="6114a-150">Жұлдызшамен (\*) белгіленген элементтер тұтынушымен қарым-қатынасты басқару (CRM) қызметінің тек 7320 қайталанатын кеңейтуді қолдайтынына байланысты шектеулерге ие.</span><span class="sxs-lookup"><span data-stu-id="6114a-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="6114a-151">Бұл шектен аспау керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="6114a-152">Ресурсты тағайындау қатынастары</span><span class="sxs-lookup"><span data-stu-id="6114a-152">Resource Assignment relationships</span></span>
<span data-ttu-id="6114a-153">Жаңартуды сәтті орындау үшін келесі қатынастарды дұрыс сақтау керек:</span><span class="sxs-lookup"><span data-stu-id="6114a-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="6114a-154">Жұмыс декомпозициясының құрылымындағы барлық ресурс тапсырмалары бірдей жобамен байланысты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="6114a-155">Жұмыс декомпозициясының құрылымындағы барлық ресурс тапсырмалары бірдей жобаның топ мүшелерімен байланысты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="6114a-156">Ықтимал жеңілдету қадамдары</span><span class="sxs-lookup"><span data-stu-id="6114a-156">Potential mitigation steps</span></span>
- <span data-ttu-id="6114a-157">Жоғарыда сипатталған жағдайлардан тыс барлық тапсырмаларды анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="6114a-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="6114a-158">Жарамсыз болып табылатын кез келген ресурс тапсырмалары жойылуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="6114a-159">Жоба тапсырмасы тәуелділігінің қатынастары</span><span class="sxs-lookup"><span data-stu-id="6114a-159">Project task dependency relationships</span></span>
<span data-ttu-id="6114a-160">Жаңартуды сәтті орындау үшін келесі қатынастарды дұрыс сақтау керек:</span><span class="sxs-lookup"><span data-stu-id="6114a-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="6114a-161">Жоба тапсырмасының барлық тәуелділіктері бір жобамен байланысты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="6114a-162">Тапсырмада бірнеше рет сілтеме жасалған бірдей тәуелділік болмауы керек.</span><span class="sxs-lookup"><span data-stu-id="6114a-162">A task can't have the same dependency referenced more than once.</span></span>
