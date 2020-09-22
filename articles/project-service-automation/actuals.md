---
title: Нақты мәндер
description: Бұл тақырыпта жобаның нақты мәндері туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753128"
---
# <a name="actuals"></a><span data-ttu-id="4aec9-103">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="4aec9-103">Actuals</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="4aec9-104">Нақты мәндер — жоба бойынша аяқталған жұмыс көлемі.</span><span class="sxs-lookup"><span data-stu-id="4aec9-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="4aec9-105">Жобаның нақты мәндерін олардың бастапқы құжаттарына белгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="4aec9-106">Бұл бастапқы құжаттар уақытты, шығыстарды және журнал жазбаларын, сондай-ақ есеп-шоттарды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="4aec9-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Жобаның нақты мәндерін олардың бастапқы құжаттарына белгілеу жолы](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="4aec9-108">Осы уақыт жазбасын жіберу</span><span class="sxs-lookup"><span data-stu-id="4aec9-108">Submitting a time entry</span></span>

<span data-ttu-id="4aec9-109">PSA жүйесінде уақыт және материалдар келісім-шарт жолына тағайындалған жобаға уақыт жазбасы жіберілген кезде екі журнал жолы жасалады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="4aec9-110">Бір жол шығынға арналған, ал екінші жол шот ұсынылмаған сатылымға арналған.</span><span class="sxs-lookup"><span data-stu-id="4aec9-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="4aec9-111">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға уақыт жазбасы жіберілген кезде журнал жолы тек құн үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="4aec9-112">Әдеттегі бағаларды енгізу логикасы журнал жолында орналасқан.</span><span class="sxs-lookup"><span data-stu-id="4aec9-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="4aec9-113">Уақыт жазбасындағы барлық өріс мәндері журнал жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4aec9-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="4aec9-114">Бұл өрістер транзакция жасалған күнді, жоба тағайындалған келісім-шарт жолын және тиісті бағатізбедегі валютаны қамтиды.</span><span class="sxs-lookup"><span data-stu-id="4aec9-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="4aec9-115">**Рөл** және **Ұйымдық бөлімше** сияқты әдепкі бағаларды көрсететін өрістер тиісті бағаның журнал жолына әдепкі бойынша енгізілуіне әкеледі.</span><span class="sxs-lookup"><span data-stu-id="4aec9-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="4aec9-116">Уақыт жазбасына реттелетін өрісті қоссаңыз және өріс мәнін нақты мәндерге тарату қажет болса, нақты мәндер нысанында өрісті жасап, өрісті уақыт жазбасынан нақты мәндер өрісіне көшіру үшін өріс салыстыруларын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="4aec9-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="4aec9-117">Шығыс жазбасын жіберу</span><span class="sxs-lookup"><span data-stu-id="4aec9-117">Submitting an expense entry</span></span>

<span data-ttu-id="4aec9-118">PSA жүйесінде уақыт және материалдар келісім-шарт жолына тағайындалған жобаға шығыс жазбасы жіберілген кезде екі журнал жолы жасалады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="4aec9-119">Бір жол шығынға арналған, ал екінші жол шот ұсынылмаған сатылымға арналған.</span><span class="sxs-lookup"><span data-stu-id="4aec9-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="4aec9-120">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға шығыс жазбасы жіберілген кезде журнал жолы тек құн үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="4aec9-121">Шығыстардың әдепкі бағаларын енгізудің логикасы **Шығыс жазбасы** бетінде таңдалған шығыс санатына негізделген.</span><span class="sxs-lookup"><span data-stu-id="4aec9-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="4aec9-122">Транзакция жасалған күн, жоба тағайындалған келісім-шарт жолы және валюта тиісті бағатізбені анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="4aec9-123">Дегенмен бағаның өзі үшін пайдаланушының енгізген сомасы, әдепкі бойынша қатысты шығыстың құн және сатылым журнал жолдарына тікелей орнатылады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="4aec9-124">PSA жүйесінің ағымдағы нұсқасында, шығыс жазбаларында бірліктің санат негізіндегі жазбасының әдепкі бағасы қолжетімді емес.</span><span class="sxs-lookup"><span data-stu-id="4aec9-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-journals-to-record-costs"></a><span data-ttu-id="4aec9-125">Шығыстарды жазу үшін журналдарды пайдалану</span><span class="sxs-lookup"><span data-stu-id="4aec9-125">Using journals to record costs</span></span>

<span data-ttu-id="4aec9-126">PSA жүйесінде журналдар құнды немесе материалдағы, алымдағы, уақыттағы, шығыстағы табысты немесе салық транзакцияларының кластарын жазуға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="4aec9-126">In PSA, journals let you record cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="4aec9-127">Журналдың тақырыбы, жолдары және **Растау** әрекеті бар.</span><span class="sxs-lookup"><span data-stu-id="4aec9-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="4aec9-128">Журналды пайдалануға болатын бірнеше сценарийлер:</span><span class="sxs-lookup"><span data-stu-id="4aec9-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="4aec9-129">Жоба бойынша материалдық нақты шығыстар мен сатылымдарды жазуыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="4aec9-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="4aec9-130">Транзакцияның нақты мәндерін басқа жүйеден PSA жүйесіне ауыстыруыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="4aec9-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="4aec9-131">Сатып алу немесе қосымша келісімшарт құндары сияқты басқа жүйеде пайда болған құндарды жазуыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="4aec9-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="4aec9-132">Жоба оқиғаларының негізінде нақты мәндерді жазу</span><span class="sxs-lookup"><span data-stu-id="4aec9-132">Recording actuals based on project events</span></span>

<span data-ttu-id="4aec9-133">PSA жүйесі жоба барысында орын алатын барлық қаржылық операцияларды жазады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-133">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="4aec9-134">Бұл операциялар **нақты мәндер** ретінде жазылады.</span><span class="sxs-lookup"><span data-stu-id="4aec9-134">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="4aec9-135">Төмендегі кестелерде жобаның уақыт және материалдық екеніне, бағасының бекітілгеніне, алдын ала сату кезеңінде екеніне немесе ішкі жоба екеніне байланысты жасалған әртүрлі нақты мәндер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="4aec9-135">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="4aec9-136">**Ресурс жобаның келісімшарт бірлігімен бірдей ұйымдық бөлімшеге тиесілі**</span><span class="sxs-lookup"><span data-stu-id="4aec9-136">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="4aec9-137">Оқиға</span><span class="sxs-lookup"><span data-stu-id="4aec9-137">Event</span></span></th>
<th colspan="4"><span data-ttu-id="4aec9-138">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="4aec9-138">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="4aec9-139">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="4aec9-139">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="4aec9-140">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="4aec9-140">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="4aec9-141">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="4aec9-141">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="4aec9-142">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="4aec9-142">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="4aec9-143">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="4aec9-143">Actuals</span></span></th>
<th><span data-ttu-id="4aec9-144">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-144">Transaction currency</span></span></th>
<th><span data-ttu-id="4aec9-145">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="4aec9-145">Fixed price</span></span></th>
<th><span data-ttu-id="4aec9-146">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-146">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="4aec9-147">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="4aec9-147">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="4aec9-148">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="4aec9-148">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-149">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="4aec9-149">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="4aec9-150">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="4aec9-150">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4aec9-151">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="4aec9-151">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4aec9-152">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-152">Cost actual</span></span></td>
<td><span data-ttu-id="4aec9-153">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-153">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-154">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-154">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-155">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-155">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="4aec9-156">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-156">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-157">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-157">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-158">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="4aec9-158">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="4aec9-159">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-159">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4aec9-160">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="4aec9-160">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4aec9-161">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-161">Cost actual</span></span></td>
<td><span data-ttu-id="4aec9-162">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-162">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-163">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-163">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-164">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-164">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-165">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-165">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-166">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-167">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="4aec9-167">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4aec9-168">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-168">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-169">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="4aec9-169">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4aec9-170">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-170">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4aec9-171">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="4aec9-171">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4aec9-172">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-172">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4aec9-173">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-173">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-174">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-174">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-175">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-175">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-176">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-176">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-177">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-177">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-178">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-178">Billed sales</span></span></td>
<td><span data-ttu-id="4aec9-179">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4aec9-180">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="4aec9-180">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4aec9-181">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4aec9-182">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-182">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-183">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-183">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-184">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-184">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-185">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-185">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-186">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-187">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="4aec9-187">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4aec9-188">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-188">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-189">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="4aec9-189">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4aec9-190">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4aec9-191">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="4aec9-191">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4aec9-192">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-192">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4aec9-193">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-193">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="4aec9-194">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-194">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="4aec9-195">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="4aec9-195">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="4aec9-196">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-196">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4aec9-197">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-197">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="4aec9-198">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-198">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-199">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-199">Billed sales</span></span></td>
<td><span data-ttu-id="4aec9-200">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-200">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4aec9-201">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="4aec9-201">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4aec9-202">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-202">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4aec9-203">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-203">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-204">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-204">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="4aec9-205">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-205">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-206">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="4aec9-206">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="4aec9-207">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-207">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="4aec9-208">**Ресурс жобаның келісім-шарт бірлігінен өзгеше ұйымдық бөлімшеге тиесілі**</span><span class="sxs-lookup"><span data-stu-id="4aec9-208">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="4aec9-209">Оқиға</span><span class="sxs-lookup"><span data-stu-id="4aec9-209">Event</span></span></th>
<th colspan="4"><span data-ttu-id="4aec9-210">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="4aec9-210">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="4aec9-211">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="4aec9-211">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="4aec9-212">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="4aec9-212">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="4aec9-213">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="4aec9-213">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="4aec9-214">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="4aec9-214">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="4aec9-215">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="4aec9-215">Actuals</span></span></th>
<th><span data-ttu-id="4aec9-216">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-216">Transaction currency</span></span></th>
<th><span data-ttu-id="4aec9-217">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="4aec9-217">Fixed price</span></span></th>
<th><span data-ttu-id="4aec9-218">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-218">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="4aec9-219">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="4aec9-219">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="4aec9-220">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="4aec9-220">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-221">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="4aec9-221">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="4aec9-222">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="4aec9-222">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="4aec9-223">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="4aec9-223">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4aec9-224">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-224">Cost actual</span></span></td>
<td><span data-ttu-id="4aec9-225">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-225">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="4aec9-226">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-226">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="4aec9-227">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-227">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="4aec9-228">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-228">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="4aec9-229">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-229">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-230">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="4aec9-230">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="4aec9-231">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-231">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-232">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-232">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="4aec9-233">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-233">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-234">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-234">Interorganizational sales</span></span></td>
<td><span data-ttu-id="4aec9-235">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-235">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="4aec9-236">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="4aec9-236">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4aec9-237">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-237">Cost actual</span></span></td>
<td><span data-ttu-id="4aec9-238">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-238">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4aec9-239">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-239">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="4aec9-240">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-240">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4aec9-241">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-241">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="4aec9-242">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-242">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-243">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="4aec9-243">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="4aec9-244">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-244">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-245">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-245">Interorganizational sales</span></span></td>
<td><span data-ttu-id="4aec9-246">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-246">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-247">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="4aec9-247">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4aec9-248">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-248">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-249">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="4aec9-249">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4aec9-250">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-250">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4aec9-251">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="4aec9-251">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4aec9-252">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-252">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4aec9-253">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-253">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-254">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-254">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-255">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-255">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-256">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-256">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="4aec9-257">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-257">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-258">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-258">Billed sales</span></span></td>
<td><span data-ttu-id="4aec9-259">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4aec9-260">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="4aec9-260">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4aec9-261">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4aec9-262">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-262">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-263">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-263">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-264">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-264">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-265">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-265">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4aec9-266">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-267">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="4aec9-267">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4aec9-268">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-268">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-269">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="4aec9-269">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4aec9-270">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-270">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4aec9-271">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="4aec9-271">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4aec9-272">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-272">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4aec9-273">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-273">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="4aec9-274">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-274">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="4aec9-275">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="4aec9-275">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="4aec9-276">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-276">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4aec9-277">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-277">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="4aec9-278">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="4aec9-278">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-279">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-279">Billed sales</span></span></td>
<td><span data-ttu-id="4aec9-280">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-280">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4aec9-281">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="4aec9-281">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4aec9-282">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="4aec9-282">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4aec9-283">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-283">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-284">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="4aec9-284">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="4aec9-285">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-285">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4aec9-286">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="4aec9-286">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="4aec9-287">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="4aec9-287">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
