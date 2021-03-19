---
title: Қолда бар тауарлар
description: Бұл тақырыпта Microsoft Dynamics 365 Project Operations бағдарламасында нақты көрсеткіштермен жұмыс жасау жолы туралы ақпарат берілген.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 6a94bd143b0d0dad2a08511a34e592a057b6d2a1
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291806"
---
# <a name="actuals"></a><span data-ttu-id="ce035-103">Қолда бар тауарлар</span><span class="sxs-lookup"><span data-stu-id="ce035-103">Actuals</span></span> 

<span data-ttu-id="ce035-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="ce035-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ce035-105">Нақты мәндер — жоба бойынша аяқталған жұмыс көлемі.</span><span class="sxs-lookup"><span data-stu-id="ce035-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="ce035-106">Олар уақыт пен шығыс жазбалары, журнал жазбалары мен есеп-шоттар нәтижесінде жасалады.</span><span class="sxs-lookup"><span data-stu-id="ce035-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="ce035-107">Журнал жолдары және уақытты ұсыну</span><span class="sxs-lookup"><span data-stu-id="ce035-107">Journal lines and time submission</span></span>

<span data-ttu-id="ce035-108">Уақыт жазбасы туралы қосымша ақпаратты [Уақыт жазбасын шолу](../time/time-entry-overview.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="ce035-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="ce035-109">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="ce035-109">Time and materials</span></span>

<span data-ttu-id="ce035-110">Уақыт жазбасы уақыт және материалдар келісім-шарт жолына тағайындалған жобамен байланыстырылған кезде, жүйе екі журнал жолын жасайды, оның біреуі өзіндік құны, екіншісі шот ұсынылмаған сатылым.</span><span class="sxs-lookup"><span data-stu-id="ce035-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="ce035-111">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="ce035-111">Fixed price</span></span>

<span data-ttu-id="ce035-112">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға уақыт жазбасы жіберілген кезде, жүйе журнал жолын тек құн үшін жасайды.</span><span class="sxs-lookup"><span data-stu-id="ce035-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="ce035-113">Әдепкі баға</span><span class="sxs-lookup"><span data-stu-id="ce035-113">Default pricing</span></span>

<span data-ttu-id="ce035-114">Әдеттегі бағаларды жасау логикасы журнал жолында орналасқан.</span><span class="sxs-lookup"><span data-stu-id="ce035-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="ce035-115">Уақыт жазбасындағы өріс мәндері журнал жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="ce035-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="ce035-116">Бұл мәндер транзакция күнін, жоба тағайындалған келісім-шарт жолын және тиісті бағатізбедегі валютаны қамтиды.</span><span class="sxs-lookup"><span data-stu-id="ce035-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="ce035-117">**Рөл** және **Бөлімше** сияқты әдепкі бағаларды көрсететін өрістер тиісті бағаның журнал жолын анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="ce035-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="ce035-118">Уақыт жазбасына реттелетін өрісті қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="ce035-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="ce035-119">Өріс мәнін нақты мәндерге тарату қажет болса, нақты мәндер нысанында өрісті жасап, өрісті уақыт жазбасынан нақты мәндер өрісіне көшіру үшін өріс салыстыруларын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="ce035-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="ce035-120">Журнал жолдары және негізгі шығысты жіберу</span><span class="sxs-lookup"><span data-stu-id="ce035-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="ce035-121">Шығыс жазбасы туралы қосымша ақпаратты [Шығыстарды шолу](../expense/expense-overview.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="ce035-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="ce035-122">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="ce035-122">Time and materials</span></span>

<span data-ttu-id="ce035-123">Негізгі шығыс жазбасы уақыт және материалдар келісім-шарт жолына тағайындалған жобамен байланыстырылған кезде, жүйе екі журнал жолын жасайды, оның біреуі өзіндік құны, екіншісі шот ұсынылмаған сатылым.</span><span class="sxs-lookup"><span data-stu-id="ce035-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="ce035-124">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="ce035-124">Fixed price</span></span>

<span data-ttu-id="ce035-125">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға негізгі шығыс жазбасы жіберілген кезде, жүйе журнал жолын тек құн үшін жасайды.</span><span class="sxs-lookup"><span data-stu-id="ce035-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="ce035-126">Әдепкі баға</span><span class="sxs-lookup"><span data-stu-id="ce035-126">Default pricing</span></span>

<span data-ttu-id="ce035-127">Шығыстар бойынша әдепкі бағаларды енгізу логикасы шығыстар санатына негізделген.</span><span class="sxs-lookup"><span data-stu-id="ce035-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="ce035-128">Транзакция жасалған күн, жоба тағайындалған келісім-шарт жолы және валюта тиісті бағатізбені анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="ce035-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="ce035-129">Дегенмен, әдепкі бойынша, бағаның өзі үшін пайдаланушының енгізген сомасы қатысты шығыстың құн және сатылым журнал жолдарына тікелей орнатылады.</span><span class="sxs-lookup"><span data-stu-id="ce035-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="ce035-130">Шығыс жазбаларында бірліктің санат негізіндегі жазбасының әдепкі бағасы қолжетімді емес.</span><span class="sxs-lookup"><span data-stu-id="ce035-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="ce035-131">Шығыстарды жазу үшін жазба журналдарын пайдалану</span><span class="sxs-lookup"><span data-stu-id="ce035-131">Use entry journals to record costs</span></span>

<span data-ttu-id="ce035-132">Құнды немесе материалдағы, алымдағы, уақыттағы, шығыстағы табысты немесе салық транзакцияларының кластарын жазу үшін жазба журналдарын пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="ce035-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="ce035-133">Журналдарды келесі мақсаттарда пайдалануға болады:</span><span class="sxs-lookup"><span data-stu-id="ce035-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="ce035-134">Жоба бойынша материалдардың нақты құны мен сатылымдарын жазыңыз.</span><span class="sxs-lookup"><span data-stu-id="ce035-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="ce035-135">Транзакцияның нақты көрсеткіштерін басқа жүйеден Microsoft Dynamics 365 Project Operations бағдарламасына ауыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="ce035-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="ce035-136">Басқа жүйеде орын алған шығындарды жазыңыз.</span><span class="sxs-lookup"><span data-stu-id="ce035-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="ce035-137">Бұл құндар сатып алу немесе қосымша келісім-шарт құнын қамтуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="ce035-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ce035-138">Бағдарлама журнал жолының түрін немесе журнал жолына енгізілген тиісті бағаны тексермейді.</span><span class="sxs-lookup"><span data-stu-id="ce035-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="ce035-139">Сондықтан, нақты көрсеткіштердің жобаға тигізетін бухгалтерлік есебінің әсерін толық білетін пайдаланушы ғана нақты көрсеткіштер жасау үшін жазба журналдарын пайдалануы керек.</span><span class="sxs-lookup"><span data-stu-id="ce035-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="ce035-140">Осы журнал түрінің әсеріне байланысты, жазба журналдарын жасауға кімнің рұқсаты бар екенін мұқият таңдау керек.</span><span class="sxs-lookup"><span data-stu-id="ce035-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="ce035-141">Жоба оқиғаларының негізінде нақты көрсеткіштерді жазу</span><span class="sxs-lookup"><span data-stu-id="ce035-141">Record actuals based on project events</span></span>

<span data-ttu-id="ce035-142">Project Operations жүйесі жоба барысында орын алатын барлық қаржылық операцияларды жазады.</span><span class="sxs-lookup"><span data-stu-id="ce035-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="ce035-143">Бұл операциялар нақты мәндер ретінде жазылады.</span><span class="sxs-lookup"><span data-stu-id="ce035-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="ce035-144">Төмендегі кестелерде жобаның уақыт және материалдық екеніне, бағасының бекітілгеніне, алдын ала сату кезеңінде екеніне немесе ішкі жоба екеніне байланысты жасалған әртүрлі нақты мәндер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="ce035-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="ce035-145">Ресурс жобаның келісімшарт бірлігімен бірдей ұйымдық бөлімшеге тиесілі</span><span class="sxs-lookup"><span data-stu-id="ce035-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="ce035-146">Оқиға</span><span class="sxs-lookup"><span data-stu-id="ce035-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="ce035-147">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="ce035-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="ce035-148">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="ce035-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="ce035-149">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="ce035-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="ce035-150">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="ce035-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="ce035-151">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="ce035-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="ce035-152">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="ce035-152">Actuals</span></span></th>
<th><span data-ttu-id="ce035-153">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-153">Transaction currency</span></span></th>
<th><span data-ttu-id="ce035-154">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="ce035-154">Fixed price</span></span></th>
<th><span data-ttu-id="ce035-155">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="ce035-156">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="ce035-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="ce035-157">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="ce035-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-158">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="ce035-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="ce035-159">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="ce035-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ce035-160">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="ce035-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ce035-161">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-161">Cost actual</span></span></td>
<td><span data-ttu-id="ce035-162">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-163">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-164">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="ce035-165">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-166">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-167">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="ce035-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="ce035-168">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ce035-169">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="ce035-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ce035-170">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-170">Cost actual</span></span></td>
<td><span data-ttu-id="ce035-171">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-172">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-173">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-174">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-175">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-176">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="ce035-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ce035-177">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-178">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="ce035-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ce035-179">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ce035-180">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="ce035-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ce035-181">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ce035-182">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-183">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-184">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-185">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-186">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-187">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-187">Billed sales</span></span></td>
<td><span data-ttu-id="ce035-188">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ce035-189">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="ce035-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ce035-190">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ce035-191">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-192">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-193">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-194">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-195">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-196">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="ce035-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ce035-197">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-198">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="ce035-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ce035-199">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ce035-200">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="ce035-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ce035-201">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ce035-202">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="ce035-203">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="ce035-204">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="ce035-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="ce035-205">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ce035-206">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="ce035-207">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-208">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-208">Billed sales</span></span></td>
<td><span data-ttu-id="ce035-209">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ce035-210">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="ce035-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ce035-211">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ce035-212">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-213">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="ce035-214">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-215">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="ce035-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="ce035-216">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="ce035-217">Ресурс жобаның келісім-шарт бірлігінен өзгеше ұйымдық бөлімшеге тиесілі</span><span class="sxs-lookup"><span data-stu-id="ce035-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="ce035-218">Оқиға</span><span class="sxs-lookup"><span data-stu-id="ce035-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="ce035-219">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="ce035-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="ce035-220">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="ce035-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="ce035-221">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="ce035-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="ce035-222">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="ce035-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="ce035-223">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="ce035-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="ce035-224">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="ce035-224">Actuals</span></span></th>
<th><span data-ttu-id="ce035-225">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-225">Transaction currency</span></span></th>
<th><span data-ttu-id="ce035-226">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="ce035-226">Fixed price</span></span></th>
<th><span data-ttu-id="ce035-227">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="ce035-228">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="ce035-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="ce035-229">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="ce035-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-230">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="ce035-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="ce035-231">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="ce035-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="ce035-232">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="ce035-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ce035-233">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-233">Cost actual</span></span></td>
<td><span data-ttu-id="ce035-234">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="ce035-235">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="ce035-236">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="ce035-237">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="ce035-238">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-239">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="ce035-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="ce035-240">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-241">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="ce035-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="ce035-242">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-243">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="ce035-244">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="ce035-245">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="ce035-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ce035-246">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-246">Cost actual</span></span></td>
<td><span data-ttu-id="ce035-247">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ce035-248">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="ce035-249">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ce035-250">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="ce035-251">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="ce035-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-252">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="ce035-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="ce035-253">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-254">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="ce035-255">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-256">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="ce035-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ce035-257">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-258">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="ce035-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ce035-259">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ce035-260">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="ce035-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ce035-261">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ce035-262">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-263">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-264">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-265">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="ce035-266">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-267">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-267">Billed sales</span></span></td>
<td><span data-ttu-id="ce035-268">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ce035-269">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="ce035-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ce035-270">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ce035-271">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-272">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-273">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-274">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ce035-275">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-276">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="ce035-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ce035-277">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-278">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="ce035-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ce035-279">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ce035-280">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="ce035-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ce035-281">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ce035-282">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="ce035-283">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="ce035-284">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="ce035-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="ce035-285">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ce035-286">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="ce035-287">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="ce035-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-288">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-288">Billed sales</span></span></td>
<td><span data-ttu-id="ce035-289">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ce035-290">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="ce035-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ce035-291">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="ce035-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ce035-292">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-293">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="ce035-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="ce035-294">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ce035-295">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="ce035-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="ce035-296">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="ce035-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]