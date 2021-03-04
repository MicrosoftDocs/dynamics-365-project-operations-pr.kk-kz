---
title: Қолда бар тауарларға шолу
description: Бұл тақырыпта жобаның нақты мәндері туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 63ad6544f0ec0a893aebd8d81f3ee895e51c294e
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146130"
---
# <a name="actuals-overview"></a><span data-ttu-id="82430-103">Қолда бар тауарларға шолу</span><span class="sxs-lookup"><span data-stu-id="82430-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="82430-104">Нақты мәндер — жоба бойынша аяқталған жұмыс көлемі.</span><span class="sxs-lookup"><span data-stu-id="82430-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="82430-105">Жобаның нақты мәндерін олардың бастапқы құжаттарына белгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="82430-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="82430-106">Бұл бастапқы құжаттар уақытты, шығыстарды және журнал жазбаларын, сондай-ақ есеп-шоттарды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="82430-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Жобаның нақты мәндерін олардың бастапқы құжаттарына белгілеу жолы](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="82430-108">Осы уақыт жазбасын жіберу</span><span class="sxs-lookup"><span data-stu-id="82430-108">Submitting a time entry</span></span>

<span data-ttu-id="82430-109">PSA жүйесінде уақыт және материалдар келісім-шарт жолына тағайындалған жобаға уақыт жазбасы жіберілген кезде екі журнал жолы жасалады.</span><span class="sxs-lookup"><span data-stu-id="82430-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="82430-110">Бір жол шығынға арналған, ал екінші жол шот ұсынылмаған сатылымға арналған.</span><span class="sxs-lookup"><span data-stu-id="82430-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="82430-111">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға уақыт жазбасы жіберілген кезде журнал жолы тек құн үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="82430-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="82430-112">Әдеттегі бағаларды енгізу логикасы журнал жолында орналасқан.</span><span class="sxs-lookup"><span data-stu-id="82430-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="82430-113">Уақыт жазбасындағы барлық өріс мәндері журнал жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="82430-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="82430-114">Бұл өрістер транзакция жасалған күнді, жоба тағайындалған келісім-шарт жолын және тиісті бағатізбедегі валютаны қамтиды.</span><span class="sxs-lookup"><span data-stu-id="82430-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="82430-115">**Рөл** және **Ұйымдық бөлімше** сияқты әдепкі бағаларды көрсететін өрістер тиісті бағаның журнал жолына әдепкі бойынша енгізілуіне әкеледі.</span><span class="sxs-lookup"><span data-stu-id="82430-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="82430-116">Уақыт жазбасына реттелетін өрісті қоссаңыз және өріс мәнін нақты мәндерге тарату қажет болса, нақты мәндер нысанында өрісті жасап, өрісті уақыт жазбасынан нақты мәндер өрісіне көшіру үшін өріс салыстыруларын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="82430-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="82430-117">Шығыс жазбасын жіберу</span><span class="sxs-lookup"><span data-stu-id="82430-117">Submitting an expense entry</span></span>

<span data-ttu-id="82430-118">PSA жүйесінде уақыт және материалдар келісім-шарт жолына тағайындалған жобаға шығыс жазбасы жіберілген кезде екі журнал жолы жасалады.</span><span class="sxs-lookup"><span data-stu-id="82430-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="82430-119">Бір жол шығынға арналған, ал екінші жол шот ұсынылмаған сатылымға арналған.</span><span class="sxs-lookup"><span data-stu-id="82430-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="82430-120">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға шығыс жазбасы жіберілген кезде журнал жолы тек құн үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="82430-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="82430-121">Шығыстардың әдепкі бағаларын енгізудің логикасы **Шығыс жазбасы** бетінде таңдалған шығыс санатына негізделген.</span><span class="sxs-lookup"><span data-stu-id="82430-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="82430-122">Транзакция жасалған күн, жоба тағайындалған келісім-шарт жолы және валюта тиісті бағатізбені анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="82430-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="82430-123">Дегенмен бағаның өзі үшін пайдаланушының енгізген сомасы, әдепкі бойынша қатысты шығыстың құн және сатылым журнал жолдарына тікелей орнатылады.</span><span class="sxs-lookup"><span data-stu-id="82430-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="82430-124">PSA жүйесінің ағымдағы нұсқасында, шығыс жазбаларында бірліктің санат негізіндегі жазбасының әдепкі бағасы қолжетімді емес.</span><span class="sxs-lookup"><span data-stu-id="82430-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="82430-125">Шығыстарды жазу үшін жазба журналдарды пайдалану</span><span class="sxs-lookup"><span data-stu-id="82430-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="82430-126">PSA жүйесінде жазба журналдары құнды немесе материалдағы, алымдағы, уақыттағы, шығыстағы табысты немесе салық транзакцияларының кластарын жазуға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="82430-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="82430-127">Журналдың тақырыбы, жолдары және **Растау** әрекеті бар.</span><span class="sxs-lookup"><span data-stu-id="82430-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="82430-128">Журналды пайдалануға болатын бірнеше сценарийлер:</span><span class="sxs-lookup"><span data-stu-id="82430-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="82430-129">Жоба бойынша материалдық нақты шығыстар мен сатылымдарды жазуыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="82430-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="82430-130">Транзакцияның нақты мәндерін басқа жүйеден PSA жүйесіне ауыстыруыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="82430-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="82430-131">Сатып алу немесе қосымша келісімшарт құндары сияқты басқа жүйеде пайда болған құндарды жазуыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="82430-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="82430-132">Нақты көрсеткіштерді жасау үшін жазба журналын тек нақты көрсетіштердің жобаға тигізетін есеп әсерін жақсы білетін пайдаланушы ғана пайдалануы керек.</span><span class="sxs-lookup"><span data-stu-id="82430-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="82430-133">Себебі, бағдарлама журнал жолының түрін немесе журнал жолына енгізілген тиісті бағаны растамайды.</span><span class="sxs-lookup"><span data-stu-id="82430-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="82430-134">Осы журнал түріне байланысты, жазба журналын жасауға рұқсат берілген тұлғаға сақтық танытыңыз.</span><span class="sxs-lookup"><span data-stu-id="82430-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="82430-135">Жоба оқиғаларының негізінде нақты мәндерді жазу</span><span class="sxs-lookup"><span data-stu-id="82430-135">Recording actuals based on project events</span></span>

<span data-ttu-id="82430-136">PSA жүйесі жоба барысында орын алатын барлық қаржылық операцияларды жазады.</span><span class="sxs-lookup"><span data-stu-id="82430-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="82430-137">Бұл операциялар **нақты мәндер** ретінде жазылады.</span><span class="sxs-lookup"><span data-stu-id="82430-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="82430-138">Төмендегі кестелерде жобаның уақыт және материалдық екеніне, бағасының бекітілгеніне, алдын ала сату кезеңінде екеніне немесе ішкі жоба екеніне байланысты жасалған әртүрлі нақты мәндер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="82430-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="82430-139">**Ресурс жобаның келісімшарт бірлігімен бірдей ұйымдық бөлімшеге тиесілі**</span><span class="sxs-lookup"><span data-stu-id="82430-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="82430-140">Оқиға</span><span class="sxs-lookup"><span data-stu-id="82430-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="82430-141">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="82430-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="82430-142">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="82430-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="82430-143">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="82430-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="82430-144">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="82430-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="82430-145">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="82430-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="82430-146">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="82430-146">Actuals</span></span></th>
<th><span data-ttu-id="82430-147">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-147">Transaction currency</span></span></th>
<th><span data-ttu-id="82430-148">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="82430-148">Fixed price</span></span></th>
<th><span data-ttu-id="82430-149">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="82430-150">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="82430-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="82430-151">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="82430-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-152">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="82430-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="82430-153">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="82430-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="82430-154">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="82430-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="82430-155">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-155">Cost actual</span></span></td>
<td><span data-ttu-id="82430-156">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-157">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-158">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="82430-159">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-160">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-161">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="82430-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="82430-162">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="82430-163">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="82430-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="82430-164">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-164">Cost actual</span></span></td>
<td><span data-ttu-id="82430-165">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-166">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-167">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-168">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-169">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-170">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="82430-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="82430-171">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-172">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="82430-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="82430-173">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="82430-174">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="82430-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="82430-175">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="82430-176">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-177">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-178">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-179">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-180">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-181">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-181">Billed sales</span></span></td>
<td><span data-ttu-id="82430-182">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="82430-183">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="82430-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="82430-184">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="82430-185">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-186">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-187">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-188">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-189">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-190">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="82430-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="82430-191">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-192">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="82430-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="82430-193">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="82430-194">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="82430-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="82430-195">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="82430-196">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="82430-197">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="82430-198">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="82430-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="82430-199">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="82430-200">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="82430-201">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-202">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-202">Billed sales</span></span></td>
<td><span data-ttu-id="82430-203">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="82430-204">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="82430-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="82430-205">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="82430-206">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-207">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="82430-208">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-209">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="82430-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="82430-210">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="82430-211">**Ресурс жобаның келісім-шарт бірлігінен өзгеше ұйымдық бөлімшеге тиесілі**</span><span class="sxs-lookup"><span data-stu-id="82430-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="82430-212">Оқиға</span><span class="sxs-lookup"><span data-stu-id="82430-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="82430-213">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="82430-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="82430-214">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="82430-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="82430-215">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="82430-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="82430-216">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="82430-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="82430-217">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="82430-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="82430-218">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="82430-218">Actuals</span></span></th>
<th><span data-ttu-id="82430-219">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-219">Transaction currency</span></span></th>
<th><span data-ttu-id="82430-220">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="82430-220">Fixed price</span></span></th>
<th><span data-ttu-id="82430-221">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="82430-222">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="82430-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="82430-223">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="82430-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-224">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="82430-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="82430-225">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="82430-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="82430-226">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="82430-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="82430-227">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-227">Cost actual</span></span></td>
<td><span data-ttu-id="82430-228">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="82430-229">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="82430-230">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="82430-231">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="82430-232">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-233">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="82430-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="82430-234">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-235">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="82430-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="82430-236">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-237">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="82430-238">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="82430-239">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="82430-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="82430-240">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-240">Cost actual</span></span></td>
<td><span data-ttu-id="82430-241">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="82430-242">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="82430-243">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="82430-244">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="82430-245">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="82430-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-246">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="82430-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="82430-247">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-248">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="82430-249">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-250">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="82430-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="82430-251">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-252">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="82430-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="82430-253">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="82430-254">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="82430-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="82430-255">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="82430-256">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-257">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-258">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-259">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="82430-260">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-261">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-261">Billed sales</span></span></td>
<td><span data-ttu-id="82430-262">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="82430-263">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="82430-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="82430-264">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="82430-265">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-266">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-267">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-268">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="82430-269">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-270">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="82430-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="82430-271">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-272">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="82430-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="82430-273">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="82430-274">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="82430-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="82430-275">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="82430-276">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="82430-277">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="82430-278">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="82430-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="82430-279">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="82430-280">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="82430-281">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="82430-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-282">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-282">Billed sales</span></span></td>
<td><span data-ttu-id="82430-283">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="82430-284">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="82430-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="82430-285">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="82430-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="82430-286">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-287">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="82430-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="82430-288">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="82430-289">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="82430-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="82430-290">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="82430-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
