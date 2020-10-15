---
title: "\"Нақты көрсеткіштер\" басты беті"
description: Бұл тақырыпта Microsoft Dynamics 365 Project Operations нақты көрсеткіштермен жұмыс істеу жолы туралы ақпарат берілген.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 75ad336a995aba3505325466433a5c5e2bb3e776
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907325"
---
# <a name="actuals"></a><span data-ttu-id="1e8fc-103">Қолда бар тауарлар</span><span class="sxs-lookup"><span data-stu-id="1e8fc-103">Actuals</span></span>

<span data-ttu-id="1e8fc-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="1e8fc-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="1e8fc-105">Нақты мәндер — жоба бойынша аяқталған жұмыс көлемі.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="1e8fc-106">Олар уақыт пен шығыс жазбалары, журнал жазбалары мен есеп-шоттар нәтижесінде жасалады.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="1e8fc-107">Журнал жолдары және уақытты ұсыну</span><span class="sxs-lookup"><span data-stu-id="1e8fc-107">Journal lines and time submission</span></span>

<span data-ttu-id="1e8fc-108">Уақыт жазбасы туралы қосымша ақпаратты [Уақыт жазбасын шолу](../time/time-entry-overview.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="1e8fc-109">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="1e8fc-109">Time and materials</span></span>

<span data-ttu-id="1e8fc-110">Уақыт жазбасы уақыт және материалдар келісім-шарт жолына тағайындалған жобамен байланыстырылған кезде, жүйе екі журнал жолын жасайды, оның біреуі өзіндік құны, екіншісі шот ұсынылмаған сатылым.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="1e8fc-111">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-111">Fixed price</span></span>

<span data-ttu-id="1e8fc-112">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға уақыт жазбасы жіберілген кезде, жүйе журнал жолын тек құн үшін жасайды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="1e8fc-113">Әдепкі баға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-113">Default pricing</span></span>

<span data-ttu-id="1e8fc-114">Әдеттегі бағаларды жасау логикасы журнал жолында орналасқан.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="1e8fc-115">Уақыт жазбасындағы өріс мәндері журнал жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="1e8fc-116">Бұл мәндер транзакция күнін, жоба тағайындалған келісім-шарт жолын және тиісті бағатізбедегі валютаны қамтиды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="1e8fc-117">**Рөл** және **Бөлімше** сияқты әдепкі бағаларды көрсететін өрістер тиісті бағаның журнал жолын анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="1e8fc-118">Уақыт жазбасына реттелетін өрісті қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="1e8fc-119">Өріс мәнін нақты мәндерге тарату қажет болса, нақты мәндер нысанында өрісті жасап, өрісті уақыт жазбасынан нақты мәндер өрісіне көшіру үшін өріс салыстыруларын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="1e8fc-120">Журнал жолдары және негізгі шығысты жіберу</span><span class="sxs-lookup"><span data-stu-id="1e8fc-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="1e8fc-121">Шығыс жазбасы туралы қосымша ақпаратты [Шығыстарды шолу](../expense/expense-overview.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="1e8fc-122">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="1e8fc-122">Time and materials</span></span>

<span data-ttu-id="1e8fc-123">Негізгі шығыс жазбасы уақыт және материалдар келісім-шарт жолына тағайындалған жобамен байланыстырылған кезде, жүйе екі журнал жолын жасайды, оның біреуі өзіндік құны, екіншісі шот ұсынылмаған сатылым.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="1e8fc-124">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-124">Fixed price</span></span>

<span data-ttu-id="1e8fc-125">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға негізгі шығыс жазбасы жіберілген кезде, жүйе журнал жолын тек құн үшін жасайды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="1e8fc-126">Әдепкі баға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-126">Default pricing</span></span>

<span data-ttu-id="1e8fc-127">Шығыстар бойынша әдепкі бағаларды енгізу логикасы шығыстар санатына негізделген.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="1e8fc-128">Транзакция жасалған күн, жоба тағайындалған келісім-шарт жолы және валюта тиісті бағатізбені анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="1e8fc-129">Дегенмен, әдепкі бойынша, бағаның өзі үшін пайдаланушының енгізген сомасы қатысты шығыстың құн және сатылым журнал жолдарына тікелей орнатылады.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="1e8fc-130">Шығыс жазбаларында бірліктің санат негізіндегі жазбасының әдепкі бағасы қолжетімді емес.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="1e8fc-131">Шығыстарды жазу үшін жазба журналдарын пайдалану</span><span class="sxs-lookup"><span data-stu-id="1e8fc-131">Use entry journals to record costs</span></span>

<span data-ttu-id="1e8fc-132">Құнды немесе материалдағы, алымдағы, уақыттағы, шығыстағы табысты немесе салық транзакцияларының кластарын жазу үшін жазба журналдарын пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="1e8fc-133">Журналдарды келесі мақсаттарда пайдалануға болады:</span><span class="sxs-lookup"><span data-stu-id="1e8fc-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="1e8fc-134">Жоба бойынша материалдардың нақты құны мен сатылымдарын жазыңыз.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="1e8fc-135">Транзакцияның нақты көрсеткіштерін басқа жүйеден Microsoft Dynamics 365 Project Operations жүйесіне ауыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="1e8fc-136">Басқа жүйеде орын алған шығындарды жазыңыз.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="1e8fc-137">Бұл құндар сатып алу немесе қосымша келісім-шарт құнын қамтуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1e8fc-138">Бағдарлама журнал жолының түрін немесе журнал жолына енгізілген тиісті бағаны тексермейді.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="1e8fc-139">Сондықтан, нақты көрсеткіштердің жобаға тигізетін бухгалтерлік есебінің әсерін толық білетін пайдаланушы ғана нақты көрсеткіштер жасау үшін жазба журналдарын пайдалануы керек.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="1e8fc-140">Осы журнал түрінің әсеріне байланысты, жазба журналдарын жасауға кімнің рұқсаты бар екенін мұқият таңдау керек.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="1e8fc-141">Жоба оқиғаларының негізінде нақты көрсеткіштерді жазу</span><span class="sxs-lookup"><span data-stu-id="1e8fc-141">Record actuals based on project events</span></span>

<span data-ttu-id="1e8fc-142">Project Operations жүйесі жоба барысында орын алатын барлық қаржылық операцияларды жазады.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="1e8fc-143">Бұл операциялар нақты мәндер ретінде жазылады.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="1e8fc-144">Төмендегі кестелерде жобаның уақыт және материалдық екеніне, бағасының бекітілгеніне, алдын ала сату кезеңінде екеніне немесе ішкі жоба екеніне байланысты жасалған әртүрлі нақты мәндер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="1e8fc-145">Ресурс жобаның келісімшарт бірлігімен бірдей ұйымдық бөлімшеге тиесілі</span><span class="sxs-lookup"><span data-stu-id="1e8fc-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="1e8fc-146">Оқиға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="1e8fc-147">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="1e8fc-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="1e8fc-148">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="1e8fc-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="1e8fc-149">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="1e8fc-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="1e8fc-150">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="1e8fc-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="1e8fc-151">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="1e8fc-152">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="1e8fc-152">Actuals</span></span></th>
<th><span data-ttu-id="1e8fc-153">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-153">Transaction currency</span></span></th>
<th><span data-ttu-id="1e8fc-154">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-154">Fixed price</span></span></th>
<th><span data-ttu-id="1e8fc-155">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="1e8fc-156">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="1e8fc-157">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="1e8fc-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-158">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="1e8fc-159">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="1e8fc-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="1e8fc-160">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="1e8fc-161">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-161">Cost actual</span></span></td>
<td><span data-ttu-id="1e8fc-162">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-163">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-164">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="1e8fc-165">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-166">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-167">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="1e8fc-168">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="1e8fc-169">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="1e8fc-170">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-170">Cost actual</span></span></td>
<td><span data-ttu-id="1e8fc-171">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-172">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-173">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-174">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-175">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-176">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="1e8fc-177">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-178">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="1e8fc-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="1e8fc-179">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="1e8fc-180">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="1e8fc-181">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="1e8fc-182">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-183">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-184">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-185">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-186">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-187">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-187">Billed sales</span></span></td>
<td><span data-ttu-id="1e8fc-188">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="1e8fc-189">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="1e8fc-190">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="1e8fc-191">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-192">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-193">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-194">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-195">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-196">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="1e8fc-197">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-198">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="1e8fc-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="1e8fc-199">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="1e8fc-200">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="1e8fc-201">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="1e8fc-202">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="1e8fc-203">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="1e8fc-204">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="1e8fc-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="1e8fc-205">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="1e8fc-206">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="1e8fc-207">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-208">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-208">Billed sales</span></span></td>
<td><span data-ttu-id="1e8fc-209">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="1e8fc-210">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="1e8fc-211">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="1e8fc-212">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-213">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="1e8fc-214">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-215">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="1e8fc-216">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="1e8fc-217">Ресурс жобаның келісім-шарт бірлігінен өзгеше ұйымдық бөлімшеге тиесілі</span><span class="sxs-lookup"><span data-stu-id="1e8fc-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="1e8fc-218">Оқиға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="1e8fc-219">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="1e8fc-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="1e8fc-220">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="1e8fc-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="1e8fc-221">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="1e8fc-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="1e8fc-222">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="1e8fc-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="1e8fc-223">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="1e8fc-224">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="1e8fc-224">Actuals</span></span></th>
<th><span data-ttu-id="1e8fc-225">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-225">Transaction currency</span></span></th>
<th><span data-ttu-id="1e8fc-226">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="1e8fc-226">Fixed price</span></span></th>
<th><span data-ttu-id="1e8fc-227">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="1e8fc-228">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="1e8fc-229">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="1e8fc-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-230">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="1e8fc-231">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="1e8fc-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="1e8fc-232">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="1e8fc-233">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-233">Cost actual</span></span></td>
<td><span data-ttu-id="1e8fc-234">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="1e8fc-235">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="1e8fc-236">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="1e8fc-237">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="1e8fc-238">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-239">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="1e8fc-240">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-241">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="1e8fc-242">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-243">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="1e8fc-244">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="1e8fc-245">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="1e8fc-246">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-246">Cost actual</span></span></td>
<td><span data-ttu-id="1e8fc-247">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="1e8fc-248">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="1e8fc-249">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="1e8fc-250">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="1e8fc-251">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-252">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="1e8fc-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="1e8fc-253">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-254">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="1e8fc-255">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-256">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="1e8fc-257">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-258">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="1e8fc-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="1e8fc-259">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="1e8fc-260">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="1e8fc-261">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="1e8fc-262">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-263">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-264">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-265">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="1e8fc-266">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-267">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-267">Billed sales</span></span></td>
<td><span data-ttu-id="1e8fc-268">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="1e8fc-269">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="1e8fc-270">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="1e8fc-271">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-272">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-273">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-274">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="1e8fc-275">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-276">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="1e8fc-277">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-278">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="1e8fc-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="1e8fc-279">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="1e8fc-280">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="1e8fc-281">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="1e8fc-282">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="1e8fc-283">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="1e8fc-284">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="1e8fc-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="1e8fc-285">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="1e8fc-286">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="1e8fc-287">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="1e8fc-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-288">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-288">Billed sales</span></span></td>
<td><span data-ttu-id="1e8fc-289">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="1e8fc-290">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="1e8fc-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="1e8fc-291">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="1e8fc-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="1e8fc-292">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-293">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="1e8fc-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="1e8fc-294">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="1e8fc-295">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="1e8fc-296">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="1e8fc-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
