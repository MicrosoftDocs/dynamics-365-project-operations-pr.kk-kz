---
title: Жобаның түзетпе есеп-шоттары
description: Бұл тақырыпта Project Operations бағдарламасында түзетпе есеп-шоттарды жасау және растау туралы ақпарат берілген.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: dfa5535597ee6e144259c9246b33075f3492285e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004088"
---
# <a name="corrective-project-invoices"></a><span data-ttu-id="b9b0e-103">Жобаның түзетпе есеп-шоттары</span><span class="sxs-lookup"><span data-stu-id="b9b0e-103">Corrective project invoices</span></span>

<span data-ttu-id="b9b0e-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="b9b0e-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b9b0e-105">Тұтынушымен және жоба менеджерімен келісілген өзгертулерді немесе кредиттерді өңдеу үшін расталған жоба есеп-шоттарын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="b9b0e-106">Расталған есеп-шотқа түзетулер енгізу үшін расталған есеп-шотты ашып, **Осы есеп-шотты түзету** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="b9b0e-107">Жоба есеп-шоты расталмайынша, бұл таңдау қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="b9b0e-108">Расталған есеп-шоттан жаңа жоба есеп-шоты жасалады.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="b9b0e-109">Алдында расталған есеп-шоттағы барлық есеп-шот жолы туралы мәліметтер жаңа жобаға көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="b9b0e-110">Төменде жаңа түзетілген есеп-шоттағы жол мәліметтері туралы түсінуге болатын бірнеше маңызды жағдайлар келтірілген:</span><span class="sxs-lookup"><span data-stu-id="b9b0e-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="b9b0e-111">Барлық шамалар нөлге дейін жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-111">All quantities are updated to zero.</span></span> <span data-ttu-id="b9b0e-112">Бағдарлама барлық есеп-шот ұсынылған элементтер толығымен жазылады деп болжайды.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="b9b0e-113">Қажет болса, бұл шамаларды есепке алынған соманы емес, есеп-шотты көрсететін мөлшерде қолмен жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="b9b0e-114">Енгізілген санға сүйене отырып, бағдарлама жазылған соманы есептейді.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="b9b0e-115">Бұл сома түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштерде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="b9b0e-116">Егер сіз салық мөлшеріне өзгертулер енгізсеңіз, онда сіз есептелетін салық мөлшерін емес, дұрыс салық мөлшерін енгізуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="b9b0e-117">Бұрын расталған өнімге негізделген келісім-шарт жолдары көшірілмейді.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="b9b0e-118">Өнімге негізделген жоба есеп-шотында түзетулерді өңдеуге қолдау көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="b9b0e-119">Аралық кезең түзетулері әрдайым толық кредиттер ретінде өңделеді.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="b9b0e-120">Егер клиент дұрыс емес сома үшін есеп-шот жасаған болса, онда қаламақы немесе аванс сомасы түзетілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="b9b0e-121">Бұрын расталған есеп-шот бойынша төлемдермен салыстыру үшін дұрыс емес сома қолданылған жағдайда, қаламақы мен аванстардың салыстыруларын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b9b0e-122">Басқа есеп-шоттар бойынша түзетулер болып табылатын есеп-шот жолы мәліметтерінде **Түзету** **Иә** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="b9b0e-123">Түзетілген есеп-шот жолы мәліметтері бар есеп-шоттарда **Түзетулері бар** өрісі **Иә** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="b9b0e-124">Түзетуші есеп-шотты растау бойынша жасалған нақты көрсеткіштер</span><span class="sxs-lookup"><span data-stu-id="b9b0e-124">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="b9b0e-125">Төмендегі кестеде түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-125">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="b9b0e-126">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b9b0e-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="b9b0e-127">
                    <strong>Растау бойынша жасалған нақты көрсеткіштер</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b9b0e-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="b9b0e-128">Есеп-шот ұсынылған аванс немесе қаламақы түзетілуін растаңыз.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b9b0e-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-129">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="b9b0e-130">Бұл сома оң болып табылады, себебі ол қаламақы немесе аванстық төлем кезінде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-131">Шот ұсынылған нақты сатылымның кері бағыттау мәні бастапқы шот ұсынылған сатылымды кері бағыттау үшін қаламақы немесе аванстағы сома үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-132">Жаңа шот ұсынылған сатылымның нақты мәні қаламақыға немесе авансқа негізделген түзетілген есеп-шот жолындағы түзетілген сома үшін жасалған.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-133">Салыстыру үшін пайдаланылатын қаламақы немесе авансқа негізделген түзетілген есеп-шот жолындағы теріс соманың шот ұсынылмаған сатылымының нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="b9b0e-134">Бұрын салыстырылған қаламақы немесе аванстың түзетілуін растау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-135">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="b9b0e-136">Бұл сома оң болып табылады, ол алдыңғы салыстыру орын алған кезде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-137">Алдыңғы есеп-шоттағы сома бойынша шот ұсынылған нақты сатылымның кері бағыттау мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-138">Түзетілген қаламақы сомасы үшін жаңа шот ұсынылған сатылымның нақты мәні түзетілген есеп-шотта қолданылады.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-139">Кейінгі есеп-шоттарда салыстыру үшін пайдаланылатын қалған түзетілген қаламақының немесе аванстың теріс сомасымен шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9b0e-140">Бұрын есеп-шот ұсынылған уақыт транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-141">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-142">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="b9b0e-143">Уақыт транзакциясы бойынша жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-144">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-145">Сағаттар мен сома бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-146">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған сағат пен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9b0e-147">Бұрын есеп-шот ұсынылған шығыс транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-148">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-149">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="b9b0e-150">Бұрын есеп-шот ұсынылған шығыс транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-151">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-152">Мөлшер бойынша және түзетілген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-153">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған мөлшер мен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9b0e-154">Бұрын есеп-шот ұсынылған материалдық транзакцияның толық несиесіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-154">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-155">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-155">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-156">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін жаңа шот ұсынылмаған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="b9b0e-157">Материалдық транзакция бойынша ішінара несие бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-157">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-158">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-159">Өңделген есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін ақы алынатын шот ұсынылмаған сатылымдардың нақты көрсеткіші және кері мәні болатын балама шот ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-160">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған мөлшер мен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-160">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9b0e-161">Бұрын есеп-шот ұсынылған ақы транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-161">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-162">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-162">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-163">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-163">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b9b0e-164">Бұрын есеп-шот ұсынылған ақы транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-164">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-165">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-165">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-166">Мөлшер бойынша және өңделген түзетуші есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-166">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="b9b0e-167">Бұрын есеп-шот ұсынылған аралық кезеңнің толық кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-167">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-168">Аралық кезең үшін бастапқы есеп-шот жолы мәліметіндегі сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-168">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="b9b0e-169">Аралық кезеңдегі есеп-шот күйі <b>Тұтынушы есеп-шоты жарияланды</b> күйінен <b>Есеп-шот ұсынуға дайын</b> күйіне жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-169">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="b9b0e-170">Бұрын есеп-шот ұсынылған аралық кезеңнің жартылай кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-170">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-171">Қолдау көрсетілмейді</span><span class="sxs-lookup"><span data-stu-id="b9b0e-171">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="b9b0e-172">Бұрын есеп-шот ұсынылған өнімге негізделген келісім-шарт жолының кредиттері мен түзетулері.</span><span class="sxs-lookup"><span data-stu-id="b9b0e-172">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="b9b0e-173">Қолдау көрсетілмейді</span><span class="sxs-lookup"><span data-stu-id="b9b0e-173">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
