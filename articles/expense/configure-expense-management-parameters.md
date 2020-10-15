---
title: Шығысты басқару параметрлерін конфигурациялау
description: Бұл тақырып шығыстарды басқарудағы жалпы тәртіпті басқаратын параметрлерді сипаттайды.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 8ecbd0abc16d0a29eea47d6bd1653a204a83de4c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897278"
---
# <a name="configure-expense-management-parameters"></a><span data-ttu-id="29118-103">Шығысты басқару параметрлерін конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="29118-103">Configure Expense management parameters</span></span>

<span data-ttu-id="29118-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="29118-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="29118-105">Бұл тақырып шығыстарды басқарудағы жалпы тәртіпті басқаратын параметрлерді сипаттайды.</span><span class="sxs-lookup"><span data-stu-id="29118-105">This topic describes the parameters the control the general behavior in Expense management.</span></span>

## <a name="general"></a><span data-ttu-id="29118-106">Жалпы мәліметтер </span><span class="sxs-lookup"><span data-stu-id="29118-106">General</span></span>

| <span data-ttu-id="29118-107">Өріс</span><span class="sxs-lookup"><span data-stu-id="29118-107">Field</span></span>                                                    | <span data-ttu-id="29118-108">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="29118-108">Description</span></span> |
|----------------------------------------------------------|-------------|
| <span data-ttu-id="29118-109">Жүрістің стандартты жылдамдығы</span><span class="sxs-lookup"><span data-stu-id="29118-109">Standard rate of mileage</span></span>                                 | <span data-ttu-id="29118-110">Жүріс шығыстарын өтеу мөлшерлемесін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-110">Enter the reimbursement rate for mileage expenses.</span></span> <span data-ttu-id="29118-111">Бұл мөлшерлеме жол шығындары үшін өтелетін соманы есептеу үшін шығыстарға енгізілген жүріске көбейтіледі.</span><span class="sxs-lookup"><span data-stu-id="29118-111">This rate is multiplied by the mileage that is entered for the expense to calculate the amount that is reimbursed for the travel expense.</span></span> |
| <span data-ttu-id="29118-112">Шығыс мақсатын растау</span><span class="sxs-lookup"><span data-stu-id="29118-112">Validate expense purpose</span></span>                                 | <span data-ttu-id="29118-113">Бұл параметрді пайдаланушылар шығыс есептерін жасағанда оларды **Шығыс есебінің мақсаты** өрісінде конфигурацияланған мәндер жиынына шектеу үшін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-113">Turn on this option to limit users to an existing set of values that is configured in the **Purpose of expense report** field when they create expense reports.</span></span> |
| <span data-ttu-id="29118-114">Жеке шығыстарды төлеуші</span><span class="sxs-lookup"><span data-stu-id="29118-114">Personal expenses paid by</span></span>                                | <span data-ttu-id="29118-115">Жеке тұлғалар санатына жатқызылған несиелік карта бойынша кез келген транзакция сомаларын төлеуге кім жауапты екенін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-115">Select who is responsible for paying any credit card transaction amounts that are categorized as personal.</span></span> |
| <span data-ttu-id="29118-116">Барлық шығындар туралы есепті көрсету</span><span class="sxs-lookup"><span data-stu-id="29118-116">Display entire expense report on drillback</span></span>               | <span data-ttu-id="29118-117">Шығындар туралы есеп орналастырылған кезде пайда болған белгілі бір ваучер үшін бастапқы құжаттың егжей-тегжейлері қаралған кезде шығыстар туралы есеп бойынша барлық шығындарды көрсету үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-117">Select this option to show all expenses for an expense report when the details of the original document are viewed for a specific voucher that was generated when the expense report was posted.</span></span> |
| <span data-ttu-id="29118-118">Сапарды алдын ала авторизациялау міндетті болып табылады</span><span class="sxs-lookup"><span data-stu-id="29118-118">Pre-authorization of travel is mandatory</span></span>                 | <span data-ttu-id="29118-119">Қызметкер шығыстар туралы есеп бергенге дейін сапарға өтініш беруді және бекітуді талап ету үшін осы параметрді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-119">Select this option to require that a travel requisition be submitted and approved before an employee can submit an expense report.</span></span> |
| <span data-ttu-id="29118-120">Орналастыруға дейін таратылымдарды өңдеуге рұқсат ету</span><span class="sxs-lookup"><span data-stu-id="29118-120">Allow editing of distributions before posting</span></span>            | <span data-ttu-id="29118-121">Шығыстар туралы есепті орналастырудан бұрын оны өңдеуге болатындығын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-121">Select whether the distributions of an expense report can be edited before it's posted.</span></span> |
| <span data-ttu-id="29118-122">Шығыстарды басқару саясатын бағалаңыз</span><span class="sxs-lookup"><span data-stu-id="29118-122">Evaluate expense management policies</span></span>                     | <span data-ttu-id="29118-123">Шығыс саясаты бұзылғанын анықтау үшін шығыстар қашан бағаланатынын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-123">Select when expenses are evaluated to determine whether an expense policy has been violated.</span></span> <span data-ttu-id="29118-124">Шығыстарды енгізу және сақтау кезінде немесе шығыстарды бекітуге ұсыну кезінде шығындарды бұзушылықтар бойынша бағалауға болады.</span><span class="sxs-lookup"><span data-stu-id="29118-124">Expenses can be evaluated for violations when the expense entry is entered and saved, or when the expense is submitted for approval.</span></span> <span data-ttu-id="29118-125">Қажетті түсімдерге қатысты саясат ережелері шығыстар үнемделген кезде бағаланады.</span><span class="sxs-lookup"><span data-stu-id="29118-125">The policy rules for receipts that are required will be evaluated when the expense line is saved.</span></span> |
| <span data-ttu-id="29118-126">Компанияаралық шығыстар желісіне рұқсат етіңіз</span><span class="sxs-lookup"><span data-stu-id="29118-126">Allow intercompany expense lines</span></span>                         | <span data-ttu-id="29118-127">Басқа заңды тұлғалар үшін шығыстарды шығыстар туралы есепке енгізуге болатындығын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-127">Select whether expenses for other legal entities can be entered on an expense report.</span></span> |
| <span data-ttu-id="29118-128">Несиелік карта бойынша шығындардың айырбас бағамын өзгертуге рұқсат етіңіз</span><span class="sxs-lookup"><span data-stu-id="29118-128">Allow editing the exchange rate for credit card expenses</span></span> | <span data-ttu-id="29118-129">Пайдаланушыға импортталған несиелік картаға арналған айырбас бағамын түзетуге мүмкіндік беру үшін осы параметрді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-129">Select this option to allow the user to edit the exchange rate for imported credit card expenses.</span></span> |
| <span data-ttu-id="29118-130">Көрсетілетін көп деңгейлі иерархия өрістері</span><span class="sxs-lookup"><span data-stu-id="29118-130">Multi-level hierarchy fields to display</span></span>                  | <span data-ttu-id="29118-131">Жұмыс ағынының тағайындау түрі иерархия ретінде орнатылғанда және **Иерархия** таңдау мақұлдау иерархиясын, шығындардың көп деңгейлі мақұлдауын пайдалану үшін орнатылғанда қандай мақұлдаушы өрістер көрсетілетінін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-131">Select which approver fields are shown when the workflow assignment type is set to be a hierarchy, and the **Hierarchy** selection is set to use the approval hierarchy, expense multi-level approval.</span></span> <span data-ttu-id="29118-132">Көп деңгейлі мақұлдау иерархиясы жұмыс процесінде пайдаланылған кезде таңдалған өрістер шығыстар туралы есепте көрсетіледі және оларды өңдеуге болады.</span><span class="sxs-lookup"><span data-stu-id="29118-132">When the multi-level approval hierarchy is used for a workflow, the selected fields will be shown on the expense report and can be edited.</span></span> |
| <span data-ttu-id="29118-133">Қызметкердің несиелік картасы нөмірін енгізіңіз</span><span class="sxs-lookup"><span data-stu-id="29118-133">Enter employee credit card number</span></span>                        | <span data-ttu-id="29118-134">Қызметкердің **Несие карталары** бетіндегі **Карта идентификаторы** өрісінде 15 таңбалы немесе 16 таңбалы нөмірді енгізуге және сақтауға болатынын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-134">Select whether a 15-character or 16-character number can be entered and saved in the **Card ID** field on the **Credit cards** page for an employee.</span></span> |
| <span data-ttu-id="29118-135">Сапар туралы сұраныстың мақсатын растаңыз</span><span class="sxs-lookup"><span data-stu-id="29118-135">Validate travel requisition purpose</span></span>                      | <span data-ttu-id="29118-136">Бұл параметрді пайдаланушылар сапар сұраныстарын жасағанда оларды **Шығыс есебінің мақсаты** өрісінде конфигурацияланған мәндер жиынына шектеу үшін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-136">Turn on this option to limit users to an existing set of values that is configured in the **Purpose of expense report** field when they create travel requisitions.</span></span> |

## <a name="financial"></a><span data-ttu-id="29118-137">Қаржы қызметі</span><span class="sxs-lookup"><span data-stu-id="29118-137">Financial</span></span>

| <span data-ttu-id="29118-138">Өріс</span><span class="sxs-lookup"><span data-stu-id="29118-138">Field</span></span>                                                                                    | <span data-ttu-id="29118-139">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="29118-139">Description</span></span> |
|------------------------------------------------------------------------------------------|-------------|
| <span data-ttu-id="29118-140">Кітаптың күнделікті журнал атауы</span><span class="sxs-lookup"><span data-stu-id="29118-140">Ledger daily journal name</span></span>                                                                | <span data-ttu-id="29118-141">Шығыстар туралы есептер орналастырылған кітап журналының атауын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-141">Select the name of the ledger journal that approved expense reports are posted to.</span></span> |
| <span data-ttu-id="29118-142">Шығыстардан салықты қалпына келтіруге мүмкіндік беру</span><span class="sxs-lookup"><span data-stu-id="29118-142">Enable tax recovery from expenses</span></span>                                                        | <span data-ttu-id="29118-143">Сәйкес шығыстар үшін шығыстар салығын қалпына келтіруді қосу үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-143">Select this option to enable expense tax recovery for eligible expenses.</span></span> <span data-ttu-id="29118-144">Егер АҚШ сату салығы мен салық салу ережелері қосылса, бұл опцияны таңдау мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="29118-144">This option can't be selected if US sales tax and use tax rules are enabled.</span></span> |
| <span data-ttu-id="29118-145">Ақшалай аванстарды дереу жариялаңыз</span><span class="sxs-lookup"><span data-stu-id="29118-145">Post cash advances immediately</span></span>                                                           | <span data-ttu-id="29118-146">Төлеу және аудару процесі аяқталғаннан кейін бекітілген ақшалай авансты орналастыру үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-146">Select this option to post an approved cash advance when the Pay and transfer process is completed.</span></span> <span data-ttu-id="29118-147">Егер бұл опция таңдалмаса, төлеу және аудару процесі жарияланбаған жалпы журнал жасайды.</span><span class="sxs-lookup"><span data-stu-id="29118-147">If this option isn't selected, the Pay and transfer process generates an unposted general journal.</span></span> |
| <span data-ttu-id="29118-148">Орналастыру кезіндегі дұрыс есептік күн</span><span class="sxs-lookup"><span data-stu-id="29118-148">Correct accounting date during posting</span></span>                                                   | <span data-ttu-id="29118-149">Ағымдағы кезең тоқтатылған немесе жабық болса, шығыстар орналастырылған кезде есептік күнді жаңарту үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-149">Select this option to update the accounting date when expenses are posted, if the current period is on hold or closed.</span></span> <span data-ttu-id="29118-150">Есепке алу күні келесі ашық кезеңге қойылады.</span><span class="sxs-lookup"><span data-stu-id="29118-150">The accounting date will be set to the next open period.</span></span> |
| <span data-ttu-id="29118-151">Төлем әдісінде көрсетілген шығындарды есепке алу шоты негізінде транзакцияларды топтауға рұқсат ету</span><span class="sxs-lookup"><span data-stu-id="29118-151">Allow grouping of transactions based on offset account specified in payment method</span></span>       | <span data-ttu-id="29118-152">Шығындарды төлеу әдісінде көрсетілген өзара есепке алу шоты негізінде шығындар туралы есепке арналған шығындар туралы есептерді жинақтау үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-152">Select this option to summarize the expense transactions for an expense report, based on the offset account that is specified in the payment method for the expenses.</span></span> |
| <span data-ttu-id="29118-153">Салық қосылған</span><span class="sxs-lookup"><span data-stu-id="29118-153">Tax included</span></span>                                                                             | <span data-ttu-id="29118-154">Сату салығын әдепкі бойынша шығындар сомасына қосу үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-154">Select this option to include sales tax in the expense amount by default.</span></span> |
| <span data-ttu-id="29118-155">Сапар сұраныстарын жабу бойынша ауыртпалықтардан босату</span><span class="sxs-lookup"><span data-stu-id="29118-155">Release encumbrances on closing travel requisitions</span></span>                                      | <span data-ttu-id="29118-156">Бекітілген сапар сұранысы жабылған кезде ауыртпалықтағы қаражатты босату үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-156">Select this option to release encumbered funds when an approved travel requisition is closed.</span></span> |
| <span data-ttu-id="29118-157">Сапар сұранысына бюджеттік тіркелім мен жобаның бюджеті үшін бюджеттің асып кетуіне рұқсат ету</span><span class="sxs-lookup"><span data-stu-id="29118-157">Allow travel requisition submit on budget overrun for budget register and project budget</span></span> | <span data-ttu-id="29118-158">Бюджеттік тіркелімде белгіленген бюджеттен немесе жобаның рұқсат етілген бюджетінен асып кетсе де, қызметкерлерге сапар сұраныстарын бекітуге жіберуге мүмкіндік беру үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-158">Select this option to allow employees to submit travel requisitions for approval, even though they exceed either the allowed budget that is set in the budget register or the allowed budget for a project.</span></span> |
| <span data-ttu-id="29118-159">Шығыстар есебіне бюджеттік тіркелім мен жобаның бюджеті үшін бюджеттің асып кетуіне рұқсат ету</span><span class="sxs-lookup"><span data-stu-id="29118-159">Allow expense report submit on budget overrun for budget register and project budget</span></span>     | <span data-ttu-id="29118-160">Бюджеттік тіркелімде белгіленген бюджеттен немесе жобаның рұқсат етілген бюджетінен асып кетсе де, қызметкерлерге шығыстар есептерін бекітуге жіберуге мүмкіндік беру үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-160">Select this option to allow employees to submit expense reports for approval, even though they exceed either the allowed budget that is set in the budget register or the allowed budget for a project.</span></span> |
| <span data-ttu-id="29118-161">Шығыстар есебін бекітуді тек бюджеттік тіркелім үшін бюджеттің асып кетуіне рұқсат ету</span><span class="sxs-lookup"><span data-stu-id="29118-161">Allow expense report approval on budget overrun for budget register only</span></span>                 | <span data-ttu-id="29118-162">Бекітушілерге бюджеттік тізілімде белгіленген рұқсат етілген бюджеттен асатын шығындар туралы есептерді бекітуге мүмкіндік беру үшін осы параметрді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-162">Select this option to allow approvers to approve expense reports that exceed the allowed budget that is set in the budget register.</span></span> |

## <a name="per-diem"></a><span data-ttu-id="29118-163">Тәуліктік</span><span class="sxs-lookup"><span data-stu-id="29118-163">Per diem</span></span>

| <span data-ttu-id="29118-164">Өріс</span><span class="sxs-lookup"><span data-stu-id="29118-164">Field</span></span>                                 | <span data-ttu-id="29118-165">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="29118-165">Description</span></span> |
|---------------------------------------|-------------|
| <span data-ttu-id="29118-166">Бір тәуліктегі минималды сағат</span><span class="sxs-lookup"><span data-stu-id="29118-166">Minimum hours for per diem</span></span>            | <span data-ttu-id="29118-167">Қызметкер сапарға байланысты шығындар үшін тәуліктік ақы алу үшін бір күнде жұмыс істеуі керек болатын әдепкі ең аз сағат санын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-167">Enter the default minimum number of hours that an employee must work in a day to be eligible to receive a per diem for travel-related expenses.</span></span> <span data-ttu-id="29118-168">Бұл мән тәуліктік ставкалар деңгейіне арналған **Минималды сағаттар** өрісі үшін әдепкі мән ретінде пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="29118-168">This value is used as a default value only for the **Minimum hours** field for per diem rate tiers.</span></span> |
| <span data-ttu-id="29118-169">Тамақтану пайызы</span><span class="sxs-lookup"><span data-stu-id="29118-169">Meal percent</span></span>                          | <span data-ttu-id="29118-170">**Тамақтануды азайтуды есептеу** өрісі **Күнделікті тағам түрі** немесе **Күнделікті тамақтану саны** параметріне орнатылғанда, іссапар шығындарының бірінші және соңғы күндерінде пайдаланылатын тағам үшін әдепкі тәуліктік пайызды енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-170">Enter the default percentage of the per diem for meals that is used on the first and last days of the travel-related expense when the **Calculate meal reduction by** field is set to either **Meal type per day** or **Number of meals per day**.</span></span> <span data-ttu-id="29118-171">Бірінші және соңғы күндердегі жұмыс күні әдеттегі жұмыс күніне қарағанда қысқа болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-171">The workday on the first and last days might be shorter than a standard workday.</span></span> <span data-ttu-id="29118-172">Сондықтан сол күндері тәуліктік төлемнің мөлшері стандартты мөлшерден өзгеше болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-172">Therefore, the amount of the per diem on those days might differ from the standard amount.</span></span> <span data-ttu-id="29118-173">Егер пайыздық мәні **0** (нөл) мәніне орнатылған болса, алғашқы және соңғы күндердегі аударымдар 0,00 құрайды.</span><span class="sxs-lookup"><span data-stu-id="29118-173">If the percentage is set to **0** (zero), the deductions for the first and last days will be 0.00.</span></span> |
| <span data-ttu-id="29118-174">Қонақ үй пайызы</span><span class="sxs-lookup"><span data-stu-id="29118-174">Hotel percent</span></span>                         | <span data-ttu-id="29118-175">Іссапар шығындарының бірінші және соңғы күндерінде пайдаланылатын қонақүйлер үшін тәуліктік төлемнің әдепкі пайызын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-175">Enter the default percentage of the per diem for hotels that is used on the first and last days of the travel-related expense.</span></span> <span data-ttu-id="29118-176">Бірінші және соңғы күндердегі жұмыс күні әдеттегі жұмыс күніне қарағанда қысқа болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-176">The workday on the first and last days might be shorter than a standard workday.</span></span> <span data-ttu-id="29118-177">Сондықтан сол күндері тәуліктік төлемнің мөлшері стандартты мөлшерден өзгеше болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-177">Therefore, the amount of the per diem on those days might differ from the standard amount.</span></span> <span data-ttu-id="29118-178">Егер пайыздық мәні **0** (нөл) мәніне орнатылған болса, алғашқы және соңғы күндердегі аударымдар 0,00 құрайды.</span><span class="sxs-lookup"><span data-stu-id="29118-178">If the percentage is set to **0** (zero), the deductions for the first and last days will be 0.00.</span></span> |
| <span data-ttu-id="29118-179">Басқа пайыздар</span><span class="sxs-lookup"><span data-stu-id="29118-179">Other percent</span></span>                         | <span data-ttu-id="29118-180">Іссапар шығындарының бірінші және соңғы күндерінде пайдаланылатын әр түрлі шығындар үшін тәуліктік төлемнің әдепкі пайызын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-180">Enter the default percentage of the per diem for miscellaneous expenses that is used on the first and last days of the travel-related expense.</span></span> <span data-ttu-id="29118-181">Бірінші және соңғы күндердегі жұмыс күні әдеттегі жұмыс күніне қарағанда қысқа болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-181">The workday on the first and last days might be shorter than a standard workday.</span></span> <span data-ttu-id="29118-182">Сондықтан сол күндері тәуліктік төлемнің мөлшері стандартты мөлшерден өзгеше болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-182">Therefore, the amount of the per diem on those days might differ from the standard amount.</span></span> <span data-ttu-id="29118-183">Егер пайыздық мәні **0** (нөл) мәніне орнатылған болса, алғашқы және соңғы күндердегі аударымдар 0,00 құрайды.</span><span class="sxs-lookup"><span data-stu-id="29118-183">If the percentage is set to **0** (zero), the deductions for the first and last days will be 0.00.</span></span> |
| <span data-ttu-id="29118-184">Таңғы асқа пайызбен төмендету</span><span class="sxs-lookup"><span data-stu-id="29118-184">Reduction in percentage for breakfast</span></span> | <span data-ttu-id="29118-185">Таңертеңгілік тамақтану күніне азайтылатын соманы енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-185">Enter the amount that the per diem is reduced by for breakfast.</span></span> <span data-ttu-id="29118-186">Мысалы, егер қызметкер тегін таңғы ас алса, сіз тәуліктік төлем мөлшерін 10 пайызға азайтуды қалауыңыз мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-186">For example, if an employee receives a complimentary breakfast, you might want to reduce the amount of the per diem by 10 percent.</span></span> |
| <span data-ttu-id="29118-187">Түскі асқа пайызбен төмендету</span><span class="sxs-lookup"><span data-stu-id="29118-187">Reduction in percentage for lunch</span></span>     | <span data-ttu-id="29118-188">Түскі уақыттағы тамақтану күніне азайтылатын соманы енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-188">Enter the amount that the per diem is reduced by for lunch.</span></span> <span data-ttu-id="29118-189">Мысалы, егер қызметкер тегін түскі ас алса, сіз тәуліктік төлем мөлшерін 15 пайызға азайтуды қалауыңыз мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-189">For example, if an employee receives a complimentary lunch, you might want to reduce the amount of the per diem by 15 percent.</span></span> |
| <span data-ttu-id="29118-190">Кешкі асқа пайызбен төмендету</span><span class="sxs-lookup"><span data-stu-id="29118-190">Reduction in percentage for dinner</span></span>    | <span data-ttu-id="29118-191">Кешкі уақыттағы тамақтану күніне азайтылатын соманы енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-191">Enter the amount that the per diem is reduced by for dinner.</span></span> <span data-ttu-id="29118-192">Мысалы, егер қызметкер тегін кешкі ас алса, сіз тәуліктік төлем мөлшерін 25 пайызға азайтуды қалауыңыз мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-192">For example, if an employee receives a complimentary dinner, you might want to reduce the amount of the per diem by 25 percent.</span></span> |
| <span data-ttu-id="29118-193">Тамақты азайтуды есептеу</span><span class="sxs-lookup"><span data-stu-id="29118-193">Calculate meal reduction by</span></span>           | <span data-ttu-id="29118-194">Бұл азайту бір реттік сапар немесе бір күндік тамақтану түріне негізделгенін немесе ол күніне рұқсат етілген тамақтану санына негізделгенін таңдау арқылы жүйенің тәуліктік тамақтануды төмендетуді қалай есептеу керектігін көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-194">Specify how the system should calculate the per diem meal reduction, by selecting whether the reduction is based on the meal type per trip or per day, or whether it's based on the number of meals that is allowed per day.</span></span> |
| <span data-ttu-id="29118-195">Тәуліктік дөңгелектеу</span><span class="sxs-lookup"><span data-stu-id="29118-195">Per diem rounding</span></span>                     | <span data-ttu-id="29118-196">Тәуліктің шығындар үшін пайдаланылатын дөңгелектеу түрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-196">Select the type of rounding that is used for per diem expenses.</span></span> <span data-ttu-id="29118-197">Егер сіз қалыпты дөңгелектеуді таңдасаңыз, тәуліктік шығындар 0,50 болса, 1,00-ге дейін, ал күндізгі шығындар 0,50-ден аз болса, 0,00-ге дейін дөңгелектенеді.</span><span class="sxs-lookup"><span data-stu-id="29118-197">If you select normal rounding, any per diem expense that has an amount of 0.50 is rounded up to 1.00, and any per diem expense that has an amount that is less than 0.50 is rounded down to 0.00.</span></span> |
| <span data-ttu-id="29118-198">Тәуліктік есептеу негізі</span><span class="sxs-lookup"><span data-stu-id="29118-198">Base per diem calculation on</span></span>          | <span data-ttu-id="29118-199">Тәуліктік төлем күнтізбелік күнге немесе 24-сағаттық мерзімге негізделгендігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-199">Select whether a per diem amount is based on a calendar day or a 24-hour period.</span></span> |

## <a name="fax-cover-pages"></a><span data-ttu-id="29118-200">Факстың мұқаба беттері</span><span class="sxs-lookup"><span data-stu-id="29118-200">Fax cover pages</span></span>

| <span data-ttu-id="29118-201">Өріс</span><span class="sxs-lookup"><span data-stu-id="29118-201">Field</span></span>                          | <span data-ttu-id="29118-202">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="29118-202">Description</span></span> |
|--------------------------------|-------------|
| <span data-ttu-id="29118-203">Нұсқаулар</span><span class="sxs-lookup"><span data-stu-id="29118-203">Instructions</span></span>                   | <span data-ttu-id="29118-204">Қызметкерлер шығындар туралы есеппен байланысты түбіртектерді жіберу үшін пайдаланылатын факс үшін мұқаба бетін жасаған кезде орындауы керек нұсқауларды енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-204">Enter the instructions that employees must follow when they create a cover page for a fax that is used to send receipts that are related to an expense report.</span></span> <span data-ttu-id="29118-205">Көрсетілетін белгілі бір мәтінді қолданушы тіліне сүйене отырып енгізу үшін **Аудармалар** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-205">To enter language-specific text that will be shown, based on the user language, select **Translations**.</span></span> |
| <span data-ttu-id="29118-206">Пайдаланушының идентификаторы (штрих-код туралы ақпарат)</span><span class="sxs-lookup"><span data-stu-id="29118-206">User ID (Bar code information)</span></span> | <span data-ttu-id="29118-207">Қызметкердің бірегей идентификаторын факстың мұқаба бетінде пайдаланылатын штрих-кодта сақтау үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-207">Select this option to store an employee's unique identifier in the bar code that is used on the cover page of the fax.</span></span> |
| <span data-ttu-id="29118-208">Штрих-код</span><span class="sxs-lookup"><span data-stu-id="29118-208">Bar code</span></span>                       | <span data-ttu-id="29118-209">Факстың мұқаба бетінде пайдаланылатын штрих-кодты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-209">Select the bar code that is used on the cover page of the fax.</span></span> <span data-ttu-id="29118-210">39 және 128 штрих-кодтарына шығыстарды басқаруда қолдау көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="29118-210">Bar codes 39 and 128 are supported in Expense management.</span></span> |

## <a name="anti-corruption"></a><span data-ttu-id="29118-211">Сыбайлас жемқорлыққа қарсы іс-қимыл</span><span class="sxs-lookup"><span data-stu-id="29118-211">Anti-corruption</span></span>

| <span data-ttu-id="29118-212">Өріс</span><span class="sxs-lookup"><span data-stu-id="29118-212">Field</span></span>                                 | <span data-ttu-id="29118-213">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="29118-213">Description</span></span> |
|---------------------------------------|-------------|
| <span data-ttu-id="29118-214">Сыбайлас жемқорлыққа қарсы аттестаттауды көрсету</span><span class="sxs-lookup"><span data-stu-id="29118-214">Display anti-corruption attestation</span></span>   | <span data-ttu-id="29118-215">Шығындар туралы есеп жасалған кезде сыбайлас жемқорлыққа қарсы мәтінді көрсету үшін осы опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-215">Select this option to show the anti-corruption text when an expense report is created.</span></span> <span data-ttu-id="29118-216">Содан кейін шығындар туралы есепте сыбайлас жемқорлыққа қарсы аттестаттауды таңдауды талап ететін шығындардың нақты санаттарын қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="29118-216">Specific expense categories can then be enabled that will require that the anti-corruption attestation be selected on the expense report.</span></span> <span data-ttu-id="29118-217">Мысалы, үкіметтің ресми шығындарымен байланысты сыйлық категориясы қызметкерден шығындардың мемлекеттік қызметкерлерге қатысты компания саясатына сәйкес келетіндігін растауын талап етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29118-217">For example, a gift category that is related to a government official expense might require that the employee confirm that the expense meets company policy that is related to government officials.</span></span> |
| <span data-ttu-id="29118-218">Жіберушіге арналған сыбайлас жемқорлыққа қарсы хабарлама</span><span class="sxs-lookup"><span data-stu-id="29118-218">Anti-corruption message for submitter</span></span> | <span data-ttu-id="29118-219">Шығындар туралы есеп құратын қызметкерге көрсетілуі керек мәтінді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-219">Enter the text that should be shown to an employee who is creating an expense report.</span></span> <span data-ttu-id="29118-220">Көрсетілетін белгілі бір мәтінді қолданушы тіліне сүйене отырып енгізу үшін **Аудармалар** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-220">To enter language-specific text that will be shown, based on the user language, select **Translations**.</span></span> |
| <span data-ttu-id="29118-221">Бекітушіге арналған сыбайлас жемқорлыққа қарсы хабарлама</span><span class="sxs-lookup"><span data-stu-id="29118-221">Anti-corruption message for approver</span></span>  | <span data-ttu-id="29118-222">Шығыстар туралы есеп жасалғанда бекітушіге көрсетілетін мәтінді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="29118-222">Enter the text that should be shown to the approver when an expense report is created.</span></span> <span data-ttu-id="29118-223">Көрсетілетін белгілі бір мәтінді қолданушы тіліне сүйене отырып енгізу үшін **Аудармалар** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29118-223">To enter language-specific text that will be shown, based on the user language, select **Translations**.</span></span> |