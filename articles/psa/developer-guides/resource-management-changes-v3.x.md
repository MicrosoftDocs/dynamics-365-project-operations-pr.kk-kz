---
title: Ресурсты басқаруға енгізілген өзгерістер (Project Service Automation 3.x)
description: Бұл тақырыпта ресурсты басқару аймағына енгізілген өзгерістер туралы ақпарат берілген.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: e888d55b93c40e08e51bd4480853fec37f2b6333
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6007823"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="2e4cb-103">Ресурсты басқаруға енгізілген өзгерістер (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="2e4cb-103">Resource management changes (Project Service Automation 3.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

<span data-ttu-id="2e4cb-104">Тақырыптың бұл бөлімінде Dynamics 365 Project Service Automation 3.x нұсқасының ресурсты басқару аймағына енгізілген өзгерістер туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="2e4cb-105">Жоба болжамдары</span><span class="sxs-lookup"><span data-stu-id="2e4cb-105">Project estimates</span></span>

<span data-ttu-id="2e4cb-106">Жоба болжамдары **msdyn\_projecttask** нысанына (**Жоба тапсырмасы**) емес, **msdyn\_resourceassignment** нысанына (**Ресурс тағайындауы**) негізделеді.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-106">Instead of being based on the **msdyn\_projecttask** entity (**Project Task**), project estimates are based on the **msdyn\_resourceassignment** entity (**Resource Assignment**).</span></span> <span data-ttu-id="2e4cb-107">Ресурс тағайындаулары тапсырманы жоспарлауда және оның бағасын белгілеуде "ақиқат көзі" болды.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="2e4cb-108">Жол тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="2e4cb-108">Line tasks</span></span>

<span data-ttu-id="2e4cb-109">PSA 3.x нұсқасында жол тапсырмалары ескірген.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="2e4cb-110">Тағайындаулар енді жол тапсырмаларын емес, барлық тапсырмаларды көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="2e4cb-111">Келесі мысалда "Сынақтық тапсырма" деп аталатын тапсырманың бұрынғы PSA нұсқаларында және PSA 3.x нұсқасында A және B топ мүшелеріне қалай тағайындалғаны көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="2e4cb-112">**PSA 3.x нұсқасына дейін:**</span><span class="sxs-lookup"><span data-stu-id="2e4cb-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="2e4cb-113">Сынақтық тапсырма</span><span class="sxs-lookup"><span data-stu-id="2e4cb-113">Test task</span></span>

        - <span data-ttu-id="2e4cb-114">Сынақтық тапсырма — жол тапсырмасы 1</span><span class="sxs-lookup"><span data-stu-id="2e4cb-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="2e4cb-115">A мүшесіне тағайындау</span><span class="sxs-lookup"><span data-stu-id="2e4cb-115">Assignment to A</span></span>

        - <span data-ttu-id="2e4cb-116">Сынақтық тапсырма — жол тапсырмасы 2</span><span class="sxs-lookup"><span data-stu-id="2e4cb-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="2e4cb-117">B мүшесіне тағайындау</span><span class="sxs-lookup"><span data-stu-id="2e4cb-117">Assignment to B</span></span>

- <span data-ttu-id="2e4cb-118">**PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="2e4cb-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="2e4cb-119">Сынақтық тапсырма</span><span class="sxs-lookup"><span data-stu-id="2e4cb-119">Test task</span></span>

        - <span data-ttu-id="2e4cb-120">A мүшесіне тағайындау</span><span class="sxs-lookup"><span data-stu-id="2e4cb-120">Assignment to A</span></span>
        - <span data-ttu-id="2e4cb-121">B мүшесіне тағайындау</span><span class="sxs-lookup"><span data-stu-id="2e4cb-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="2e4cb-122">Тағайындалмаған тағайындама</span><span class="sxs-lookup"><span data-stu-id="2e4cb-122">Unassigned assignment</span></span>

<span data-ttu-id="2e4cb-123">PSA 3.x нұсқасындағы тағайындалмаған тағайындама дегеніміз — **БОС** топ мүшесіне немесе **БОС** ресурсқа тағайындалған тағайындама.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="2e4cb-124">Тағайындалмаған тағайындамалар бірнеше сценарийде орын алуы мүмкін:</span><span class="sxs-lookup"><span data-stu-id="2e4cb-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="2e4cb-125">Тапсырма жасалса, бірақ ешқандай топ мүшесіне тағайындалмаса, тағайындалмаған тағайындама жасалады.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="2e4cb-126">Тапсырмадағы тағайындалушылар өшірілсе, тапсырмада тағайындалмаған тағайындама қайтадан жасалады.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="2e4cb-127">Жобаның тапсырмасы нысанындағы өрістерді жоспарлау</span><span class="sxs-lookup"><span data-stu-id="2e4cb-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="2e4cb-128">**msdyn\_projecttask** нысанындағы өрістер ескірген немесе **msdyn\_resourceassignment** нысанына көшірілген, болмаса олардың сілтемесі ағымда **msdyn\_projectteam** нысанынан (**Жобаның топ мүшесі**) берілген.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity (**Project Team Member**).</span></span>

| <span data-ttu-id="2e4cb-129">msdyn\_projecttask (Жоба тапсырмасы) нысанындағы ескірген өріс</span><span class="sxs-lookup"><span data-stu-id="2e4cb-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="2e4cb-130">msdyn\_resourceassignment (Ресурс тағайындауы) нысанындағы жаңа өріс</span><span class="sxs-lookup"><span data-stu-id="2e4cb-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="2e4cb-131">Пікір</span><span class="sxs-lookup"><span data-stu-id="2e4cb-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="2e4cb-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="2e4cb-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="2e4cb-133">Ешқандай</span><span class="sxs-lookup"><span data-stu-id="2e4cb-133">None</span></span> | |
| <span data-ttu-id="2e4cb-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="2e4cb-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="2e4cb-135">Ешқандай</span><span class="sxs-lookup"><span data-stu-id="2e4cb-135">None</span></span> | |
| <span data-ttu-id="2e4cb-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="2e4cb-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="2e4cb-137">Ешқандай</span><span class="sxs-lookup"><span data-stu-id="2e4cb-137">None</span></span> | |
| <span data-ttu-id="2e4cb-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="2e4cb-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="2e4cb-139">Ешқандай</span><span class="sxs-lookup"><span data-stu-id="2e4cb-139">None</span></span> | |
| <span data-ttu-id="2e4cb-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="2e4cb-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="2e4cb-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="2e4cb-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="2e4cb-142">Өрісте сақталған JavaScript пішіміндегі нысан нотациясының (JSON) деректер құрылымының пішімі өзгерді.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="2e4cb-143">Кесте контуры</span><span class="sxs-lookup"><span data-stu-id="2e4cb-143">Schedule contour</span></span>

<span data-ttu-id="2e4cb-144">Кесте контуры әрбір **Ресурс тағайындауы** нысанының (**msdyn\_resourceassignment**) **Жоспарланған жұмыс** өрісінде (**msdyn\_plannedwork**) сақталады.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-144">The schedule contour is stored in the **Planned Work** field (**msdyn\_plannedwork**) of each **Resource Assignment** entity (**msdyn\_resourceassignment**).</span></span>

### <a name="structure"></a><span data-ttu-id="2e4cb-145">Құрылым</span><span class="sxs-lookup"><span data-stu-id="2e4cb-145">Structure</span></span>

<span data-ttu-id="2e4cb-146">Кесте контурының жаңа құрылымы кестенің әрбір күні үшін анықталған икемді уақыт кесінділерінен тұрады.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="2e4cb-147">Әрбір икемді уақыт кесіндісінің төмендегідей сипаттары бар:</span><span class="sxs-lookup"><span data-stu-id="2e4cb-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="2e4cb-148">**Басталуы** — жоба күнтізбесіне сәйкес, әрбір күннің жұмыс істеу сағаттарының басталатын уақыты.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="2e4cb-149">**Аяқталуы** — жоба күнтізбесіне сәйкес, әрбір күннің жұмыс істеу сағаттарының аяқталатын уақыты.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="2e4cb-150">**Сағат** — күн бойынша тағайындалған сағат саны.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="2e4cb-151">**Мысал**</span><span class="sxs-lookup"><span data-stu-id="2e4cb-151">**Example**</span></span>

<span data-ttu-id="2e4cb-152">Бұл мысалда жұмыс күні UTC-8 уақыт белдеуіндегі 9:00 - 17:00 уақытына сәйкес жоба күнтізбесі қолданылған.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="2e4cb-153">Автоматты түрде және қолмен жоспарлау</span><span class="sxs-lookup"><span data-stu-id="2e4cb-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="2e4cb-154">Тапсырма автоматты түрде жоспарланса, сағаттар төмендеп жүктеледі және тапсырма ұзақтығы азаюы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="2e4cb-155">**Мысал**</span><span class="sxs-lookup"><span data-stu-id="2e4cb-155">**Example**</span></span>

<span data-ttu-id="2e4cb-156">Келесі тапсырма үш күн ішіндегі (2018 жылғы 3 желтоқсан - 2018 жылғы 5 желтоқсан) 18 сағатқа автоматты түрде жоспарланған.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="2e4cb-157">Тапсырма қолмен жоспарланса, сағаттар барлық күндер үшін біркелкі етіп үлестіріледі.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="2e4cb-158">**Мысал**</span><span class="sxs-lookup"><span data-stu-id="2e4cb-158">**Example**</span></span>

<span data-ttu-id="2e4cb-159">Келесі тапсырма үш күн ішіндегі (2018 жылғы 3 желтоқсан - 2018 жылғы 5 желтоқсан) 18 сағатқа қолмен жоспарланған.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="2e4cb-160">Тағайындау бірлігі</span><span class="sxs-lookup"><span data-stu-id="2e4cb-160">Assignment unit</span></span>

<span data-ttu-id="2e4cb-161">Тағайындау бірлігі PSA 3.x. нұсқасында ескірген.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="2e4cb-162">Тапсырманың талпыныс сағаттары барлық тағайындалған ресурстар үшін әр күнге біркелкі етіп бөлінеді.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="2e4cb-163">**Мысал**</span><span class="sxs-lookup"><span data-stu-id="2e4cb-163">**Example**</span></span>

<span data-ttu-id="2e4cb-164">Бұл мысалда тапсырма екі ресурсқа тағайындалған және үш күн ішіндегі (2018 жылғы 3 желтоқсан - 2018 жылғы 5 желтоқсан) 36 сағатқа автоматты түрде жоспарланған.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="2e4cb-165">Тағайындау 1:</span><span class="sxs-lookup"><span data-stu-id="2e4cb-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="2e4cb-166">Тағайындау 2:</span><span class="sxs-lookup"><span data-stu-id="2e4cb-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="2e4cb-167">Бағалар өлшемдері</span><span class="sxs-lookup"><span data-stu-id="2e4cb-167">Pricing dimensions</span></span>

<span data-ttu-id="2e4cb-168">PSA 3.x нұсқасында ресурсқа тән баға белгілеудің өлшемі өрістері (**Рөл** және **Ұйымдық бөлімше** сияқты) **msdyn\_projecttask** нысанынан өшірілді.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit**) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="2e4cb-169">Жобаның болжамды мәндері құрылған кезде, бұл өрістерді енді ресурс тағайындауының (**msdyn\_resourceassignment**) сәйкес топ мүшесінен (**msdyn\_projectteam**) шығарып алуға болады.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-169">These fields can now be retrieved from the corresponding project team member (**msdyn\_projectteam**) of the resource assignment (**msdyn\_resourceassignment**) when project estimates are generated.</span></span> <span data-ttu-id="2e4cb-170">Жаңа **msdyn\_organizationalunit** өрісі **msdyn\_projectteam** нысанына қосылды.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-170">A new field, **msdyn\_organizationalunit**, has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="2e4cb-171">msdyn\_projecttask (Жоба тапсырмасы) нысанындағы ескірген өріс</span><span class="sxs-lookup"><span data-stu-id="2e4cb-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="2e4cb-172">Оның орнына қолданылатын msdyn\_projectteam (Жобаның топ мүшесі) нысанынан алынған өріс</span><span class="sxs-lookup"><span data-stu-id="2e4cb-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="2e4cb-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="2e4cb-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="2e4cb-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="2e4cb-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="2e4cb-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="2e4cb-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="2e4cb-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="2e4cb-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="2e4cb-177">Контурлар</span><span class="sxs-lookup"><span data-stu-id="2e4cb-177">Contours</span></span>

<span data-ttu-id="2e4cb-178">Баға белгілеу және болжам контуры өрістері **msdyn\_projecttask** нысанында ескірген.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="2e4cb-179">Олар **msdyn\_resourceassignment** нысанына көшірілді.</span><span class="sxs-lookup"><span data-stu-id="2e4cb-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="2e4cb-180">msdyn\_projecttask (Жоба тапсырмасы) нысанындағы ескірген өріс</span><span class="sxs-lookup"><span data-stu-id="2e4cb-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="2e4cb-181">msdyn\_resourceassignment (Ресурс тағайындауы) нысанындағы жаңа өріс</span><span class="sxs-lookup"><span data-stu-id="2e4cb-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="2e4cb-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="2e4cb-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="2e4cb-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="2e4cb-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="2e4cb-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="2e4cb-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="2e4cb-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="2e4cb-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="2e4cb-186">Келесі өрістер **msdyn\_resourceassignment** нысанына қосылды:</span><span class="sxs-lookup"><span data-stu-id="2e4cb-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="2e4cb-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="2e4cb-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="2e4cb-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="2e4cb-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="2e4cb-189">Жоспарланған, нақты және қалған құн мен сатылымға арналған келесі өрістер **msdyn\_projecttask** нысанында өзгертілмеді:</span><span class="sxs-lookup"><span data-stu-id="2e4cb-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="2e4cb-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="2e4cb-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="2e4cb-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="2e4cb-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="2e4cb-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="2e4cb-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="2e4cb-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="2e4cb-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="2e4cb-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="2e4cb-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="2e4cb-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="2e4cb-195">msdyn\_remainingsales</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]