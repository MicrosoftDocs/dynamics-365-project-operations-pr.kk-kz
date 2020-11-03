---
title: Жобаның барысы және құн шығыны
description: Бұл тақырыпта жоба барысы және құн шығынын бақылау туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 08/21/2020
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
ms.openlocfilehash: 3b60f72b371a76a59216b0b528d8e63513b06e0d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079821"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="b12f2-103">Жобаның барысы және құн шығыны</span><span class="sxs-lookup"><span data-stu-id="b12f2-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b12f2-104">Орындалу барысын кестеге сәйкес бақылау қажеттілігі салаға байланысты өзгереді.</span><span class="sxs-lookup"><span data-stu-id="b12f2-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="b12f2-105">Кейбір салалар нақты деңгейде, ал басқа салалар одан жоғары деңгейде бақыланады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="b12f2-106">Бұл тақырыпта ұйымыңыздың талаптарын қанағаттандыру үшін жоспарлау жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="b12f2-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="b12f2-107">Талпынысты бақылау көрінісі</span><span class="sxs-lookup"><span data-stu-id="b12f2-107">Effort tracking view</span></span>

<span data-ttu-id="b12f2-108">**Талпынысты бақылау** көрінісі кестедегі тапсырмалардың орындалу барысын қадағалайды.</span><span class="sxs-lookup"><span data-stu-id="b12f2-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="b12f2-109">Ол тапсырманың жоспарланған талпыныс сағаттарын тапсырмаға жұмсалған нақты талпыныс сағаттарымен салыстырады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-109">It compares the actual effort hours spent on a task to the task's planned effort hours.</span></span> <span data-ttu-id="b12f2-110">Project Service Automation бақылау өлшемдерін есептеу үшін келесі формулаларды қолданады:</span><span class="sxs-lookup"><span data-stu-id="b12f2-110">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="b12f2-111">Бастапқыда тапсырманы құру кезінде: Жоспарлы шығын толықтай есептелген құнға қойылады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-111">Initially on the task creation: Planned cost will be set to the Estimated cost at complete.</span></span> <span data-ttu-id="b12f2-112">Тапсырмаға нақты көрсеткіштерді жазғаннан кейін, келесі талпынысты бақылау көрінісі бойынша есептеледі</span><span class="sxs-lookup"><span data-stu-id="b12f2-112">Once Actuals are recorded on the task, the following will be calculation on the Tracking view for Effort</span></span>

- <span data-ttu-id="b12f2-113">Орындалу пайызы = бүгінгі күнге жұмсалған нақты талпыныс ÷ Аяқтау кезіндегі құн болжамы (EAC)</span><span class="sxs-lookup"><span data-stu-id="b12f2-113">Progress percentage = Actual effort spent to date ÷ Estimate at complete (EAC)</span></span> 
- <span data-ttu-id="b12f2-114">Аяқтауды бағалау (ETC) = Аяқтау кезіндегі құн болжамы (EAC) – бүгінгі күнге жұмсалған нақты талпыныс</span><span class="sxs-lookup"><span data-stu-id="b12f2-114">Estimate to complete (ETC) = Estimate at complete (EAC)  – Actual effort spent to date</span></span> 
- <span data-ttu-id="b12f2-115">Аяқтау кезіндегі бағалау (EAC) = қалған талпыныс + бүгінгі күнге жұмсалған нақты талпыныс</span><span class="sxs-lookup"><span data-stu-id="b12f2-115">EAC = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="b12f2-116">Жоспарланған талпыныстың ауытқуы = жоспарланған талпыныс – EAC</span><span class="sxs-lookup"><span data-stu-id="b12f2-116">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="b12f2-117">Project Service Automation бағдарламасында тапсырма бойынша талпыныс ауытқуының проекциясы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="b12f2-117">Project Service Automation shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="b12f2-118">Егер EAC жоспарланған талпыныстан көп болса, онда тапсырма бастапқыда жоспарланғаннан көп уақытты алады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-118">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="b12f2-119">Сондықтан, бұл кесте бойынша кешігетін болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-119">Therefore, it's behind schedule.</span></span> <span data-ttu-id="b12f2-120">Егер EAC жоспарланған талпыныстан кем болса, онда тапсырма бастапқыда жоспарланғаннан аз уақытты алады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-120">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="b12f2-121">Сондықтан, бұл кесте бойынша ілгері болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-121">Therefore, it's ahead of schedule.</span></span>

## <a name="reprojecting-effort"></a><span data-ttu-id="b12f2-122">Қайта жобалау әрекеті</span><span class="sxs-lookup"><span data-stu-id="b12f2-122">Reprojecting effort</span></span>

<span data-ttu-id="b12f2-123">Жоба менеджері үшін тапсырманың бастапқы болжамдарын қайта қарау әдеттегідей болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-123">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="b12f2-124">Жобаның қайта болжаулары – бұл жобаның қазіргі күйін ескере отырып, жоба менеджерінің бағалауды қабылдауы.</span><span class="sxs-lookup"><span data-stu-id="b12f2-124">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="b12f2-125">Алайда, біз жоба менеджерлеріне бастапқы сандарды өзгертуге кеңес бермейміз, себебі жобаның бастапқы мәні жоба кестесі мен құн болжамы үшін шындықтың бекітілген көзі болып табылады және барлық мүдделі тараптар бұған келіскен.</span><span class="sxs-lookup"><span data-stu-id="b12f2-125">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="b12f2-126">Жоба менеджері үшін тапсырмалар бойынша талпынысты қайта жобалаудың екі жолы бар:</span><span class="sxs-lookup"><span data-stu-id="b12f2-126">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="b12f2-127">Тапсырмада нақты қалған талпыныстың жаңа болжамын әдепкі ETC элементімен ауыстыру.</span><span class="sxs-lookup"><span data-stu-id="b12f2-127">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="b12f2-128">Тапсырма бойынша нақты орындалу барысының жаңа болжамын әдепкі орындалу барысының пайызымен ауыстыру.</span><span class="sxs-lookup"><span data-stu-id="b12f2-128">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="b12f2-129">Осы тәсілдердің әрқайсысы тапсырманың ETC, аяқтау кезіндегі құн болжамы (EAC) және орындалу пайызын қайта есептеуді және тапсырма бойынша талпыныстың ауытқуын тудырады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-129">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="b12f2-130">Аяқтау кезіндегі құн болжамы (EAC), ETC және жиынтық тапсырмалар бойынша орындалу пайызы да қайта есептелінеді және талпыныс ауытқуының жаңа болжамын жасайды.</span><span class="sxs-lookup"><span data-stu-id="b12f2-130">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="reprojection-of-effort-on-summary-tasks"></a><span data-ttu-id="b12f2-131">Жиынтық тапсырмалар бойынша талпынысты қайта жобалау</span><span class="sxs-lookup"><span data-stu-id="b12f2-131">Reprojection of effort on summary tasks</span></span>

<span data-ttu-id="b12f2-132">Жиынтық тапсырмалар немесе контейнер тапсырмалары бойынша талпынысты қайта жобалауға болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-132">Effort on summary tasks or container tasks can be reprojected.</span></span> <span data-ttu-id="b12f2-133">Пайдаланушы қалған талпынысты немесе жиынтық тапсырмалар бойынша орындалу пайызын қолдана отырып жобаны қайтадан жобалауына қарамастан, келесі есептеулер жиынтығы басталады:</span><span class="sxs-lookup"><span data-stu-id="b12f2-133">Regardless of whether the user reprojects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="b12f2-134">Аяқтау кезіндегі құн болжамы (EAC), ETC және тапсырманың орындалу пайызы есептеледі.</span><span class="sxs-lookup"><span data-stu-id="b12f2-134">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="b12f2-135">Жаңа аяқтау кезіндегі құн болжамы (EAC) қосалқы тапсырмаларға тапсырмада болған бастапқы аяқтау кезіндегі құн болжамымен (EAC) бірдей пропорцияда үлестірілді.</span><span class="sxs-lookup"><span data-stu-id="b12f2-135">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="b12f2-136">Жаңа аяқтау кезіндегі құн болжамы (EAC) әрбір жеке тапсырмалардан бастап, соңғы түйін тапсырмаларына дейін есептеледі.</span><span class="sxs-lookup"><span data-stu-id="b12f2-136">The new EAC on each of the individual tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="b12f2-137">Әсер ететін қосалқы тапсырмалар соңғы түйіндерге дейін EAC мәні негізінде қайта есептелген ETC және орындалу пайызын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="b12f2-137">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="b12f2-138">Нәтижесінде тапсырма бойынша талпыныс ауытқуы үшін жаңа проекция пайда болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-138">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="b12f2-139">Жиынтық тапсырмалардың EAC мәндері түбірлік түйінге дейін қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="b12f2-139">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="b12f2-140">Құн бақылауы көрінісі</span><span class="sxs-lookup"><span data-stu-id="b12f2-140">Cost tracking view</span></span> 

<span data-ttu-id="b12f2-141">**Құн бақылауы** көрінісі тапсырмаға жұмсалған нақты құнын жоспарланған құнмен салыстырады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-141">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost.</span></span> 

> [!NOTE]
> <span data-ttu-id="b12f2-142">Бұл көрініс тек еңбек шығындарын көрсетеді және шығын болжамдарының шығындарды қамтымайды.</span><span class="sxs-lookup"><span data-stu-id="b12f2-142">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="b12f2-143">Project Service Automation бақылау өлшемдерін есептеу үшін келесі формулаларды қолданады:</span><span class="sxs-lookup"><span data-stu-id="b12f2-143">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="b12f2-144">Тапсырма жасалған кезде, жоспарланған шығын аяқтау кезіндегі есептелген өзіндік құнға тең болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-144">When a task is created, the planned cost is equal to the estimated cost at complete.</span></span> <span data-ttu-id="b12f2-145">Тапсырмаға нақты көрсеткіштерді жазғаннан кейін, келесі шығынның **Бақылау** көрінісі бойынша есептеледі:</span><span class="sxs-lookup"><span data-stu-id="b12f2-145">After actuals are recorded on the task, the following is calculated on the **Tracking** view for cost:</span></span>

 - <span data-ttu-id="b12f2-146">Тұтынылған шығындар пайызы = осы күнге жұмсалған нақты шығындар ÷ тапсырманың аяқтау кезіндегі есептелген құны</span><span class="sxs-lookup"><span data-stu-id="b12f2-146">Percentage of cost consumed = Actual cost spent to date ÷ Estimated cost at complete for the task</span></span>
 - <span data-ttu-id="b12f2-147">Аяқтауды бағалау (CTC) = аяқтау кезіндегі есептелген құн – осы күнге жұмсалған нақты шығындар</span><span class="sxs-lookup"><span data-stu-id="b12f2-147">Cost to complete (CTC) = Estimated cost at complete – Actual cost spent to date</span></span>
 - <span data-ttu-id="b12f2-148">Аяқтау кезіндегі есептелген құн = СТС + осы күнге жұмсалған нақты шығындар</span><span class="sxs-lookup"><span data-stu-id="b12f2-148">Estimated cost at complete = CTC + Actual cost spent to date</span></span>
 - <span data-ttu-id="b12f2-149">Жоспарланған құнның ауытқуы = жоспарланған құн – аяқтау кезіндегі есептелген құн</span><span class="sxs-lookup"><span data-stu-id="b12f2-149">Projected cost variance = Planned cost – Estimated cost at complete</span></span>

<span data-ttu-id="b12f2-150">Құн ауытқуының проекциясы тапсырмада көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="b12f2-150">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="b12f2-151">Егер аяқтау кезіндегі есептелген құн жоспарланған құннан көп болса, онда тапсырма құны бастапқыда жоспарланғаннан көп болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-151">If the estimated cost at complete is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="b12f2-152">Сондықтан, бұл бюджеттен тыс болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-152">Therefore, it's trending over budget.</span></span> <span data-ttu-id="b12f2-153">Егер аяқтау кезіндегі есептелген құн жоспарланған құннан аз болса, онда тапсырма құны бастапқыда жоспарланғаннан аз болады және бюджет шеңберінде болады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-153">If the Estimated cost at complete is less than the planned cost, the task is projected to cost less than was originally planned and is trending under budget.</span></span>

## <a name="project-managers-reprojection-of-cost"></a><span data-ttu-id="b12f2-154">Жоба менеджерінің құнды қайта жобалауы</span><span class="sxs-lookup"><span data-stu-id="b12f2-154">Project manager’s reprojection of cost</span></span>

<span data-ttu-id="b12f2-155">Талпыныс қайта жобаланған кезде, CTC, аяқтау кезіндегі есептелген құн, тұтынылған шығынның пайызы және шығындардың болжамды ауытқуы **Құн бақылауы** көрінісінде қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="b12f2-155">When effort is reprojected, the CTC, Estimated cost at complete, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="b12f2-156">Жоба күйінің қорытындысы</span><span class="sxs-lookup"><span data-stu-id="b12f2-156">Project status summary</span></span>

<span data-ttu-id="b12f2-157">**Талпынысты бақылау** және **Құн бақылауы** көріністеріндегі бақылау деректері жобаның түпкі түйініндегі, жиынтық тапсырмалардағы және соңғы түйін тапсырмалар деңгейіндегі орындалу барысы мен құн шығынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="b12f2-157">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="b12f2-158">**Жоба нысаны** бетіндегі **Күй** бөлімінде жоба деңгейіндегі күйдің қорытындысы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="b12f2-158">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="b12f2-159">Күй қорытындысының өрістері</span><span class="sxs-lookup"><span data-stu-id="b12f2-159">Status summary fields</span></span>

<span data-ttu-id="b12f2-160">**Жобаның жалпы күйі** өрісі — бұл жобаның жалпы күйін көрсететін өңделетін өріс.</span><span class="sxs-lookup"><span data-stu-id="b12f2-160">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="b12f2-161">Ол артып келе жатқан қауіпті көрсету үшін жасыл, сары және қызыл сияқты түрлі түсті кодтауды қолданады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-161">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="b12f2-162">**Пікірлер** өрісі жоба менеджеріне күй туралы нақты түсініктемелер енгізуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="b12f2-162">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="b12f2-163">**Күйі жаңартылған күн** өрісі өңделмейді және мән күйдің соңғы рет жаңартылған уақытын көрсететін уақыт белгісі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-163">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="b12f2-164">**Кесте өнімділігі** және **Құн өнімділігі** өрістері бақылау күнінен бастап орнатылады.</span><span class="sxs-lookup"><span data-stu-id="b12f2-164">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="b12f2-165">**Талпынысты бақылау** көрінісіндегі түбірлік түйіннің кесте мен құн ауытқуы оң болғанда, осы өрістерді **Ahead** мәніне орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="b12f2-165">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="b12f2-166">Түбірлік түйіннің кесте мен құн ауытқуы теріс болса, оларды **Артында** мәніне орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="b12f2-166">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
