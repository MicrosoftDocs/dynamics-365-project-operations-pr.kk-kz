---
title: Шығындарды басқаруды конфигурациялау
description: Бұл мақалада Microsoft Dynamics 365 Finance бағдарламасында шығындарды басқаруды конфигурацияламас бұрын жоспарлау процесі кезінде жасалатын жағдайлар мен шешімдер сипатталған.
author: KimANelson
manager: AnnBe
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 74a8435464c8573ca831b7886f00c2695fd29827
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271360"
---
# <a name="configure-expense-management"></a><span data-ttu-id="fd2be-103">Шығындарды басқаруды конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="fd2be-103">Configure expense management</span></span>

<span data-ttu-id="fd2be-104">Бұл тақырыпта шығындарды басқаруды конфигурацияламас бұрын жоспарлау процесі кезінде жасалатын жағдайлар мен шешімдер сипатталған.</span><span class="sxs-lookup"><span data-stu-id="fd2be-104">This topic describes the considerations and the decisions that you must make during the planning process before you configure Expense management.</span></span> <span data-ttu-id="fd2be-105">Шығындарды басқару жүйесінде сіз төлем әдістері, іссапар талаптары, шығындар туралы есептер, саясаттар және т.б. туралы ақпаратты сақтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-105">In Expense management, you can store information about payment methods, travel requisitions, expense reports, policies, and so on.</span></span>

<span data-ttu-id="fd2be-106">Шығындарды басқару конфигурациясын жоспарлау кезінде қабылданған көптеген шешімдер ұйымның иерархиясы мен қаржылық құрылымына негізделгендіктен, осы салалар бойынша жоспарлау құжаттарына жүгіну қажет.</span><span class="sxs-lookup"><span data-stu-id="fd2be-106">Because many of the decisions that you make when you plan your configuration for Expense management are based on your organization’s hierarchy and financial structure, you must refer to the planning documents for those areas.</span></span>

## <a name="intercompany-expenses"></a><span data-ttu-id="fd2be-107">Компанияаралық шығыстар</span><span class="sxs-lookup"><span data-stu-id="fd2be-107">Intercompany expenses</span></span>

<span data-ttu-id="fd2be-108">Компанияаралық шығындарды қосқанда, сіз заңды тұлғалар мен қызметкерлерге басқа заңды тұлғаның атынан шығындарды өтеуге және ұйымыңыздағы жалдау ақысын алуға рұқсат бересіз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-108">When you enable intercompany expenses, you allow legal entities and employees to incur expenses on behalf of another legal entity, and collect payment from the legal entity of employment within your organization.</span></span> <span data-ttu-id="fd2be-109">Мысалы, «А» заңды тұлғасының қызметкері «В» заңды тұлғасы үшін жобаны аяқтайды және бұл жоба іссапарларға байланысты шығындарды көтереді.</span><span class="sxs-lookup"><span data-stu-id="fd2be-109">For example, an employee in legal entity A completes a project for legal entity B, and the project incurs travel related expenses.</span></span> <span data-ttu-id="fd2be-110">Егер компанияаралық шығындар қосылса, қызметкер шығынды B заңды тұлғасына ауыстыратын шығындар туралы есеп бере алады, содан кейін шығындарды А заңды тұлғасы төлеуі керек. Егер сіздің ұйымыңызда бірнеше заңды тұлға болмаса, сізге компанияаралық шығындарды қосудың қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="fd2be-110">If intercompany expenses are enabled, the employee can then file an expense report that will post the expense to legal entity B, and the expense must then be paid by legal entity A. If your organization doesn’t have multiple legal entities, you don’t have to enable intercompany expenses.</span></span>

<span data-ttu-id="fd2be-111">**Шешім:** Компанияаралық шығындарды қосқыңыз келе ме?</span><span class="sxs-lookup"><span data-stu-id="fd2be-111">**Decision:** Do you want to enable intercompany expenses?</span></span>

## <a name="financial-management"></a><span data-ttu-id="fd2be-112">Қаржыны басқару</span><span class="sxs-lookup"><span data-stu-id="fd2be-112">Financial management</span></span>

<span data-ttu-id="fd2be-113">Шығындарды басқару Сіздің ұйымыңыздың қаржылық басқаруымен тығыз байланысты.</span><span class="sxs-lookup"><span data-stu-id="fd2be-113">Expense management is tightly integrated with the financial management of your organization.</span></span> <span data-ttu-id="fd2be-114">Шығындарды басқаруға арналған конфигурацияның көп бөлігі сіздің ұйымыңыздың қаржысы туралы қабылдаған шешімдеріңізге негізделеді.</span><span class="sxs-lookup"><span data-stu-id="fd2be-114">Lots of your configuration for Expense management will be based on the decisions that you’ve made about your organization’s finances.</span></span> <span data-ttu-id="fd2be-115">Келесі бөлімдерде сіздің ұйымыңыздың қаржылық шешімдері мен басшылық топтың ұсыныстары негізінде жоспарлау мен шешім қабылдауды қажет ететін әртүрлі салалар сипатталған.</span><span class="sxs-lookup"><span data-stu-id="fd2be-115">The following sections describe the various areas that require planning and decisions, based on your organization’s financial decisions and guidance from your leadership team.</span></span>

### <a name="per-diems"></a><span data-ttu-id="fd2be-116">Тәуліктік</span><span class="sxs-lookup"><span data-stu-id="fd2be-116">Per diems</span></span>

<span data-ttu-id="fd2be-117">Сіз ұйымыңыз қамтамасыз ететін қызметкерлердің тәуліктік ақыларын анықтауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="fd2be-117">You must define the employee per diems that your organization provides.</span></span> <span data-ttu-id="fd2be-118">Тәуліктік ақылар әдетте тамақтану, өмір сүру және басқа да кенеттен болатын шығындар сияқты шығындарды өтеу үшін пайдаланылатындықтан, сіз ұйым ұсынатын тәуліктік жәрдемақыларға арналған ережелер жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-118">Because per diems are typically used to cover expenses such as meals, lodging, and other incidental expenses, you can create rules for the per diem allowances that your organization offers.</span></span> <span data-ttu-id="fd2be-119">тәуліктік ақы мөлшері жыл мезгіліне, іссапар орнына немесе екеуіне де негізделуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="fd2be-119">per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="fd2be-120">Тәуліктік ақы ережесін анықтаған кезде, жұмысшы тегін тамақтанса немесе қызмет алса, тәуліктік ақы мөлшерлемесінің пайыздық мөлшері ұсталатынын көрсетуге болады.</span><span class="sxs-lookup"><span data-stu-id="fd2be-120">When you define a per diem rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="fd2be-121">Сондай-ақ жұмысшылардың іссапарларына қолдануға болатын минималды және максималды сағаттарды белгілеу үшін тәуліктік ақы мөлшерлемесінің деңгейлерін анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="fd2be-121">You can also define per diem rate tiers to set the minimum and maximum number of hours that the per diem rate can be applied to a worker’s travel.</span></span>

<span data-ttu-id="fd2be-122">**Шешімдер:**</span><span class="sxs-lookup"><span data-stu-id="fd2be-122">**Decisions:**</span></span>

- <span data-ttu-id="fd2be-123">Бірінші және соңғы күндер бойынша тәуліктік ақы ережелері:</span><span class="sxs-lookup"><span data-stu-id="fd2be-123">Default per diem rules for the first and last days:</span></span>

    - <span data-ttu-id="fd2be-124">Қызметкер бір күнге талап ете алатын және сонымен бірге тәуліктік ақы ала алатын минималды сағаттар саны қанша?</span><span class="sxs-lookup"><span data-stu-id="fd2be-124">What is the minimum number of hours that an employee can claim for a day and still receive a per diem?</span></span>
    - <span data-ttu-id="fd2be-125">Бірінші күні және соңғы күні тамақтануға ұсынылатын сомада ақы қысқартылады ма?</span><span class="sxs-lookup"><span data-stu-id="fd2be-125">Is there a reduction in the amount that is offered for meals for the first day and last day?</span></span> <span data-ttu-id="fd2be-126">Егер қысқартылса, онда қысқартылу пайызы қанша?</span><span class="sxs-lookup"><span data-stu-id="fd2be-126">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="fd2be-127">Бірінші күні және соңғы күні қонақ үйге ұсынылатын сомада ақы қысқартылады ма?</span><span class="sxs-lookup"><span data-stu-id="fd2be-127">Is there a reduction in the amount that is offered for a hotel for the first day and last day?</span></span> <span data-ttu-id="fd2be-128">Егер қысқартылса, онда қысқартылу пайызы қанша?</span><span class="sxs-lookup"><span data-stu-id="fd2be-128">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="fd2be-129">Бірінші және соңғы күнде жасалатын басқа шығындар үшін ұсынылатын сома қысқартылады ма?</span><span class="sxs-lookup"><span data-stu-id="fd2be-129">Is there a reduction in the amount that is offered for other expenses that are incurred on the first day and last day?</span></span> <span data-ttu-id="fd2be-130">Егер қысқартылса, онда қысқартылу пайызы қанша?</span><span class="sxs-lookup"><span data-stu-id="fd2be-130">If there is a reduction, what is the percentage of the reduction?</span></span>

- <span data-ttu-id="fd2be-131">Әдепкі тәуліктік ақы ережелері:</span><span class="sxs-lookup"><span data-stu-id="fd2be-131">Default per diem rules:</span></span>

    - <span data-ttu-id="fd2be-132">Мысалы, егер тамақ тегін болса, әрбір тамақтану кезінде тәуліктік ақының пайыздық төмендеуі бар ма?</span><span class="sxs-lookup"><span data-stu-id="fd2be-132">Is there a percentage reduction in the per diem allowance for each meal if, for example, the meal is complimentary?</span></span> <span data-ttu-id="fd2be-133">Егер төмендеу болса, онда әрбір тамақтану үшін төмендеу пайызы қанша?</span><span class="sxs-lookup"><span data-stu-id="fd2be-133">If there is a reduction, what is the reduction percentage for each meal?</span></span>
    - <span data-ttu-id="fd2be-134">Тамақтану бойынша қысқарту күніне, бәр іссапарға немесе тәулігіне тамақтану санына есептеле ме?</span><span class="sxs-lookup"><span data-stu-id="fd2be-134">Is the meal reduction calculated per day, per trip, or by the number of meals per day?</span></span>
    - <span data-ttu-id="fd2be-135">Тәуліктік ақы сомаларын әдеттегідей дөңгелектеу керек пе немесе оларды үлкен жағына дөңгелектеу керек пе?</span><span class="sxs-lookup"><span data-stu-id="fd2be-135">Should per diem amounts be rounded in the regular manner or rounded up?</span></span>
    - <span data-ttu-id="fd2be-136">Тәуліктік ақылар 24 сағаттық кезеңге немесе күнтізбелік күнге есептеледі ме?</span><span class="sxs-lookup"><span data-stu-id="fd2be-136">Are per diems calculated on a 24-hour period or on a calendar day?</span></span>

- <span data-ttu-id="fd2be-137">Тәуліктік ақы ережелері орналасу орнына негізделген:</span><span class="sxs-lookup"><span data-stu-id="fd2be-137">Per diem rules that are based on location:</span></span>

    - <span data-ttu-id="fd2be-138">Тәуліктік ақы мөлшерлемесі орналасқан жерге байланысты өзгере ме?</span><span class="sxs-lookup"><span data-stu-id="fd2be-138">Do per diem rates vary according to location?</span></span> <span data-ttu-id="fd2be-139">Оған қандай орындар кіреді?</span><span class="sxs-lookup"><span data-stu-id="fd2be-139">What locations are included?</span></span>
    - <span data-ttu-id="fd2be-140">Егер тәуліктік ақылар орналасқан жеріне байланысты өзгеріп отырса, әр орын үшін келесі шығын түрлері үшін қанша пайыздық мөлшерлеме қарастырылған:</span><span class="sxs-lookup"><span data-stu-id="fd2be-140">If per diem rates vary according to location, for each location, what percentage amount is provided for the following types of expenses:</span></span>

        - <span data-ttu-id="fd2be-141">Тамақтану</span><span class="sxs-lookup"><span data-stu-id="fd2be-141">Meals</span></span>
        - <span data-ttu-id="fd2be-142">Қонақүй</span><span class="sxs-lookup"><span data-stu-id="fd2be-142">Hotel</span></span>
        - <span data-ttu-id="fd2be-143">Басқа шығыстар</span><span class="sxs-lookup"><span data-stu-id="fd2be-143">Other expenses</span></span>

### <a name="expense-management-journals-and-accounts"></a><span data-ttu-id="fd2be-144">Шығыстарды басқаруға арналған журналдар мен шоттар</span><span class="sxs-lookup"><span data-stu-id="fd2be-144">Expense management journals and accounts</span></span>

<span data-ttu-id="fd2be-145">Шығыстарды басқару бірнеше журналдар мен шоттарды пайдалануды талап етеді.</span><span class="sxs-lookup"><span data-stu-id="fd2be-145">Expense management requires that you use multiple journals and accounts.</span></span> <span data-ttu-id="fd2be-146">Сіз, мысалы, ақшалай аванстық төлемдер мен несие карталары бойынша даулар үшін бірдей шот пайдаланылатынын шешуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="fd2be-146">You must decide, for example, whether the same account is used for cash advances and credit card disputes.</span></span>

<span data-ttu-id="fd2be-147">**Шешімдер:**</span><span class="sxs-lookup"><span data-stu-id="fd2be-147">**Decisions:**</span></span>

- <span data-ttu-id="fd2be-148">Бекітілген шығындар туралы есептер қандай кітап журналына орналастырылады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-148">Which ledger journal are approved expense reports posted to?</span></span>
- <span data-ttu-id="fd2be-149">Ақшалай аванстық төлемдер үшін қандай шот пайдаланылады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-149">Which account is used for cash advances?</span></span>
- <span data-ttu-id="fd2be-150">Ақшалай аванстық төлемдерді тез арада орналастыру керек пе?</span><span class="sxs-lookup"><span data-stu-id="fd2be-150">Should cash advances be posted immediately?</span></span>

### <a name="payment-methods"></a><span data-ttu-id="fd2be-151">Төлем әдістері</span><span class="sxs-lookup"><span data-stu-id="fd2be-151">Payment methods</span></span>

<span data-ttu-id="fd2be-152">Қызметкерлерге сіздің бизнесіңіздің атынан шығындар жасауға рұқсат берген кезде, сіз қызметкерлерге пайдалануға рұқсат етілген төлем әдістерін анықтауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="fd2be-152">When you allow employees to incur expenses on behalf of your business, you must define the payment methods that employees are allowed to use.</span></span> <span data-ttu-id="fd2be-153">Мысалы, сіз қызметкерлерге қолма-қол ақшаны немесе корпоративтік несие картасын пайдалануға рұқсат бере аласыз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-153">For example, you might allow employees to use cash or a corporate credit card.</span></span> <span data-ttu-id="fd2be-154">Сіз сондай-ақ қызметкерлерге жеке несиелік карталарды пайдалануға рұқсат беріп, содан кейін олардың шығындарын өтей аласыз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-154">You might also allow employees to use personal credit cards, and then reimburse the employees.</span></span> <span data-ttu-id="fd2be-155">Сіз рұқсат еткен әрбір төлем әдісі үшін келесі шешімдерді қабылдауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="fd2be-155">You must make the following decisions for each payment method that you allow.</span></span>

<span data-ttu-id="fd2be-156">**Шешімдер:**</span><span class="sxs-lookup"><span data-stu-id="fd2be-156">**Decisions:**</span></span>

- <span data-ttu-id="fd2be-157">Қандай төлем әдістеріне рұқсат етілген?</span><span class="sxs-lookup"><span data-stu-id="fd2be-157">What payment methods are allowed?</span></span>
- <span data-ttu-id="fd2be-158">Төлем әдісі бойынша шығындар кімге тиесілі?</span><span class="sxs-lookup"><span data-stu-id="fd2be-158">Who owns the payment method expenses?</span></span>
- <span data-ttu-id="fd2be-159">Өтемақылық шот түрі бар ма?</span><span class="sxs-lookup"><span data-stu-id="fd2be-159">Is there an offset account type?</span></span> <span data-ttu-id="fd2be-160">Егер өтемақылық шот түрі болса, ол қандай?</span><span class="sxs-lookup"><span data-stu-id="fd2be-160">If there is an offset account type, what is it?</span></span>
- <span data-ttu-id="fd2be-161">Егер өтемақылық шот түрі болса, шот қандай?</span><span class="sxs-lookup"><span data-stu-id="fd2be-161">If there is an offset account, what is the account?</span></span>
- <span data-ttu-id="fd2be-162">Егер төлем әдісі несиелік карта болса, төлем әдісін тек импортталған операциялармен пайдалану керек пе?</span><span class="sxs-lookup"><span data-stu-id="fd2be-162">If the payment method is a credit card, should the payment method be used only with imported transactions?</span></span>

### <a name="expense-categories-and-shared-categories"></a><span data-ttu-id="fd2be-163">Шығыс санаттары және жалпы санаттар</span><span class="sxs-lookup"><span data-stu-id="fd2be-163">Expense categories and shared categories</span></span>

<span data-ttu-id="fd2be-164">Қызметкерлер шығындар туралы есеп жасаған кезде, олар жазған әрбір шығын шығындар санатымен байланысты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="fd2be-164">When employees create an expense report, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="fd2be-165">Шығыстар санаттары ұйымыңыздағы нысандармен ортақ пайдалануға болатын ортақ санаттардан алынады.</span><span class="sxs-lookup"><span data-stu-id="fd2be-165">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="fd2be-166">Бұл санаттар ұйымды анықтау әдісіне байланысты жобаларды басқаруда және бухгалтерлік есепте де ортақ болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="fd2be-166">These categories can also be shared in Project management and accounting, depending on the way that your organization is defined.</span></span> <span data-ttu-id="fd2be-167">Сіздің ұйымыңыздың анықтамасына және іске асыру тобының ұсыныстарына сүйене отырып, шығындарды басқаруда пайдаланылатын санаттардың тек шығындарды басқаруда пайдаланылатынын немесе оларды жобаларды басқару және бухгалтерлік есеп пен шығындарды басқару арасында ортақ пайдалану қажеттігін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-167">Based on the definition of your organization and guidance from the implementation team, determine whether the categories that are used in Expense management will be used only in Expense management, or whether they should be shared between Project management and accounting and Expense management.</span></span> <span data-ttu-id="fd2be-168">Бұл санаттарды шығыстар мен өндіріс арасында емес, жоба мен шығындар немесе жоба мен өндіріс арасында ортақ пайдалануға болатынын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-168">Note that these categories can be shared between Project and Expense or Project and Production, but not between Expense and Production.</span></span> <span data-ttu-id="fd2be-169">Шығындардың әрбір санаты үшін келесі шешімдерді қабылдау қажет.</span><span class="sxs-lookup"><span data-stu-id="fd2be-169">You must make the following decisions for each expense category.</span></span>

<span data-ttu-id="fd2be-170">**Шешімдер:**</span><span class="sxs-lookup"><span data-stu-id="fd2be-170">**Decisions:**</span></span>

- <span data-ttu-id="fd2be-171">Шығыс санаты дегеніміз не?</span><span class="sxs-lookup"><span data-stu-id="fd2be-171">What is the expense category?</span></span> <span data-ttu-id="fd2be-172">Мысал ретінде рейстерге, қонақ үйге немесе жүгіруге арналған санаттарды алуға болады.</span><span class="sxs-lookup"><span data-stu-id="fd2be-172">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="fd2be-173">Шығындар санатын жобаны басқару және есепке алу кезінде де пайдалануға бола ма?</span><span class="sxs-lookup"><span data-stu-id="fd2be-173">Can the expense category also be used in Project management and accounting?</span></span>
- <span data-ttu-id="fd2be-174">Шығыс түрі дегеніміз не?</span><span class="sxs-lookup"><span data-stu-id="fd2be-174">What is the expense type?</span></span>
- <span data-ttu-id="fd2be-175">Шығындар санаты үшін төлеудің әдепкі әдісі қандай?</span><span class="sxs-lookup"><span data-stu-id="fd2be-175">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="fd2be-176">Шығындар санатындағы шығындарды бөлу керек пе?</span><span class="sxs-lookup"><span data-stu-id="fd2be-176">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="fd2be-177">Шығындар санаты үшін негізгі әдепкі есеп қандай?</span><span class="sxs-lookup"><span data-stu-id="fd2be-177">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="fd2be-178">Шығындар санаты бойынша сатудан алынатын салық тобы қандай болады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-178">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="fd2be-179">Шығындар санаты үшін қосымша төлем әдістеріне жол беріле ме?</span><span class="sxs-lookup"><span data-stu-id="fd2be-179">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="fd2be-180">Егер қосымша төлем әдістеріне рұқсат берілсе, олар қандай?</span><span class="sxs-lookup"><span data-stu-id="fd2be-180">If additional payment methods are allowed, what are they?</span></span>
- <span data-ttu-id="fd2be-181">Бұл шығыстар санатында ішкі санаттар бар ма?</span><span class="sxs-lookup"><span data-stu-id="fd2be-181">Are there subcategories in this expense category?</span></span> <span data-ttu-id="fd2be-182">Егер ішкі санаттар болса, сонымен қатар мына шешімдерді жасауыңыз керек:</span><span class="sxs-lookup"><span data-stu-id="fd2be-182">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="fd2be-183">Ішкі санаттардың біреуі салықты қалпына келтіруден шығарылған ба?</span><span class="sxs-lookup"><span data-stu-id="fd2be-183">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="fd2be-184">Ішкі санаттардың сатылым салығының тобы қандай?</span><span class="sxs-lookup"><span data-stu-id="fd2be-184">What is the item sales tax group of the subcategories?</span></span>

<span data-ttu-id="fd2be-185">Егер шығындар санаты жобаны басқару және есепке алу кезінде де пайдаланылса, қалған сұрақтарға жауап беріңіз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-185">If the expense category is also used in Project management and accounting, answer the remaining questions.</span></span> <span data-ttu-id="fd2be-186">Не болмаса, келесі бөлімге өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-186">Otherwise, move on to the next section.</span></span>

- <span data-ttu-id="fd2be-187">Келесі шығындар үшін қандай шығындар есептері пайдаланылады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-187">Which cost accounts will be used for the following expenses?</span></span>

    - <span data-ttu-id="fd2be-188">Құны</span><span class="sxs-lookup"><span data-stu-id="fd2be-188">Cost</span></span>
    - <span data-ttu-id="fd2be-189">Жалақы бөлу</span><span class="sxs-lookup"><span data-stu-id="fd2be-189">Payroll allocation</span></span>
    - <span data-ttu-id="fd2be-190">WIP-шығын мәні</span><span class="sxs-lookup"><span data-stu-id="fd2be-190">WIP-cost value</span></span>
    - <span data-ttu-id="fd2be-191">Шығындар-элемент</span><span class="sxs-lookup"><span data-stu-id="fd2be-191">Cost-item</span></span>
    - <span data-ttu-id="fd2be-192">WIP-шығын құнының элементі</span><span class="sxs-lookup"><span data-stu-id="fd2be-192">WIP-cost value-item</span></span>
    - <span data-ttu-id="fd2be-193">Есептелген шығын</span><span class="sxs-lookup"><span data-stu-id="fd2be-193">Accrued loss</span></span>
    - <span data-ttu-id="fd2be-194">WIP-есептелген шығын</span><span class="sxs-lookup"><span data-stu-id="fd2be-194">WIP-accrued loss</span></span>

- <span data-ttu-id="fd2be-195">Келесі мақсаттар үшін қандай кіріс шоттары пайдаланылады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-195">Which revenue accounts will be used for the following?</span></span>

    - <span data-ttu-id="fd2be-196">Шот-фактура бойынша табыс</span><span class="sxs-lookup"><span data-stu-id="fd2be-196">Invoiced revenue</span></span>
    - <span data-ttu-id="fd2be-197">Есептелген табыс-сатылым құны</span><span class="sxs-lookup"><span data-stu-id="fd2be-197">Accrued revenue-sales value</span></span>
    - <span data-ttu-id="fd2be-198">WIP-сату құны</span><span class="sxs-lookup"><span data-stu-id="fd2be-198">WIP-sales value</span></span>
    - <span data-ttu-id="fd2be-199">Есептелген кіріс-өндіріс</span><span class="sxs-lookup"><span data-stu-id="fd2be-199">Accrued revenue-production</span></span>
    - <span data-ttu-id="fd2be-200">WIP-өндіріс</span><span class="sxs-lookup"><span data-stu-id="fd2be-200">WIP-production</span></span>
    - <span data-ttu-id="fd2be-201">Есептелген кіріс-пайда</span><span class="sxs-lookup"><span data-stu-id="fd2be-201">Accrued revenue-profit</span></span>
    - <span data-ttu-id="fd2be-202">WIP-пайда</span><span class="sxs-lookup"><span data-stu-id="fd2be-202">WIP-profit</span></span>
    - <span data-ttu-id="fd2be-203">Есептелген кіріс-жазылым</span><span class="sxs-lookup"><span data-stu-id="fd2be-203">Accrued revenue-subscription</span></span>
    - <span data-ttu-id="fd2be-204">WIP-жазылым</span><span class="sxs-lookup"><span data-stu-id="fd2be-204">WIP-subscription</span></span>

### <a name="taxes"></a><span data-ttu-id="fd2be-205">Салықтар</span><span class="sxs-lookup"><span data-stu-id="fd2be-205">Taxes</span></span>

<span data-ttu-id="fd2be-206">Шығындарға байланысты салықтар бойынша шығындар туралы есептерге не енгізілетінін немесе қосылатынын анықтауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="fd2be-206">For expense-related taxes, you must determine what is included or enabled on expense reports.</span></span>

<span data-ttu-id="fd2be-207">**Шешімдер:**</span><span class="sxs-lookup"><span data-stu-id="fd2be-207">**Decisions:**</span></span>

- <span data-ttu-id="fd2be-208">Сату салығы шығындар сомаларына кіреді ме?</span><span class="sxs-lookup"><span data-stu-id="fd2be-208">Is sales tax included in the expense amounts?</span></span>
- <span data-ttu-id="fd2be-209">Шығындар бойынша салықты қалпына келтіруді қосу керек пе?</span><span class="sxs-lookup"><span data-stu-id="fd2be-209">Should tax recovery be enabled on expenses?</span></span>

    > [!NOTE]
    > <span data-ttu-id="fd2be-210">Бас кітапты жоспарлаған кезде, егер сіз АҚШ сатылым салығын қолдануды және салық ережелерін қолдануды шешсеңіз, шығындар бойынша салықты қалпына келтіруге мүмкіндік бере алмайсыз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-210">When you were planning the general ledger, if you decided to apply U.S. sales tax and use tax rules, you can’t enable tax recovery on expenses.</span></span> <span data-ttu-id="fd2be-211">(АҚШ сату салығын қолдану және салық ережелерін қолдану үшін, **Сатуға салынатын салық салу ережелерін қолдану** опциясын **Иә** параметріне орнатыңыз.)</span><span class="sxs-lookup"><span data-stu-id="fd2be-211">(To apply U.S. sales tax and use tax rules, set the **Apply sales tax taxations rules** option to **Yes**.)</span></span>

## <a name="policies"></a><span data-ttu-id="fd2be-212">саясат</span><span class="sxs-lookup"><span data-stu-id="fd2be-212">Policies</span></span>

<span data-ttu-id="fd2be-213">Шығындар туралы есеп саясатын құра отырып, сіз қызметкерлерге өз атынан шығын жасаған кезде ұйымыңызға уақыт пен ақшаны үнемдеуге көмектесе аласыз.</span><span class="sxs-lookup"><span data-stu-id="fd2be-213">By creating expense report policies, you can help your organization save time and money when employees incur expenses on its behalf.</span></span> <span data-ttu-id="fd2be-214">Саясат қызметкерлердің бюджетте қалуына, барлық қажетті ақпаратты ұсынуына және ақшаны олар қажет болған жағдайда ғана жұмсауға кепілдік беруге көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="fd2be-214">Policies help guarantee that employees stay in budget, provide all required information, and spend money only as they require it.</span></span> <span data-ttu-id="fd2be-215">Сіз жасаған әрбір шығындар туралы есеп саясаты және шығындар туралы есептерді бекіту саясаты үшін келесі шешімдерді қабылдауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="fd2be-215">You must make the following decisions for each expense report policy and each expense report approval policy that you create.</span></span>

<span data-ttu-id="fd2be-216">**Шешімдер:**</span><span class="sxs-lookup"><span data-stu-id="fd2be-216">**Decisions:**</span></span>

- <span data-ttu-id="fd2be-217">Саясат қалай аталады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-217">What is the name of the policy?</span></span>
- <span data-ttu-id="fd2be-218">Шығындар саясаты не үшін қажет?</span><span class="sxs-lookup"><span data-stu-id="fd2be-218">What is the expense policy for?</span></span>
- <span data-ttu-id="fd2be-219">Егер сіз бұрын компанияаралық шығыстарды қосуға шешім қабылдаған болсаңыз, онда бұл саясат сіздің ұйымыңыздағы қай компанияларға қолданылады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-219">If you previously decided to enable intercompany expenses, which companies in your organization will this policy apply to?</span></span>
- <span data-ttu-id="fd2be-220">Саясат қашан тиімді болады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-220">When does the policy become effective?</span></span>
- <span data-ttu-id="fd2be-221">Саясаттың қолданылу мерзімі қашан аяқталады?</span><span class="sxs-lookup"><span data-stu-id="fd2be-221">When does the policy expire?</span></span>
- <span data-ttu-id="fd2be-222">Саясат ережесі қандай?</span><span class="sxs-lookup"><span data-stu-id="fd2be-222">What is the policy rule?</span></span>
- <span data-ttu-id="fd2be-223">Бұл саяси ереженің нәтижесі қандай?</span><span class="sxs-lookup"><span data-stu-id="fd2be-223">What is the outcome of the policy rule?</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]