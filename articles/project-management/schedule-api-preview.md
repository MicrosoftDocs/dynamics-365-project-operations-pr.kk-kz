---
title: Жоспарлау нысандары операцияларын орындау үшін жоспарлау API интерфейстерін пайдалану
description: Бұл тақырыпта жоспарлау API интерфейстерін қолдануға арналған ақпарат пен үлгілері берілген.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4a032dc7bcbdf23fce3c3b2ca63c51d473bd8e26
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116804"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="da6eb-103">Жоспарлау нысандары операцияларын орындау үшін жоспарлау API интерфейстерін пайдалану</span><span class="sxs-lookup"><span data-stu-id="da6eb-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="da6eb-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="da6eb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="da6eb-105">Осы бөлімде айтылған кейбір немесе барлық мүмкіндіктер алдын ала қарау бөлігі ретінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="da6eb-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="da6eb-106">Мазмұны мен функциялар өзгеруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da6eb-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="da6eb-107">Жоспарлау нысандары</span><span class="sxs-lookup"><span data-stu-id="da6eb-107">Scheduling entities</span></span>

<span data-ttu-id="da6eb-108">Жоспарлау API интерфейстері **Жоспарлау нысандары** арқылы операцияларды жасау, жаңарту және жою мүмкіндіктерін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="da6eb-109">Бұл нысандар веб-нұсқаға арналған жобада жоспарлау механизмі арқылы басқарылады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="da6eb-110">**Жоспарлау нысандары** көмегімен операцияларды жасау, жаңарту және жою алдыңғы Dynamics 365 Project Operations шығарылымдарында шектеулі болды.</span><span class="sxs-lookup"><span data-stu-id="da6eb-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="da6eb-111">Келесі кестеде **Жоспарлау нысандарының** толық тізімі берілген.</span><span class="sxs-lookup"><span data-stu-id="da6eb-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="da6eb-112">Нысан атауы</span><span class="sxs-lookup"><span data-stu-id="da6eb-112">Entity name</span></span>  | <span data-ttu-id="da6eb-113">Нысанның логикалық атауы</span><span class="sxs-lookup"><span data-stu-id="da6eb-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="da6eb-114">Project</span><span class="sxs-lookup"><span data-stu-id="da6eb-114">Project</span></span> | <span data-ttu-id="da6eb-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="da6eb-115">msdyn_project</span></span> |
| <span data-ttu-id="da6eb-116">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="da6eb-116">Project Task</span></span>  | <span data-ttu-id="da6eb-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="da6eb-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="da6eb-118">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="da6eb-118">Project Task Dependency</span></span>  | <span data-ttu-id="da6eb-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="da6eb-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="da6eb-120">Ресурс тағайындауы</span><span class="sxs-lookup"><span data-stu-id="da6eb-120">Resource Assignment</span></span> | <span data-ttu-id="da6eb-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="da6eb-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="da6eb-122">Жоба контейнері</span><span class="sxs-lookup"><span data-stu-id="da6eb-122">Project Bucket</span></span>  | <span data-ttu-id="da6eb-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="da6eb-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="da6eb-124">Жоба тобы мүшесі</span><span class="sxs-lookup"><span data-stu-id="da6eb-124">Project Team Member</span></span> | <span data-ttu-id="da6eb-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="da6eb-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="da6eb-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="da6eb-126">OperationSet</span></span>

<span data-ttu-id="da6eb-127">OperationSet — транзакция шеңберінде бірнеше кестеге әсер ететін сұраныстарды өңдеу қажет болған кезде қолдануға болатын жұмыс бірлігінің үлгісі.</span><span class="sxs-lookup"><span data-stu-id="da6eb-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="da6eb-128">Жоспарлау API интерфейстері</span><span class="sxs-lookup"><span data-stu-id="da6eb-128">Schedule APIs</span></span>

<span data-ttu-id="da6eb-129">Төменде қазіргі жоспарлау API интерфейстерінің тізімі берілген.</span><span class="sxs-lookup"><span data-stu-id="da6eb-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="da6eb-130">**msdyn_CreateProjectV1**: бұл API интерфейсін жобаны құру үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="da6eb-131">Жоба және әдепкі жоба контейнері дереу жасалады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="da6eb-132">**msdyn_CreateTeamMemberV1**: бұл API интерфейсін жоба тобының мүшесін құру үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="da6eb-133">Топ мүшелерінің жазбасы дереу жасалады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="da6eb-134">**msdyn_CreateOperationSetV1**: бұл API интерфейсін транзакция кезінде орындалуы керек бірнеше сұраныстарды жоспарлау үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="da6eb-135">**msdyn_PSSCreateV1**: бұл API интерфейсін нысанды құру үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="da6eb-136">Нысан құру операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da6eb-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="da6eb-137">**msdyn_PSSUpdateV1**: бұл API интерфейсін нысанды жаңарту үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="da6eb-138">Нысанды жаңарту операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da6eb-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="da6eb-139">**msdyn_PSSDeleteV1**: бұл API интерфейсін нысанды жою үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="da6eb-140">Нысанды жою операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da6eb-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="da6eb-141">**msdyn_ExecuteOperationSetV1**: бұл API берілген операциялар жиынтығындағы барлық әрекеттерді орындау үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="da6eb-142">OperationSet көмегімен жоспарлау API интерфейстерін пайдалану</span><span class="sxs-lookup"><span data-stu-id="da6eb-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="da6eb-143">**CreateProjectV1** және **CreateTeamMemberV1** дереу жасалатындықтан, бұл API интерфейстерін тікелей **OperationSet** жинағында пайдалануға болмайды.</span><span class="sxs-lookup"><span data-stu-id="da6eb-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="da6eb-144">Алайда API интерфейсін қажетті жазбаларды, **OperationSet** жасау үшін, содан кейін осы алдын ала жасалған жазбаларды **OperationSet** ішінде пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="da6eb-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="da6eb-145">Қолдау көрсетілетін операциялар</span><span class="sxs-lookup"><span data-stu-id="da6eb-145">Supported operations</span></span>

| <span data-ttu-id="da6eb-146">Жоспарлау нысаны</span><span class="sxs-lookup"><span data-stu-id="da6eb-146">Scheduling entity</span></span> | <span data-ttu-id="da6eb-147">Жасау</span><span class="sxs-lookup"><span data-stu-id="da6eb-147">Create</span></span> | <span data-ttu-id="da6eb-148">Жаңарту</span><span class="sxs-lookup"><span data-stu-id="da6eb-148">Update</span></span> | <span data-ttu-id="da6eb-149">Delete</span><span class="sxs-lookup"><span data-stu-id="da6eb-149">Delete</span></span> | <span data-ttu-id="da6eb-150">Маңызды жайттар</span><span class="sxs-lookup"><span data-stu-id="da6eb-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="da6eb-151">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="da6eb-151">Project task</span></span> | <span data-ttu-id="da6eb-152">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-152">Yes</span></span> | <span data-ttu-id="da6eb-153">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-153">Yes</span></span> | <span data-ttu-id="da6eb-154">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-154">Yes</span></span> | <span data-ttu-id="da6eb-155">Ешқайсысы</span><span class="sxs-lookup"><span data-stu-id="da6eb-155">None</span></span> |
| <span data-ttu-id="da6eb-156">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="da6eb-156">Project task dependency</span></span> | <span data-ttu-id="da6eb-157">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-157">Yes</span></span> | <span data-ttu-id="da6eb-158">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-158">Yes</span></span> | | <span data-ttu-id="da6eb-159">Жоба тапсырмасына тәуелділік туралы жазбалар жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="da6eb-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="da6eb-160">Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="da6eb-161">Ресурс тағайындауы</span><span class="sxs-lookup"><span data-stu-id="da6eb-161">Resource assignment</span></span> | <span data-ttu-id="da6eb-162">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-162">Yes</span></span> | <span data-ttu-id="da6eb-163">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-163">Yes</span></span> | | <span data-ttu-id="da6eb-164">Келесі өрістермен операцияларға қолдау көрсетілмейді: **BookableResourceID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining** және **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="da6eb-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="da6eb-165">Ресурстарды тағайындау туралы жазбалар жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="da6eb-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="da6eb-166">Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="da6eb-167">Жоба контейнері</span><span class="sxs-lookup"><span data-stu-id="da6eb-167">Project bucket</span></span> | <span data-ttu-id="da6eb-168">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="da6eb-168">N/A</span></span> | <span data-ttu-id="da6eb-169">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="da6eb-169">N/A</span></span> | <span data-ttu-id="da6eb-170">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="da6eb-170">N/A</span></span> | <span data-ttu-id="da6eb-171">Әдепкі контейнер **CreateProjectV1** API интерфейсі арқылы жасалады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="da6eb-172">Жоба тобының мүшесі</span><span class="sxs-lookup"><span data-stu-id="da6eb-172">Project team member</span></span> | <span data-ttu-id="da6eb-173">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-173">Yes</span></span> | <span data-ttu-id="da6eb-174">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-174">Yes</span></span> | <span data-ttu-id="da6eb-175">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-175">Yes</span></span> | <span data-ttu-id="da6eb-176">Жасау операциясы үшін **CreateTeamMemberV1** API интерфейсін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="da6eb-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="da6eb-177">Project</span><span class="sxs-lookup"><span data-stu-id="da6eb-177">Project</span></span> | <span data-ttu-id="da6eb-178">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-178">Yes</span></span> | <span data-ttu-id="da6eb-179">Иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-179">Yes</span></span> | <span data-ttu-id="da6eb-180">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="da6eb-180">N/A</span></span> | <span data-ttu-id="da6eb-181">Келесі өрістермен операцияларға қолдау көрсетілмейді: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining**, **Орындалу барысы**, **Аяқтау**, **TaskEarliestStart** және **Ұзақтығы**.</span><span class="sxs-lookup"><span data-stu-id="da6eb-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="da6eb-182">Бұл API интерфейсін реттелетін өрістерді қамтитын нысан объектілерімен шақыруға болады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="da6eb-183">ID сипаты міндетті емес.</span><span class="sxs-lookup"><span data-stu-id="da6eb-183">The ID property is optional.</span></span> <span data-ttu-id="da6eb-184">Егер ол қарастырылған болса, жүйе оны қолдануға әрекет жасайды және оны пайдалану мүмкін болмаса, ерекше жағдай жасайды.</span><span class="sxs-lookup"><span data-stu-id="da6eb-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="da6eb-185">Егер ол қарастырылмаған болса, жүйе оны жасайды.</span><span class="sxs-lookup"><span data-stu-id="da6eb-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="da6eb-186">Шектеулі өрістер</span><span class="sxs-lookup"><span data-stu-id="da6eb-186">Restricted fields</span></span>

<span data-ttu-id="da6eb-187">Келесі кестелер **Жасау** және **Өңдеу** параметрлерінен шектелген өрістерді анықтайды.</span><span class="sxs-lookup"><span data-stu-id="da6eb-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="da6eb-188">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="da6eb-188">Project task</span></span>

| <span data-ttu-id="da6eb-189">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da6eb-189">**Logical name**</span></span>                       | <span data-ttu-id="da6eb-190">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da6eb-190">**Can create**</span></span> | <span data-ttu-id="da6eb-191">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da6eb-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="da6eb-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="da6eb-193">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-193">no</span></span>             | <span data-ttu-id="da6eb-194">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-194">no</span></span>               |
| <span data-ttu-id="da6eb-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="da6eb-196">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-196">no</span></span>             | <span data-ttu-id="da6eb-197">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-197">no</span></span>               |
| <span data-ttu-id="da6eb-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="da6eb-198">msdyn_actualend</span></span>                        | <span data-ttu-id="da6eb-199">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-199">no</span></span>             | <span data-ttu-id="da6eb-200">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-200">no</span></span>               |
| <span data-ttu-id="da6eb-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="da6eb-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="da6eb-202">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-202">no</span></span>             | <span data-ttu-id="da6eb-203">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-203">no</span></span>               |
| <span data-ttu-id="da6eb-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="da6eb-205">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-205">no</span></span>             | <span data-ttu-id="da6eb-206">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-206">no</span></span>               |
| <span data-ttu-id="da6eb-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="da6eb-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="da6eb-208">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-208">no</span></span>             | <span data-ttu-id="da6eb-209">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-209">no</span></span>               |
| <span data-ttu-id="da6eb-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="da6eb-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="da6eb-211">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-211">no</span></span>             | <span data-ttu-id="da6eb-212">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-212">no</span></span>               |
| <span data-ttu-id="da6eb-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="da6eb-214">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-214">no</span></span>             | <span data-ttu-id="da6eb-215">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-215">no</span></span>               |
| <span data-ttu-id="da6eb-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="da6eb-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="da6eb-217">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-217">no</span></span>             | <span data-ttu-id="da6eb-218">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-218">no</span></span>               |
| <span data-ttu-id="da6eb-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="da6eb-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="da6eb-220">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-220">no</span></span>             | <span data-ttu-id="da6eb-221">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-221">no</span></span>               |
| <span data-ttu-id="da6eb-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="da6eb-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="da6eb-223">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-223">no</span></span>             | <span data-ttu-id="da6eb-224">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-224">no</span></span>               |
| <span data-ttu-id="da6eb-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="da6eb-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="da6eb-226">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-226">no</span></span>             | <span data-ttu-id="da6eb-227">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-227">no</span></span>               |
| <span data-ttu-id="da6eb-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="da6eb-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="da6eb-229">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-229">no</span></span>             | <span data-ttu-id="da6eb-230">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-230">no</span></span>               |
| <span data-ttu-id="da6eb-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="da6eb-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="da6eb-232">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-232">no</span></span>             | <span data-ttu-id="da6eb-233">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-233">no</span></span>               |
| <span data-ttu-id="da6eb-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="da6eb-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="da6eb-235">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-235">no</span></span>             | <span data-ttu-id="da6eb-236">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-236">no</span></span>               |
| <span data-ttu-id="da6eb-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="da6eb-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="da6eb-238">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-238">no</span></span>             | <span data-ttu-id="da6eb-239">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-239">no</span></span>               |
| <span data-ttu-id="da6eb-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="da6eb-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="da6eb-241">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-241">no</span></span>             | <span data-ttu-id="da6eb-242">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-242">no</span></span>               |
| <span data-ttu-id="da6eb-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="da6eb-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="da6eb-244">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-244">no</span></span>             | <span data-ttu-id="da6eb-245">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-245">no</span></span>               |
| <span data-ttu-id="da6eb-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="da6eb-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="da6eb-247">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-247">no</span></span>             | <span data-ttu-id="da6eb-248">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-248">no</span></span>               |
| <span data-ttu-id="da6eb-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="da6eb-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="da6eb-250">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-250">no</span></span>             | <span data-ttu-id="da6eb-251">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-251">no</span></span>               |
| <span data-ttu-id="da6eb-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="da6eb-253">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-253">no</span></span>             | <span data-ttu-id="da6eb-254">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-254">no</span></span>               |
| <span data-ttu-id="da6eb-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="da6eb-256">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-256">no</span></span>             | <span data-ttu-id="da6eb-257">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-257">no</span></span>               |
| <span data-ttu-id="da6eb-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="da6eb-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="da6eb-259">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-259">no</span></span>             | <span data-ttu-id="da6eb-260">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-260">no</span></span>               |
| <span data-ttu-id="da6eb-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="da6eb-262">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-262">no</span></span>             | <span data-ttu-id="da6eb-263">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-263">no</span></span>               |
| <span data-ttu-id="da6eb-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="da6eb-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="da6eb-265">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-265">no</span></span>             | <span data-ttu-id="da6eb-266">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-266">no</span></span>               |
| <span data-ttu-id="da6eb-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="da6eb-267">msdyn_progress</span></span>                         | <span data-ttu-id="da6eb-268">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-268">no</span></span>             | <span data-ttu-id="da6eb-269">жоқ (P4W үшін "иә")</span><span class="sxs-lookup"><span data-stu-id="da6eb-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="da6eb-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="da6eb-271">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-271">no</span></span>             | <span data-ttu-id="da6eb-272">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-272">no</span></span>               |
| <span data-ttu-id="da6eb-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="da6eb-274">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-274">no</span></span>             | <span data-ttu-id="da6eb-275">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-275">no</span></span>               |
| <span data-ttu-id="da6eb-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="da6eb-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="da6eb-277">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-277">no</span></span>             | <span data-ttu-id="da6eb-278">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-278">no</span></span>               |
| <span data-ttu-id="da6eb-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="da6eb-280">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-280">no</span></span>             | <span data-ttu-id="da6eb-281">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-281">no</span></span>               |
| <span data-ttu-id="da6eb-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="da6eb-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="da6eb-283">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-283">no</span></span>             | <span data-ttu-id="da6eb-284">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-284">no</span></span>               |
| <span data-ttu-id="da6eb-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="da6eb-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="da6eb-286">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-286">no</span></span>             | <span data-ttu-id="da6eb-287">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-287">no</span></span>               |
| <span data-ttu-id="da6eb-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="da6eb-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="da6eb-289">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-289">no</span></span>             | <span data-ttu-id="da6eb-290">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-290">no</span></span>               |
| <span data-ttu-id="da6eb-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="da6eb-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="da6eb-292">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-292">no</span></span>             | <span data-ttu-id="da6eb-293">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-293">no</span></span>               |
| <span data-ttu-id="da6eb-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="da6eb-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="da6eb-295">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-295">no</span></span>             | <span data-ttu-id="da6eb-296">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-296">no</span></span>               |
| <span data-ttu-id="da6eb-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="da6eb-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="da6eb-298">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-298">no</span></span>             | <span data-ttu-id="da6eb-299">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-299">no</span></span>               |
| <span data-ttu-id="da6eb-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="da6eb-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="da6eb-301">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-301">no</span></span>             | <span data-ttu-id="da6eb-302">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-302">no</span></span>               |
| <span data-ttu-id="da6eb-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="da6eb-304">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-304">no</span></span>             | <span data-ttu-id="da6eb-305">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-305">no</span></span>               |
| <span data-ttu-id="da6eb-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="da6eb-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="da6eb-307">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-307">no</span></span>             | <span data-ttu-id="da6eb-308">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-308">no</span></span>               |
| <span data-ttu-id="da6eb-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="da6eb-310">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-310">no</span></span>             | <span data-ttu-id="da6eb-311">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-311">no</span></span>               |
| <span data-ttu-id="da6eb-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="da6eb-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="da6eb-313">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-313">no</span></span>             | <span data-ttu-id="da6eb-314">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-314">no</span></span>               |
| <span data-ttu-id="da6eb-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="da6eb-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="da6eb-316">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-316">no</span></span>             | <span data-ttu-id="da6eb-317">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-317">no</span></span>               |
| <span data-ttu-id="da6eb-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="da6eb-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="da6eb-319">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-319">no</span></span>             | <span data-ttu-id="da6eb-320">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-320">no</span></span>               |
| <span data-ttu-id="da6eb-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="da6eb-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="da6eb-322">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-322">no</span></span>             | <span data-ttu-id="da6eb-323">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-323">no</span></span>               |
| <span data-ttu-id="da6eb-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="da6eb-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="da6eb-325">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-325">no</span></span>             | <span data-ttu-id="da6eb-326">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-326">no</span></span>               |
| <span data-ttu-id="da6eb-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="da6eb-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="da6eb-328">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-328">no</span></span>             | <span data-ttu-id="da6eb-329">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-329">no</span></span>               |
| <span data-ttu-id="da6eb-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="da6eb-330">msdyn_summary</span></span>                          | <span data-ttu-id="da6eb-331">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-331">no</span></span>             | <span data-ttu-id="da6eb-332">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-332">no</span></span>               |
| <span data-ttu-id="da6eb-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="da6eb-334">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-334">no</span></span>             | <span data-ttu-id="da6eb-335">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-335">no</span></span>               |
| <span data-ttu-id="da6eb-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="da6eb-337">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-337">no</span></span>             | <span data-ttu-id="da6eb-338">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="da6eb-339">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="da6eb-339">Project task dependency</span></span>

| <span data-ttu-id="da6eb-340">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da6eb-340">**Logical name**</span></span>              | <span data-ttu-id="da6eb-341">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da6eb-341">**Can create**</span></span> | <span data-ttu-id="da6eb-342">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da6eb-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="da6eb-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="da6eb-343">msdyn_linktype</span></span>                | <span data-ttu-id="da6eb-344">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-344">no</span></span>             | <span data-ttu-id="da6eb-345">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-345">no</span></span>           |
| <span data-ttu-id="da6eb-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="da6eb-346">msdyn_linktypename</span></span>            | <span data-ttu-id="da6eb-347">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-347">no</span></span>             | <span data-ttu-id="da6eb-348">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-348">no</span></span>           |
| <span data-ttu-id="da6eb-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="da6eb-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="da6eb-350">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-350">yes</span></span>            | <span data-ttu-id="da6eb-351">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-351">no</span></span>           |
| <span data-ttu-id="da6eb-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="da6eb-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="da6eb-353">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-353">yes</span></span>            | <span data-ttu-id="da6eb-354">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-354">no</span></span>           |
| <span data-ttu-id="da6eb-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="da6eb-355">msdyn_project</span></span>                 | <span data-ttu-id="da6eb-356">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-356">yes</span></span>            | <span data-ttu-id="da6eb-357">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-357">no</span></span>           |
| <span data-ttu-id="da6eb-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="da6eb-358">msdyn_projectname</span></span>             | <span data-ttu-id="da6eb-359">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-359">yes</span></span>            | <span data-ttu-id="da6eb-360">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-360">no</span></span>           |
| <span data-ttu-id="da6eb-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="da6eb-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="da6eb-362">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-362">yes</span></span>            | <span data-ttu-id="da6eb-363">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-363">no</span></span>           |
| <span data-ttu-id="da6eb-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="da6eb-364">msdyn_successortask</span></span>           | <span data-ttu-id="da6eb-365">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-365">yes</span></span>            | <span data-ttu-id="da6eb-366">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-366">no</span></span>           |
| <span data-ttu-id="da6eb-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="da6eb-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="da6eb-368">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-368">yes</span></span>            | <span data-ttu-id="da6eb-369">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="da6eb-370">Ресурс тағайындауы</span><span class="sxs-lookup"><span data-stu-id="da6eb-370">Resource assignment</span></span>

| <span data-ttu-id="da6eb-371">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da6eb-371">**Logical name**</span></span>             | <span data-ttu-id="da6eb-372">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da6eb-372">**Can create**</span></span> | <span data-ttu-id="da6eb-373">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da6eb-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="da6eb-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="da6eb-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="da6eb-375">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-375">yes</span></span>            | <span data-ttu-id="da6eb-376">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-376">no</span></span>           |
| <span data-ttu-id="da6eb-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="da6eb-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="da6eb-378">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-378">yes</span></span>            | <span data-ttu-id="da6eb-379">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-379">no</span></span>           |
| <span data-ttu-id="da6eb-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="da6eb-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="da6eb-381">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-381">no</span></span>             | <span data-ttu-id="da6eb-382">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-382">no</span></span>           |
| <span data-ttu-id="da6eb-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="da6eb-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="da6eb-384">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-384">no</span></span>             | <span data-ttu-id="da6eb-385">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-385">no</span></span>           |
| <span data-ttu-id="da6eb-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="da6eb-386">msdyn_committype</span></span>             | <span data-ttu-id="da6eb-387">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-387">no</span></span>             | <span data-ttu-id="da6eb-388">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-388">no</span></span>           |
| <span data-ttu-id="da6eb-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="da6eb-389">msdyn_committypename</span></span>         | <span data-ttu-id="da6eb-390">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-390">no</span></span>             | <span data-ttu-id="da6eb-391">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-391">no</span></span>           |
| <span data-ttu-id="da6eb-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="da6eb-392">msdyn_effort</span></span>                 | <span data-ttu-id="da6eb-393">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-393">no</span></span>             | <span data-ttu-id="da6eb-394">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-394">no</span></span>           |
| <span data-ttu-id="da6eb-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="da6eb-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="da6eb-396">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-396">no</span></span>             | <span data-ttu-id="da6eb-397">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-397">no</span></span>           |
| <span data-ttu-id="da6eb-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="da6eb-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="da6eb-399">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-399">no</span></span>             | <span data-ttu-id="da6eb-400">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-400">no</span></span>           |
| <span data-ttu-id="da6eb-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="da6eb-401">msdyn_finish</span></span>                 | <span data-ttu-id="da6eb-402">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-402">no</span></span>             | <span data-ttu-id="da6eb-403">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-403">no</span></span>           |
| <span data-ttu-id="da6eb-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="da6eb-405">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-405">no</span></span>             | <span data-ttu-id="da6eb-406">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-406">no</span></span>           |
| <span data-ttu-id="da6eb-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="da6eb-408">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-408">no</span></span>             | <span data-ttu-id="da6eb-409">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-409">no</span></span>           |
| <span data-ttu-id="da6eb-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="da6eb-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="da6eb-411">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-411">no</span></span>             | <span data-ttu-id="da6eb-412">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-412">no</span></span>           |
| <span data-ttu-id="da6eb-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="da6eb-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="da6eb-414">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-414">no</span></span>             | <span data-ttu-id="da6eb-415">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-415">no</span></span>           |
| <span data-ttu-id="da6eb-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="da6eb-417">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-417">no</span></span>             | <span data-ttu-id="da6eb-418">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-418">no</span></span>           |
| <span data-ttu-id="da6eb-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="da6eb-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="da6eb-420">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-420">no</span></span>             | <span data-ttu-id="da6eb-421">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-421">no</span></span>           |
| <span data-ttu-id="da6eb-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="da6eb-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="da6eb-423">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-423">no</span></span>             | <span data-ttu-id="da6eb-424">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-424">no</span></span>           |
| <span data-ttu-id="da6eb-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="da6eb-425">msdyn_projectid</span></span>              | <span data-ttu-id="da6eb-426">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-426">yes</span></span>            | <span data-ttu-id="da6eb-427">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-427">no</span></span>           |
| <span data-ttu-id="da6eb-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="da6eb-428">msdyn_projectidname</span></span>          | <span data-ttu-id="da6eb-429">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-429">no</span></span>             | <span data-ttu-id="da6eb-430">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-430">no</span></span>           |
| <span data-ttu-id="da6eb-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="da6eb-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="da6eb-432">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-432">no</span></span>             | <span data-ttu-id="da6eb-433">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-433">no</span></span>           |
| <span data-ttu-id="da6eb-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="da6eb-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="da6eb-435">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-435">no</span></span>             | <span data-ttu-id="da6eb-436">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-436">no</span></span>           |
| <span data-ttu-id="da6eb-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="da6eb-437">msdyn_start</span></span>                  | <span data-ttu-id="da6eb-438">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-438">no</span></span>             | <span data-ttu-id="da6eb-439">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-439">no</span></span>           |
| <span data-ttu-id="da6eb-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="da6eb-440">msdyn_taskid</span></span>                 | <span data-ttu-id="da6eb-441">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-441">no</span></span>             | <span data-ttu-id="da6eb-442">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-442">no</span></span>           |
| <span data-ttu-id="da6eb-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="da6eb-443">msdyn_taskidname</span></span>             | <span data-ttu-id="da6eb-444">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-444">no</span></span>             | <span data-ttu-id="da6eb-445">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-445">no</span></span>           |
| <span data-ttu-id="da6eb-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="da6eb-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="da6eb-447">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-447">no</span></span>             | <span data-ttu-id="da6eb-448">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="da6eb-449">Жоба тобының мүшесі</span><span class="sxs-lookup"><span data-stu-id="da6eb-449">Project team member</span></span>

| <span data-ttu-id="da6eb-450">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da6eb-450">**Logical name**</span></span>                                 | <span data-ttu-id="da6eb-451">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da6eb-451">**Can create**</span></span> | <span data-ttu-id="da6eb-452">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da6eb-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="da6eb-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="da6eb-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="da6eb-454">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-454">no</span></span>             | <span data-ttu-id="da6eb-455">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-455">no</span></span>           |
| <span data-ttu-id="da6eb-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="da6eb-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="da6eb-457">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-457">no</span></span>             | <span data-ttu-id="da6eb-458">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-458">no</span></span>           |
| <span data-ttu-id="da6eb-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="da6eb-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="da6eb-460">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-460">no</span></span>             | <span data-ttu-id="da6eb-461">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-461">no</span></span>           |
| <span data-ttu-id="da6eb-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="da6eb-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="da6eb-463">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-463">no</span></span>             | <span data-ttu-id="da6eb-464">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-464">no</span></span>           |
| <span data-ttu-id="da6eb-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="da6eb-465">msdyn_effort</span></span>                                     | <span data-ttu-id="da6eb-466">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-466">no</span></span>             | <span data-ttu-id="da6eb-467">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-467">no</span></span>           |
| <span data-ttu-id="da6eb-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="da6eb-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="da6eb-469">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-469">no</span></span>             | <span data-ttu-id="da6eb-470">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-470">no</span></span>           |
| <span data-ttu-id="da6eb-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="da6eb-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="da6eb-472">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-472">no</span></span>             | <span data-ttu-id="da6eb-473">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-473">no</span></span>           |
| <span data-ttu-id="da6eb-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="da6eb-474">msdyn_finish</span></span>                                     | <span data-ttu-id="da6eb-475">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-475">no</span></span>             | <span data-ttu-id="da6eb-476">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-476">no</span></span>           |
| <span data-ttu-id="da6eb-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="da6eb-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="da6eb-478">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-478">no</span></span>             | <span data-ttu-id="da6eb-479">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-479">no</span></span>           |
| <span data-ttu-id="da6eb-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="da6eb-480">msdyn_hours</span></span>                                      | <span data-ttu-id="da6eb-481">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-481">no</span></span>             | <span data-ttu-id="da6eb-482">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-482">no</span></span>           |
| <span data-ttu-id="da6eb-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="da6eb-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="da6eb-484">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-484">no</span></span>             | <span data-ttu-id="da6eb-485">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-485">no</span></span>           |
| <span data-ttu-id="da6eb-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="da6eb-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="da6eb-487">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-487">no</span></span>             | <span data-ttu-id="da6eb-488">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-488">no</span></span>           |
| <span data-ttu-id="da6eb-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="da6eb-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="da6eb-490">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-490">no</span></span>             | <span data-ttu-id="da6eb-491">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-491">no</span></span>           |
| <span data-ttu-id="da6eb-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="da6eb-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="da6eb-493">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-493">no</span></span>             | <span data-ttu-id="da6eb-494">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-494">no</span></span>           |
| <span data-ttu-id="da6eb-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="da6eb-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="da6eb-496">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-496">no</span></span>             | <span data-ttu-id="da6eb-497">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-497">no</span></span>           |
| <span data-ttu-id="da6eb-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="da6eb-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="da6eb-499">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-499">no</span></span>             | <span data-ttu-id="da6eb-500">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-500">no</span></span>           |
| <span data-ttu-id="da6eb-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="da6eb-501">msdyn_start</span></span>                                      | <span data-ttu-id="da6eb-502">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-502">no</span></span>             | <span data-ttu-id="da6eb-503">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="da6eb-504">Project</span><span class="sxs-lookup"><span data-stu-id="da6eb-504">Project</span></span>

| <span data-ttu-id="da6eb-505">**Логикалық атау**</span><span class="sxs-lookup"><span data-stu-id="da6eb-505">**Logical name**</span></span>                       | <span data-ttu-id="da6eb-506">**Жасалады**</span><span class="sxs-lookup"><span data-stu-id="da6eb-506">**Can create**</span></span> | <span data-ttu-id="da6eb-507">**Өңделеді**</span><span class="sxs-lookup"><span data-stu-id="da6eb-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="da6eb-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="da6eb-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="da6eb-509">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-509">no</span></span>             | <span data-ttu-id="da6eb-510">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-510">no</span></span>           |
| <span data-ttu-id="da6eb-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="da6eb-512">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-512">no</span></span>             | <span data-ttu-id="da6eb-513">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-513">no</span></span>           |
| <span data-ttu-id="da6eb-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="da6eb-515">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-515">no</span></span>             | <span data-ttu-id="da6eb-516">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-516">no</span></span>           |
| <span data-ttu-id="da6eb-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="da6eb-518">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-518">no</span></span>             | <span data-ttu-id="da6eb-519">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-519">no</span></span>           |
| <span data-ttu-id="da6eb-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="da6eb-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="da6eb-521">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-521">no</span></span>             | <span data-ttu-id="da6eb-522">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-522">no</span></span>           |
| <span data-ttu-id="da6eb-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="da6eb-524">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-524">no</span></span>             | <span data-ttu-id="da6eb-525">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-525">no</span></span>           |
| <span data-ttu-id="da6eb-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="da6eb-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="da6eb-527">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-527">yes</span></span>            | <span data-ttu-id="da6eb-528">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-528">no</span></span>           |
| <span data-ttu-id="da6eb-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="da6eb-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="da6eb-530">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-530">yes</span></span>            | <span data-ttu-id="da6eb-531">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-531">no</span></span>           |
| <span data-ttu-id="da6eb-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="da6eb-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="da6eb-533">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-533">yes</span></span>            | <span data-ttu-id="da6eb-534">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-534">no</span></span>           |
| <span data-ttu-id="da6eb-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="da6eb-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="da6eb-536">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-536">no</span></span>             | <span data-ttu-id="da6eb-537">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-537">no</span></span>           |
| <span data-ttu-id="da6eb-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="da6eb-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="da6eb-539">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-539">no</span></span>             | <span data-ttu-id="da6eb-540">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-540">no</span></span>           |
| <span data-ttu-id="da6eb-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="da6eb-542">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-542">no</span></span>             | <span data-ttu-id="da6eb-543">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-543">no</span></span>           |
| <span data-ttu-id="da6eb-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="da6eb-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="da6eb-545">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-545">no</span></span>             | <span data-ttu-id="da6eb-546">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-546">no</span></span>           |
| <span data-ttu-id="da6eb-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="da6eb-548">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-548">no</span></span>             | <span data-ttu-id="da6eb-549">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-549">no</span></span>           |
| <span data-ttu-id="da6eb-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="da6eb-550">msdyn_duration</span></span>                         | <span data-ttu-id="da6eb-551">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-551">no</span></span>             | <span data-ttu-id="da6eb-552">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-552">no</span></span>           |
| <span data-ttu-id="da6eb-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="da6eb-553">msdyn_effort</span></span>                           | <span data-ttu-id="da6eb-554">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-554">no</span></span>             | <span data-ttu-id="da6eb-555">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-555">no</span></span>           |
| <span data-ttu-id="da6eb-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="da6eb-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="da6eb-557">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-557">no</span></span>             | <span data-ttu-id="da6eb-558">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-558">no</span></span>           |
| <span data-ttu-id="da6eb-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="da6eb-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="da6eb-560">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-560">no</span></span>             | <span data-ttu-id="da6eb-561">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-561">no</span></span>           |
| <span data-ttu-id="da6eb-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="da6eb-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="da6eb-563">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-563">no</span></span>             | <span data-ttu-id="da6eb-564">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-564">no</span></span>           |
| <span data-ttu-id="da6eb-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="da6eb-565">msdyn_finish</span></span>                           | <span data-ttu-id="da6eb-566">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-566">yes</span></span>            | <span data-ttu-id="da6eb-567">иә</span><span class="sxs-lookup"><span data-stu-id="da6eb-567">yes</span></span>          |
| <span data-ttu-id="da6eb-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="da6eb-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="da6eb-569">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-569">no</span></span>             | <span data-ttu-id="da6eb-570">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-570">no</span></span>           |
| <span data-ttu-id="da6eb-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="da6eb-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="da6eb-572">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-572">no</span></span>             | <span data-ttu-id="da6eb-573">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-573">no</span></span>           |
| <span data-ttu-id="da6eb-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="da6eb-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="da6eb-575">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-575">no</span></span>             | <span data-ttu-id="da6eb-576">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-576">no</span></span>           |
| <span data-ttu-id="da6eb-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="da6eb-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="da6eb-578">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-578">no</span></span>             | <span data-ttu-id="da6eb-579">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-579">no</span></span>           |
| <span data-ttu-id="da6eb-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="da6eb-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="da6eb-581">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-581">no</span></span>             | <span data-ttu-id="da6eb-582">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-582">no</span></span>           |
| <span data-ttu-id="da6eb-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="da6eb-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="da6eb-584">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-584">no</span></span>             | <span data-ttu-id="da6eb-585">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-585">no</span></span>           |
| <span data-ttu-id="da6eb-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="da6eb-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="da6eb-587">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-587">no</span></span>             | <span data-ttu-id="da6eb-588">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-588">no</span></span>           |
| <span data-ttu-id="da6eb-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="da6eb-590">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-590">no</span></span>             | <span data-ttu-id="da6eb-591">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-591">no</span></span>           |
| <span data-ttu-id="da6eb-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="da6eb-593">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-593">no</span></span>             | <span data-ttu-id="da6eb-594">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-594">no</span></span>           |
| <span data-ttu-id="da6eb-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="da6eb-596">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-596">no</span></span>             | <span data-ttu-id="da6eb-597">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-597">no</span></span>           |
| <span data-ttu-id="da6eb-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="da6eb-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="da6eb-599">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-599">no</span></span>             | <span data-ttu-id="da6eb-600">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-600">no</span></span>           |
| <span data-ttu-id="da6eb-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="da6eb-602">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-602">no</span></span>             | <span data-ttu-id="da6eb-603">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-603">no</span></span>           |
| <span data-ttu-id="da6eb-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="da6eb-604">msdyn_progress</span></span>                         | <span data-ttu-id="da6eb-605">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-605">no</span></span>             | <span data-ttu-id="da6eb-606">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-606">no</span></span>           |
| <span data-ttu-id="da6eb-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="da6eb-608">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-608">no</span></span>             | <span data-ttu-id="da6eb-609">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-609">no</span></span>           |
| <span data-ttu-id="da6eb-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="da6eb-611">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-611">no</span></span>             | <span data-ttu-id="da6eb-612">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-612">no</span></span>           |
| <span data-ttu-id="da6eb-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="da6eb-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="da6eb-614">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-614">no</span></span>             | <span data-ttu-id="da6eb-615">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-615">no</span></span>           |
| <span data-ttu-id="da6eb-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="da6eb-617">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-617">no</span></span>             | <span data-ttu-id="da6eb-618">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-618">no</span></span>           |
| <span data-ttu-id="da6eb-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="da6eb-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="da6eb-620">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-620">no</span></span>             | <span data-ttu-id="da6eb-621">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-621">no</span></span>           |
| <span data-ttu-id="da6eb-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="da6eb-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="da6eb-623">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-623">no</span></span>             | <span data-ttu-id="da6eb-624">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-624">no</span></span>           |
| <span data-ttu-id="da6eb-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="da6eb-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="da6eb-626">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-626">no</span></span>             | <span data-ttu-id="da6eb-627">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-627">no</span></span>           |
| <span data-ttu-id="da6eb-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="da6eb-629">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-629">no</span></span>             | <span data-ttu-id="da6eb-630">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-630">no</span></span>           |
| <span data-ttu-id="da6eb-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="da6eb-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="da6eb-632">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-632">no</span></span>             | <span data-ttu-id="da6eb-633">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-633">no</span></span>           |
| <span data-ttu-id="da6eb-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="da6eb-635">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-635">no</span></span>             | <span data-ttu-id="da6eb-636">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-636">no</span></span>           |
| <span data-ttu-id="da6eb-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="da6eb-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="da6eb-638">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-638">no</span></span>             | <span data-ttu-id="da6eb-639">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-639">no</span></span>           |
| <span data-ttu-id="da6eb-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="da6eb-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="da6eb-641">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-641">no</span></span>             | <span data-ttu-id="da6eb-642">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-642">no</span></span>           |
| <span data-ttu-id="da6eb-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="da6eb-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="da6eb-644">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-644">no</span></span>             | <span data-ttu-id="da6eb-645">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-645">no</span></span>           |
| <span data-ttu-id="da6eb-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="da6eb-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="da6eb-647">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-647">no</span></span>             | <span data-ttu-id="da6eb-648">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-648">no</span></span>           |
| <span data-ttu-id="da6eb-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="da6eb-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="da6eb-650">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-650">no</span></span>             | <span data-ttu-id="da6eb-651">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-651">no</span></span>           |
| <span data-ttu-id="da6eb-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="da6eb-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="da6eb-653">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-653">no</span></span>             | <span data-ttu-id="da6eb-654">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-654">no</span></span>           |
| <span data-ttu-id="da6eb-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="da6eb-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="da6eb-656">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-656">no</span></span>             | <span data-ttu-id="da6eb-657">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-657">no</span></span>           |
| <span data-ttu-id="da6eb-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="da6eb-659">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-659">no</span></span>             | <span data-ttu-id="da6eb-660">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-660">no</span></span>           |
| <span data-ttu-id="da6eb-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="da6eb-662">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-662">no</span></span>             | <span data-ttu-id="da6eb-663">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-663">no</span></span>           |
| <span data-ttu-id="da6eb-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="da6eb-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="da6eb-665">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-665">no</span></span>             | <span data-ttu-id="da6eb-666">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-666">no</span></span>           |
| <span data-ttu-id="da6eb-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="da6eb-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="da6eb-668">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-668">no</span></span>             | <span data-ttu-id="da6eb-669">жоқ</span><span class="sxs-lookup"><span data-stu-id="da6eb-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="da6eb-670">Шектеулер мен белгілі қателер</span><span class="sxs-lookup"><span data-stu-id="da6eb-670">Limitations and known issues</span></span>
<span data-ttu-id="da6eb-671">Төменде шектеулер мен белгілі мәселелер тізімі берілген:</span><span class="sxs-lookup"><span data-stu-id="da6eb-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="da6eb-672">Жоспарлау API интерфейстерін тек **Microsoft жоба лицензиясы бар пайдаланушылар** пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="da6eb-673">Оларды пайдалана алмайды:</span><span class="sxs-lookup"><span data-stu-id="da6eb-673">They can't be used by:</span></span>
    - <span data-ttu-id="da6eb-674">Бағдарлама пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="da6eb-674">Application users</span></span>
    - <span data-ttu-id="da6eb-675">Жүйе пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="da6eb-675">System users</span></span>
    - <span data-ttu-id="da6eb-676">Интеграция пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="da6eb-676">Integration users</span></span>
    - <span data-ttu-id="da6eb-677">Қажетті лицензиясы жоқ басқа пайдаланушылар</span><span class="sxs-lookup"><span data-stu-id="da6eb-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="da6eb-678">Әр **OperationSet** ең көбі 100 операция жасай алады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="da6eb-679">Әрбір пайдаланушыда ең көбі 10 ашық **OperationSets** бола алады.</span><span class="sxs-lookup"><span data-stu-id="da6eb-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="da6eb-680">Қазіргі уақытта Project Operations жобадағы ең көбі 500 тапсырманы қолдайды.</span><span class="sxs-lookup"><span data-stu-id="da6eb-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="da6eb-681">**OperationSet** ақаулық күйі және сәтсіздік журналдары қазіргі уақытта қолжетімді емес.</span><span class="sxs-lookup"><span data-stu-id="da6eb-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="da6eb-682">Жобалар мен тапсырмалар шектеулері мен шекаралары</span><span class="sxs-lookup"><span data-stu-id="da6eb-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="da6eb-683">Қатені өңдеу</span><span class="sxs-lookup"><span data-stu-id="da6eb-683">Error handling</span></span>

   - <span data-ttu-id="da6eb-684">Операциялық жиындардан туындаған қателерді қарап шығу үшін **Параметрлер** \> **Кесте интеграциясы** \> **Операциялар жиындары** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="da6eb-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="da6eb-685">Жобаны жоспарлау қызметінен туындаған қателерді қарау үшін **Параметрлер** \> **Кесте интеграциясы** \> **PSS қателерін тіркеу журналы** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="da6eb-685">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="da6eb-686">Үлгі сценарий</span><span class="sxs-lookup"><span data-stu-id="da6eb-686">Sample scenario</span></span>

<span data-ttu-id="da6eb-687">Бұл сценарийде сіз жоба, топ мүшесі, төрт тапсырма және екі ресурстық тағайындама жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="da6eb-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="da6eb-688">Әрі қарай бір тапсырманы жаңартасыз, жобаны жаңартасыз, бір тапсырманы жоясыз, ресурстардың бір тағайындамасын жоясыз және тапсырмаға тәуелділікті жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="da6eb-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="da6eb-689">Қосымша үлгілер</span><span class="sxs-lookup"><span data-stu-id="da6eb-689">Additional samples</span></span>

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
