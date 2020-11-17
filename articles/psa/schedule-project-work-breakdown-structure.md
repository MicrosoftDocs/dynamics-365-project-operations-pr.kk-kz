---
title: Жұмыс декомпозициясының құрылымымен жобаны жоспарлау
description: Project Service жүйесінде жұмыс декомпозициясының құрылымымен жобаны жоспарлау жолы
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
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
ms.openlocfilehash: 04f30f2f2ed93dd1525f1c86a7521cdbf39a77bc
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127885"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a><span data-ttu-id="026c1-103">Жұмыс декомпозициясының құрылымымен жобаны жоспарлау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="026c1-103">Schedule a project with a work breakdown structure (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="026c1-104">Жоба кестесі орындалатын жұмыспен, жұмысты орындайтын ресурстармен және жұмыс аяқталатын уақыт шкаласымен байланысады.</span><span class="sxs-lookup"><span data-stu-id="026c1-104">A project schedule communicates what work needs to be performed, which resources will perform the work, and the timeframe in which that work needs to be completed.</span></span> <span data-ttu-id="026c1-105">Жоба кестесі жобаны уақытылы жеткізумен байланысты барлық жұмысқа әсер етеді.</span><span class="sxs-lookup"><span data-stu-id="026c1-105">The project schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="026c1-106">Жобаның бастапқы фазасындағы алғашқы қадамдардың бірі — жоба кестесімен келу.</span><span class="sxs-lookup"><span data-stu-id="026c1-106">One of the first steps in the initiation phase of the project is to come up with a project schedule.</span></span> <span data-ttu-id="026c1-107">Жоба кестесін анықтау үшін жұмыс декомпозициясының құрылымын жасау керек.</span><span class="sxs-lookup"><span data-stu-id="026c1-107">To establish a project schedule, you need to create a work breakdown structure.</span></span>  
  
 <span data-ttu-id="026c1-108">Келесі әрекеттермен көмектесетін жұмыс декомпозициясының құрылымымен жоба құрылымын жасаңыз:</span><span class="sxs-lookup"><span data-stu-id="026c1-108">Create a project structure with a work breakdown structure, which helps you:</span></span>  
  
- <span data-ttu-id="026c1-109">Жұмысты басқарылатын тапсырмаларға бөлу</span><span class="sxs-lookup"><span data-stu-id="026c1-109">Break down work into manageable tasks</span></span>  
  
- <span data-ttu-id="026c1-110">Тапсырманы аяқтауға талап етілетін уақытты бағалау</span><span class="sxs-lookup"><span data-stu-id="026c1-110">Estimate the time required to complete a task</span></span>  
  
- <span data-ttu-id="026c1-111">Тапсырма тәуелділіктерін және тапсырма ұзақтығын орнату</span><span class="sxs-lookup"><span data-stu-id="026c1-111">Set task dependencies and task duration</span></span>  
  
- <span data-ttu-id="026c1-112">Әрбір тапсырманы аяқтауға қажетті рөлдерді анықтау</span><span class="sxs-lookup"><span data-stu-id="026c1-112">Determine the roles required to complete each task</span></span>  
  
  <span data-ttu-id="026c1-113">Жұмыс декомпозициясының құрылымындағы жоба кестесінде таныс көрініс пен түсінік бар, интерактивті Гант диаграммасымен аяқтаңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-113">The project schedule in the work breakdown structure has a familiar look and feel, complete with an interactive Gantt chart.</span></span>  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a><span data-ttu-id="026c1-114">Жоба үшін жұмыс декомпозициясының құрылымын жасау</span><span class="sxs-lookup"><span data-stu-id="026c1-114">Create a work breakdown structure for a project</span></span>  
 <span data-ttu-id="026c1-115">Жобадағы тапсырмалар ретін көрсету үшін жұмыс декомпозициясының құрылымын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-115">Create a work breakdown structure to represent the sequence of tasks in a project.</span></span> <span data-ttu-id="026c1-116">Жұмыс декомпозициясының құрылымына тапсырмалар, әрбір тапсырма талаптары, табыс пен шығын туралы ақпарат кіреді.</span><span class="sxs-lookup"><span data-stu-id="026c1-116">The work breakdown structure includes tasks, requirements for each task, and revenue and cost information.</span></span> <span data-ttu-id="026c1-117">Жұмыс декомпозициясының құрылымында келесілерді қосуға болады:</span><span class="sxs-lookup"><span data-stu-id="026c1-117">In your work breakdown structure, you can add:</span></span>  
  
-   <span data-ttu-id="026c1-118">Иерархиядағы тапсырмалар реті</span><span class="sxs-lookup"><span data-stu-id="026c1-118">The sequence of tasks in a hierarchy</span></span>  
  
-   <span data-ttu-id="026c1-119">Тапсырманы бастау алдында аяқталуы қажет басқа тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="026c1-119">Other tasks, if any, that must be completed before a task can be started</span></span>  
  
-   <span data-ttu-id="026c1-120">Тапсырманың басталу күні, аяқталу күні және ұзақтығы</span><span class="sxs-lookup"><span data-stu-id="026c1-120">The starting date, ending date, and duration of a task</span></span>  
  
-   <span data-ttu-id="026c1-121">Тапсырмаға қажетті сағаттар саны</span><span class="sxs-lookup"><span data-stu-id="026c1-121">The number of hours required for a task</span></span>  
  
-   <span data-ttu-id="026c1-122">Кез келген қажетті жұмысшы біліктіліктері және білімі</span><span class="sxs-lookup"><span data-stu-id="026c1-122">Any required worker skills and education</span></span>  
  
-   <span data-ttu-id="026c1-123">Тапсырмаға тағайындалған жұмысшылар</span><span class="sxs-lookup"><span data-stu-id="026c1-123">The workers who are assigned to a task</span></span>  
  
-   <span data-ttu-id="026c1-124">Болжалды табыс пен шығындар</span><span class="sxs-lookup"><span data-stu-id="026c1-124">Estimated revenue and costs</span></span>  
  
## <a name="task-types"></a><span data-ttu-id="026c1-125">Тапсырма түрлері</span><span class="sxs-lookup"><span data-stu-id="026c1-125">Task types</span></span>  
<span data-ttu-id="026c1-126">Жұмыс декомпозициясының құрылымын жасау кезінде келесі тапсырма түрлерін пайдалануға болады:</span><span class="sxs-lookup"><span data-stu-id="026c1-126">You’ll use the following types of tasks when creating your work breakdown structure:</span></span>  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| <span data-ttu-id="026c1-127">**Жобаның түбірлік түйіні**</span><span class="sxs-lookup"><span data-stu-id="026c1-127">**Project root node**</span></span> | <span data-ttu-id="026c1-128">Жобаға арналған жоғарғы деңгейлі қорытынды тапсырма.</span><span class="sxs-lookup"><span data-stu-id="026c1-128">The top-level summary task for the project.</span></span> <span data-ttu-id="026c1-129">Барлық басқа жоба тапсырмалары осының астында жасалады.</span><span class="sxs-lookup"><span data-stu-id="026c1-129">All other project tasks are created under it.</span></span> <span data-ttu-id="026c1-130">Түбірлік тапсырма аты — жоба аты.</span><span class="sxs-lookup"><span data-stu-id="026c1-130">The name of the root task is the project name.</span></span> <span data-ttu-id="026c1-131">Түбірлік түйін талпынысы, күндері және ұзақтығы төмендегі иерархиядағы мәндерге негізделеді.</span><span class="sxs-lookup"><span data-stu-id="026c1-131">The effort, dates, and duration of the root node are based on the values on the hierarchy below it.</span></span> <span data-ttu-id="026c1-132">Түбірлік түйін сипаттарын өңдеу немесе түбірлік түйінді өшіру мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="026c1-132">You can’t edit root node properties or delete the root node.</span></span> | 
| <span data-ttu-id="026c1-133">**Қорытынды немесе контейнер тапсырмалары**</span><span class="sxs-lookup"><span data-stu-id="026c1-133">**Summary or container tasks**</span></span> | <span data-ttu-id="026c1-134">Қорытынды тапсырма — қосалқы тапсырмалардан тұратын тапсырма.</span><span class="sxs-lookup"><span data-stu-id="026c1-134">A summary task is a task that has sub-tasks under it.</span></span> <span data-ttu-id="026c1-135">Қорытынды тапсырмада ешбір жұмыс талпынысы немесе өзіндік құны жоқ.</span><span class="sxs-lookup"><span data-stu-id="026c1-135">A summary task doesn’t have any work effort or cost of its own.</span></span> <span data-ttu-id="026c1-136">Жұмыс талпынысы мен құны — қосалқы тапсырмалар жиынтығы.</span><span class="sxs-lookup"><span data-stu-id="026c1-136">Its work effort and cost are a rollup of its sub-tasks.</span></span> <span data-ttu-id="026c1-137">Қорытынды тапсырма атын өзгертуге болады, бірақ талпынысты, күндерді немесе ұзақтықты өзгерту мүмкін емес, себебі олар автоматты түрде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="026c1-137">You can change the name of a summary task, but you can’t change the effort, dates, or duration, because those are automatically calculated.</span></span> <span data-ttu-id="026c1-138">Қорытынды тапсырманы өшіру тапсырма мен барлық қосалқы тапсырмаларды өшіреді.</span><span class="sxs-lookup"><span data-stu-id="026c1-138">Deleting a summary task deletes the task and all of its sub-tasks.</span></span>|  
| <span data-ttu-id="026c1-139">**Соңғы түйін тапсырмалары**</span><span class="sxs-lookup"><span data-stu-id="026c1-139">**Leaf node tasks**</span></span> | <span data-ttu-id="026c1-140">Соңғы түйін тапсырмасы жобадағы толық мәліметті жұмысты көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="026c1-140">A leaf node task represents the most detailed work on the project.</span></span> <span data-ttu-id="026c1-141">Мұнда болжалды талпыныс, жоспарлы ресурстар саны, жоспарлы басталу және аяқталу күндері, ұзақтығы бар.</span><span class="sxs-lookup"><span data-stu-id="026c1-141">It has an estimated effort, a planned number of resources, planned start and end dates, and a duration.</span></span>|

  
## <a name="task-hierarchy"></a><span data-ttu-id="026c1-142">Тапсырма иерархиясы</span><span class="sxs-lookup"><span data-stu-id="026c1-142">Task hierarchy</span></span>  
 <span data-ttu-id="026c1-143">Тапсырма иерархиясын жасау кезінде келесі опциялар бар:</span><span class="sxs-lookup"><span data-stu-id="026c1-143">You have the following options when creating a task hierarchy:</span></span>  
  
- <span data-ttu-id="026c1-144">**Тапсырма қосу**.</span><span class="sxs-lookup"><span data-stu-id="026c1-144">**Add task**.</span></span>   <span data-ttu-id="026c1-145">Тапсырма иерархиясында таңдау кезінде орынға тапсырма қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="026c1-145">You can add a task at a position you choose in the task hierarchy.</span></span> <span data-ttu-id="026c1-146">Егер орын таңдалмаса, жаңа тапсырма соңында пайда болады.</span><span class="sxs-lookup"><span data-stu-id="026c1-146">If you don’t select a position, your new task appears at the end.</span></span>  
  
- <span data-ttu-id="026c1-147">**Тапсырма жасау**.</span><span class="sxs-lookup"><span data-stu-id="026c1-147">**Indent task**.</span></span>   <span data-ttu-id="026c1-148">Тапсырманың тікелей үстінде еншілес жасау үшін тапсырма жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-148">Indent a task to make it a child of the task directly above it.</span></span>  
  
- <span data-ttu-id="026c1-149">**Тапсырма шығару**.</span><span class="sxs-lookup"><span data-stu-id="026c1-149">**Outdent task**.</span></span>   <span data-ttu-id="026c1-150">Бастапқы негізгі тапсырманың қосалқы тапсырмасын болдырмау үшін тапсырманы шығарыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-150">Outdent a task to make it so it’s no longer a sub-task of its original parent task.</span></span>  
  
- <span data-ttu-id="026c1-151">**Жоғары жылжыту және төмен жылжыту**.</span><span class="sxs-lookup"><span data-stu-id="026c1-151">**Move up and Move down**.</span></span>   <span data-ttu-id="026c1-152">Негізгі тапсырма иерархиясында тапсырмаларды жоғары және төмен жылжытыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-152">Move tasks up and down in the hierarchy of its parent task.</span></span> <span data-ttu-id="026c1-153">Тапсырманы жоғары немесе төмен жылжыту талпынысқа, құнға, күндерге немесе ұзақтыққа әсер етпейді.</span><span class="sxs-lookup"><span data-stu-id="026c1-153">Moving a task up or down has no effect on its effort, cost, dates, or duration.</span></span>  
  
## <a name="task-attributes"></a><span data-ttu-id="026c1-154">Тапсырма төлсипаттары</span><span class="sxs-lookup"><span data-stu-id="026c1-154">Task attributes</span></span>  
 <span data-ttu-id="026c1-155">Тапсырма аты орындалуы керек жұмысты сипаттайды.</span><span class="sxs-lookup"><span data-stu-id="026c1-155">A task’s name describes the work that needs to be completed.</span></span> <span data-ttu-id="026c1-156">Тапсырма кестесін және материал талаптарын сипаттауға түрлі тапсырма төлсипаттарын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-156">You use various task attributes to describe the schedule and staffing requirements for the task.</span></span>  
  
### <a name="schedule-attributes"></a><span data-ttu-id="026c1-157">Кесте төлсипаттары</span><span class="sxs-lookup"><span data-stu-id="026c1-157">Schedule attributes</span></span>

 - <span data-ttu-id="026c1-158">Тапсырма кестесін анықтау үшін **Талпыныс сағаттары**, **Ресурстар саны**, **Басталу күні**, **Аяқталу күні** және **Ұзақтық** параметрлеріне мән белгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="026c1-158">Assign values to **Effort hours**, **Number of resources**, **Start date**, **End date**, and **Duration** to determine the schedule for the task.</span></span> 
 - <span data-ttu-id="026c1-159">**Талпыныс** — тапсырманы аяқтауға кететін сағаттар болжамы.</span><span class="sxs-lookup"><span data-stu-id="026c1-159">**Effort** is an estimate of the hours it takes to complete the task.</span></span>
 - <span data-ttu-id="026c1-160">**Ресурстар саны** — ең ықтимал кестені алу үшін жоба менеджерінің болжалды салымы.</span><span class="sxs-lookup"><span data-stu-id="026c1-160">**Number of resources** is an estimate that the project manager puts in the task to help come up with the best possible schedule.</span></span> 
 - <span data-ttu-id="026c1-161">**Ұзақтық** (күндер бойынша) тапсырманы аяқтауға кететін жұмыс күндері санын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="026c1-161">**Duration** (in days) indicates the number of work days it will take to complete the task.</span></span>  
  
### <a name="staffing-attributes"></a><span data-ttu-id="026c1-162">Материал төлсипаттары</span><span class="sxs-lookup"><span data-stu-id="026c1-162">Staffing attributes</span></span>

 - <span data-ttu-id="026c1-163">**Рөл**, **Ресурс ұйымдық бірлігі**, **Ресурстар саны** және **Ресурстар** тапсырманың материалдық талаптарын сипаттайды.</span><span class="sxs-lookup"><span data-stu-id="026c1-163">**Role**, **Resource organizational unit**, **Number of resources**, and **Resources** describe the staffing requirements for the task.</span></span> 
 - <span data-ttu-id="026c1-164">**Рөл** тапсырманы орындауға керек ресурс түрін сипаттайды.</span><span class="sxs-lookup"><span data-stu-id="026c1-164">**Role** describes the type of resource needed to perform the task.</span></span> 
 - <span data-ttu-id="026c1-165">**Ресурс ұйымдық бірлігі** осы тапсырмаға берілетін ресурстардың ұйымдық бірлігін көрсетеді; сонымен қатар, бұл құн мен сатылым болжамына әсер етеді, себебі ресурстың бірлік сатылым бағасын анықтау кезінде есепке алынады.</span><span class="sxs-lookup"><span data-stu-id="026c1-165">**Resource organizational unit** indicates the organizational unit from which resources should be staffed for that task; this also impacts the cost and sales estimate of the task, since this is accounted for when determining the unit sales price for the resource.</span></span> 
 - <span data-ttu-id="026c1-166">**Ресурстар** біреуі табылған кезінде жалпы ресурсты немесе атаулы ресурсты сақтайды.</span><span class="sxs-lookup"><span data-stu-id="026c1-166">**Resources** holds a generic resource or a named resource when one is found.</span></span>  
  
## <a name="task-dependencies"></a><span data-ttu-id="026c1-167">Тапсырма тәуелділіктері</span><span class="sxs-lookup"><span data-stu-id="026c1-167">Task dependencies</span></span>  
 <span data-ttu-id="026c1-168">Жұмыс декомпозициясының құрылымындағы бір немесе бірнеше тапсырма арасындағы алдыңғы қарым-қатынастарды жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="026c1-168">You can create predecessor relationships between one or more tasks in the work breakdown structure.</span></span> <span data-ttu-id="026c1-169">Тәуелді болатын тапсырмаларды көрсету үшін тапсырмаларды алдыңғы өрістің бір немесе бірнеше мәнін орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="026c1-169">You can set one or more values for the predecessor field on tasks to indicate the tasks that it will be dependent on.</span></span> <span data-ttu-id="026c1-170">Тапсырма алдыңғы мән белгіленген кезде барлық алдыңғы тапсырмалар аяқталған кезде ғана тапсырма басталуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="026c1-170">When you assign a predecessor value to a task, the task can only start when all the predecessor tasks have completed.</span></span> <span data-ttu-id="026c1-171">Тапсырмаға осы тәуелділікті орнату тапсырманың жоспарлы басталу күнін барлық бастапқыларының ең соңғы аяқталуы ретінде қайта есептеуге әкеледі.</span><span class="sxs-lookup"><span data-stu-id="026c1-171">Setting this dependency on a task will result in the recalculation of the planned start date of the task as the latest end of all of its predecessors.</span></span> <span data-ttu-id="026c1-172">Кестедегі бастапқысына қатысты әсерлер тапсырмада анықталған тапсырма режимімен шектелмейді.</span><span class="sxs-lookup"><span data-stu-id="026c1-172">Predecessor-related impacts on a schedule are not limited by the task mode defined on the task.</span></span>  
  
## <a name="task-mode"></a><span data-ttu-id="026c1-173">Тапсырма режимі</span><span class="sxs-lookup"><span data-stu-id="026c1-173">Task mode</span></span>  
 <span data-ttu-id="026c1-174">Тапсырма режимі — жоспарлы соңғы түйін тапсырмаларын анықтайтын маңызды факторлардың бірі.</span><span class="sxs-lookup"><span data-stu-id="026c1-174">Task mode is one of the important factors that determine scheduling leaf node tasks.</span></span> <span data-ttu-id="026c1-175">Әрбір тапсырма үшін екі тапсырма режимі бар: авто жоспарлау режимі және қолмен жоспарлау режимі.</span><span class="sxs-lookup"><span data-stu-id="026c1-175">There are two task modes for every task: auto scheduling mode and manual scheduling mode.</span></span>  
  
-   <span data-ttu-id="026c1-176">**Авто жоспарлау**.</span><span class="sxs-lookup"><span data-stu-id="026c1-176">**Auto scheduling**.</span></span>   <span data-ttu-id="026c1-177">Тапсырма режимін «Автоматты түрде жоспарланады» күйіне орнатқан кезде тапсырманы жоспарлау механизмінде тапсырма кестесін анықтау үшін келесі тапсырма төлсипаттарындағы жоспарлау ережелері пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="026c1-177">When you set the task mode to Automatically Scheduled, the task scheduling engine uses the scheduling rules on the following task attributes to determine the schedule for the task:</span></span>  
  
    -   <span data-ttu-id="026c1-178">Бастапқылар</span><span class="sxs-lookup"><span data-stu-id="026c1-178">Predecessors</span></span>  
  
    -   <span data-ttu-id="026c1-179">Күш-жігер</span><span class="sxs-lookup"><span data-stu-id="026c1-179">Effort</span></span>  
  
    -   <span data-ttu-id="026c1-180">Ресурстар саны</span><span class="sxs-lookup"><span data-stu-id="026c1-180">Number of resources</span></span>  
  
    -   <span data-ttu-id="026c1-181">Басталу және аяқталу күндері</span><span class="sxs-lookup"><span data-stu-id="026c1-181">Start and end dates</span></span>  
  
-   <span data-ttu-id="026c1-182">**Жоспарлау ережелері**.</span><span class="sxs-lookup"><span data-stu-id="026c1-182">**Scheduling rules**.</span></span>   <span data-ttu-id="026c1-183">Бұрынғы тапсырмалардың әдепкі мәндері жоқ соңғы түйін тапсырмасының басталу күні әдепкі бойынша жобаның жоспарланған басталу күніне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="026c1-183">The start date of a leaf node task that does not have predecessors defaults to the project’s scheduling start date.</span></span> <span data-ttu-id="026c1-184">Соңғы түйін тапсырмасының ұзақтығы басталу және аяқталу күндері арасындағы жұмыс күндері ретінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="026c1-184">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="026c1-185">Тапсырма автоматты түрде жоспарланған кезде жоспарлау механизмі төмендегі ережелерге сәйкес болады:</span><span class="sxs-lookup"><span data-stu-id="026c1-185">When a task is automatically scheduled, the scheduling engine follows the rules below:</span></span>  
  
    -   <span data-ttu-id="026c1-186">Тапсырманың басталу және аяқталу күндері жобаның жоспарлау күнтізбесіне сәйкес жұмыс күндері болуы қажет</span><span class="sxs-lookup"><span data-stu-id="026c1-186">Start and end dates of a task must always be working days according to the project’s scheduling calendar</span></span>  
  
    -   <span data-ttu-id="026c1-187">Бұрынғы тапсырмалардың әдепкі мәндері бар тапсырманың басталу күні әдепкі бойынша алдыңғы тапсырмалардың аяқталу күніне орнатылады</span><span class="sxs-lookup"><span data-stu-id="026c1-187">The start date of a task that has predecessors defaults to the latest end date of its predecessors</span></span>  
  
    -   <span data-ttu-id="026c1-188">Талпыныс = Адамдар саны \* Ұзақтық \* жоба күнтізбесінің стандартты жұмыс күніндегі сағаттар</span><span class="sxs-lookup"><span data-stu-id="026c1-188">Effort = Number of people \* Duration \* hours in a standard work day of the project calendar</span></span>  
  
-   <span data-ttu-id="026c1-189">**Қолмен жоспарлау**.</span><span class="sxs-lookup"><span data-stu-id="026c1-189">**Manual scheduling**.</span></span>   <span data-ttu-id="026c1-190">Кейбір жағдайларда осы ережелерден ауытқу керек болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="026c1-190">In some cases, you might want to deviate from these rules.</span></span> <span data-ttu-id="026c1-191">Осы жағдайларда қолмен жоспарланатын тапсырма режимін орнату керек болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="026c1-191">In these cases, you can set the task mode for the task to be manually scheduled.</span></span> <span data-ttu-id="026c1-192">Бұл жоспарлау механизмін басқа жоспарлау төлсипаттары мәндерін есептеуден тоқтатады.</span><span class="sxs-lookup"><span data-stu-id="026c1-192">This stops the scheduling engine from calculating the values for other scheduling attributes.</span></span> <span data-ttu-id="026c1-193">Тапсырмаларда бастапқыларды орнату тәуелді тапсырманың басталу күніне әсер етеді.</span><span class="sxs-lookup"><span data-stu-id="026c1-193">Setting predecessors on tasks always impacts the dependent task’s start date.</span></span>  
  
## <a name="create-a-work-breakdown-structure"></a><span data-ttu-id="026c1-194">Жұмыс декомпозициясының құрылымын жасау</span><span class="sxs-lookup"><span data-stu-id="026c1-194">Create a work breakdown structure</span></span>  
  
1.  <span data-ttu-id="026c1-195">**Project Service > Жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="026c1-195">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="026c1-196">Жұмыс істеу керек жобаны басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-196">Click the project you want to work on.</span></span>  
  
3.  <span data-ttu-id="026c1-197">Экран үстіндегі жолақтан жоба атынан кейінгі төмен көрсеткісін таңдап, «Жұмыс декомпозициясының құрылымы» тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-197">In the bar across the top of the screen, select the down arrow next to the project name, and then click Work breakdown structure.</span></span>  
  
4.  <span data-ttu-id="026c1-198">Тапсырма қосу үшін **Тапсырма қосу** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-198">To add a task, click **Add Task**.</span></span> <span data-ttu-id="026c1-199">Тапсырма өрістерін толтырып, кейін **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-199">Fill in the fields for the task, and then click **Save**.</span></span>  
  
5.  <span data-ttu-id="026c1-200">Жұмыс декомпозициясының құрылымы аяқталғанша тапсырмалар қосуды жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-200">Continue adding tasks until your work breakdown structure is complete.</span></span> <span data-ttu-id="026c1-201">Жұмыс декомпозициясының құрылымын жасау кезінде тапсырмаларды ұйымдастыру үшін келесіні орындауға болады:</span><span class="sxs-lookup"><span data-stu-id="026c1-201">While creating your work breakdown structure, you can do the following to organize your tasks:</span></span>  
  
    -   <span data-ttu-id="026c1-202">Тапсырманы таңдап, оны басқа тапсырма астына жылжыту үшін **Туралау** түймешігін басыңыз немесе оны бір деңгейден шығару үшін «Шығару» түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-202">Select a task and click **Indent** to move it under another task or click Outdent to move it out a level.</span></span>  
  
    -   <span data-ttu-id="026c1-203">Тапсырманы таңдап, тізімде жоғары немесе төмен жылжыту үшін **Жоғары жылжыту** немесе **Төмен жылжыту** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-203">Select a task and click **Move Up** or **Move Down** to move it up or down in the list.</span></span>  
  
    -   <span data-ttu-id="026c1-204">Гант диаграммасын жасыру үшін **Гант диаграммасын жасыру** түймешігін басыңыз және оны қайта көрсету үшін **Гант диаграммасын көрсету** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-204">Click **Hide Gantt** to hide the Gantt chart, and click **Show Gantt** to display it again.</span></span>  
  
    -   <span data-ttu-id="026c1-205">**Уақыт шкаласы** ішінен Гант диаграммасының басқа уақыт кезеңін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-205">Select a different period of time for the Gantt chart in **Time Scale**.</span></span>  
  
6.  <span data-ttu-id="026c1-206">Жұмыс декомпозициясының құрылымында көрсетілген рөлдерді жобаның топ мүшелеріне қосу үшін **Жоба тобын құру** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-206">To add the roles you specified in your work breakdown structure to your project’s team members, click **Generate Project Team**.</span></span>  
  
7.  <span data-ttu-id="026c1-207">Өзгерістерді жасап болғаннан кейін экранның төменгі оң жақ бұрышында **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="026c1-207">Click **Save** at the bottom right corner of the screen when you’re done making changes.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="026c1-208">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="026c1-208">See Also</span></span>  
 [<span data-ttu-id="026c1-209">Жоба менеджерінің нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="026c1-209">Project manager guide</span></span>](../psa/project-manager-guide.md)
