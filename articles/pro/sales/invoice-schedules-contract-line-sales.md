---
title: Жобаға негізделген келісім-шарт жолы бойынша есеп-шот кестелерін жасау
description: Бұл тақырыпта есеп-шот кестесін құру және келісім-шарт жолдары үшін кезеңдер туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/17/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2183b915dd2f67e03964246cb0689003e48363f7
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/20/2020
ms.locfileid: "4079894"
---
# <a name="creating-invoice-schedules-on-a-project-based-contract-line"></a><span data-ttu-id="c976f-103">Жобаға негізделген келісім-шарт жолы бойынша есеп-шот кестелерін жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-103">Creating invoice schedules on a project-based contract line</span></span>

<span data-ttu-id="c976f-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="c976f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c976f-105">Жобаға негізделген келісім-шарт жолына есеп-шот кестесін ұсына аласыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-105">You can an invoice schedule to a  project-based contract line.</span></span> <span data-ttu-id="c976f-106">Есеп-шот ұсыну келісім-шарт жасалып, жоба келісім-шартын жасағаннан кейін ғана жүзеге асырылады.</span><span class="sxs-lookup"><span data-stu-id="c976f-106">Invoicing is only allowed after the contract is won to and you are creating a project contract.</span></span> <span data-ttu-id="c976f-107">Есеп-шот кестесі жобаға негізделген келісім-шарт жолы үшін жоба есеп-шоттардың автоматты түрде жасалуына мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="c976f-107">An invoice schedule allows draft invoices for a project-based contract line to be automatically created.</span></span> <span data-ttu-id="c976f-108">Егер есеп-шоттарды тек қолмен жасасаңыз, келісім-шарттар жолдарындағы есеп-шот кестелерін құруды өткізіп жібере аласыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-108">If however, you only manually create invoices, you can skip creating invoice schedules on contract lines.</span></span>

## <a name="create-a-time-and-material-invoice-schedule-for-a-contract-line"></a><span data-ttu-id="c976f-109">Келісім-шарт жолы үшін уақыт пен материал бойынша есеп-шот кестесін жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-109">Create a time and material invoice schedule for a contract line</span></span>

<span data-ttu-id="c976f-110">Жобаға негізделген келісім-шарт жолында уақыт және материалдық шот ұсыну әдісі болғанда, күні бойынша есеп-шот кестесін жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="c976f-110">When a project-based contract line has a time and material billing method, you can create a date-based invoice schedule.</span></span> <span data-ttu-id="c976f-111">Шот-фактура кестесін автоматты түрде жасау үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-111">To automatically generate a date-based invoice schedule, complete the following steps.</span></span>

1. <span data-ttu-id="c976f-112">**Параметрлер** > **Есеп-шот ұсыну жиіліктері** тармағына өтіп, есеп-шот ұсыну жиілігін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-112">Go to **Settings** > **Invoice frequencies** and set up an invoice frequence.</span></span>
2. <span data-ttu-id="c976f-113">Жоба келісім-шарт жазбасына өтіп, **Сұралған жеткізу күні** өрісіндегі **Қысқаша мазмұны** қойыншасында күнді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-113">Go to the project contract record, and on the **Summary** tab, in the **Requested Delivery Date** field, select a date.</span></span>
3. <span data-ttu-id="c976f-114">Күні бойынша есеп-шот кестесін жасайтын **Уақыт пен материал** келісім-шарт жолын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-114">Open the **Time and Material** contract line that you are making the date-based invoice schedule for.</span></span> 
4. <span data-ttu-id="c976f-115">**Есеп-шот кестесі** қойыншасында шот ұсынудың басталу күні мен есеп-шот ұсыну жиілігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-115">On the **Invoice Schedule** tab, select the billing start date and the invoice frequency.</span></span>
5. <span data-ttu-id="c976f-116">Ішкі тордан **Шот-фактура кестесін құру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-116">On the subgrid, select **Generate Invoice Schedule**.</span></span> <span data-ttu-id="c976f-117">**Есеп-шоттың орындалу күні** , **Транзакция мерзімі соңы** және **Орындау күйі** өрістері келесідей орнатылған есеп-шот кестесі жасалады:</span><span class="sxs-lookup"><span data-stu-id="c976f-117">The invoice schedule is generated with the **Invoice Run Date** , **Transaction Cutoff Date** and **Run Status** fields set as follows:</span></span>

    - <span data-ttu-id="c976f-118">**Есеп-шоттың орындалу күні** : бұл күн есеп-шот жиілігі негізінде жазылады.</span><span class="sxs-lookup"><span data-stu-id="c976f-118">**Invoice Run Date** : This date is dictated by the invoice frequency.</span></span>
    - <span data-ttu-id="c976f-119">**Транзакцияны тоқтату күні** : бұл есеп-шотты орындау күнінен бір күн бұрынғы күн.</span><span class="sxs-lookup"><span data-stu-id="c976f-119">**Transaction Cutoff Date** : The day before the invoice run date.</span></span>
    - <span data-ttu-id="c976f-120">**Орындалу күйі** : автоматты түрде **Орындалмаған** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="c976f-120">**Run Status** : Automatically set to **Not Run**.</span></span> <span data-ttu-id="c976f-121">Нақты шот ұсыну күні үшін автоматты есеп-шот жасау жұмысы орындалғанда ол осы өрісті **Сәтті түрде орындау** немесе **Орындау сәтсіз аяқталды** күйлеріне жаңартады.</span><span class="sxs-lookup"><span data-stu-id="c976f-121">When the automatic invoice creation job runs for a certain invoice run date, this field is updated to **Run Successful** or **Run Failed**.</span></span>


## <a name="create-a-fixed-price-invoice-schedule-for-a-contract-line"></a><span data-ttu-id="c976f-122">Келісім-шарт жолы үшін бекітілген баға бойынша есеп-шот кестесін жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-122">Create a fixed price invoice schedule for a contract line</span></span>

<span data-ttu-id="c976f-123">Келісім-шарт жолында бекітілген шот ұсыну әдісі болғанда, кезеңдер негізінде есеп-шот кестесін жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="c976f-123">When the contract line has a fixed billing method, you can create a milestone-based invoice schedule.</span></span> <span data-ttu-id="c976f-124">Күнтізбелік кезеңге біркелкі бөлінген кезеңдердің белгіленген жиынтығына арналған кезеңге негізделген есеп-шот кестесін жасау үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-124">Complete the following steps to generate a milestone-based invoice schedule for a fixed set of equally distributed milestones for the calendar period.</span></span>

1. <span data-ttu-id="c976f-125">**Параметрлер** > **Есеп-шот ұсыну жиіліктері** тармағына өтіп, есеп-шот ұсыну жиілігін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-125">Go to **Settings** > **Invoice frequencies** and set up an invoice frequence.</span></span>
2. <span data-ttu-id="c976f-126">Жоба келісім-шарт жазбасына өтіп, **Сұралған жеткізу күні** өрісіндегі **Қысқаша мазмұны** қойыншасында күнді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-126">Go to the project contract record, and on the **Summary** tab, in the **Requested Delivery Date** field, select a date.</span></span>
3. <span data-ttu-id="c976f-127">Кезең кестесін жасайтын **Белгіленген баға** келісім-шарт жолын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-127">Open the **Fixed Price** contract line that you are creating the milestone schedule for.</span></span> <span data-ttu-id="c976f-128">**Шот ұсыну кезеңдері** қойыншасында шот ұсынудың басталу күні мен есеп-шот ұсыну жиілігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-128">On the **Billing Milestones** tab, select the billing start date and the invoice frequency.</span></span> 
4. <span data-ttu-id="c976f-129">Ішкі тордан **Мерзімді бақылау нүктелері** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-129">On the subgrid, select **Generate Periodic Milestones**.</span></span> <span data-ttu-id="c976f-130">Есеп-шот кестесі **Кезең атауы** , **Кезең күні** және **Кезең сомасы** өрістері келесідей орнатылғанда жасалады:</span><span class="sxs-lookup"><span data-stu-id="c976f-130">The  invoice schedule is generated with the **Milestone Name** , **Milestone Date** , and **Milestone Amount** fields set as follows:</span></span>

    - <span data-ttu-id="c976f-131">**Кезең атауы** : бұл күн есеп-шот жиілігі негізінде жазылады.</span><span class="sxs-lookup"><span data-stu-id="c976f-131">**Milestone Name** : This date is dictated by the invoice frequency.</span></span>
    - <span data-ttu-id="c976f-132">**Кезең күні** : бұл күн есеп-шот жиілігі негізінде жазылады.</span><span class="sxs-lookup"><span data-stu-id="c976f-132">**Milestone Date** : This date is dictated by the invoice frequency.</span></span>
    - <span data-ttu-id="c976f-133">**Кезең сомасы** : келісім-шарт жолындағы келісім-шарт сомасын шоттарды беру және сұралатын жеткізілімнің басталу жиілігі мен күндерімен айқындалатын бақылау кезеңдерінің санына бөлу жолымен есептеледі.</span><span class="sxs-lookup"><span data-stu-id="c976f-133">**Milestone Amount** : This amount is calculated by dividing the contract amount on the contract line by the number of milestones as dictated by the frequency, billing start, and requested delivery dates.</span></span>

    <span data-ttu-id="c976f-134">Егер келісім-шарт жолының **Болжалды салық сомасы** өрісінде мәні болса, онда бұл өріс мерзімді кезеңдерді құрған кезде әр кезеңге бірдей бөлінеді.</span><span class="sxs-lookup"><span data-stu-id="c976f-134">If the contract line has a value in the **Estimated Tax amount** field, then this field is also apportioned to each milestone equally when generating periodic milestones.</span></span>

<span data-ttu-id="c976f-135">Шот ұсыну кезеңдері келісім-шарт жолының келісілген мәніне тең болуы керек.</span><span class="sxs-lookup"><span data-stu-id="c976f-135">Billing milestones should equal the contracted value of the contract line.</span></span> <span data-ttu-id="c976f-136">Олай болмаса, **Келісім-шарт жолы** бетінде қате туралы хабар аласыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-136">If they don't, you will receive an  error on the **Contract Line** page.</span></span> <span data-ttu-id="c976f-137">Шот ұсыну кезеңдері жолдың келісілген жалпы мәнін кезеңдерді құру, өңдеу немесе өшіру арқылы тексеріп, қатені түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="c976f-137">You can fix the error by verifying that the billing milestones total the contracted value of the line by creating, editing, or deleting milestones.</span></span> <span data-ttu-id="c976f-138">Өзгерістер енгізілгеннен кейін қатені жою үшін бетті жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-138">After the changes are made, refresh the page to remove the error.</span></span>

### <a name="manually-create-milestones"></a><span data-ttu-id="c976f-139">Кезеңдерді қолмен жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-139">Manually create milestones</span></span>

<span data-ttu-id="c976f-140">Белгіленген бағаның кезеңдерін олар мезгілді түрде бөлінбесе, қолмен жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="c976f-140">You can generate fixed price milestones manually when they are not periodically split.</span></span> <span data-ttu-id="c976f-141">Кезең қолмен жасау үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-141">Complete the following steps to manually create a milestone.</span></span>

1. <span data-ttu-id="c976f-142">Кезең жасайтын бағасы белгіленген келісім-шарт жолын ашыңыз және ішкі тордағы **Есеп-шот кестесі** қойыншасында **+ келісім-шарт жолының жаңа кезеңін жасау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-142">Open the fixed price contract line that you are creating a milestone for, and on the **Invoice Schedule** tab, on the subgrid, select **+ Create new Contract line milestone**.</span></span> 
2. <span data-ttu-id="c976f-143">**Кезеңді құру** бетінде, келесі кесте негізінде қажетті ақпаратты енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="c976f-143">On the **Milestone Creation** page, enter the required information based on the following table.</span></span>

| <span data-ttu-id="c976f-144">Өріс</span><span class="sxs-lookup"><span data-stu-id="c976f-144">Field</span></span> | <span data-ttu-id="c976f-145">Орналасқан жері</span><span class="sxs-lookup"><span data-stu-id="c976f-145">Location</span></span> | <span data-ttu-id="c976f-146">Маңыздылық, мақсаты және нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="c976f-146">Relevance, purpose, and guidance</span></span> | <span data-ttu-id="c976f-147">Төменгі әсер</span><span class="sxs-lookup"><span data-stu-id="c976f-147">Downstream impact</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="c976f-148">Аралық кезеңнің атауы</span><span class="sxs-lookup"><span data-stu-id="c976f-148">Milestone Name</span></span> | <span data-ttu-id="c976f-149">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-149">Quick Create</span></span> | <span data-ttu-id="c976f-150">Кезеңнің атына арналған мәтін өрісі.</span><span class="sxs-lookup"><span data-stu-id="c976f-150">Text field for the name of the milestone.</span></span> | <span data-ttu-id="c976f-151">Бұл жоба келісім-шарты жолының кезеңіне және есеп-шотқа жасалады.</span><span class="sxs-lookup"><span data-stu-id="c976f-151">This is carried over to the project contract line milestone and the invoice.</span></span> |
| <span data-ttu-id="c976f-152">Жоба тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="c976f-152">Project Task</span></span> | <span data-ttu-id="c976f-153">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-153">Quick Create</span></span> | <span data-ttu-id="c976f-154">Егер межелік жоба тапсырмасымен байланысты болса, сіз осы сілтемені тапсырма күйіне негізделген межелік мәртебені орнататын теңшелетін логика қосу үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-154">If the milestone is tied to project task, use this reference to add custom logic to set the milestone status based on the task status.</span></span> | <span data-ttu-id="c976f-155">Бағдарлама тапсырмаға сілтеме жасау кезінде ешқандай әсер етпейді.</span><span class="sxs-lookup"><span data-stu-id="c976f-155">The application, doesn't have any downstream impact of this reference to a task.</span></span> |
| <span data-ttu-id="c976f-156">Аралық кезеңнің күні</span><span class="sxs-lookup"><span data-stu-id="c976f-156">Milestone Date</span></span> | <span data-ttu-id="c976f-157">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-157">Quick Create</span></span> | <span data-ttu-id="c976f-158">Шот-фактураны автоматты түрде жасау процесі осы кезеңнің мәртебесін іздеуі керек болатын күнді белгілеңіз, оны шот-фактура үшін қарастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-158">Set the date on which the automatic invoice creation process should look for the status of this milestone to consider it for invoicing.</span></span> | <span data-ttu-id="c976f-159">Бұл жоба келісім-шарты жолының кезеңіне және есеп-шотқа жасалады.</span><span class="sxs-lookup"><span data-stu-id="c976f-159">This is carried over to the project contract line milestone and the invoice.</span></span> |
| <span data-ttu-id="c976f-160">Есеп-шот күйі</span><span class="sxs-lookup"><span data-stu-id="c976f-160">Invoice Status</span></span> | <span data-ttu-id="c976f-161">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-161">Quick Create</span></span> | <span data-ttu-id="c976f-162">Кезең жасалған кезде бұл күй әрдайым **Шот-фактура ұсынуға дайын емес** немесе **Басталмаған** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="c976f-162">When a milestone is created, this status is always set to **Not Ready for Invoicing** or **Not Started**.</span></span> | <span data-ttu-id="c976f-163">Бұл жоба келісім-шарты жолының кезеңіне және есеп-шотқа жасалады.</span><span class="sxs-lookup"><span data-stu-id="c976f-163">This is carried over to the project contract line milestone and the invoice.</span></span> |
| <span data-ttu-id="c976f-164">Жол сомасы</span><span class="sxs-lookup"><span data-stu-id="c976f-164">Line Amount</span></span> | <span data-ttu-id="c976f-165">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-165">Quick Create</span></span> | <span data-ttu-id="c976f-166">Тұтынушыға есепшот ұсынылатын кезеңнің мөлшері немесе мәні.</span><span class="sxs-lookup"><span data-stu-id="c976f-166">Amount or value of the milestone that will be invoiced to the customer.</span></span> | <span data-ttu-id="c976f-167">Бұл жоба келісім-шарты жолының кезеңіне және есеп-шотқа жасалады.</span><span class="sxs-lookup"><span data-stu-id="c976f-167">This is carried over to the project contract line milestone and the invoice.</span></span> |
| <span data-ttu-id="c976f-168">Салық</span><span class="sxs-lookup"><span data-stu-id="c976f-168">Tax</span></span> | <span data-ttu-id="c976f-169">Жылдам жасау</span><span class="sxs-lookup"><span data-stu-id="c976f-169">Quick Create</span></span> | <span data-ttu-id="c976f-170">Кезеңде қолданылатын салық сомасы.</span><span class="sxs-lookup"><span data-stu-id="c976f-170">The tax amount applied on the milestone.</span></span> | <span data-ttu-id="c976f-171">Бұл жоба келісім-шарты жолының кезеңіне және есеп-шотқа жасалады.</span><span class="sxs-lookup"><span data-stu-id="c976f-171">This is carried over to the project contract line milestone and the invoice.</span></span> |

3. <span data-ttu-id="c976f-172">**Сақтап жабу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c976f-172">Select **Save and Close**.</span></span>
<span data-ttu-id="c976f-173">| Жол сомасы | Жылдам жасау | Тұтынушыға есеп-шот ұсынылатын кезеңнің сомасы немесе мәні | Бұл жоба келісім-шарты жолының кезеңіне және есеп-шотқа таратылады | | Салық | Жылдам жасау | Мерзімінде қолданылатын салық сомасы | Бұл жоба келісім-шарты жолының кезеңіне және есеп-шотқа таратылады |</span><span class="sxs-lookup"><span data-stu-id="c976f-173">| Line Amount | Quick create | Amount or Value of the Milestone that will be invoiced to the customer | This is propagated to the Project contract line Milestone and to the Invoice | | Tax | Quick create | Tax amount that will be applied on the Milestone | This is propagated to the Project contract line Milestone and to the Invoice |</span></span>