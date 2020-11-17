---
title: Ресурсты тапсырмаға белгілеу
description: Бұл тақырыпта ресурстарды тапсырмаларға белгілеу жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
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
ms.openlocfilehash: b7aef799ec4b90d602a6f3641cbac06264664f00
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125140"
---
# <a name="assign-a-resource-to-a-task"></a><span data-ttu-id="f325a-103">Ресурсты тапсырмаға белгілеу</span><span class="sxs-lookup"><span data-stu-id="f325a-103">Assign a resource to a task</span></span>

<span data-ttu-id="f325a-104">Microsoft Dynamics 365 Project Service Automation бағдарламасындағы тапсырмаға ресурсты белгілеудің үш жолы бар.</span><span class="sxs-lookup"><span data-stu-id="f325a-104">There are three ways to assign a resource to a task in Microsoft Dynamics 365 Project Service Automation.</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="f325a-105">Ресурсты топ мүшесі ретінде тіркеп, оны тапсырмаға белгілеу</span><span class="sxs-lookup"><span data-stu-id="f325a-105">Book a resource as a team member, and then assign the resource to a task</span></span>

<span data-ttu-id="f325a-106">Ресурсты жоба тобына қосып, оны жоба кестесіндегі тапсырмаға белгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="f325a-106">You can add a resource to the project team, and then assign the resource to tasks in the project schedule.</span></span>

1. <span data-ttu-id="f325a-107">**Топ мүшесі** қойыншасында **Жаңа** параметрін таңдау арқылы жаңа топ мүшесін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-107">On the **Team Member** tab, add a new team member by selecting **New**.</span></span> 

2. <span data-ttu-id="f325a-108">Осы кезде тапсырыс беруге болатын ресурс атауын таңдап, рөлін орнатуға болатын **Топ мүшесін жылдам жасау** тақтасы ашылады.</span><span class="sxs-lookup"><span data-stu-id="f325a-108">The **Team Member Quick Create** panel opens, where you can select the bookable resource name and set a role.</span></span> 

    <span data-ttu-id="f325a-109">Ресурс тапсырысы үшін келесі тағайындау әдістерінің бірін таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="f325a-109">Select one of the following allocation methods for the resource’s booking:</span></span>

    - <span data-ttu-id="f325a-110">**Толық мүмкіндік** көрсетілген басталу және аяқталу күндері ресурстың толық мүмкіндігін тіркейді.</span><span class="sxs-lookup"><span data-stu-id="f325a-110">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="f325a-111">**Пайыздық мүмкіндік** көрсетілген басталу және аяқталу күндері үшін ресурс мүмкіндігінің пайызын тіркейді.</span><span class="sxs-lookup"><span data-stu-id="f325a-111">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="f325a-112">**Сағаттарды бірқалыпты тарату бойынша** әдісі көрсетілген басталу және аяқталу күндері бойынша күн сайын уақытылы біркелкі таратумен, ресурсты көрсетілген сағат санына тіркейді.</span><span class="sxs-lookup"><span data-stu-id="f325a-112">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing them evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="f325a-113">**Сағат бойынша алдыңғы жүктеме** пәрмені көрсетілген басталу және аяқталу күндері бойынша күн сайын алдыңғы жүктемеге көрсетілген ресурстың сағат санын тіркейді.</span><span class="sxs-lookup"><span data-stu-id="f325a-113">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>
    - <span data-ttu-id="f325a-114">**Ешқандай** параметрі ресурсты топқа қосады, бірақ оның мүмкіндігін сіңіретін тапсырыстарды жасамайды.</span><span class="sxs-lookup"><span data-stu-id="f325a-114">**None** adds the resource to the team but doesn’t create any bookings that absorb their capacity.</span></span>

3. <span data-ttu-id="f325a-115">Тапсырманың **Кесте** торындағы ресурс ұяшығынан **Ресурс** белгішесін таңдап, **Топ мүшелері** аймағында жаңа қосылған топ мүшесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-115">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell, and then under **Team Members**, select the team member you just added.</span></span> 

> [!NOTE]
> <span data-ttu-id="f325a-116">**Топ мүшесі** және **Салыстырып тексеру** қойыншаларында ресурс тіркелген және белгіленген сағат санын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="f325a-116">On the **Team Member** and **Reconciliation** tabs, the resource shows booked and assigned hours.</span></span> <span data-ttu-id="f325a-117">Сағат саны бірдей болуы керек, бірақ бұл тапсырыстар мен тағайындаулар тығыз байланысты емес болғандықтан, талап етілмейді.</span><span class="sxs-lookup"><span data-stu-id="f325a-117">The hours should be the same, but it isn't required as bookings and assignments are not tightly coupled.</span></span> <span data-ttu-id="f325a-118">Олар әртүрлі болған кезде, мысалы ресурсқа тіркегеннен көбірек сағатты тағайындаған жағдайда, **Салыстырып тексеру** қойыншасында мәліметтер көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="f325a-118">The **Reconciliation** tab gives you details when they are different, such as when you assign a resource more hours than you have booked.</span></span> <span data-ttu-id="f325a-119">Қажет болса, ресурс тапсырыстарын кеңейту немесе тағайындауды өзгерту арқылы ақпаратты түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="f325a-119">If needed, you can correct the information by extending the resource's bookings or changing the assignment.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="f325a-120">Тапсырма тағайындауы арқылы жалпы топ мүшесін жасау</span><span class="sxs-lookup"><span data-stu-id="f325a-120">Create a generic team member through task assignment</span></span>

<span data-ttu-id="f325a-121">Тапсырма тағайындауы арқылы жалпы топ мүшесін жасаған кезде, тапсырмаларда жұмыс істеуін қалайтын аталған ресурс сипаттамаларын сипаттайтын толтырғышты немесе жалпы ресурсты жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-121">When you create a generic team member through task assignment, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="f325a-122">Содан кейін аталған ресурсты іздеу және тіркеу үшін пайдаланылатын талапты (немесе талаптың көмегімен сұрауды жібересіз) жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-122">You then generate a requirement (or submit a request using the requirement) that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="f325a-123">Тапсырманың **Кесте** торындағы ресурс ұяшығынан **Ресурс** белгішесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-123">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="f325a-124">Толтырғыш ресурсының атауы ретінде қызмет ететін атауды теріңіз.</span><span class="sxs-lookup"><span data-stu-id="f325a-124">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="f325a-125">Мысалы, "Бағдарлама менеджері".</span><span class="sxs-lookup"><span data-stu-id="f325a-125">For example, Program Manager.</span></span>

3. <span data-ttu-id="f325a-126">**Жасау** опциясын таңдап, **Жоба тобы мүшесін жылдам жасау** өрісінде жалпы ресурстың рөлін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-126">Select **Create**, and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>

4. <span data-ttu-id="f325a-127">Тапсырманың **Ресурс таңдау құралынан** ресурсты таңдау арқылы осы толтырғыш ресурсқа тапсырмалар белгілеуді жалғастыруға болады.</span><span class="sxs-lookup"><span data-stu-id="f325a-127">You can continue to assign tasks to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="f325a-128">Олар **Топ мүшелері** аймағында тізімделген.</span><span class="sxs-lookup"><span data-stu-id="f325a-128">They’re listed under **Team Members**.</span></span>

5. <span data-ttu-id="f325a-129">Жалпы ресурсты белгілегеннен кейін, жалпы ресурс үшін ресурс талабын жасау үшін, **Топ** қойыншасында жалпы ресурсты таңдап, **Талап жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-129">When you’re done assigning the generic resource, select the generic resource on the **Team** tab, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>

6. <span data-ttu-id="f325a-130">Жалпы ресурс үшін **Тапсырыс беру** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-130">Select **Book** for the generic resource.</span></span> <span data-ttu-id="f325a-131">Содан кейін нақты ресурсты тауып, тапсырыс беру үшін кесте тақтасын пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="f325a-131">You can then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="f325a-132">Сонымен қатар, ресурс менеджерінің орындау талабын жібере аласыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-132">You can also submit the requirement for fulfillment by a resource manager.</span></span>

7. <span data-ttu-id="f325a-133">Жалпы ресурс атаулы ресурспен орындалса, жалпы ресурс топтан жойылады және жалпы ресурстың тапсырма тағайындаулары жалпы ресурс талабына сәйкес атаулы ресурсқа белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="f325a-133">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="f325a-134">Барлық тапсырыс берілетін ресурстар тізімінен аталған ресурсты белгілеу</span><span class="sxs-lookup"><span data-stu-id="f325a-134">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="f325a-135">Барлық тапсырыс берілетін ресурстарды іздеп, оларды тапсырмаға белгілеу үшін, **Ресурс таңдау құралы** қойыншасындағы іздеу өрісін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="f325a-135">You can use the search box in the **Resource Selector** to search all bookable resources and assign them to a task.</span></span>

<span data-ttu-id="f325a-136">Осылайша тағайындалған ресурстар топқа тапсырыссыз қосылады.</span><span class="sxs-lookup"><span data-stu-id="f325a-136">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="f325a-137">Бұл топ мүшесін қосуға және тағайындау әдісі ретінде "Ешқайсы" параметрін таңдауға ұқсас.</span><span class="sxs-lookup"><span data-stu-id="f325a-137">This is similar to adding a team member and selecting None as the allocation method.</span></span> <span data-ttu-id="f325a-138">Бұл ресурс **Топ** және **Салыстырып тексеру** қойыншаларында тек тағайындаулары мен тапсырыс кемшілігі бар ресурстар ретінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="f325a-138">The resource is displayed in the **Team** and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="f325a-139">Олардың қолжетімділігін пайдалану керек болса, оларды тіркеңіз.</span><span class="sxs-lookup"><span data-stu-id="f325a-139">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="f325a-140">Тапсырманың **Кесте** торындағы ресурс ұяшығынан **Ресурс** белгішесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-140">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="f325a-141">Атын теруді бастаңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-141">Start typing a name.</span></span> <span data-ttu-id="f325a-142">**Басқа ресурстар** аймағындағы **Ресурс таңдау құралы** қойыншасында көрсетілген атау нәтижелерін іздеңіз.</span><span class="sxs-lookup"><span data-stu-id="f325a-142">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>

3. <span data-ttu-id="f325a-143">Тапсырмаға тағайындау керек ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f325a-143">Select the resource that you want to assign to the task.</span></span>

