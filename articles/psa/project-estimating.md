---
title: Жоба шығындары мен табысы
description: Бұл тақырыпта жоба шығындары мен табысын есептеу жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: 9862b6c69596f5b998cf40691f8478bb87251583
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079690"
---
# <a name="project-costs-and-revenue"></a><span data-ttu-id="a2716-103">Жоба шығындары мен табысы</span><span class="sxs-lookup"><span data-stu-id="a2716-103">Project costs and revenue</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a2716-104">Жоба болжамдары жоба кестесінде болжанған және жоспарланған жұмыстың қаржылық көрінісін береді.</span><span class="sxs-lookup"><span data-stu-id="a2716-104">Project estimates provide the financial view for work that is estimated and scheduled in the project schedule.</span></span> <span data-ttu-id="a2716-105">**Жобалар** бетіндегі **Болжамдар** қойыншасында жоспарланатын жұмыстың құны мен табысы әсері көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="a2716-105">The **Estimates** tab on the **Projects** page shows the cost and revenue impact of the work that you’re planning.</span></span> <span data-ttu-id="a2716-106">Онда сонымен қатар көптеген алдын ала анықталған өлшемдер туралы ақпарат беріледі.</span><span class="sxs-lookup"><span data-stu-id="a2716-106">It also provides information about many predefined dimensions.</span></span> 

> ![Болжамдар қойыншасы](media/project-5.png)

## <a name="cost-and-sales-values-of-the-project"></a><span data-ttu-id="a2716-108">Жобаның құны мен сатылым мәндері</span><span class="sxs-lookup"><span data-stu-id="a2716-108">Cost and sales values of the project</span></span>

<span data-ttu-id="a2716-109">Бағатізбелер жобадағы рөлдер құны мен шот мөлшерлемелерін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="a2716-109">Price lists define the cost and bill rates for roles in a project.</span></span> <span data-ttu-id="a2716-110">Тапсырмаға тағайындалған күй атауымен және аталған ресурспен байланысты рөлдерге сүйене отырып, жұмыстың құны мен табысы әсерін анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="a2716-110">You can determine the cost and revenue impact of the work, based on the roles that are associated with the position name and the named resource that is assigned to a task.</span></span> <span data-ttu-id="a2716-111">Егер тағайындамалары (жалпы немесе аталған) жоқ тапсырмалар бар болса, құн мен сатылым болжамдарын ала алмайсыз.</span><span class="sxs-lookup"><span data-stu-id="a2716-111">If there are tasks that don't have any assignments (generic or named), you can’t get cost or sales estimates.</span></span> <span data-ttu-id="a2716-112">Құн мен сатылым мәндері бағатізбелерде анықталған күнді ескереді.</span><span class="sxs-lookup"><span data-stu-id="a2716-112">Cost and sales values consider the date that is defined in the price lists.</span></span>

### <a name="default-cost-price"></a><span data-ttu-id="a2716-113">Әдепкі шығын</span><span class="sxs-lookup"><span data-stu-id="a2716-113">Default cost price</span></span>  

<span data-ttu-id="a2716-114">Әр жоба ұйымға тиесілі болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-114">Every project belongs to an organization.</span></span> <span data-ttu-id="a2716-115">Бұл ұйым жобадағы **Келісім-шарт бірлігі** өрісінде көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="a2716-115">This organization is shown in the **Contracting Unit** field in the project.</span></span> <span data-ttu-id="a2716-116">Бірліктің шығынын анықтау үшін, келісім-шарт бірлігімен байланысты бағатізбе пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-116">The price list that is associated with the contracting unit is used to determine the unit cost price.</span></span> <span data-ttu-id="a2716-117">Болжам жолдарында белгіленген күн бойынша рөлдердің дұрыс шығынын анықтау үшін, шығындар тізімінде рөлдің, бірліктің және ұйымдық бөлімшенің тіркесімін табыңыз.</span><span class="sxs-lookup"><span data-stu-id="a2716-117">To determine the correct cost prices on roles for the date that is defined on estimate lines, search for the combination of role, unit, and organizational unit in the cost price list.</span></span> 

<span data-ttu-id="a2716-118">Олардың шығындарын есептеу үшін, барлық тапсырмалар ресурсқа тағайындалуы керек.</span><span class="sxs-lookup"><span data-stu-id="a2716-118">So that their cost prices can be calculated, all tasks must be assigned to a resource.</span></span> <span data-ttu-id="a2716-119">Тағайындалмаған кез келген тапсырманың шығыны 0,00 болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-119">Any uwnassigned tasks will have a cost price of 0.00.</span></span>

<span data-ttu-id="a2716-120">Егер рөлдің, бірліктің және ұйымдық бөлімшенің тіркесімі келісімшарт бірлігінің бағатізбесіндегі шығынды қайтармаса, жүйе бірлікті ескермейтін болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-120">If the combination of role, unit, and organizational unit doesn't return a cost price from the contracting unit's price list, the system ignores the unit.</span></span> <span data-ttu-id="a2716-121">Оның орнына, ол тек рөл мен ұйымдық бөлімшенің тіркесімін іздейді.</span><span class="sxs-lookup"><span data-stu-id="a2716-121">Instead, it searches for the combination of just role and organizational unit.</span></span> <span data-ttu-id="a2716-122">Егер шығын табылса, оны болжам жолында таңдалған бірлікке айналдыру үшін түрлендіру факторлары қолданылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-122">If a cost price is found, conversion factors are used to convert it to the unit that you selected on the estimate line.</span></span>

<span data-ttu-id="a2716-123">Егер рөлдің және ұйымдық бөлімшенің тіркесімі шығынды қайтармаса, жүйе ұйымдық бөлімшені ескермейтін болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-123">If the combination of role and organizational unit doesn't return a cost price, the system ignores the organizational unit.</span></span> <span data-ttu-id="a2716-124">Оның орнына, ол әдепкі бағаны белгілеу үшін рөл мен бірліктің тіркесімін іздейді (кез келген түрлендіру қолданылғаннан кейін).</span><span class="sxs-lookup"><span data-stu-id="a2716-124">Instead, it searches for the combination of role and unit to set the default price (after any conversion is applied).</span></span>

<span data-ttu-id="a2716-125">Егер жүйеде рөл бағасы табылмаса, болжам жолындағы шығын әдепкі бойынша **0,00** мәніне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-125">If the system doesn't find a price for the role, the cost price on the estimate line is set to a default value of **0.00**.</span></span> <span data-ttu-id="a2716-126">Жоба құны болжалды жолдарындағы барлық құн сомалары ұйымдық бөлімше валютасында жазылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-126">All cost amounts on the project cost estimate lines are recorded in the currency of the contracting unit.</span></span>

> [!NOTE]
> <span data-ttu-id="a2716-127">Әдепкі бойынша Microsoft Dynamics 365 бағдарламасы құн сомаларын сіздің негізгі валютаңызда сақтайды.</span><span class="sxs-lookup"><span data-stu-id="a2716-127">By default, Microsoft Dynamics 365 stores cost amounts in your base currency.</span></span> <span data-ttu-id="a2716-128">Алайда, **Болжамдар** қойыншасында көрсетілген құн сомалары келісімшарт бірлігінің валютасында болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-128">However, the cost amounts that are shown on the **Estimates** tab are in the currency of the contracting unit.</span></span>  

### <a name="default-sales-price"></a><span data-ttu-id="a2716-129">Әдепкі сатылым бағасы</span><span class="sxs-lookup"><span data-stu-id="a2716-129">Default sales price</span></span> 

<span data-ttu-id="a2716-130">Сатылым бағатізбесі жоба тіркелген сатылым нысаны немесе жоба тұтынушысы арқылы анықталады.</span><span class="sxs-lookup"><span data-stu-id="a2716-130">The sales price list is determined by either the sales entity that the project is attached to or the project customer.</span></span> <span data-ttu-id="a2716-131">Мүмкіндік, баға ұсынысы немесе келісім-шарт сияқты сатылым нысаны жобамен байланысты болған кезде, сатылым нысанының сатылым бағасы баға ұсынысымен немесе келісім-шартпен байланысты бағатізбемен анықталады.</span><span class="sxs-lookup"><span data-stu-id="a2716-131">When a sales entity, such as opportunity, quote, or contract, is associated with the project, the sales entity's sales price is determined by the price list that is associated with the quote or contract.</span></span> <span data-ttu-id="a2716-132">Егер баға ұсынысы немесе келісім-шарт ішінде реттелетін бағатізбе бар болса, сол бағатізбе жоба болжамдарының әдепкі сатылым бағатізбесі ретінде пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-132">If the quote or contract has a custom price list, that price list is used as the default sales price list for project estimates.</span></span> <span data-ttu-id="a2716-133">Егер сатылым нысандарымен байланыс болмаса, параметрлердегі әдепкі сатылым бағатізбесі жобада анықталған тұтынушы валютасымен сәйкестендірілген жобаның әдепкі сатылым бағатізбесі ретінде пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-133">If there is no association with sales entities, the default sales price list from the parameters is used as the project's default sales price list matched by the customer currency that is defined on the project.</span></span>

<span data-ttu-id="a2716-134">Әр болжам жолында оған байланысты ресурс бірлігі болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-134">Each estimate line has a resourcing unit that is associated with it.</span></span> <span data-ttu-id="a2716-135">Ресурс бірлігі тапсырманы орындау үшін ресурстары резервтелген ұйымдық бөлімшені білдіреді.</span><span class="sxs-lookup"><span data-stu-id="a2716-135">The resourcing unit indicates the organizational unit that resources are booked from to complete the task.</span></span> <span data-ttu-id="a2716-136">Байланысты рөлдердің сатылым бағаларын анықтау үшін, сатылым бағатізбесіндегі рөлдің, бірліктің және ресурс бірлігінің тіркесімін іздеңіз.</span><span class="sxs-lookup"><span data-stu-id="a2716-136">To determine the sales price for the associated roles, search for the combination of role, unit, and resourcing unit in the sales price list.</span></span> <span data-ttu-id="a2716-137">Егер тапсырмада ешқандай тағайындаулар болмаса, тапсырманың сатылым бағасы 0,00 мәнін құрайды.</span><span class="sxs-lookup"><span data-stu-id="a2716-137">If there are no assignments on the task, the sales price for the task is 0.00.</span></span>

<span data-ttu-id="a2716-138">Егер рөлдің, бірліктің және ресурс бірлігінің тіркесімі сатылым бағатізбесіндегі сатылым бағасын қайтармаса, жүйе бірлікті ескермейтін болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-138">If the combination of role, unit, and resourcing unit doesn't return a sales price from the sales price list, the system ignores the unit.</span></span> <span data-ttu-id="a2716-139">Оның орнына, ол тек рөл мен ресурс бірлігінің тіркесімін іздейді.</span><span class="sxs-lookup"><span data-stu-id="a2716-139">Instead, it searches for the combination of just role and resourcing unit.</span></span> <span data-ttu-id="a2716-140">Егер сатылым бағасы табылса, оны сатылымның болжам жолында таңдалған бірлікке айналдыру үшін түрлендіру факторлары қолданылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-140">If a sales price is found, conversion factors are used to convert it to the unit that you selected on the sales estimate line.</span></span> 

<span data-ttu-id="a2716-141">Егер рөлдің және ресурс бірлігінің тіркесімі сатылым бағатізбесіндегі сатылым бағасын қайтармаса, жүйе ресурс бірлігін ескермейтін болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-141">If the combination of role and resourcing unit doesn't return a sales price from the sales price list, the system ignores the resourcing unit.</span></span> <span data-ttu-id="a2716-142">Оның орнына, ол әдепкі бағаны белгілеу үшін рөл мен бірліктің тіркесімін іздейді (кез келген түрлендіру қолданылғаннан кейін).</span><span class="sxs-lookup"><span data-stu-id="a2716-142">Instead, it searches for the combination of role and unit to set the default price (after any conversion is applied).</span></span>

<span data-ttu-id="a2716-143">Егер жүйеде рөл бағасы табылмаса, болжам жолындағы сатылым бағасы әдепкі бойынша **0,00** мәніне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-143">If the system doesn't find a price for the role, the sales price on the estimate line is set to a default value of **0.00**.</span></span>

<span data-ttu-id="a2716-144">**Болжамдар** қойыншасында болжам жолдары көрсетілген тор көрінісі бар.</span><span class="sxs-lookup"><span data-stu-id="a2716-144">The **Estimates** tab has a grid view that shows estimate lines.</span></span> <span data-ttu-id="a2716-145">Торға келесі суретте көрсетілгендей бірлік бағандары, жалпы шығын және сатылымның жалпы бағасы кіреді.</span><span class="sxs-lookup"><span data-stu-id="a2716-145">The grid includes columns for the unit, total cost price, and total sales price, as shown in the following illustration.</span></span> 

> ![Болжамдар қойыншасындағы тор көрінісі](media/project-6.png)

## <a name="time-phased-view-of-project-estimates"></a><span data-ttu-id="a2716-147">Жоба болжамдарының уақыт көрінісі</span><span class="sxs-lookup"><span data-stu-id="a2716-147">Time-phased view of project estimates</span></span>

<span data-ttu-id="a2716-148">Жоба болжамдарының уақыт кезеңіндегі көрінісінде таңдалған уақыт шкаласындағы уақыт кестесі бойынша тор көрінісіндегі болжам деректері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a2716-148">The time-phased view of project estimates shows the estimate data from the grid view across the timeline, in a time scale that you select.</span></span> <span data-ttu-id="a2716-149">Әдепкі бойынша, болжам деректері **Рөл** өлшемінде беріледі.</span><span class="sxs-lookup"><span data-stu-id="a2716-149">By default, the estimate data is pivoted on the **Role** dimension.</span></span>

> ![Жоба болжамдарының уақыт кезеңіндегі көрінісі](media/project-7.png)

## <a name="allocating-estimated-effort-based-on-the-task-mode"></a><span data-ttu-id="a2716-151">Болжалды талпынысты тапсырма режимі негізінде тағайындау</span><span class="sxs-lookup"><span data-stu-id="a2716-151">Allocating estimated effort based on the task mode</span></span>

<span data-ttu-id="a2716-152">Уақыт кезеңіндегі көріністе жалпы талпынысты талпыныс сағаттарын таңдалған уақыт шкаласындағы әрбір бірлік уақыт кезеңі бойынша болжау арқылы бөлесіз.</span><span class="sxs-lookup"><span data-stu-id="a2716-152">In the time-phased view, you distribute the total effort that is estimated for the task by allocating effort hours per unit time period in the selected time scale.</span></span> <span data-ttu-id="a2716-153">Тапсырма режимі тапсырма ұзақтығы бойынша талпынысты тағайындау әдісін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="a2716-153">The task mode determines how effort is allocated across the duration of the task.</span></span> <span data-ttu-id="a2716-154">Тағайындаудың екі түрі — **Бірдей** және **Жұмыс сағаттары негізіндегі**.</span><span class="sxs-lookup"><span data-stu-id="a2716-154">The two kinds of allocation are **Even** and **Work hours–based**.</span></span>

### <a name="work-hours-based-allocation"></a><span data-ttu-id="a2716-155">Жұмыс сағаттары негізіндегі тағайындау</span><span class="sxs-lookup"><span data-stu-id="a2716-155">Work hours-based allocation</span></span>
 
<span data-ttu-id="a2716-156">Автоматты түрде жоспарлау режимінде, тапсырма ресурстарының күнделікті сағаттары жұмыс уақытының толық көлемінде орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-156">In auto-scheduling task mode, the daily default hours for task resources are set at the full work hour rate.</span></span> <span data-ttu-id="a2716-157">Бұл әрекет талпынысты уақыт көрінісіндегі тапсырмалар ұзақтығына бөлу арқылы тағайындау кезінде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="a2716-157">This behavior applies when effort is allocated by splitting it across the duration of the task in the time-phased view.</span></span> <span data-ttu-id="a2716-158">Мысалы, егер тапсырманы **Күн** уақыт шкаласындағы бір ресурспен аяқтайсыз деп болжасаңыз, күнделікті тағайындалған талпыныс жоба күнтізбесінде анықталған күнделікті жұмыс сағаттарынан аспайды.</span><span class="sxs-lookup"><span data-stu-id="a2716-158">For example, if you estimate that a task will be completed by one resource in the **Day** time scale, the effort that is allocated per day won't exceed the work hours per day that are defined in the project calendar.</span></span> <span data-ttu-id="a2716-159">Сол себепті, талпыныс тағайындау ресурстар толық күнде пайдаланылады деп болжанады.</span><span class="sxs-lookup"><span data-stu-id="a2716-159">Therefore, the effort allocation always makes sure that the resources are estimated to be used for the full day.</span></span>

### <a name="even-allocation"></a><span data-ttu-id="a2716-160">Бірдей тағайындау</span><span class="sxs-lookup"><span data-stu-id="a2716-160">Even allocation</span></span>

<span data-ttu-id="a2716-161">Қолмен жоспарланған тапсырма режимінде жоба күнтізбесіндегі жұмыс сағаттары пайдаланылмайды.</span><span class="sxs-lookup"><span data-stu-id="a2716-161">In manually scheduled task mode, the work hours from the project calendar aren't used.</span></span> <span data-ttu-id="a2716-162">Оның орнына, тапсырма кестесі пайдаланушы енгізіліміне негізделеді.</span><span class="sxs-lookup"><span data-stu-id="a2716-162">Instead, the task schedule is based on user input.</span></span> <span data-ttu-id="a2716-163">Осы тапсырмалар үшін таңдалған уақыт шкаласындағы әрбір бірлік уақыт кезеңі бойынша талпыныс тағайындауында ешқандай шектеу факторы болмайды.</span><span class="sxs-lookup"><span data-stu-id="a2716-163">For these tasks, the effort allocation per unit time period in the selected time scale doesn't have any limiting factor.</span></span> <span data-ttu-id="a2716-164">Тапсырмадағы жалпы талпыныс теңдей бөлініп, таңдалған уақыт шкаласындағы әрбір бірлік уақыт кезеңіне тағайындалады.</span><span class="sxs-lookup"><span data-stu-id="a2716-164">The total effort on the task is equally split and allocated for each unit time period in the selected time scale.</span></span> <span data-ttu-id="a2716-165">Сондықтан, тапсырмада анықталған тапсырма режимі уақыт болжамдарындағы әрбір бірлік уақыт кезеңінде талпыныс тағайындалуын немесе таралуын анықтайды.</span><span class="sxs-lookup"><span data-stu-id="a2716-165">Therefore, the task mode that is defined on the task determines the effort distribution, or the allocation of effort per unit time period in time-phased estimates.</span></span>

## <a name="grouping-and-time-phasing-options"></a><span data-ttu-id="a2716-166">Топтастыру және уақыт опциялары</span><span class="sxs-lookup"><span data-stu-id="a2716-166">Grouping and time-phasing options</span></span>

<span data-ttu-id="a2716-167">Уақыт кезеңіндегі көріністе күн, апта, ай немесе жыл негізінде талпыныс, құн және сатылым болжамдарының таралуы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a2716-167">The time-phased view shows the distribution of the effort, cost, and sales estimates on a daily, weekly, monthly, or yearly basis.</span></span> <span data-ttu-id="a2716-168">Әдепкі бойынша, болжам деректері **Рөл** өлшемінде беріледі.</span><span class="sxs-lookup"><span data-stu-id="a2716-168">By default, the estimate data is pivoted on the **Role** dimension.</span></span> <span data-ttu-id="a2716-169">Алайда, келесі екі өлшем бойынша еркін түрде айналу үшін **Топтау әдісі** опциясын пайдалануға болады: **Санат** және **Ресурс**.</span><span class="sxs-lookup"><span data-stu-id="a2716-169">However, you can use the **Group By** option to pivot on two other dimensions: **Category** and **Resource**.</span></span>

<span data-ttu-id="a2716-170">Тор көрінісінде де, уақыт кезеңіндегі көріністе де көрсетілетін өрістерді таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-170">In both the grid view and the time-phased view, you can select which fields are shown.</span></span> <span data-ttu-id="a2716-171">Әр уақыт блогының жиынтығы жобаның төменгі жағында көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a2716-171">Totals for each time block are shown at the bottom of the project.</span></span> <span data-ttu-id="a2716-172">Онда күн, апта, ай немесе жылдың жалпы есептелген талпынысы, құны және сатылымы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a2716-172">They show the total estimated effort, cost, and sales for the day, week, month, or year.</span></span> <span data-ttu-id="a2716-173">Әдепкі шығын және сатылым бағасы мерзімге сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="a2716-173">The default cost price and sales price are date-effective.</span></span> <span data-ttu-id="a2716-174">Басқаша айтқанда, олар таңдалған уақыт кезеңіндегі көрініске негізделген әр ресурс бойынша өзгереді.</span><span class="sxs-lookup"><span data-stu-id="a2716-174">In other words, they change for each resource, based on the time-phased view that you select.</span></span>

## <a name="expense-estimates"></a><span data-ttu-id="a2716-175">Шығыс болжамдары</span><span class="sxs-lookup"><span data-stu-id="a2716-175">Expense estimates</span></span>

<span data-ttu-id="a2716-176">Тор көрінісіндегі **Жаңа шығыс болжамын қосу** түймешігі жобада келтірілген, бірақ еңбекке тікелей қатысы жоқ кез келген шығыстарды жазуға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="a2716-176">The **Add a New Expense Estimate** button in the grid view lets you record any expenses that are incurred in the project, but that aren't directly related to labor.</span></span> <span data-ttu-id="a2716-177">Белгілі бір тапсырма немесе бүкіл жоба бойынша шығын болжамдарын жазып алуға болады.</span><span class="sxs-lookup"><span data-stu-id="a2716-177">You can record the expense estimates for a specific task or for the entire project.</span></span> <span data-ttu-id="a2716-178">Шығыс санаттары мен шығындар күтілетін күнді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a2716-178">Select expense categories and the tentative date when you expect to incur the expense.</span></span> <span data-ttu-id="a2716-179">Егер байланысты құн бағатізбесі және сатылым бағатізбесінде әдепкі бағалар бар болса (немесе үстеме баға пайыздары шығыс санаттары үшін анықталған болса), байланыс орнаған кезде олар автоматты түрде болжам жолына өтеді.</span><span class="sxs-lookup"><span data-stu-id="a2716-179">If the associated cost price list and sales price list have default prices (or if markup percentages are defined for expense categories), they are automatically entered on the estimate line when the association occurs.</span></span>