---
title: Веб-бағдарламадағы тапсырмаға тапсырыс беруге болатын ресурсты белгілеу жолы
description: Тапсырыс беруге болатын ресурстарды белгілеу жолы туралы жалпы мәліметтер.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 27a93c41243f300cadb632c697672180e5a3817b
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146580"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="71b8c-103">Веб-қолданбаға тапсырыс берілетін ресурсты қалай белгілей аламын (Project Service қолданбасы v2.x)?</span><span class="sxs-lookup"><span data-stu-id="71b8c-103">How do I assign a bookable resource to a task in the web app (Project Service app v2.x)?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="71b8c-104">Project Service ішіндегі тапсырмаға ресурсты белгілеудің екі жолы бар.</span><span class="sxs-lookup"><span data-stu-id="71b8c-104">There are two ways to assign a resource to a task in Project Service.</span></span> <span data-ttu-id="71b8c-105">Топ мүшесі ретінде ресурсқа тапсырыс беріп, оны тапсырмаға белгілей аласыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-105">You can book a resource as a team member and then assign it to a task.</span></span> <span data-ttu-id="71b8c-106">Болмаса, тапсырмалардағы рөл тағайындауы арқылы жалпы топ мүшесін жасауға, топты құруға және атаулы ресурспен бэкинг талаптарын орындауға болады.</span><span class="sxs-lookup"><span data-stu-id="71b8c-106">Or, you can create a generic team member through role assignment on tasks, generate a team, and then fulfill the backing requirements with a named resource.</span></span>

<span data-ttu-id="71b8c-107">Тапсырмаға тапсырыс берілетін ресурсты белгілеу керек болса, тапсырыс берілетін ресурс тобы мүшесінің тапсырыстары жеткілікті болуы керек екендігін ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-107">Note that if you’d like to assign a bookable resource to a task, the bookable resource team member must have enough available bookings.</span></span> <span data-ttu-id="71b8c-108">Тапсырыс күйі "Бекіту түріндегі қатты кітап" және "Күйі бекітілген" болуы керек.</span><span class="sxs-lookup"><span data-stu-id="71b8c-108">The status of the booking must be Commit Type Hard Book and Status Committed.</span></span> <span data-ttu-id="71b8c-109">Ресурс тапсырыстары жеткілікті болмаса, Project Service жүйесі тағайындауды жойып, келесі қате туралы хабарды көрсетеді:</span><span class="sxs-lookup"><span data-stu-id="71b8c-109">If there aren’t enough bookings for the resource, Project Service removes the assignment and displays the following error message:</span></span>

<span data-ttu-id="71b8c-110">*Ресурсты тапсырмаға белгілеу мүмкін емес - Келесі ресурс(тар)да жоба бойынша тапсырыс беруге жеткілікті уақыт жоқ*</span><span class="sxs-lookup"><span data-stu-id="71b8c-110">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project*</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="71b8c-111">Ресурсты топ мүшесі ретінде тіркеп, оны тапсырмаға белгілеу</span><span class="sxs-lookup"><span data-stu-id="71b8c-111">Book a resource as a team member and then assign the resource to a task</span></span>

<span data-ttu-id="71b8c-112">Осы әдіс арқылы жоба тобына ресурсты қосып, тапсырмаларды жоба кестесіндегі ресурсқа белгілей аласыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-112">With this method you add a resource to the project team and then assign tasks to the resource in the project schedule.</span></span> <span data-ttu-id="71b8c-113">Мұнда осыны орындау жолы көрсетілген:</span><span class="sxs-lookup"><span data-stu-id="71b8c-113">Here’s how you do this:</span></span>
1.  <span data-ttu-id="71b8c-114">Топ мүшесі торында **Жаңа** параметрін таңдау арқылы жаңа топ мүшесін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-114">On the team member grid, add a new team member by selecting **New**.</span></span>
2.  <span data-ttu-id="71b8c-115">Топ мүшесін жылдам жасау экранынан тапсырыс берілетін ресурс атын таңдап, рөлін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-115">On the Team Member Quick Create screen, select the bookable resource name and set a role.</span></span>
3.  <span data-ttu-id="71b8c-116">**Басталу** және **Аяқталу** күндерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-116">Select the **From** and **To** dates.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="71b8c-117">![Топ мүшесін қосу қадамының скриншоты](media/FAQ-Resources-to-Tasks2-1.png "Топ мүшесін қосу қадамының скриншоты")</span><span class="sxs-lookup"><span data-stu-id="71b8c-117">![Screenshot of adding team member](media/FAQ-Resources-to-Tasks2-1.png "Screenshot of adding team member")</span></span>
 
4.  <span data-ttu-id="71b8c-118">Ресурсқа тапсырыс беру үшін келесі тағайындау әдістерінің бірін таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="71b8c-118">Select one of the following allocation methods for booking the resource:</span></span>
    - <span data-ttu-id="71b8c-119">**Толық мүмкіндік** көрсетілген басталу және аяқталу күндері ресурстың толық мүмкіндігін тіркейді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-119">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="71b8c-120">**Пайыздық мүмкіндік** көрсетілген басталу және аяқталу күндері үшін ресурс мүмкіндігінің пайызын тіркейді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-120">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="71b8c-121">**Сағат бойынша бірқалыпты тарату** пәрмені көрсетілген басталу және аяқталу күндері бойынша күн сайын бірқалыпты таратумен ресурсқа көрсетілген сағат санын тіркейді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-121">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing it evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="71b8c-122">**Сағат бойынша алдыңғы жүктеме** пәрмені көрсетілген басталу және аяқталу күндері бойынша күн сайын алдыңғы жүктемеге көрсетілген ресурстың сағат санын тіркейді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-122">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>

    <span data-ttu-id="71b8c-123">**Ешқандай** параметрін таңдауға болмайды, себебі ол ресурсты топқа қосады, бірақ ресурс мүмкіндігін сіңіретін тапсырыстарды жасамайды.</span><span class="sxs-lookup"><span data-stu-id="71b8c-123">Don’t select **None** because it adds the resource to the team but doesn’t create any bookings that absorb the resource's capacity.</span></span>
5.  <span data-ttu-id="71b8c-124">**Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-124">Select **Save**.</span></span>

    <span data-ttu-id="71b8c-125">Тапсырыс уақыты осы ресурс тағайындалған тапсырмалардың қолданыс уақыты мен күні ауқымын қамтуға жеткілікті болуы керектігін ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-125">Note that the hours of the booking must be enough to cover the effort hours and date ranges of the tasks that you assign this resource to.</span></span> <span data-ttu-id="71b8c-126">Олар тураланбаса, тапсырмаға ресурс белгілей алмайсыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-126">If they aren’t in alignment, you can’t assign the resource to the task.</span></span>

6.  <span data-ttu-id="71b8c-127">Тапсырманың жұмыс декомпозициясының құрылымында (WBS) ресурс ұяшығы ашылмалы терезесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-127">On the work breakdown structure (WBS) for the task, click the resource cell dropdown.</span></span> <span data-ttu-id="71b8c-128">Онда:</span><span class="sxs-lookup"><span data-stu-id="71b8c-128">Then:</span></span> 

    1. <span data-ttu-id="71b8c-129">**Қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-129">Select **Add**.</span></span>
    2. <span data-ttu-id="71b8c-130">**Ресурстар** астынан ашылмалы терезені таңдап, жоғарыда қосылған топ мүшесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-130">Select the dropdown under **Resources** and select the team member you added above.</span></span>
    3. <span data-ttu-id="71b8c-131">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-131">Select **OK**.</span></span> <span data-ttu-id="71b8c-132">Топ мүшесі енді тапсырмаға белгіленді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-132">The team member is now assigned to the task.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="71b8c-133">![WBS көмегімен ресурстарды қосу қадамының скриншоты](media/FAQ-Resources-to-Tasks2-2.png "WBS көмегімен ресурстарды қосу қадамының скриншоты")</span><span class="sxs-lookup"><span data-stu-id="71b8c-133">![Screenshot of adding resources with WBS](media/FAQ-Resources-to-Tasks2-2.png "Screenshot of adding resources with WBS")</span></span>
 
<span data-ttu-id="71b8c-134">Топ мүшесі торынан Белгіленген уақыт астынан ресурсқа белгіленген уақыт қосындысын көре аласыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-134">On the team member grid, you’ll see the aggregate of the resource’s assigned hours under Assigned Hours.</span></span> <span data-ttu-id="71b8c-135">Ол ресурсқа тіркелген уақыттан кіші немесе тең.</span><span class="sxs-lookup"><span data-stu-id="71b8c-135">It will be less than or equal to the booked hours for the resource.</span></span> 

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="71b8c-136">![Ресурсқа тағайындалған сағаттардың скриншоты](media/FAQ-Resources-to-Tasks2-3.png "Ресурсқа тағайындалған сағаттардың скриншоты")</span><span class="sxs-lookup"><span data-stu-id="71b8c-136">![Screenshot of assigned hours for a resource](media/FAQ-Resources-to-Tasks2-3.png "Screenshot of assigned hours for a resource")</span></span>
 
<span data-ttu-id="71b8c-137">Ресурсқа белгілейін деп жатқан тапсырыс ресурстар тапсырыстарының аяқталу күнінен басталса, ашылмалы терезеде ресурс пайда болмайды.</span><span class="sxs-lookup"><span data-stu-id="71b8c-137">If the task you’re attempting to assign to the resource starts after the end date of the resources bookings, the resource won’t appear in the dropdown.</span></span>

<span data-ttu-id="71b8c-138">Ресурста белгіленбеген мүмкіндік қалған болса, ресурсты тіркелген уақыттан көп уақытқа белгілей алатыныңызды ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-138">Note that you can assign a resource to more hours than their booked hours if the resource has some remaining unassigned capacity.</span></span> <span data-ttu-id="71b8c-139">Бұндай жағдайда ресурс тапсырыстарыңызға ішінара ғана белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-139">In this case the resource will only be partially assigned up to their bookings.</span></span> <span data-ttu-id="71b8c-140">Жұмыс декомпозициясының құрылымына Автоматты уақыт бағанын қосу арқылы осы қалған белгіленбеген тапсырма уақытын көре аласыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-140">You can see these remaining unassigned task hours by adding the Unstaffed Hours column to the work breakdown structure.</span></span>

<span data-ttu-id="71b8c-141">Ресурстар тіркелген уақытқа (тіркелген уақыт белгіленген уақытқа тең) белгіленсе, қосымша тапсырмалар тағайындауға әрекет жасаған кезде келесі қате туралы хабарды көресіз:</span><span class="sxs-lookup"><span data-stu-id="71b8c-141">If resources are assigned to their booked hours (their booked hours equals their assigned hours), you’ll see the following error message when you attempt to assign them further tasks:</span></span>

<span data-ttu-id="71b8c-142">*Ресурсты тапсырмаға белгілеу мүмкін емес - Келесі ресурс(тар)да жоба бойынша тапсырыс беруге жеткілікті уақыт жоқ.*</span><span class="sxs-lookup"><span data-stu-id="71b8c-142">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project.*</span></span>

<span data-ttu-id="71b8c-143">Оған қоса, жобаны жасау кезінде топқа қосылған әдепкі жоба менеджерінің топ мүшесі ешбір тапсырыстарсыз қосылады және ешбір тапсырмаға белгіленбейді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-143">Additionally, the default project manager team member that is added to the team when you create the project is added without any bookings and can’t be assigned to any task.</span></span> <span data-ttu-id="71b8c-144">Олар тапсырмалардың ресурс ашылмалы терезесінде көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-144">They won’t show up in the resource dropdown for tasks.</span></span>

<span data-ttu-id="71b8c-145">Осы ресурсты белгілеу керек болса, оларды топтан жойып, оларды Ешқандай күйінен басқа тағайындау әдісімен қайта қосу керек.</span><span class="sxs-lookup"><span data-stu-id="71b8c-145">If you want to assign this resource, you need to remove them from the team and then re-add them with an allocation method other than None.</span></span> <span data-ttu-id="71b8c-146">Жоба жасалған кезде топқа қосу себебі - әдепкі бойынша жобада кемінде бір жобаны растаушының болуы.</span><span class="sxs-lookup"><span data-stu-id="71b8c-146">The reason they’re added to the team when the project is created is so that a project has at least one project approver by default.</span></span>

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a><span data-ttu-id="71b8c-147">Тапсырмаларға рөл тағайындау арқылы жалпы топ мүшесін жасау</span><span class="sxs-lookup"><span data-stu-id="71b8c-147">Create a generic team member through role assignment on tasks</span></span>

<span data-ttu-id="71b8c-148">Бұл әдіс ресурстарда тапсырмаларға жеткілікті тапсырыстар бар болуын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-148">This method assures that resources have enough bookings for tasks.</span></span> <span data-ttu-id="71b8c-149">Алдымен, тапсырмаларға рөлдер тағайындағаннан кейін топ құру арқылы тапсырмаларды жұмыс істеуді қалайтын атаулы ресурс сипаттамаларын сипаттайтын орын толтырғыш немесе жалпы ресурс жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-149">First, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks by generating a team after assigning roles to tasks.</span></span> <span data-ttu-id="71b8c-150">Мұнда осыны орындау жолы көрсетілген:</span><span class="sxs-lookup"><span data-stu-id="71b8c-150">Here’s how you do this:</span></span>

1. <span data-ttu-id="71b8c-151">Жұмыс декомпозициясының құрылымынан тапсырманы таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-151">On the work breakdown structure, select a task.</span></span>
2. <span data-ttu-id="71b8c-152">Ресурс ұяшығынан **Белгіленген рөл** ашылмалы белгішесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-152">Select the **Assigned Role** dropdown icon in the resource cell.</span></span>
3. <span data-ttu-id="71b8c-153">**Рөл** ашылмалы терезесін таңдап, жалпы ресурс рөлін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-153">Select the **Role** dropdown and select the role for the generic resource.</span></span>
4. <span data-ttu-id="71b8c-154">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-154">Select **OK**.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="71b8c-155">![Ресурсты қосу үшін WBS құрылымын пайдалану қадамының скриншоты](media/FAQ-Resources-to-Tasks2-4.png "Ресурсты қосу үшін WBS құрылымын пайдалану қадамының скриншоты")</span><span class="sxs-lookup"><span data-stu-id="71b8c-155">![Screenshot of using WBS to add resource](media/FAQ-Resources-to-Tasks2-4.png "Screenshot of using WBS to add resource")</span></span>
 
<span data-ttu-id="71b8c-156">WBS жүйесінде тапсырмаларға рөлдер тағайындау аяқталса, **Жоба тобын құру** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-156">Once you’ve completed assigning roles to the tasks in the WBS, select **Generate Project Team**.</span></span> <span data-ttu-id="71b8c-157">Жоба қызметі тапсырма тағайындауларын біріктіру арқылы рөлдер, ресурс ұйымы бірліктері және жоба күнтізбесі негізінде жалпы топ мүшелерінің минималды санын жасайды.</span><span class="sxs-lookup"><span data-stu-id="71b8c-157">Project Service creates the minimum number of generic team members based on the roles, resourcing organization units, and project calendar by aggregating the task assignments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="71b8c-158">![Жоба тобын жасау қадамының скриншоты](media/FAQ-Resources-to-Tasks2-5.png "Жоба тобын жасау қадамының скриншоты")</span><span class="sxs-lookup"><span data-stu-id="71b8c-158">![Screenshot of generating project team](media/FAQ-Resources-to-Tasks2-5.png "Screenshot of generating project team")</span></span>
 
<span data-ttu-id="71b8c-159">Топ мүшесі торында рөлі мен орын атауы бар Жалпы ресурс түрінің ресурстарын көресіз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-159">On the Team Member grid, you’ll see resources of the Generic Resource type with the role and position name.</span></span> <span data-ttu-id="71b8c-160">Жұмысты аяқтау үшін рөлге екі ресурс қажет болса, Жалпы топ мүмкіндігі екі топ мүшесін жасайды және оларды орнату үшін орын атауын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="71b8c-160">If two resources are needed for a role to complete the work, the Generate Team feature creates two team members and uses position name to set them apart.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="71b8c-161">![Екі жалпы ресурсты қосу қадамының скриншоты](media/FAQ-Resources-to-Tasks2-6.png "Екі жалпы ресурсты қосу қадамының скриншоты")</span><span class="sxs-lookup"><span data-stu-id="71b8c-161">![Screenshot of adding two generic resources](media/FAQ-Resources-to-Tasks2-6.png "Screenshot of adding two generic resources")</span></span>
 
<span data-ttu-id="71b8c-162">Ресурс талабы астынан сілтемені таңдау арқылы жалпы топ мүшесінің бэкинг ресурсы талабын аша аласыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-162">You can open the backing resource requirement for the generic team member by selecting the link under Resource Requirement.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="71b8c-163">![Бэкинг ресурсы талабын ашу қадамының скриншоты](media/FAQ-Resources-to-Tasks2-7.png "Бэкинг ресурсы талабын ашу қадамының скриншоты")</span><span class="sxs-lookup"><span data-stu-id="71b8c-163">![Screenshot of opening backing resource requirement](media/FAQ-Resources-to-Tasks2-7.png "Screenshot of opening backing resource requirement")</span></span>

<span data-ttu-id="71b8c-164">Жалпы ресурс үшін **Тапсырыс беру** параметрін таңдап, нақты ресурсты тауып тапсырыс беру үшін кесте тақтасын пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-164">Select **Book** for the generic resource, and then you can use the schedule board to find and book a real resource.</span></span> <span data-ttu-id="71b8c-165">Сонымен қатар **Сұрау жіберу** параметрін таңдау арқылы ресурс менеджерінің орындау талабын жібере аласыз.</span><span class="sxs-lookup"><span data-stu-id="71b8c-165">You can also submit the requirement for fulfillment by a resource manager by selecting **Submit Request**.</span></span>

<span data-ttu-id="71b8c-166">Жалпы ресурс атаулы ресурспен орындалса, жалпы ресурс топтан жойылады және жалпы ресурстың тапсырма тағайындаулары жалпы ресурс талабына сәйкес атаулы ресурсқа белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="71b8c-166">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>
 

