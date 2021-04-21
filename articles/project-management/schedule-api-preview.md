---
title: Жоспарлау нысандары операцияларын орындау үшін жоспарлау API интерфейстерін пайдалану
description: Бұл тақырыпта жоспарлау API интерфейстерін қолдануға арналған ақпарат пен үлгілері берілген.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868136"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="0fe64-103">Жоспарлау нысандары операцияларын орындау үшін жоспарлау API интерфейстерін пайдалану</span><span class="sxs-lookup"><span data-stu-id="0fe64-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="0fe64-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="0fe64-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="0fe64-105">Осы бөлімде айтылған кейбір немесе барлық мүмкіндіктер алдын ала қарау бөлігі ретінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="0fe64-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="0fe64-106">Мазмұны мен функциялар өзгеруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="0fe64-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="0fe64-107">Жоспарлау нысандары</span><span class="sxs-lookup"><span data-stu-id="0fe64-107">Scheduling entities</span></span>

<span data-ttu-id="0fe64-108">Жоспарлау API интерфейстері **Жоспарлау нысандары** арқылы операцияларды жасау, жаңарту және жою мүмкіндіктерін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="0fe64-109">Бұл нысандар веб-нұсқаға арналған жобада жоспарлау механизмі арқылы басқарылады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="0fe64-110">**Жоспарлау нысандары** көмегімен операцияларды жасау, жаңарту және жою алдыңғы Dynamics 365 Project Operations шығарылымдарында шектеулі болды.</span><span class="sxs-lookup"><span data-stu-id="0fe64-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="0fe64-111">Келесі кестеде **Жоспарлау нысандарының** толық тізімі берілген.</span><span class="sxs-lookup"><span data-stu-id="0fe64-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="0fe64-112">Нысан атауы</span><span class="sxs-lookup"><span data-stu-id="0fe64-112">Entity name</span></span>  | <span data-ttu-id="0fe64-113">Нысанның логикалық атауы</span><span class="sxs-lookup"><span data-stu-id="0fe64-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="0fe64-114">Project</span><span class="sxs-lookup"><span data-stu-id="0fe64-114">Project</span></span> | <span data-ttu-id="0fe64-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="0fe64-115">msdyn_project</span></span> |
| <span data-ttu-id="0fe64-116">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="0fe64-116">Project Task</span></span>  | <span data-ttu-id="0fe64-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="0fe64-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="0fe64-118">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="0fe64-118">Project Task Dependency</span></span>  | <span data-ttu-id="0fe64-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="0fe64-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="0fe64-120">Ресурс тағайындауы</span><span class="sxs-lookup"><span data-stu-id="0fe64-120">Resource Assignment</span></span> | <span data-ttu-id="0fe64-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="0fe64-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="0fe64-122">Жоба контейнері</span><span class="sxs-lookup"><span data-stu-id="0fe64-122">Project Bucket</span></span>  | <span data-ttu-id="0fe64-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="0fe64-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="0fe64-124">Жоба тобы мүшесі</span><span class="sxs-lookup"><span data-stu-id="0fe64-124">Project Team Member</span></span> | <span data-ttu-id="0fe64-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="0fe64-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="0fe64-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="0fe64-126">OperationSet</span></span>

<span data-ttu-id="0fe64-127">OperationSet — транзакция шеңберінде бірнеше кестеге әсер ететін сұраныстарды өңдеу қажет болған кезде қолдануға болатын жұмыс бірлігінің үлгісі.</span><span class="sxs-lookup"><span data-stu-id="0fe64-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="0fe64-128">Жоспарлау API интерфейстері</span><span class="sxs-lookup"><span data-stu-id="0fe64-128">Schedule APIs</span></span>

<span data-ttu-id="0fe64-129">Төменде қазіргі жоспарлау API интерфейстерінің тізімі берілген.</span><span class="sxs-lookup"><span data-stu-id="0fe64-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="0fe64-130">**msdyn_CreateProjectV1**: бұл API интерфейсін жобаны құру үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="0fe64-131">Жоба және әдепкі жоба контейнері дереу жасалады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="0fe64-132">**msdyn_CreateTeamMemberV1**: бұл API интерфейсін жоба тобының мүшесін құру үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="0fe64-133">Топ мүшелерінің жазбасы дереу жасалады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="0fe64-134">**msdyn_CreateOperationSetV1**: бұл API интерфейсін транзакция кезінде орындалуы керек бірнеше сұраныстарды жоспарлау үшін қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="0fe64-135">**msdyn_PSSCreateV1**: бұл API интерфейсін нысанды құру үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="0fe64-136">Нысан құру операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="0fe64-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="0fe64-137">**msdyn_PSSUpdateV1**: бұл API интерфейсін нысанды жаңарту үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="0fe64-138">Нысанды жаңарту операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="0fe64-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="0fe64-139">**msdyn_PSSDeleteV1**: бұл API интерфейсін нысанды жою үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="0fe64-140">Нысанды жою операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="0fe64-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="0fe64-141">**msdyn_ExecuteOperationSetV1**: бұл API берілген операциялар жиынтығындағы барлық әрекеттерді орындау үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="0fe64-142">OperationSet көмегімен жоспарлау API интерфейстерін пайдалану</span><span class="sxs-lookup"><span data-stu-id="0fe64-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="0fe64-143">**CreateProjectV1** және **CreateTeamMemberV1** дереу жасалатындықтан, бұл API интерфейстерін тікелей **OperationSet** жинағында пайдалануға болмайды.</span><span class="sxs-lookup"><span data-stu-id="0fe64-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="0fe64-144">Алайда API интерфейсін қажетті жазбаларды, **OperationSet** жасау үшін, содан кейін осы алдын ала жасалған жазбаларды **OperationSet** ішінде пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="0fe64-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="0fe64-145">Қолдау көрсетілетін операциялар</span><span class="sxs-lookup"><span data-stu-id="0fe64-145">Supported operations</span></span>

| <span data-ttu-id="0fe64-146">Жоспарлау нысаны</span><span class="sxs-lookup"><span data-stu-id="0fe64-146">Scheduling entity</span></span> | <span data-ttu-id="0fe64-147">Жасау</span><span class="sxs-lookup"><span data-stu-id="0fe64-147">Create</span></span> | <span data-ttu-id="0fe64-148">Жаңарту</span><span class="sxs-lookup"><span data-stu-id="0fe64-148">Update</span></span> | <span data-ttu-id="0fe64-149">Delete</span><span class="sxs-lookup"><span data-stu-id="0fe64-149">Delete</span></span> | <span data-ttu-id="0fe64-150">Маңызды жайттар</span><span class="sxs-lookup"><span data-stu-id="0fe64-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="0fe64-151">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="0fe64-151">Project task</span></span> | <span data-ttu-id="0fe64-152">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-152">Yes</span></span> | <span data-ttu-id="0fe64-153">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-153">Yes</span></span> | <span data-ttu-id="0fe64-154">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-154">Yes</span></span> | <span data-ttu-id="0fe64-155">Ешқайсысы</span><span class="sxs-lookup"><span data-stu-id="0fe64-155">None</span></span> |
| <span data-ttu-id="0fe64-156">Жоба тапсырмасы тәуелділігі</span><span class="sxs-lookup"><span data-stu-id="0fe64-156">Project task dependency</span></span> | <span data-ttu-id="0fe64-157">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-157">Yes</span></span> | <span data-ttu-id="0fe64-158">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-158">Yes</span></span> | | <span data-ttu-id="0fe64-159">Жоба тапсырмасына тәуелділік туралы жазбалар жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="0fe64-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="0fe64-160">Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="0fe64-161">Ресурс тағайындауы</span><span class="sxs-lookup"><span data-stu-id="0fe64-161">Resource assignment</span></span> | <span data-ttu-id="0fe64-162">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-162">Yes</span></span> | <span data-ttu-id="0fe64-163">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-163">Yes</span></span> | | <span data-ttu-id="0fe64-164">Келесі өрістермен операцияларға қолдау көрсетілмейді: **BookableResourceID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining** және **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="0fe64-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="0fe64-165">Ресурстарды тағайындау туралы жазбалар жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="0fe64-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="0fe64-166">Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="0fe64-167">Жоба контейнері</span><span class="sxs-lookup"><span data-stu-id="0fe64-167">Project bucket</span></span> | <span data-ttu-id="0fe64-168">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="0fe64-168">N/A</span></span> | <span data-ttu-id="0fe64-169">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="0fe64-169">N/A</span></span> | <span data-ttu-id="0fe64-170">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="0fe64-170">N/A</span></span> | <span data-ttu-id="0fe64-171">Әдепкі контейнер **CreateProjectV1** API интерфейсі арқылы жасалады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="0fe64-172">Жоба тобының мүшесі</span><span class="sxs-lookup"><span data-stu-id="0fe64-172">Project team member</span></span> | <span data-ttu-id="0fe64-173">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-173">Yes</span></span> | <span data-ttu-id="0fe64-174">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-174">Yes</span></span> | <span data-ttu-id="0fe64-175">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-175">Yes</span></span> | <span data-ttu-id="0fe64-176">Жасау операциясы үшін **CreateTeamMemberV1** API интерфейсін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="0fe64-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="0fe64-177">Project</span><span class="sxs-lookup"><span data-stu-id="0fe64-177">Project</span></span> | <span data-ttu-id="0fe64-178">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-178">Yes</span></span> | <span data-ttu-id="0fe64-179">Иә</span><span class="sxs-lookup"><span data-stu-id="0fe64-179">Yes</span></span> | <span data-ttu-id="0fe64-180">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="0fe64-180">N/A</span></span> | <span data-ttu-id="0fe64-181">Келесі өрістермен операцияларға қолдау көрсетілмейді: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining**, **Орындалу барысы**, **Аяқтау**, **TaskEarliestStart** және **Ұзақтығы**.</span><span class="sxs-lookup"><span data-stu-id="0fe64-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="0fe64-182">Бұл API интерфейсін реттелетін өрістерді қамтитын нысан объектілерімен шақыруға болады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="0fe64-183">ID сипаты міндетті емес.</span><span class="sxs-lookup"><span data-stu-id="0fe64-183">The ID property is optional.</span></span> <span data-ttu-id="0fe64-184">Егер ол қарастырылған болса, жүйе оны қолдануға әрекет жасайды және оны пайдалану мүмкін болмаса, ерекше жағдай жасайды.</span><span class="sxs-lookup"><span data-stu-id="0fe64-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="0fe64-185">Егер ол қарастырылмаған болса, жүйе оны жасайды.</span><span class="sxs-lookup"><span data-stu-id="0fe64-185">If it isn't provided, the system will generate it.</span></span>

## <a name="limitations-and-known-issues"></a><span data-ttu-id="0fe64-186">Шектеулер мен белгілі қателер</span><span class="sxs-lookup"><span data-stu-id="0fe64-186">Limitations and known issues</span></span>
<span data-ttu-id="0fe64-187">Төменде шектеулер мен белгілі мәселелер тізімі берілген:</span><span class="sxs-lookup"><span data-stu-id="0fe64-187">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="0fe64-188">Жоспарлау API интерфейстерін тек **Microsoft жоба лицензиясы бар пайдаланушылар** пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-188">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="0fe64-189">Оларды пайдалана алмайды:</span><span class="sxs-lookup"><span data-stu-id="0fe64-189">They can't be used by:</span></span>
    - <span data-ttu-id="0fe64-190">Бағдарлама пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="0fe64-190">Application users</span></span>
    - <span data-ttu-id="0fe64-191">Жүйе пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="0fe64-191">System users</span></span>
    - <span data-ttu-id="0fe64-192">Интеграция пайдаланушылары</span><span class="sxs-lookup"><span data-stu-id="0fe64-192">Integration users</span></span>
    - <span data-ttu-id="0fe64-193">Қажетті лицензиясы жоқ басқа пайдаланушылар</span><span class="sxs-lookup"><span data-stu-id="0fe64-193">Other users that don't have the required license</span></span>
- <span data-ttu-id="0fe64-194">Әр **OperationSet** ең көбі 100 операция жасай алады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-194">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="0fe64-195">Әрбір пайдаланушыда ең көбі 10 ашық **OperationSets** бола алады.</span><span class="sxs-lookup"><span data-stu-id="0fe64-195">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="0fe64-196">Қазіргі уақытта Project Operations жобадағы ең көбі 500 тапсырманы қолдайды.</span><span class="sxs-lookup"><span data-stu-id="0fe64-196">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="0fe64-197">**OperationSet** ақаулық күйі және сәтсіздік журналдары қазіргі уақытта қолжетімді емес.</span><span class="sxs-lookup"><span data-stu-id="0fe64-197">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="0fe64-198">Жоспарлау API интерфейстері жалпыға қолжетімді алдын ала қарау нұсқасында орналасқан.</span><span class="sxs-lookup"><span data-stu-id="0fe64-198">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="0fe64-199">Бұл API интерфейстерін жұмыс ортасында пайдалануға Microsoft қолдау көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="0fe64-199">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="0fe64-200">Үлгі сценарий</span><span class="sxs-lookup"><span data-stu-id="0fe64-200">Sample scenario</span></span>

<span data-ttu-id="0fe64-201">Бұл сценарийде сіз жоба, топ мүшесі, төрт тапсырма және екі ресурстық тағайындама жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="0fe64-201">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="0fe64-202">Әрі қарай бір тапсырманы жаңартасыз, жобаны жаңартасыз, бір тапсырманы жоясыз, ресурстардың бір тағайындамасын жоясыз және тапсырмаға тәуелділікті жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="0fe64-202">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```C#
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
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="0fe64-203">Қосымша үлгілер</span><span class="sxs-lookup"><span data-stu-id="0fe64-203">Additional samples</span></span>

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
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
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
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
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
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
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
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
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
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
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
