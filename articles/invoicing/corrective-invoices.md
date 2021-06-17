---
title: Жобаға негізделген түзетпе есеп-шоттарын жасау
description: Бұл тақырыпта Project Operations бағдарламасындағы түзетпе есеп-шоттары туралы ақпарат берілген.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f0423fe9895b91431b2a83a8fff81118205b0736
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001627"
---
# <a name="create-corrective-project-based-invoices"></a><span data-ttu-id="6b1c0-103">Жобаға негізделген түзетпе есеп-шоттарын жасау</span><span class="sxs-lookup"><span data-stu-id="6b1c0-103">Create corrective project-based invoices</span></span> 

<span data-ttu-id="6b1c0-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="6b1c0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="6b1c0-105">Тұтынушымен және жоба менеджерімен келісілген өзгертулерді немесе кредиттерді өңдеу үшін расталған жоба есеп-шоттарын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="6b1c0-106">Расталған есеп-шотқа түзетулер енгізу үшін расталған есеп-шотты ашып, **Осы есеп-шотты түзету** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="6b1c0-107">Жоба есеп-шоты расталмайынша, бұл таңдау қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="6b1c0-108">Расталған есеп-шоттан жаңа жоба есеп-шоты жасалады.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="6b1c0-109">Алдында расталған есеп-шоттағы барлық есеп-шот жолы туралы мәліметтер жаңа жобаға көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="6b1c0-110">Төменде жаңа түзетілген есеп-шоттардағы жол мәліметтері туралы көбірек білуге көмектесетін бірнеше маңызды жағдайлар келтірілген:</span><span class="sxs-lookup"><span data-stu-id="6b1c0-110">The following are some key points to help you understand more about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="6b1c0-111">Барлық шамалар нөлге дейін жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-111">All quantities are updated to zero.</span></span> <span data-ttu-id="6b1c0-112">Бұл барлық есеп-шоттар толығымен есептелген деп болжайды.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-112">This assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="6b1c0-113">Қажет болса, бұл шамаларды есепке алынған соманы емес, есеп-шотты көрсететін мөлшерде қолмен жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="6b1c0-114">Енгізілген санға сүйене отырып, бағдарлама жазылған соманы есептейді.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="6b1c0-115">Бұл сома түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштерде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="6b1c0-116">Егер сіз салық мөлшеріне өзгертулер енгізсеңіз, онда сіз есептелетін салық мөлшерін емес, дұрыс салық мөлшерін енгізуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="6b1c0-117">Аралық кезең түзетулері әрдайым толық кредиттер ретінде өңделеді.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-117">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="6b1c0-118">Егер клиент дұрыс емес сома үшін есеп-шот жасаған болса, онда қаламақы немесе аванс сомасы түзетілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-118">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="6b1c0-119">Бұрын расталған есеп-шот бойынша төлемдермен салыстыру үшін дұрыс емес сома қолданылған жағдайда, қаламақы мен аванстардың салыстыруларын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-119">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6b1c0-120">Басқа есеп-шот ұсынылған төлемдер үшін түзетулер болып табылатын есеп-шоттар туралы мәліметтерде **Түзету** өрісі **Иә** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-120">Invoice line details that are corrections to other already invoiced charges have the **Correction** field set to **Yes**.</span></span> <span data-ttu-id="6b1c0-121">Түзетілген есеп-шот жолы мәліметтері бар есеп-шоттарда **Түзетулері бар** өрісі **Иә** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-121">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="6b1c0-122">Түзетуші есеп-шотты растау бойынша жасалған нақты көрсеткіштер</span><span class="sxs-lookup"><span data-stu-id="6b1c0-122">Actuals created on confirmation of a corrective invoice</span></span>

<span data-ttu-id="6b1c0-123">Төмендегі кестеде түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-123">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="6b1c0-124">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="6b1c0-124">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="6b1c0-125">
                    <strong>Растау бойынша жасалған нақты көрсеткіштер</strong>
                </span><span class="sxs-lookup"><span data-stu-id="6b1c0-125">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="6b1c0-126">Есеп-шот ұсынылған аванс немесе қаламақы түзетілуін растаңыз.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="6b1c0-126">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-127">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-127">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="6b1c0-128">Бұл сома оң болып табылады, себебі ол қаламақы немесе аванстық төлем кезінде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-128">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-129">Шот ұсынылған нақты сатылымның кері бағыттау мәні бастапқы шот ұсынылған сатылымды кері бағыттау үшін қаламақы немесе аванстағы сома үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-129">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-130">Жаңа шот ұсынылған сатылымның нақты мәні қаламақыға немесе авансқа негізделген түзетілген есеп-шот жолындағы түзетілген сома үшін жасалған.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-130">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-131">Салыстыру үшін пайдаланылатын қаламақы немесе авансқа негізделген түзетілген есеп-шот жолындағы теріс соманың шот ұсынылмаған сатылымының нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-131">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="6b1c0-132">Бұрын салыстырылған қаламақы немесе аванстың түзетілуін растау.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-132">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-133">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-133">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="6b1c0-134">Бұл сома оң болып табылады, ол алдыңғы салыстыру орын алған кезде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-134">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-135">Алдыңғы есеп-шоттағы сома бойынша шот ұсынылған нақты сатылымның кері бағыттау мәні.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-135">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-136">Түзетілген қаламақы сомасы үшін жаңа шот ұсынылған сатылымның нақты мәні түзетілген есеп-шотта қолданылады.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-136">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-137">Кейінгі есеп-шоттарда салыстыру үшін пайдаланылатын қалған түзетілген қаламақының немесе аванстың теріс сомасымен шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-137">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6b1c0-138">Бұрын есеп-шот ұсынылған уақыт транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-138">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-139">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-139">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-140">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-140">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="6b1c0-141">Уақыт транзакциясы бойынша жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-141">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-142">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-142">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-143">Сағаттар мен сома бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-143">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-144">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған сағат пен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-144">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6b1c0-145">Бұрын есеп-шот ұсынылған шығыс транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-145">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-146">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-147">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="6b1c0-148">Бұрын есеп-шот ұсынылған шығыс транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-148">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-149">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-150">Мөлшер бойынша және түзетілген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-150">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-151">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған мөлшер мен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-151">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6b1c0-152">Бұрын есеп-шот ұсынылған ақы транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-152">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-153">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-153">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-154">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-154">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6b1c0-155">Бұрын есеп-шот ұсынылған ақы транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-155">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-156">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-156">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-157">Мөлшер бойынша және өңделген түзетуші есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-157">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="6b1c0-158">Бұрын есеп-шот ұсынылған аралық кезеңнің толық кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-158">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-159">Аралық кезең үшін бастапқы есеп-шот жолы мәліметіндегі сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-159">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="6b1c0-160">Аралық кезеңдегі есеп-шот күйі <b>Тұтынушы есеп-шоты жарияланды</b> күйінен <b>Есеп-шот ұсынуға дайын</b> күйіне жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-160">The invoice status on the milestone is updated from <b>Customer invoice posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="6b1c0-161">Бұрын есеп-шот ұсынылған аралық кезеңнің жартылай кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6b1c0-161">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6b1c0-162">Қолдау көрсетілмейді</span><span class="sxs-lookup"><span data-stu-id="6b1c0-162">Unsupported</span></span> </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
