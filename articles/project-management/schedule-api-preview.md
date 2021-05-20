---
title: Жоспарлау нысандары операцияларын орындау үшін жоспарлау API интерфейстерін пайдалану
description: Бұл тақырыпта жоспарлау API интерфейстерін қолдануға арналған ақпарат пен үлгілері берілген.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950811"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="da3a4-103">Жоспарлау нысандары операцияларын орындау үшін жоспарлау API интерфейстерін пайдалану</span><span class="sxs-lookup"><span data-stu-id="da3a4-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="da3a4-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="da3a4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="da3a4-105">Осы бөлімде айтылған кейбір немесе барлық мүмкіндіктер алдын ала қарау бөлігі ретінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="da3a4-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="da3a4-106">Мазмұны мен функциялар өзгеруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da3a4-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="da3a4-107">Жоспарлау нысандары</span><span class="sxs-lookup"><span data-stu-id="da3a4-107">Scheduling entities</span></span>

<span data-ttu-id="da3a4-108">Жоспарлау API интерфейстері **Жоспарлау нысандары** арқылы операцияларды жасау, жаңарту және жою мүмкіндіктерін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="da3a4-109">Бұл нысандар веб-нұсқаға арналған жобада жоспарлау механизмі арқылы басқарылады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="da3a4-110">**Жоспарлау нысандары** көмегімен операцияларды жасау, жаңарту және жою алдыңғы Dynamics 365 Project Operations шығарылымдарында шектеулі болды.</span><span class="sxs-lookup"><span data-stu-id="da3a4-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="da3a4-111">Келесі кестеде **Жоспарлау нысандарының** толық тізімі берілген.</span><span class="sxs-lookup"><span data-stu-id="da3a4-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="da3a4-112">Нысан атауы</span><span class="sxs-lookup"><span data-stu-id="da3a4-112">Entity name</span></span>  | <span data-ttu-id="da3a4-113">Нысанның логикалық атауы</span><span class="sxs-lookup"><span data-stu-id="da3a4-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="da3a4-114">Project</span><span class="sxs-lookup"><span data-stu-id="da3a4-114">Project</span></span> | <span data-ttu-id="da3a4-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="da3a4-115">msdyn_project</span></span> |
| <span data-ttu-id="da3a4-116">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="da3a4-116">Project Task</span></span>  | <span data-ttu-id="da3a4-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="da3a4-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="da3a4-118">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="da3a4-118">Project Task Dependency</span></span>  | <span data-ttu-id="da3a4-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="da3a4-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="da3a4-120">Ресурс тағайындауы</span><span class="sxs-lookup"><span data-stu-id="da3a4-120">Resource Assignment</span></span> | <span data-ttu-id="da3a4-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="da3a4-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="da3a4-122">Жоба контейнері</span><span class="sxs-lookup"><span data-stu-id="da3a4-122">Project Bucket</span></span>  | <span data-ttu-id="da3a4-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="da3a4-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="da3a4-124">Жоба тобы мүшесі</span><span class="sxs-lookup"><span data-stu-id="da3a4-124">Project Team Member</span></span> | <span data-ttu-id="da3a4-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="da3a4-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="da3a4-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="da3a4-126">OperationSet</span></span>

<span data-ttu-id="da3a4-127">OperationSet — транзакция шеңберінде бірнеше кестеге әсер ететін сұраныстарды өңдеу қажет болған кезде қолдануға болатын жұмыс бірлігінің үлгісі.</span><span class="sxs-lookup"><span data-stu-id="da3a4-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="da3a4-128">Жоспарлау API интерфейстері</span><span class="sxs-lookup"><span data-stu-id="da3a4-128">Schedule APIs</span></span>

<span data-ttu-id="da3a4-129">Төменде қазіргі жоспарлау API интерфейстерінің тізімі берілген.</span><span class="sxs-lookup"><span data-stu-id="da3a4-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="da3a4-130">**msdyn_CreateProjectV1**: бұл API интерфейсін жобаны құру үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="da3a4-131">Жоба және әдепкі жоба контейнері дереу жасалады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="da3a4-132">**msdyn_CreateTeamMemberV1**: бұл API интерфейсін жоба тобының мүшесін құру үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="da3a4-133">Топ мүшелерінің жазбасы дереу жасалады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="da3a4-134">**msdyn_CreateOperationSetV1**: бұл API интерфейсін транзакция кезінде орындалуы керек бірнеше сұраныстарды жоспарлау үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="da3a4-135">**msdyn_PSSCreateV1**: бұл API интерфейсін нысанды құру үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="da3a4-136">Нысан құру операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da3a4-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="da3a4-137">**msdyn_PSSUpdateV1**: бұл API интерфейсін нысанды жаңарту үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="da3a4-138">Нысанды жаңарту операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da3a4-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="da3a4-139">**msdyn_PSSDeleteV1**: бұл API интерфейсін нысанды жою үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="da3a4-140">Нысанды жою операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da3a4-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="da3a4-141">**msdyn_ExecuteOperationSetV1**: бұл API берілген операциялар жиынтығындағы барлық әрекеттерді орындау үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="da3a4-142">OperationSet көмегімен жоспарлау API интерфейстерін пайдалану</span><span class="sxs-lookup"><span data-stu-id="da3a4-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="da3a4-143">**CreateProjectV1** және **CreateTeamMemberV1** дереу жасалатындықтан, бұл API интерфейстерін тікелей **OperationSet** жинағында пайдалануға болмайды.</span><span class="sxs-lookup"><span data-stu-id="da3a4-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="da3a4-144">Алайда API интерфейсін қажетті жазбаларды, **OperationSet** жасау үшін, содан кейін осы алдын ала жасалған жазбаларды **OperationSet** ішінде пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="da3a4-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="da3a4-145">Қолдау көрсетілетін операциялар</span><span class="sxs-lookup"><span data-stu-id="da3a4-145">Supported operations</span></span>

| <span data-ttu-id="da3a4-146">Жоспарлау нысаны</span><span class="sxs-lookup"><span data-stu-id="da3a4-146">Scheduling entity</span></span> | <span data-ttu-id="da3a4-147">Жасау</span><span class="sxs-lookup"><span data-stu-id="da3a4-147">Create</span></span> | <span data-ttu-id="da3a4-148">Жаңарту</span><span class="sxs-lookup"><span data-stu-id="da3a4-148">Update</span></span> | <span data-ttu-id="da3a4-149">Delete</span><span class="sxs-lookup"><span data-stu-id="da3a4-149">Delete</span></span> | <span data-ttu-id="da3a4-150">Маңызды жайттар</span><span class="sxs-lookup"><span data-stu-id="da3a4-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="da3a4-151">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="da3a4-151">Project task</span></span> | <span data-ttu-id="da3a4-152">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-152">Yes</span></span> | <span data-ttu-id="da3a4-153">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-153">Yes</span></span> | <span data-ttu-id="da3a4-154">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-154">Yes</span></span> | <span data-ttu-id="da3a4-155">Ешқайсысы</span><span class="sxs-lookup"><span data-stu-id="da3a4-155">None</span></span> |
| <span data-ttu-id="da3a4-156">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="da3a4-156">Project task dependency</span></span> | <span data-ttu-id="da3a4-157">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-157">Yes</span></span> | <span data-ttu-id="da3a4-158">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-158">Yes</span></span> | | <span data-ttu-id="da3a4-159">Жоба тапсырмасына тәуелділік туралы жазбалар жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="da3a4-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="da3a4-160">Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="da3a4-161">Ресурс тағайындауы</span><span class="sxs-lookup"><span data-stu-id="da3a4-161">Resource assignment</span></span> | <span data-ttu-id="da3a4-162">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-162">Yes</span></span> | <span data-ttu-id="da3a4-163">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-163">Yes</span></span> | | <span data-ttu-id="da3a4-164">Келесі өрістермен операцияларға қолдау көрсетілмейді: **BookableResourceID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining** және **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="da3a4-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="da3a4-165">Ресурстарды тағайындау туралы жазбалар жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="da3a4-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="da3a4-166">Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="da3a4-167">Жоба контейнері</span><span class="sxs-lookup"><span data-stu-id="da3a4-167">Project bucket</span></span> | <span data-ttu-id="da3a4-168">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="da3a4-168">N/A</span></span> | <span data-ttu-id="da3a4-169">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="da3a4-169">N/A</span></span> | <span data-ttu-id="da3a4-170">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="da3a4-170">N/A</span></span> | <span data-ttu-id="da3a4-171">Әдепкі контейнер **CreateProjectV1** API интерфейсі арқылы жасалады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="da3a4-172">Жоба тобының мүшесі</span><span class="sxs-lookup"><span data-stu-id="da3a4-172">Project team member</span></span> | <span data-ttu-id="da3a4-173">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-173">Yes</span></span> | <span data-ttu-id="da3a4-174">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-174">Yes</span></span> | <span data-ttu-id="da3a4-175">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-175">Yes</span></span> | <span data-ttu-id="da3a4-176">Жасау операциясы үшін **CreateTeamMemberV1** API интерфейсін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="da3a4-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="da3a4-177">Project</span><span class="sxs-lookup"><span data-stu-id="da3a4-177">Project</span></span> | <span data-ttu-id="da3a4-178">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-178">Yes</span></span> | <span data-ttu-id="da3a4-179">Иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-179">Yes</span></span> | <span data-ttu-id="da3a4-180">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="da3a4-180">N/A</span></span> | <span data-ttu-id="da3a4-181">Келесі өрістермен операцияларға қолдау көрсетілмейді: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining**, **Орындалу барысы**, **Аяқтау**, **TaskEarliestStart** және **Ұзақтығы**.</span><span class="sxs-lookup"><span data-stu-id="da3a4-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="da3a4-182">Бұл API интерфейсін реттелетін өрістерді қамтитын нысан объектілерімен шақыруға болады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="da3a4-183">ID сипаты міндетті емес.</span><span class="sxs-lookup"><span data-stu-id="da3a4-183">The ID property is optional.</span></span> <span data-ttu-id="da3a4-184">Егер ол қарастырылған болса, жүйе оны қолдануға әрекет жасайды және оны пайдалану мүмкін болмаса, ерекше жағдай жасайды.</span><span class="sxs-lookup"><span data-stu-id="da3a4-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="da3a4-185">Егер ол қарастырылмаған болса, жүйе оны жасайды.</span><span class="sxs-lookup"><span data-stu-id="da3a4-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="da3a4-186">Шектеулі өрістер</span><span class="sxs-lookup"><span data-stu-id="da3a4-186">Restricted fields</span></span>

<span data-ttu-id="da3a4-187">Келесі кестелер **Жасау** және **Өңдеу** параметрлерінен шектелген өрістерді анықтайды.</span><span class="sxs-lookup"><span data-stu-id="da3a4-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="da3a4-188">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="da3a4-188">Project task</span></span>

| <span data-ttu-id="da3a4-189">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da3a4-189">**Logical name**</span></span>                       | <span data-ttu-id="da3a4-190">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da3a4-190">**Can create**</span></span> | <span data-ttu-id="da3a4-191">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da3a4-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="da3a4-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="da3a4-193">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-193">no</span></span>             | <span data-ttu-id="da3a4-194">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-194">no</span></span>               |
| <span data-ttu-id="da3a4-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="da3a4-196">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-196">no</span></span>             | <span data-ttu-id="da3a4-197">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-197">no</span></span>               |
| <span data-ttu-id="da3a4-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="da3a4-198">msdyn_actualend</span></span>                        | <span data-ttu-id="da3a4-199">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-199">no</span></span>             | <span data-ttu-id="da3a4-200">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-200">no</span></span>               |
| <span data-ttu-id="da3a4-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="da3a4-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="da3a4-202">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-202">no</span></span>             | <span data-ttu-id="da3a4-203">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-203">no</span></span>               |
| <span data-ttu-id="da3a4-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="da3a4-205">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-205">no</span></span>             | <span data-ttu-id="da3a4-206">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-206">no</span></span>               |
| <span data-ttu-id="da3a4-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="da3a4-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="da3a4-208">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-208">no</span></span>             | <span data-ttu-id="da3a4-209">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-209">no</span></span>               |
| <span data-ttu-id="da3a4-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="da3a4-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="da3a4-211">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-211">no</span></span>             | <span data-ttu-id="da3a4-212">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-212">no</span></span>               |
| <span data-ttu-id="da3a4-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="da3a4-214">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-214">no</span></span>             | <span data-ttu-id="da3a4-215">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-215">no</span></span>               |
| <span data-ttu-id="da3a4-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="da3a4-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="da3a4-217">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-217">no</span></span>             | <span data-ttu-id="da3a4-218">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-218">no</span></span>               |
| <span data-ttu-id="da3a4-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="da3a4-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="da3a4-220">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-220">no</span></span>             | <span data-ttu-id="da3a4-221">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-221">no</span></span>               |
| <span data-ttu-id="da3a4-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="da3a4-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="da3a4-223">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-223">no</span></span>             | <span data-ttu-id="da3a4-224">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-224">no</span></span>               |
| <span data-ttu-id="da3a4-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="da3a4-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="da3a4-226">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-226">no</span></span>             | <span data-ttu-id="da3a4-227">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-227">no</span></span>               |
| <span data-ttu-id="da3a4-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="da3a4-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="da3a4-229">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-229">no</span></span>             | <span data-ttu-id="da3a4-230">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-230">no</span></span>               |
| <span data-ttu-id="da3a4-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="da3a4-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="da3a4-232">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-232">no</span></span>             | <span data-ttu-id="da3a4-233">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-233">no</span></span>               |
| <span data-ttu-id="da3a4-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="da3a4-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="da3a4-235">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-235">no</span></span>             | <span data-ttu-id="da3a4-236">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-236">no</span></span>               |
| <span data-ttu-id="da3a4-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="da3a4-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="da3a4-238">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-238">no</span></span>             | <span data-ttu-id="da3a4-239">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-239">no</span></span>               |
| <span data-ttu-id="da3a4-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="da3a4-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="da3a4-241">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-241">no</span></span>             | <span data-ttu-id="da3a4-242">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-242">no</span></span>               |
| <span data-ttu-id="da3a4-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="da3a4-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="da3a4-244">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-244">no</span></span>             | <span data-ttu-id="da3a4-245">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-245">no</span></span>               |
| <span data-ttu-id="da3a4-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="da3a4-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="da3a4-247">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-247">no</span></span>             | <span data-ttu-id="da3a4-248">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-248">no</span></span>               |
| <span data-ttu-id="da3a4-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="da3a4-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="da3a4-250">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-250">no</span></span>             | <span data-ttu-id="da3a4-251">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-251">no</span></span>               |
| <span data-ttu-id="da3a4-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="da3a4-253">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-253">no</span></span>             | <span data-ttu-id="da3a4-254">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-254">no</span></span>               |
| <span data-ttu-id="da3a4-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="da3a4-256">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-256">no</span></span>             | <span data-ttu-id="da3a4-257">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-257">no</span></span>               |
| <span data-ttu-id="da3a4-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="da3a4-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="da3a4-259">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-259">no</span></span>             | <span data-ttu-id="da3a4-260">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-260">no</span></span>               |
| <span data-ttu-id="da3a4-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="da3a4-262">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-262">no</span></span>             | <span data-ttu-id="da3a4-263">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-263">no</span></span>               |
| <span data-ttu-id="da3a4-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="da3a4-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="da3a4-265">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-265">no</span></span>             | <span data-ttu-id="da3a4-266">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-266">no</span></span>               |
| <span data-ttu-id="da3a4-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="da3a4-267">msdyn_progress</span></span>                         | <span data-ttu-id="da3a4-268">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-268">no</span></span>             | <span data-ttu-id="da3a4-269">жоқ (P4W үшін "иә")</span><span class="sxs-lookup"><span data-stu-id="da3a4-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="da3a4-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="da3a4-271">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-271">no</span></span>             | <span data-ttu-id="da3a4-272">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-272">no</span></span>               |
| <span data-ttu-id="da3a4-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="da3a4-274">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-274">no</span></span>             | <span data-ttu-id="da3a4-275">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-275">no</span></span>               |
| <span data-ttu-id="da3a4-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="da3a4-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="da3a4-277">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-277">no</span></span>             | <span data-ttu-id="da3a4-278">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-278">no</span></span>               |
| <span data-ttu-id="da3a4-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="da3a4-280">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-280">no</span></span>             | <span data-ttu-id="da3a4-281">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-281">no</span></span>               |
| <span data-ttu-id="da3a4-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="da3a4-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="da3a4-283">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-283">no</span></span>             | <span data-ttu-id="da3a4-284">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-284">no</span></span>               |
| <span data-ttu-id="da3a4-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="da3a4-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="da3a4-286">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-286">no</span></span>             | <span data-ttu-id="da3a4-287">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-287">no</span></span>               |
| <span data-ttu-id="da3a4-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="da3a4-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="da3a4-289">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-289">no</span></span>             | <span data-ttu-id="da3a4-290">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-290">no</span></span>               |
| <span data-ttu-id="da3a4-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="da3a4-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="da3a4-292">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-292">no</span></span>             | <span data-ttu-id="da3a4-293">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-293">no</span></span>               |
| <span data-ttu-id="da3a4-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="da3a4-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="da3a4-295">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-295">no</span></span>             | <span data-ttu-id="da3a4-296">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-296">no</span></span>               |
| <span data-ttu-id="da3a4-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="da3a4-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="da3a4-298">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-298">no</span></span>             | <span data-ttu-id="da3a4-299">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-299">no</span></span>               |
| <span data-ttu-id="da3a4-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="da3a4-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="da3a4-301">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-301">no</span></span>             | <span data-ttu-id="da3a4-302">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-302">no</span></span>               |
| <span data-ttu-id="da3a4-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="da3a4-304">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-304">no</span></span>             | <span data-ttu-id="da3a4-305">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-305">no</span></span>               |
| <span data-ttu-id="da3a4-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="da3a4-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="da3a4-307">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-307">no</span></span>             | <span data-ttu-id="da3a4-308">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-308">no</span></span>               |
| <span data-ttu-id="da3a4-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="da3a4-310">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-310">no</span></span>             | <span data-ttu-id="da3a4-311">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-311">no</span></span>               |
| <span data-ttu-id="da3a4-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="da3a4-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="da3a4-313">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-313">no</span></span>             | <span data-ttu-id="da3a4-314">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-314">no</span></span>               |
| <span data-ttu-id="da3a4-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="da3a4-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="da3a4-316">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-316">no</span></span>             | <span data-ttu-id="da3a4-317">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-317">no</span></span>               |
| <span data-ttu-id="da3a4-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="da3a4-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="da3a4-319">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-319">no</span></span>             | <span data-ttu-id="da3a4-320">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-320">no</span></span>               |
| <span data-ttu-id="da3a4-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="da3a4-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="da3a4-322">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-322">no</span></span>             | <span data-ttu-id="da3a4-323">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-323">no</span></span>               |
| <span data-ttu-id="da3a4-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="da3a4-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="da3a4-325">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-325">no</span></span>             | <span data-ttu-id="da3a4-326">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-326">no</span></span>               |
| <span data-ttu-id="da3a4-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="da3a4-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="da3a4-328">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-328">no</span></span>             | <span data-ttu-id="da3a4-329">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-329">no</span></span>               |
| <span data-ttu-id="da3a4-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="da3a4-330">msdyn_summary</span></span>                          | <span data-ttu-id="da3a4-331">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-331">no</span></span>             | <span data-ttu-id="da3a4-332">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-332">no</span></span>               |
| <span data-ttu-id="da3a4-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="da3a4-334">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-334">no</span></span>             | <span data-ttu-id="da3a4-335">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-335">no</span></span>               |
| <span data-ttu-id="da3a4-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="da3a4-337">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-337">no</span></span>             | <span data-ttu-id="da3a4-338">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="da3a4-339">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="da3a4-339">Project task dependency</span></span>

| <span data-ttu-id="da3a4-340">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da3a4-340">**Logical name**</span></span>              | <span data-ttu-id="da3a4-341">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da3a4-341">**Can create**</span></span> | <span data-ttu-id="da3a4-342">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da3a4-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="da3a4-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="da3a4-343">msdyn_linktype</span></span>                | <span data-ttu-id="da3a4-344">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-344">no</span></span>             | <span data-ttu-id="da3a4-345">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-345">no</span></span>           |
| <span data-ttu-id="da3a4-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="da3a4-346">msdyn_linktypename</span></span>            | <span data-ttu-id="da3a4-347">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-347">no</span></span>             | <span data-ttu-id="da3a4-348">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-348">no</span></span>           |
| <span data-ttu-id="da3a4-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="da3a4-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="da3a4-350">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-350">yes</span></span>            | <span data-ttu-id="da3a4-351">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-351">no</span></span>           |
| <span data-ttu-id="da3a4-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="da3a4-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="da3a4-353">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-353">yes</span></span>            | <span data-ttu-id="da3a4-354">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-354">no</span></span>           |
| <span data-ttu-id="da3a4-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="da3a4-355">msdyn_project</span></span>                 | <span data-ttu-id="da3a4-356">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-356">yes</span></span>            | <span data-ttu-id="da3a4-357">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-357">no</span></span>           |
| <span data-ttu-id="da3a4-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="da3a4-358">msdyn_projectname</span></span>             | <span data-ttu-id="da3a4-359">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-359">yes</span></span>            | <span data-ttu-id="da3a4-360">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-360">no</span></span>           |
| <span data-ttu-id="da3a4-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="da3a4-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="da3a4-362">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-362">yes</span></span>            | <span data-ttu-id="da3a4-363">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-363">no</span></span>           |
| <span data-ttu-id="da3a4-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="da3a4-364">msdyn_successortask</span></span>           | <span data-ttu-id="da3a4-365">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-365">yes</span></span>            | <span data-ttu-id="da3a4-366">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-366">no</span></span>           |
| <span data-ttu-id="da3a4-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="da3a4-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="da3a4-368">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-368">yes</span></span>            | <span data-ttu-id="da3a4-369">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="da3a4-370">Ресурс тағайындауы</span><span class="sxs-lookup"><span data-stu-id="da3a4-370">Resource assignment</span></span>

| <span data-ttu-id="da3a4-371">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da3a4-371">**Logical name**</span></span>             | <span data-ttu-id="da3a4-372">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da3a4-372">**Can create**</span></span> | <span data-ttu-id="da3a4-373">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da3a4-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="da3a4-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="da3a4-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="da3a4-375">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-375">yes</span></span>            | <span data-ttu-id="da3a4-376">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-376">no</span></span>           |
| <span data-ttu-id="da3a4-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="da3a4-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="da3a4-378">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-378">yes</span></span>            | <span data-ttu-id="da3a4-379">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-379">no</span></span>           |
| <span data-ttu-id="da3a4-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="da3a4-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="da3a4-381">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-381">no</span></span>             | <span data-ttu-id="da3a4-382">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-382">no</span></span>           |
| <span data-ttu-id="da3a4-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="da3a4-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="da3a4-384">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-384">no</span></span>             | <span data-ttu-id="da3a4-385">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-385">no</span></span>           |
| <span data-ttu-id="da3a4-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="da3a4-386">msdyn_committype</span></span>             | <span data-ttu-id="da3a4-387">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-387">no</span></span>             | <span data-ttu-id="da3a4-388">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-388">no</span></span>           |
| <span data-ttu-id="da3a4-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="da3a4-389">msdyn_committypename</span></span>         | <span data-ttu-id="da3a4-390">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-390">no</span></span>             | <span data-ttu-id="da3a4-391">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-391">no</span></span>           |
| <span data-ttu-id="da3a4-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="da3a4-392">msdyn_effort</span></span>                 | <span data-ttu-id="da3a4-393">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-393">no</span></span>             | <span data-ttu-id="da3a4-394">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-394">no</span></span>           |
| <span data-ttu-id="da3a4-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="da3a4-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="da3a4-396">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-396">no</span></span>             | <span data-ttu-id="da3a4-397">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-397">no</span></span>           |
| <span data-ttu-id="da3a4-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="da3a4-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="da3a4-399">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-399">no</span></span>             | <span data-ttu-id="da3a4-400">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-400">no</span></span>           |
| <span data-ttu-id="da3a4-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="da3a4-401">msdyn_finish</span></span>                 | <span data-ttu-id="da3a4-402">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-402">no</span></span>             | <span data-ttu-id="da3a4-403">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-403">no</span></span>           |
| <span data-ttu-id="da3a4-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="da3a4-405">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-405">no</span></span>             | <span data-ttu-id="da3a4-406">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-406">no</span></span>           |
| <span data-ttu-id="da3a4-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="da3a4-408">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-408">no</span></span>             | <span data-ttu-id="da3a4-409">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-409">no</span></span>           |
| <span data-ttu-id="da3a4-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="da3a4-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="da3a4-411">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-411">no</span></span>             | <span data-ttu-id="da3a4-412">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-412">no</span></span>           |
| <span data-ttu-id="da3a4-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="da3a4-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="da3a4-414">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-414">no</span></span>             | <span data-ttu-id="da3a4-415">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-415">no</span></span>           |
| <span data-ttu-id="da3a4-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="da3a4-417">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-417">no</span></span>             | <span data-ttu-id="da3a4-418">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-418">no</span></span>           |
| <span data-ttu-id="da3a4-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="da3a4-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="da3a4-420">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-420">no</span></span>             | <span data-ttu-id="da3a4-421">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-421">no</span></span>           |
| <span data-ttu-id="da3a4-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="da3a4-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="da3a4-423">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-423">no</span></span>             | <span data-ttu-id="da3a4-424">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-424">no</span></span>           |
| <span data-ttu-id="da3a4-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="da3a4-425">msdyn_projectid</span></span>              | <span data-ttu-id="da3a4-426">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-426">yes</span></span>            | <span data-ttu-id="da3a4-427">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-427">no</span></span>           |
| <span data-ttu-id="da3a4-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="da3a4-428">msdyn_projectidname</span></span>          | <span data-ttu-id="da3a4-429">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-429">no</span></span>             | <span data-ttu-id="da3a4-430">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-430">no</span></span>           |
| <span data-ttu-id="da3a4-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="da3a4-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="da3a4-432">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-432">no</span></span>             | <span data-ttu-id="da3a4-433">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-433">no</span></span>           |
| <span data-ttu-id="da3a4-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="da3a4-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="da3a4-435">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-435">no</span></span>             | <span data-ttu-id="da3a4-436">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-436">no</span></span>           |
| <span data-ttu-id="da3a4-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="da3a4-437">msdyn_start</span></span>                  | <span data-ttu-id="da3a4-438">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-438">no</span></span>             | <span data-ttu-id="da3a4-439">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-439">no</span></span>           |
| <span data-ttu-id="da3a4-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="da3a4-440">msdyn_taskid</span></span>                 | <span data-ttu-id="da3a4-441">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-441">no</span></span>             | <span data-ttu-id="da3a4-442">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-442">no</span></span>           |
| <span data-ttu-id="da3a4-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="da3a4-443">msdyn_taskidname</span></span>             | <span data-ttu-id="da3a4-444">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-444">no</span></span>             | <span data-ttu-id="da3a4-445">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-445">no</span></span>           |
| <span data-ttu-id="da3a4-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="da3a4-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="da3a4-447">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-447">no</span></span>             | <span data-ttu-id="da3a4-448">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="da3a4-449">Жоба тобының мүшесі</span><span class="sxs-lookup"><span data-stu-id="da3a4-449">Project team member</span></span>

| <span data-ttu-id="da3a4-450">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da3a4-450">**Logical name**</span></span>                                 | <span data-ttu-id="da3a4-451">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da3a4-451">**Can create**</span></span> | <span data-ttu-id="da3a4-452">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da3a4-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="da3a4-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="da3a4-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="da3a4-454">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-454">no</span></span>             | <span data-ttu-id="da3a4-455">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-455">no</span></span>           |
| <span data-ttu-id="da3a4-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="da3a4-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="da3a4-457">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-457">no</span></span>             | <span data-ttu-id="da3a4-458">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-458">no</span></span>           |
| <span data-ttu-id="da3a4-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="da3a4-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="da3a4-460">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-460">no</span></span>             | <span data-ttu-id="da3a4-461">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-461">no</span></span>           |
| <span data-ttu-id="da3a4-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="da3a4-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="da3a4-463">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-463">no</span></span>             | <span data-ttu-id="da3a4-464">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-464">no</span></span>           |
| <span data-ttu-id="da3a4-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="da3a4-465">msdyn_effort</span></span>                                     | <span data-ttu-id="da3a4-466">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-466">no</span></span>             | <span data-ttu-id="da3a4-467">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-467">no</span></span>           |
| <span data-ttu-id="da3a4-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="da3a4-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="da3a4-469">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-469">no</span></span>             | <span data-ttu-id="da3a4-470">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-470">no</span></span>           |
| <span data-ttu-id="da3a4-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="da3a4-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="da3a4-472">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-472">no</span></span>             | <span data-ttu-id="da3a4-473">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-473">no</span></span>           |
| <span data-ttu-id="da3a4-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="da3a4-474">msdyn_finish</span></span>                                     | <span data-ttu-id="da3a4-475">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-475">no</span></span>             | <span data-ttu-id="da3a4-476">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-476">no</span></span>           |
| <span data-ttu-id="da3a4-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="da3a4-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="da3a4-478">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-478">no</span></span>             | <span data-ttu-id="da3a4-479">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-479">no</span></span>           |
| <span data-ttu-id="da3a4-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="da3a4-480">msdyn_hours</span></span>                                      | <span data-ttu-id="da3a4-481">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-481">no</span></span>             | <span data-ttu-id="da3a4-482">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-482">no</span></span>           |
| <span data-ttu-id="da3a4-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="da3a4-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="da3a4-484">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-484">no</span></span>             | <span data-ttu-id="da3a4-485">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-485">no</span></span>           |
| <span data-ttu-id="da3a4-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="da3a4-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="da3a4-487">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-487">no</span></span>             | <span data-ttu-id="da3a4-488">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-488">no</span></span>           |
| <span data-ttu-id="da3a4-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="da3a4-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="da3a4-490">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-490">no</span></span>             | <span data-ttu-id="da3a4-491">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-491">no</span></span>           |
| <span data-ttu-id="da3a4-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="da3a4-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="da3a4-493">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-493">no</span></span>             | <span data-ttu-id="da3a4-494">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-494">no</span></span>           |
| <span data-ttu-id="da3a4-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="da3a4-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="da3a4-496">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-496">no</span></span>             | <span data-ttu-id="da3a4-497">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-497">no</span></span>           |
| <span data-ttu-id="da3a4-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="da3a4-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="da3a4-499">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-499">no</span></span>             | <span data-ttu-id="da3a4-500">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-500">no</span></span>           |
| <span data-ttu-id="da3a4-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="da3a4-501">msdyn_start</span></span>                                      | <span data-ttu-id="da3a4-502">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-502">no</span></span>             | <span data-ttu-id="da3a4-503">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="da3a4-504">Project</span><span class="sxs-lookup"><span data-stu-id="da3a4-504">Project</span></span>

| <span data-ttu-id="da3a4-505">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da3a4-505">**Logical name**</span></span>                       | <span data-ttu-id="da3a4-506">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da3a4-506">**Can create**</span></span> | <span data-ttu-id="da3a4-507">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da3a4-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="da3a4-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="da3a4-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="da3a4-509">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-509">no</span></span>             | <span data-ttu-id="da3a4-510">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-510">no</span></span>           |
| <span data-ttu-id="da3a4-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="da3a4-512">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-512">no</span></span>             | <span data-ttu-id="da3a4-513">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-513">no</span></span>           |
| <span data-ttu-id="da3a4-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="da3a4-515">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-515">no</span></span>             | <span data-ttu-id="da3a4-516">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-516">no</span></span>           |
| <span data-ttu-id="da3a4-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="da3a4-518">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-518">no</span></span>             | <span data-ttu-id="da3a4-519">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-519">no</span></span>           |
| <span data-ttu-id="da3a4-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="da3a4-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="da3a4-521">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-521">no</span></span>             | <span data-ttu-id="da3a4-522">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-522">no</span></span>           |
| <span data-ttu-id="da3a4-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="da3a4-524">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-524">no</span></span>             | <span data-ttu-id="da3a4-525">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-525">no</span></span>           |
| <span data-ttu-id="da3a4-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="da3a4-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="da3a4-527">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-527">yes</span></span>            | <span data-ttu-id="da3a4-528">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-528">no</span></span>           |
| <span data-ttu-id="da3a4-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="da3a4-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="da3a4-530">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-530">yes</span></span>            | <span data-ttu-id="da3a4-531">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-531">no</span></span>           |
| <span data-ttu-id="da3a4-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="da3a4-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="da3a4-533">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-533">yes</span></span>            | <span data-ttu-id="da3a4-534">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-534">no</span></span>           |
| <span data-ttu-id="da3a4-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="da3a4-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="da3a4-536">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-536">no</span></span>             | <span data-ttu-id="da3a4-537">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-537">no</span></span>           |
| <span data-ttu-id="da3a4-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="da3a4-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="da3a4-539">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-539">no</span></span>             | <span data-ttu-id="da3a4-540">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-540">no</span></span>           |
| <span data-ttu-id="da3a4-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="da3a4-542">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-542">no</span></span>             | <span data-ttu-id="da3a4-543">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-543">no</span></span>           |
| <span data-ttu-id="da3a4-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="da3a4-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="da3a4-545">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-545">no</span></span>             | <span data-ttu-id="da3a4-546">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-546">no</span></span>           |
| <span data-ttu-id="da3a4-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="da3a4-548">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-548">no</span></span>             | <span data-ttu-id="da3a4-549">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-549">no</span></span>           |
| <span data-ttu-id="da3a4-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="da3a4-550">msdyn_duration</span></span>                         | <span data-ttu-id="da3a4-551">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-551">no</span></span>             | <span data-ttu-id="da3a4-552">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-552">no</span></span>           |
| <span data-ttu-id="da3a4-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="da3a4-553">msdyn_effort</span></span>                           | <span data-ttu-id="da3a4-554">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-554">no</span></span>             | <span data-ttu-id="da3a4-555">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-555">no</span></span>           |
| <span data-ttu-id="da3a4-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="da3a4-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="da3a4-557">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-557">no</span></span>             | <span data-ttu-id="da3a4-558">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-558">no</span></span>           |
| <span data-ttu-id="da3a4-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="da3a4-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="da3a4-560">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-560">no</span></span>             | <span data-ttu-id="da3a4-561">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-561">no</span></span>           |
| <span data-ttu-id="da3a4-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="da3a4-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="da3a4-563">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-563">no</span></span>             | <span data-ttu-id="da3a4-564">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-564">no</span></span>           |
| <span data-ttu-id="da3a4-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="da3a4-565">msdyn_finish</span></span>                           | <span data-ttu-id="da3a4-566">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-566">yes</span></span>            | <span data-ttu-id="da3a4-567">иә</span><span class="sxs-lookup"><span data-stu-id="da3a4-567">yes</span></span>          |
| <span data-ttu-id="da3a4-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="da3a4-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="da3a4-569">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-569">no</span></span>             | <span data-ttu-id="da3a4-570">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-570">no</span></span>           |
| <span data-ttu-id="da3a4-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="da3a4-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="da3a4-572">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-572">no</span></span>             | <span data-ttu-id="da3a4-573">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-573">no</span></span>           |
| <span data-ttu-id="da3a4-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="da3a4-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="da3a4-575">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-575">no</span></span>             | <span data-ttu-id="da3a4-576">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-576">no</span></span>           |
| <span data-ttu-id="da3a4-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="da3a4-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="da3a4-578">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-578">no</span></span>             | <span data-ttu-id="da3a4-579">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-579">no</span></span>           |
| <span data-ttu-id="da3a4-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="da3a4-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="da3a4-581">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-581">no</span></span>             | <span data-ttu-id="da3a4-582">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-582">no</span></span>           |
| <span data-ttu-id="da3a4-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="da3a4-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="da3a4-584">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-584">no</span></span>             | <span data-ttu-id="da3a4-585">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-585">no</span></span>           |
| <span data-ttu-id="da3a4-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="da3a4-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="da3a4-587">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-587">no</span></span>             | <span data-ttu-id="da3a4-588">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-588">no</span></span>           |
| <span data-ttu-id="da3a4-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="da3a4-590">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-590">no</span></span>             | <span data-ttu-id="da3a4-591">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-591">no</span></span>           |
| <span data-ttu-id="da3a4-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="da3a4-593">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-593">no</span></span>             | <span data-ttu-id="da3a4-594">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-594">no</span></span>           |
| <span data-ttu-id="da3a4-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="da3a4-596">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-596">no</span></span>             | <span data-ttu-id="da3a4-597">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-597">no</span></span>           |
| <span data-ttu-id="da3a4-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="da3a4-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="da3a4-599">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-599">no</span></span>             | <span data-ttu-id="da3a4-600">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-600">no</span></span>           |
| <span data-ttu-id="da3a4-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="da3a4-602">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-602">no</span></span>             | <span data-ttu-id="da3a4-603">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-603">no</span></span>           |
| <span data-ttu-id="da3a4-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="da3a4-604">msdyn_progress</span></span>                         | <span data-ttu-id="da3a4-605">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-605">no</span></span>             | <span data-ttu-id="da3a4-606">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-606">no</span></span>           |
| <span data-ttu-id="da3a4-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="da3a4-608">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-608">no</span></span>             | <span data-ttu-id="da3a4-609">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-609">no</span></span>           |
| <span data-ttu-id="da3a4-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="da3a4-611">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-611">no</span></span>             | <span data-ttu-id="da3a4-612">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-612">no</span></span>           |
| <span data-ttu-id="da3a4-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="da3a4-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="da3a4-614">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-614">no</span></span>             | <span data-ttu-id="da3a4-615">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-615">no</span></span>           |
| <span data-ttu-id="da3a4-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="da3a4-617">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-617">no</span></span>             | <span data-ttu-id="da3a4-618">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-618">no</span></span>           |
| <span data-ttu-id="da3a4-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="da3a4-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="da3a4-620">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-620">no</span></span>             | <span data-ttu-id="da3a4-621">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-621">no</span></span>           |
| <span data-ttu-id="da3a4-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="da3a4-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="da3a4-623">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-623">no</span></span>             | <span data-ttu-id="da3a4-624">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-624">no</span></span>           |
| <span data-ttu-id="da3a4-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="da3a4-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="da3a4-626">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-626">no</span></span>             | <span data-ttu-id="da3a4-627">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-627">no</span></span>           |
| <span data-ttu-id="da3a4-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="da3a4-629">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-629">no</span></span>             | <span data-ttu-id="da3a4-630">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-630">no</span></span>           |
| <span data-ttu-id="da3a4-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="da3a4-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="da3a4-632">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-632">no</span></span>             | <span data-ttu-id="da3a4-633">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-633">no</span></span>           |
| <span data-ttu-id="da3a4-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="da3a4-635">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-635">no</span></span>             | <span data-ttu-id="da3a4-636">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-636">no</span></span>           |
| <span data-ttu-id="da3a4-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="da3a4-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="da3a4-638">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-638">no</span></span>             | <span data-ttu-id="da3a4-639">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-639">no</span></span>           |
| <span data-ttu-id="da3a4-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="da3a4-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="da3a4-641">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-641">no</span></span>             | <span data-ttu-id="da3a4-642">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-642">no</span></span>           |
| <span data-ttu-id="da3a4-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="da3a4-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="da3a4-644">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-644">no</span></span>             | <span data-ttu-id="da3a4-645">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-645">no</span></span>           |
| <span data-ttu-id="da3a4-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="da3a4-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="da3a4-647">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-647">no</span></span>             | <span data-ttu-id="da3a4-648">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-648">no</span></span>           |
| <span data-ttu-id="da3a4-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="da3a4-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="da3a4-650">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-650">no</span></span>             | <span data-ttu-id="da3a4-651">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-651">no</span></span>           |
| <span data-ttu-id="da3a4-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="da3a4-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="da3a4-653">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-653">no</span></span>             | <span data-ttu-id="da3a4-654">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-654">no</span></span>           |
| <span data-ttu-id="da3a4-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="da3a4-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="da3a4-656">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-656">no</span></span>             | <span data-ttu-id="da3a4-657">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-657">no</span></span>           |
| <span data-ttu-id="da3a4-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="da3a4-659">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-659">no</span></span>             | <span data-ttu-id="da3a4-660">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-660">no</span></span>           |
| <span data-ttu-id="da3a4-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="da3a4-662">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-662">no</span></span>             | <span data-ttu-id="da3a4-663">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-663">no</span></span>           |
| <span data-ttu-id="da3a4-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="da3a4-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="da3a4-665">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-665">no</span></span>             | <span data-ttu-id="da3a4-666">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-666">no</span></span>           |
| <span data-ttu-id="da3a4-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="da3a4-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="da3a4-668">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-668">no</span></span>             | <span data-ttu-id="da3a4-669">жоқ</span><span class="sxs-lookup"><span data-stu-id="da3a4-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="da3a4-670">Шектеулер мен белгілі қателер</span><span class="sxs-lookup"><span data-stu-id="da3a4-670">Limitations and known issues</span></span>
<span data-ttu-id="da3a4-671">Төменде шектеулер мен белгілі мәселелер тізімі берілген:</span><span class="sxs-lookup"><span data-stu-id="da3a4-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="da3a4-672">Жоспарлау API интерфейстерін тек **Microsoft жоба лицензиясы бар пайдаланушылар** пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="da3a4-673">Оларды пайдалана алмайды:</span><span class="sxs-lookup"><span data-stu-id="da3a4-673">They can't be used by:</span></span>
    - <span data-ttu-id="da3a4-674">Бағдарлама пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="da3a4-674">Application users</span></span>
    - <span data-ttu-id="da3a4-675">Жүйе пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="da3a4-675">System users</span></span>
    - <span data-ttu-id="da3a4-676">Интеграция пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="da3a4-676">Integration users</span></span>
    - <span data-ttu-id="da3a4-677">Қажетті лицензиясы жоқ басқа пайдаланушылар</span><span class="sxs-lookup"><span data-stu-id="da3a4-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="da3a4-678">Әр **OperationSet** ең көбі 100 операция жасай алады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="da3a4-679">Әрбір пайдаланушыда ең көбі 10 ашық **OperationSets** бола алады.</span><span class="sxs-lookup"><span data-stu-id="da3a4-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="da3a4-680">Қазіргі уақытта Project Operations жобадағы ең көбі 500 тапсырманы қолдайды.</span><span class="sxs-lookup"><span data-stu-id="da3a4-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="da3a4-681">**OperationSet** ақаулық күйі және сәтсіздік журналдары қазіргі уақытта қолжетімді емес.</span><span class="sxs-lookup"><span data-stu-id="da3a4-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="da3a4-682">Жоспарлау API интерфейстері жалпыға қолжетімді алдын ала қарау нұсқасында орналасқан.</span><span class="sxs-lookup"><span data-stu-id="da3a4-682">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="da3a4-683">Бұл API интерфейстерін жұмыс ортасында пайдалануға Microsoft қолдау көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="da3a4-683">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>
- [<span data-ttu-id="da3a4-684">Жобалар мен тапсырмалар шектеулері мен шекаралары</span><span class="sxs-lookup"><span data-stu-id="da3a4-684">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="da3a4-685">Қатені өңдеу</span><span class="sxs-lookup"><span data-stu-id="da3a4-685">Error handling</span></span>

   - <span data-ttu-id="da3a4-686">Операциялық жиындардан туындаған қателерді қарап шығу үшін **Параметрлер** \> **Кесте интеграциясы** \> **Операциялар жиындары** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="da3a4-686">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="da3a4-687">Жобаны жоспарлау қызметінен туындаған қателерді қарау үшін **Параметрлер** \> **Кесте интеграциясы** \> **PSS қателерін тіркеу журналы** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="da3a4-687">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="da3a4-688">Үлгі сценарий</span><span class="sxs-lookup"><span data-stu-id="da3a4-688">Sample scenario</span></span>

<span data-ttu-id="da3a4-689">Бұл сценарийде сіз жоба, топ мүшесі, төрт тапсырма және екі ресурстық тағайындама жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="da3a4-689">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="da3a4-690">Әрі қарай бір тапсырманы жаңартасыз, жобаны жаңартасыз, бір тапсырманы жоясыз, ресурстардың бір тағайындамасын жоясыз және тапсырмаға тәуелділікті жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="da3a4-690">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="da3a4-691">Қосымша үлгілер</span><span class="sxs-lookup"><span data-stu-id="da3a4-691">Additional samples</span></span>

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;

    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
