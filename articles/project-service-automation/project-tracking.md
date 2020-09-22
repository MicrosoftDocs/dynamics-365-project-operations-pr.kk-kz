---
title: Жобаның орындалу барысы және құн шығыны
description: Бұл тақырыпта жобаның орындалу барысы және құн шығынын бақылау жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753124"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="265c9-103">Жобаның орындалу барысы және құн шығыны</span><span class="sxs-lookup"><span data-stu-id="265c9-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="265c9-104">Орындалу барысын кестеге сәйкес бақылау қажеттілігі салаға байланысты өзгереді.</span><span class="sxs-lookup"><span data-stu-id="265c9-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="265c9-105">Кейбір салалар нақты деңгейде, ал басқа салалар одан жоғары деңгейде бақыланады.</span><span class="sxs-lookup"><span data-stu-id="265c9-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="265c9-106">Бұл тақырыпта ұйымыңыздың талаптарын қанағаттандыру үшін жоспарлау жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="265c9-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="265c9-107">Талпынысты бақылау көрінісі</span><span class="sxs-lookup"><span data-stu-id="265c9-107">Effort tracking view</span></span>

<span data-ttu-id="265c9-108">**Талпынысты бақылау** көрінісі кестедегі тапсырмалардың орындалу барысын қадағалайды.</span><span class="sxs-lookup"><span data-stu-id="265c9-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="265c9-109">Ол тапсырма бойынша жұмсалған жалпы талпыныс сағаттарын тапсырма бойынша жоспарланған талпыныс сағаттарымен салыстырады.</span><span class="sxs-lookup"><span data-stu-id="265c9-109">It compares the actual effort hours that have been spent on a task to the planned effort hours for that task.</span></span> <span data-ttu-id="265c9-110">PSA бағдарламасы бақылау өлшемдерін есептеу үшін келесі формулаларды қолданады:</span><span class="sxs-lookup"><span data-stu-id="265c9-110">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="265c9-111">Орындалу пайызы = бүгінгі күнге жұмсалған нақты талпыныс ÷ тапсырма үшін жоспарланған талпыныс</span><span class="sxs-lookup"><span data-stu-id="265c9-111">Progress percentage = Actual effort spent to date ÷ Planned effort for the task</span></span> 
- <span data-ttu-id="265c9-112">Аяқтауды бағалау (ETC) = жоспарланған талпыныс - бүгінгі күнге жұмсалған нақты талпыныс</span><span class="sxs-lookup"><span data-stu-id="265c9-112">Estimate to complete (ETC) = Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="265c9-113">Аяқтау кезіндегі бағалау (EAC) = қалған талпыныс + бүгінгі күнге жұмсалған нақты талпыныс</span><span class="sxs-lookup"><span data-stu-id="265c9-113">Estimate at complete (EAC) = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="265c9-114">Жоспарланған талпыныстың ауытқуы = жоспарланған талпыныс – EAC</span><span class="sxs-lookup"><span data-stu-id="265c9-114">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="265c9-115">PSA бағдарламасында тапсырма бойынша талпыныс ауытқуының проекциясы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="265c9-115">PSA shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="265c9-116">Егер EAC жоспарланған талпыныстан көп болса, онда тапсырма бастапқыда жоспарланғаннан көп уақытты алады.</span><span class="sxs-lookup"><span data-stu-id="265c9-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="265c9-117">Сондықтан, бұл кесте бойынша кешігетін болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-117">Therefore, it's behind schedule.</span></span> <span data-ttu-id="265c9-118">Егер EAC жоспарланған талпыныстан кем болса, онда тапсырма бастапқыда жоспарланғаннан аз уақытты алады.</span><span class="sxs-lookup"><span data-stu-id="265c9-118">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="265c9-119">Сондықтан, бұл кесте бойынша ілгері болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-119">Therefore, it's ahead of schedule.</span></span>

## <a name="re-projecting-effort"></a><span data-ttu-id="265c9-120">Қайта жобалау әрекеті</span><span class="sxs-lookup"><span data-stu-id="265c9-120">Re-projecting effort</span></span>

<span data-ttu-id="265c9-121">Жоба менеджері үшін тапсырманың бастапқы болжамдарын қайта қарау әдеттегідей болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-121">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="265c9-122">Жобаның қайта болжаулары – бұл жобаның қазіргі күйін ескере отырып, жоба менеджерінің бағалауды қабылдауы.</span><span class="sxs-lookup"><span data-stu-id="265c9-122">Project re-projections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="265c9-123">Алайда, біз жоба менеджерлеріне бастапқы сандарды өзгертуге кеңес бермейміз, себебі жобаның бастапқы мәні жоба кестесі мен құн болжамы үшін шындықтың бекітілген көзі болып табылады және барлық мүдделі тараптар бұған келіскен.</span><span class="sxs-lookup"><span data-stu-id="265c9-123">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="265c9-124">Жоба менеджері үшін тапсырмалар бойынша талпынысты қайта жобалаудың екі жолы бар:</span><span class="sxs-lookup"><span data-stu-id="265c9-124">There are two ways that a project manager can re-project effort on tasks:</span></span>

- <span data-ttu-id="265c9-125">Тапсырмада нақты қалған талпыныстың жаңа болжамын әдепкі ETC элементімен ауыстыру.</span><span class="sxs-lookup"><span data-stu-id="265c9-125">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="265c9-126">Тапсырма бойынша нақты орындалу барысының жаңа болжамын әдепкі орындалу барысының пайызымен ауыстыру.</span><span class="sxs-lookup"><span data-stu-id="265c9-126">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="265c9-127">Осы тәсілдердің әрқайсысы тапсырманың ETC, аяқтау кезіндегі құн болжамы (EAC) және орындалу пайызын қайта есептеуді және тапсырма бойынша талпыныстың ауытқуын тудырады.</span><span class="sxs-lookup"><span data-stu-id="265c9-127">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="265c9-128">Аяқтау кезіндегі құн болжамы (EAC), ETC және жиынтық тапсырмалар бойынша орындалу пайызы да қайта есептелінеді және талпыныс ауытқуының жаңа болжамын жасайды.</span><span class="sxs-lookup"><span data-stu-id="265c9-128">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="re-projection-of-effort-on-summary-tasks"></a><span data-ttu-id="265c9-129">Жиынтық тапсырмалар бойынша талпынысты қайта жобалау</span><span class="sxs-lookup"><span data-stu-id="265c9-129">Re-projection of effort on summary tasks</span></span>

<span data-ttu-id="265c9-130">Жиынтық тапсырмалар немесе контейнер тапсырмалары бойынша талпынысты қайта жобалауға болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-130">Effort on summary tasks or container tasks can be re-projected.</span></span> <span data-ttu-id="265c9-131">Пайдаланушы қалған талпынысты немесе жиынтық тапсырмалар бойынша орындалу пайызын қолдана отырып жобаны қайтадан жобалауына қарамастан, келесі есептеулер жиынтығы басталады:</span><span class="sxs-lookup"><span data-stu-id="265c9-131">Regardless of whether the user re-projects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="265c9-132">Аяқтау кезіндегі құн болжамы (EAC), ETC және тапсырманың орындалу пайызы есептеледі.</span><span class="sxs-lookup"><span data-stu-id="265c9-132">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="265c9-133">Жаңа аяқтау кезіндегі құн болжамы (EAC) қосалқы тапсырмаларға тапсырмада болған бастапқы аяқтау кезіндегі құн болжамымен (EAC) бірдей пропорцияда үлестірілді.</span><span class="sxs-lookup"><span data-stu-id="265c9-133">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="265c9-134">Жаңа аяқтау кезіндегі құн болжамы (EAC) әрбір жеке тапсырмалардан бастап, соңғы түйін тапсырмаларына дейін есептеледі.</span><span class="sxs-lookup"><span data-stu-id="265c9-134">The new EAC on each of the individualt tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="265c9-135">Әсер ететін қосалқы тапсырмалар соңғы түйіндерге дейін EAC мәні негізінде қайта есептелген ETC және орындалу пайызын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="265c9-135">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="265c9-136">Нәтижесінде тапсырма бойынша талпыныс ауытқуы үшін жаңа проекция пайда болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-136">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="265c9-137">Жиынтық тапсырмалардың EAC мәндері түбірлік түйінге дейін қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="265c9-137">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="265c9-138">Құн бақылауы көрінісі</span><span class="sxs-lookup"><span data-stu-id="265c9-138">Cost tracking view</span></span> 

<span data-ttu-id="265c9-139">**Құн бақылауы** көрінісі тапсырмаға жұмсалған нақты құнын тапсырманың жоспарланған құнымен салыстырады.</span><span class="sxs-lookup"><span data-stu-id="265c9-139">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="265c9-140">Бұл көрініс тек еңбек шығындарын көрсетеді және шығын болжамдарының шығындарды қамтымайды.</span><span class="sxs-lookup"><span data-stu-id="265c9-140">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="265c9-141">PSA бағдарламасы бақылау өлшемдерін есептеу үшін келесі формулаларды қолданады:</span><span class="sxs-lookup"><span data-stu-id="265c9-141">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="265c9-142">Тұтынылған шығындар пайызы = осы күнге жұмсалған нақты шығындар ÷ тапсырманың жоспарланған құны</span><span class="sxs-lookup"><span data-stu-id="265c9-142">Percentage of cost consumed = Actual cost spent to date ÷ Planned cost for the task</span></span>
- <span data-ttu-id="265c9-143">Аяқтауды бағалау (CTC) = жоспарланған құн – осы күнге жұмсалған нақты шығындар</span><span class="sxs-lookup"><span data-stu-id="265c9-143">Cost to complete (CTC) = Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="265c9-144">EAC = CTC + осы күнге жұмсалған нақты шығындар</span><span class="sxs-lookup"><span data-stu-id="265c9-144">EAC = CTC + Actual cost spent to date</span></span>
- <span data-ttu-id="265c9-145">Жобаланған құнның ауытқуы = жоспарланған құны – EAC</span><span class="sxs-lookup"><span data-stu-id="265c9-145">Projected cost variance = Planned cost – EAC</span></span>

<span data-ttu-id="265c9-146">Құн ауытқуының проекциясы тапсырмада көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="265c9-146">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="265c9-147">Егер аяқтау кезіндегі құн болжамы (EAC) жоспарланған құннан көп болса, онда тапсырма құны бастапқыда жоспарланғаннан көп болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-147">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="265c9-148">Сондықтан, бұл бюджеттен тыс болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-148">Therefore, it's trending over budget.</span></span> <span data-ttu-id="265c9-149">Егер аяқтау кезіндегі құн болжамы (EAC) жоспарланған құннан кем болса, онда тапсырма құны бастапқыда жоспарланғаннан аз болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-149">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="265c9-150">Сондықтан, бұл бюджет шеңберінде болады.</span><span class="sxs-lookup"><span data-stu-id="265c9-150">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-re-projection-of-cost"></a><span data-ttu-id="265c9-151">Жоба менеджерінің құнды қайта жобалауы</span><span class="sxs-lookup"><span data-stu-id="265c9-151">Project manager’s re-projection of cost</span></span>

<span data-ttu-id="265c9-152">Талпыныс қайта жобаланған кезде, CTC, аяқтау кезіндегі құн болжамы (EAC), тұтынылған шығынның пайызы және шығындардың болжамды ауытқуы **Құн бақылауы** көрінісінде қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="265c9-152">When effort is re-projected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="265c9-153">Жоба күйінің қорытындысы</span><span class="sxs-lookup"><span data-stu-id="265c9-153">Project status summary</span></span>

<span data-ttu-id="265c9-154">**Талпынысты бақылау** және **Құн бақылауы** көріністеріндегі бақылау деректері жобаның түпкі түйініндегі, жиынтық тапсырмалардағы және соңғы түйін тапсырмалар деңгейіндегі орындалу барысы мен құн шығынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="265c9-154">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="265c9-155">**Жоба нысаны** бетіндегі **Күй** бөлімінде жоба деңгейіндегі күйдің қорытындысы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="265c9-155">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="265c9-156">Күй қорытындысының өрістері</span><span class="sxs-lookup"><span data-stu-id="265c9-156">Status summary fields</span></span>

<span data-ttu-id="265c9-157">**Жобаның жалпы күйі** өрісі — бұл жобаның жалпы күйін көрсететін өңделетін өріс.</span><span class="sxs-lookup"><span data-stu-id="265c9-157">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="265c9-158">Ол артып келе жатқан қауіпті көрсету үшін жасыл, сары және қызыл сияқты түрлі түсті кодтауды қолданады.</span><span class="sxs-lookup"><span data-stu-id="265c9-158">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="265c9-159">**Пікірлер** өрісі жоба менеджеріне күй туралы нақты түсініктемелер енгізуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="265c9-159">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="265c9-160">**Күйі жаңартылған күн** өрісі өңделмейді және мән күйдің соңғы рет жаңартылған уақытын көрсететін уақыт белгісі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="265c9-160">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="265c9-161">**Кесте өнімділігі** және **Құн өнімділігі** өрістері бақылау күнінен бастап орнатылады.</span><span class="sxs-lookup"><span data-stu-id="265c9-161">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="265c9-162">**Талпынысты бақылау** көрінісіндегі түбірлік түйіннің кесте мен құн ауытқуы оң болғанда, осы өрістерді **Ahead** мәніне орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="265c9-162">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="265c9-163">Түбірлік түйіннің кесте мен құн ауытқуы теріс болса, оларды **Артында** мәніне орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="265c9-163">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
