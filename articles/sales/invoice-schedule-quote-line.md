---
title: жоба негізіндегі баға ұсыну жолдарындағы шот-фактура кестелері
description: Бұл тақырып шот-фактура кестесін құру және баға ұсыну жолдары үшін кезеңдер туралы ақпарат береді.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0ecaf4d872873473b0e7fe3b08d62c6fe5af9c3d
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908325"
---
# <a name="invoice-schedules-on-project-based-quote-lines"></a><span data-ttu-id="a0da8-103">Жоба негізіндегі баға ұсыну жолдарындағы шот-фактура кестелері</span><span class="sxs-lookup"><span data-stu-id="a0da8-103">Invoice schedules on project-based quote lines</span></span>

<span data-ttu-id="a0da8-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="a0da8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a0da8-105">Жоба негізіндегі баға ұсыну жолы шот-фактуралардың кестесін көрсетуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="a0da8-105">A project-based quote line gives the ability to express an invoice schedule.</span></span> <span data-ttu-id="a0da8-106">Бұл баға белгілеу кезеңінде міндетті емес, өйткені бағдарлама баға ұсыну жолына қосылған кезде жобаға шот-фактураны ұсынуды қолдамайды.</span><span class="sxs-lookup"><span data-stu-id="a0da8-106">This is optional during the quote phase because the application does not support invoicing a project when it is tied to a Quote line.</span></span> <span data-ttu-id="a0da8-107">Шот-фактура ұсынуға баға ұсыныстарын ұтып алғаннан кейін ғана рұқсат етіледі.</span><span class="sxs-lookup"><span data-stu-id="a0da8-107">Invoicing is only allowed after the quote is won.</span></span> <span data-ttu-id="a0da8-108">Баға ұсыну кезеңінде шот-фактуралар кестесін құрудың бірден-бір төменгі ағынды әсері - бұл шот-фактуралар кестесінің жоба негізінде келісім-шарт жолына көшірілуі.</span><span class="sxs-lookup"><span data-stu-id="a0da8-108">The only downstream impact of creating an invoice schedule during the quote phase, is that this invoice schedule is copied over to the project-based contract line.</span></span> <span data-ttu-id="a0da8-109">Егер сіз баға ұсыну кезеңінде шот-фактураның кестесін жасамасаңыз, онда сіз оны жоба негізінде келісімшарттар желісінде жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-109">If you do not create an invoice schedule during the quote phase, you will be able to do so on the project-based contract line.</span></span>

<span data-ttu-id="a0da8-110">Тұтастай алғанда, шот-фактуралар кестесінің мақсаты жоба негізінде келісімшарттар желісі үшін шот-фактуралардың автоматты түрде жасалуына мүмкіндік беру болып табылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-110">Overall, the purpose of invoice schedules is to allow for the automatic creation of draft invoices for a project-based contract line.</span></span> 

## <a name="create-a-time-and-material-invoice-schedule-for-a-project-based-quote-line"></a><span data-ttu-id="a0da8-111">Жобаға негізделген баға ұсынысы үшін уақыт пен материал бойынша шот-фактуралар кестесін жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-111">Create a Time and material invoice schedule for a project-based quote line</span></span>

<span data-ttu-id="a0da8-112">Жобаға негізделген баға ұсынысы әдісі «Уақыт пен материал» болған кезде, жүйе шот-фактура кестесін жасайды.</span><span class="sxs-lookup"><span data-stu-id="a0da8-112">When the billing method for a project-based quote line is Time and material, the system generates a date-based invoice schedule.</span></span> <span data-ttu-id="a0da8-113">Шот-фактура кестесін автоматты түрде жасау үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-113">To automatically generate a date-based invoice schedule, complete the following steps.</span></span>

1. <span data-ttu-id="a0da8-114">**Параметрлер** > **шот-фактура ұсыну жиіліктері** тармағына өтіп, шот-фактура ұсыну жиілігін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-114">Go to **Settings** > **invoice frequencies** and set up an invoice frequency.</span></span>
2. <span data-ttu-id="a0da8-115">**Баға ұсыныстары** бетінде жобаның баға ұсынысын ашып, **Жиынтық** қойыншасында сұралған жеткізу күнін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-115">On the **Quotes** page, open the Project quote and on the **Summary** tab, set a requested delivery date.</span></span>
3. <span data-ttu-id="a0da8-116">Күні бойынша шот-фактура кестесін жасауыңыз керек уақыт пен материалдың баға ұсыну жолын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-116">Open the time and material quote line that you need to create a date-based invoice schedule for.</span></span> 
4. <span data-ttu-id="a0da8-117">**Шот-фактуралар кестесі** қойыншасында **Шот ұсыну басталу күні** және **Шот ұсыну жиілігі** өрістерінде мәндерді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-117">On the **Invoice Schedule** tab, select values in the **Billing start** and **Invoice Frequency** fields.</span></span> 
5. <span data-ttu-id="a0da8-118">Ішкі тордан **Шот-фактура кестесін құру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-118">On the sub-grid, select **Generate Invoice Schedule**.</span></span>
6. <span data-ttu-id="a0da8-119">Бағдарлама келесі жолда орнатылған **Есеп-шоттың орындалу күні**, **Транзакция мерзімі соңы** және **Орындау күйі** өрістерімен шот ұсыну кестесін жасайды.</span><span class="sxs-lookup"><span data-stu-id="a0da8-119">The application generates the invoice schedule with the **Invoice Run Date**, **Transaction Cutoff Date**, and **Run Status** fields set in the following way:</span></span>

    - <span data-ttu-id="a0da8-120">**Шот-фактураның орындалу күні** шот-фактураның жиілігі негізінде жазылатын күнге қойылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-120">**Invoice Run Date** is set to the date that is dictated based on the invoice frequency.</span></span>
    - <span data-ttu-id="a0da8-121">**Транзакцияны тоқтату күні** **Шот ұсынуды орындау күнінен** бір күн бұрын уақытқа орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-121">**Transaction cut-off date** is set to the day before the **Invoice Run Date**.</span></span>
    - <span data-ttu-id="a0da8-122">**Орындалу күйі** автоматты түрде **Іске қосылмау** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-122">**Run Status** is automatically set to **Not Run**.</span></span> <span data-ttu-id="a0da8-123">Нақты шот ұсыну күні үшін автоматты шот-фактура жасау жұмысы орындалғанда ол осы өрісті **Сәтті түрде орындау** немесе **Орындау сәтсіз аяқталды** күйлеріне жаңартады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-123">When the automatic invoice creation job runs for a certain invoice run date, it will update this field to either **Run Successful** or **Run Failed**.</span></span>

## <a name="create-a-fixed-price-invoice-schedule-for-a-project-based-quote-line"></a><span data-ttu-id="a0da8-124">Жобаға негізделген баға ұсынысы үшін бекітілген баға бойынша шот-фактуралар кестесін жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-124">Create a Fixed price invoice schedule for a project-based quote line</span></span>

<span data-ttu-id="a0da8-125">Жобаға негізделген баға ұсыну жолында **Бекітілген** шот ұсыну әдісі болғанда, жүйе кезеңдер негізінде шот-фактуралар кестесін жасайды.</span><span class="sxs-lookup"><span data-stu-id="a0da8-125">When the project-based quote line has a **Fixed** billing method, the system creates a milestone-based invoice schedule.</span></span> <span data-ttu-id="a0da8-126">Күнтізбелік кезеңге біркелкі бөлінген бақылау нүктелерінің белгіленген жиынтығы үшін осы диаграмманы автоматты түрде жасау үшін келесі әрекеттерді орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-126">Complete the following steps to automatically generate this schedule for a fixed set of milestones that are equally distributed for the calendar period.</span></span>

1. <span data-ttu-id="a0da8-127">**Параметрлер** > **шот-фактура ұсыну жиіліктері** тармағына өтіп, шот-фактура ұсыну жиілігін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-127">Go to **Settings** > **invoice frequencies** and set up an invoice frequency.</span></span>
2. <span data-ttu-id="a0da8-128">**Баға ұсыныстары** бетінде жобаның баға ұсынысын ашып, **Жиынтық** қойыншасында сұралған жеткізу күнін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-128">On the **Quotes** page, open the Project quote and on the **Summary** tab, set a requested delivery date.</span></span>
3. <span data-ttu-id="a0da8-129">Белгіленген уақыт кестесін жасау қажет белгіленген баға ұсыну жолын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-129">Open the fixed price quote line that you need to create a milestone schedule for.</span></span> 
4. <span data-ttu-id="a0da8-130">**Шот-фактуралар кестесі** қойыншасында **Шот ұсыну басталу күні** және **Шот ұсыну жиілігі** өрістерінде мәндерді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-130">On the **Invoice Schedule** tab, select values in the **Billing start** and **Invoice Frequency** fields.</span></span> 
5. <span data-ttu-id="a0da8-131">Ішкі тордан **Мерзімді бақылау нүктелері** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-131">On the sub-grid, select **Generate Periodic Milestones**.</span></span>
6. <span data-ttu-id="a0da8-132">Бағдарлама бақылау нүктесінің атауын, күнін және сомасын көрсете отырып, шот-фактуралардың кестесін жасайды.</span><span class="sxs-lookup"><span data-stu-id="a0da8-132">The application generates the invoice schedule with a milestone name, date, and amount.</span></span>

    - <span data-ttu-id="a0da8-133">Негізгі кезең атауы шот-фактураның жиілігі негізінде жазылатын күнге қойылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-133">The milestone name is set to the date that is dictated based on the invoice frequency.</span></span>
    - <span data-ttu-id="a0da8-134">Негізгі кезең күні шот-фактураның жиілігі негізінде жазылатын күнге қойылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-134">The milestone date is set to the date that is dictated based on the invoice frequency.</span></span>
    - <span data-ttu-id="a0da8-135">Бақылау кезеңінің сомасы жоба негізінде ұсыныс жолындағы баға ұсыну сомасын шоттарды беру және сұралатын жеткізілімнің басталу жиілігі мен күндерімен айқындалатын бақылау кезеңдерінің санына бөлу жолымен есептеледі.</span><span class="sxs-lookup"><span data-stu-id="a0da8-135">The milestone amount is computed by dividing the quote amount on the project-based quote line by the number of milestones as dictated by the frequency and billing start and requested delivery dates.</span></span>
    - <span data-ttu-id="a0da8-136">Егер баға ұсыну жолында салықтың есептелген сомасы болса, онда бұл мән мерзімді кезеңдерді құру кезінде әр кезең арасында бірдей бөлінеді.</span><span class="sxs-lookup"><span data-stu-id="a0da8-136">If the Quote line also has as estimated tax amount, this value is split between each milestone equally when generating periodic milestones.</span></span>

### <a name="manually-create-milestones"></a><span data-ttu-id="a0da8-137">Кезеңдерді қолмен жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-137">Manually create milestones</span></span>

<span data-ttu-id="a0da8-138">Белгіленген бағаның кезеңдері олар мезгілді түрде бөлінбесе, қолмен жасалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="a0da8-138">Fixed price milestones can also be generated manually when they are not periodically split.</span></span> <span data-ttu-id="a0da8-139">Кезеңдерді қолмен жасау үшін:</span><span class="sxs-lookup"><span data-stu-id="a0da8-139">To create a milestone manually:</span></span>

<span data-ttu-id="a0da8-140">Кезең жасау қажет белгіленген баға ұсыну жолын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-140">Open the Fixed price quote line where you need to create a milestone.</span></span> <span data-ttu-id="a0da8-141">**Шот-фактура кестесі** қойыншасындағы ішкі торда **+ Жаңа баға ұсыну жолы кезеңін жасау** опциясын таңдап, келесі кестеге негізделген қажетті ақпаратты енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-141">On the **Invoice Schedule** tab, on the sub-grid, select **+ Create new quote line milestone** and enter the required information based on the following table.</span></span>

| <span data-ttu-id="a0da8-142">**Өріс**</span><span class="sxs-lookup"><span data-stu-id="a0da8-142">**Field**</span></span> | <span data-ttu-id="a0da8-143">**Орны**</span><span class="sxs-lookup"><span data-stu-id="a0da8-143">**Location**</span></span> | <span data-ttu-id="a0da8-144">**Маңыздылық, мақсаты және нұсқаулығы**</span><span class="sxs-lookup"><span data-stu-id="a0da8-144">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="a0da8-145">**Төменгі әсер**</span><span class="sxs-lookup"><span data-stu-id="a0da8-145">**Downstream impact**</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="a0da8-146">Аралық кезеңнің атауы</span><span class="sxs-lookup"><span data-stu-id="a0da8-146">Milestone name</span></span> | <span data-ttu-id="a0da8-147">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-147">Quick create</span></span> | <span data-ttu-id="a0da8-148">Кезең атауы.</span><span class="sxs-lookup"><span data-stu-id="a0da8-148">The name of the milestone.</span></span> | <span data-ttu-id="a0da8-149">Бұл жоба келісімшартының маңызды кезеңіне және шот-фактураға таратылады</span><span class="sxs-lookup"><span data-stu-id="a0da8-149">This is propagated to the project contract line milestone and to the invoice</span></span> |
| <span data-ttu-id="a0da8-150">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="a0da8-150">Project Task</span></span> | <span data-ttu-id="a0da8-151">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-151">Quick create</span></span> | <span data-ttu-id="a0da8-152">Егер межелік жоба тапсырмасымен байланысты болса, сіз осы сілтемені тапсырма күйіне негізделген межелік мәртебені орнататын теңшелетін логика қосу үшін пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-152">If the milestone is tied to project task, you can use this reference to add custom logic set the milestone status based on the task status.</span></span> | <span data-ttu-id="a0da8-153">Бағдарлама тапсырмаға сілтеме жасау кезінде ешқандай әсер етпейді.</span><span class="sxs-lookup"><span data-stu-id="a0da8-153">The application, does not have any downstream impact of this reference to a task.</span></span> |
| <span data-ttu-id="a0da8-154">Аралық кезеңнің күні</span><span class="sxs-lookup"><span data-stu-id="a0da8-154">Milestone date</span></span> | <span data-ttu-id="a0da8-155">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-155">Quick create</span></span> | <span data-ttu-id="a0da8-156">Шот-фактураны автоматты түрде жасау процесі осы кезеңнің мәртебесін іздеуі керек болатын күнді белгілеңіз, оны шот-фактура үшін қарастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="a0da8-156">Set the date on which the automatic invoice creation process should look for the status of this milestone to consider it for invoicing.</span></span> | <span data-ttu-id="a0da8-157">Бұл жоба келісімшартының маңызды кезеңіне және шот-фактураға таратылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-157">This is propagated to the project contract line milestone and to the invoice.</span></span> |
| <span data-ttu-id="a0da8-158">Есеп-шот күйі</span><span class="sxs-lookup"><span data-stu-id="a0da8-158">Invoice status</span></span> | <span data-ttu-id="a0da8-159">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-159">Quick create</span></span> | <span data-ttu-id="a0da8-160">Кезең жасалған кезде бұл күй әрдайым **Шот-фактура ұсынуға дайын емес** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-160">When a milestone is created, this status is always set to **Not ready for invoicing**.</span></span> | <span data-ttu-id="a0da8-161">Бұл жоба келісімшартының маңызды кезеңіне және шот-фактураға таратылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-161">This is propagated to the project contract line milestone and to the invoice.</span></span> |
| <span data-ttu-id="a0da8-162">Жол сомасы</span><span class="sxs-lookup"><span data-stu-id="a0da8-162">Line Amount</span></span> | <span data-ttu-id="a0da8-163">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-163">Quick create</span></span> | <span data-ttu-id="a0da8-164">Тұтынушыға есепшот ұсынылатын кезеңнің мөлшері немесе мәні.</span><span class="sxs-lookup"><span data-stu-id="a0da8-164">Amount or value of the milestone that will be invoiced to the customer.</span></span> | <span data-ttu-id="a0da8-165">Бұл жоба келісімшартының маңызды кезеңіне және шот-фактураға таратылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-165">This is propagated to the project contract line milestone and to the invoice.</span></span> |
| <span data-ttu-id="a0da8-166">Салық</span><span class="sxs-lookup"><span data-stu-id="a0da8-166">Tax</span></span> | <span data-ttu-id="a0da8-167">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="a0da8-167">Quick create</span></span> | <span data-ttu-id="a0da8-168">Кезеңге қолданылатын салық сомасы.</span><span class="sxs-lookup"><span data-stu-id="a0da8-168">Tax amount that will be applied to the milestone.</span></span> | <span data-ttu-id="a0da8-169">Бұл жоба келісімшартының маңызды кезеңіне және шот-фактураға таратылады.</span><span class="sxs-lookup"><span data-stu-id="a0da8-169">This is propagated to the project contract line milestone and to the invoice.</span></span> |