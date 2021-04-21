---
title: Жобаның түзетпе есеп-шоттары
description: Бұл тақырыпта Project Operations бағдарламасында түзетпе есеп-шоттарды жасау және растау туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 04/05/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ae6d881e4e68b9f467478afe9735fc3186e6b0a8
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/07/2021
ms.locfileid: "5866598"
---
# <a name="corrective-project-invoices"></a><span data-ttu-id="4b6cf-103">Жобаның түзетпе есеп-шоттары</span><span class="sxs-lookup"><span data-stu-id="4b6cf-103">Corrective project invoices</span></span>

<span data-ttu-id="4b6cf-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="4b6cf-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4b6cf-105">Тұтынушымен және жоба менеджерімен келісілген өзгертулерді немесе кредиттерді өңдеу үшін расталған жоба есеп-шоттарын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="4b6cf-106">Расталған есеп-шотқа түзетулер енгізу үшін расталған есеп-шотты ашып, **Осы есеп-шотты түзету** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="4b6cf-107">Жоба есеп-шоты расталмайынша, бұл таңдау қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="4b6cf-108">Расталған есеп-шоттан жаңа жоба есеп-шоты жасалады.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="4b6cf-109">Алдында расталған есеп-шоттағы барлық есеп-шот жолы туралы мәліметтер жаңа жобаға көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="4b6cf-110">Төменде жаңа түзетілген есеп-шоттағы жол мәліметтері туралы түсінуге болатын бірнеше маңызды жағдайлар келтірілген:</span><span class="sxs-lookup"><span data-stu-id="4b6cf-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="4b6cf-111">Барлық шамалар нөлге дейін жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-111">All quantities are updated to zero.</span></span> <span data-ttu-id="4b6cf-112">Бағдарлама барлық есеп-шот ұсынылған элементтер толығымен жазылады деп болжайды.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="4b6cf-113">Қажет болса, бұл шамаларды есепке алынған соманы емес, есеп-шотты көрсететін мөлшерде қолмен жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="4b6cf-114">Енгізілген санға сүйене отырып, бағдарлама жазылған соманы есептейді.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="4b6cf-115">Бұл сома түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштерде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="4b6cf-116">Егер сіз салық мөлшеріне өзгертулер енгізсеңіз, онда сіз есептелетін салық мөлшерін емес, дұрыс салық мөлшерін енгізуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="4b6cf-117">Бұрын расталған өнімге негізделген келісім-шарт жолдары көшірілмейді.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="4b6cf-118">Өнімге негізделген жоба есеп-шотында түзетулерді өңдеуге қолдау көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="4b6cf-119">Аралық кезең түзетулері әрдайым толық кредиттер ретінде өңделеді.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="4b6cf-120">Егер клиент дұрыс емес сома үшін есеп-шот жасаған болса, онда қаламақы немесе аванс сомасы түзетілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="4b6cf-121">Бұрын расталған есеп-шот бойынша төлемдермен салыстыру үшін дұрыс емес сома қолданылған жағдайда, қаламақы мен аванстардың салыстыруларын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4b6cf-122">Басқа есеп-шоттар бойынша түзетулер болып табылатын есеп-шот жолы мәліметтерінде **Түзету** **Иә** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="4b6cf-123">Түзетілген есеп-шот жолы мәліметтері бар есеп-шоттарда **Түзетулері бар** өрісі **Иә** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="4b6cf-124">Түзетуші есеп-шотты растау бойынша жасалған нақты көрсеткіштер</span><span class="sxs-lookup"><span data-stu-id="4b6cf-124">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="4b6cf-125">Төмендегі кестеде түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-125">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="4b6cf-126">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4b6cf-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="4b6cf-127">
                    <strong>Растау бойынша жасалған нақты көрсеткіштер</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4b6cf-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="4b6cf-128">Есеп-шот ұсынылған аванс немесе қаламақы түзетілуін растаңыз.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="4b6cf-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-129">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="4b6cf-130">Бұл сома оң болып табылады, себебі ол қаламақы немесе аванстық төлем кезінде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-131">Шот ұсынылған нақты сатылымның кері бағыттау мәні бастапқы шот ұсынылған сатылымды кері бағыттау үшін қаламақы немесе аванстағы сома үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-132">Жаңа шот ұсынылған сатылымның нақты мәні қаламақыға немесе авансқа негізделген түзетілген есеп-шот жолындағы түзетілген сома үшін жасалған.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-133">Салыстыру үшін пайдаланылатын қаламақы немесе авансқа негізделген түзетілген есеп-шот жолындағы теріс соманың шот ұсынылмаған сатылымының нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="4b6cf-134">Бұрын салыстырылған қаламақы немесе аванстың түзетілуін растау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-135">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="4b6cf-136">Бұл сома оң болып табылады, ол алдыңғы салыстыру орын алған кезде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-137">Алдыңғы есеп-шоттағы сома бойынша шот ұсынылған нақты сатылымның кері бағыттау мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-138">Түзетілген қаламақы сомасы үшін жаңа шот ұсынылған сатылымның нақты мәні түзетілген есеп-шотта қолданылады.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-139">Кейінгі есеп-шоттарда салыстыру үшін пайдаланылатын қалған түзетілген қаламақының немесе аванстың теріс сомасымен шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4b6cf-140">Бұрын есеп-шот ұсынылған уақыт транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-141">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-142">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="4b6cf-143">Уақыт транзакциясы бойынша жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-144">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-145">Сағаттар мен сома бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-146">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған сағат пен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4b6cf-147">Бұрын есеп-шот ұсынылған шығыс транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-148">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-149">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="4b6cf-150">Бұрын есеп-шот ұсынылған шығыс транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-151">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-152">Мөлшер бойынша және түзетілген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-153">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған мөлшер мен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4b6cf-154">Бұрын есеп-шот ұсынылған материалдық транзакцияның толық несиесіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-154">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-155">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-155">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-156">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін жаңа шот ұсынылмаған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="4b6cf-157">Материалдық транзакция бойынша ішінара несие бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-157">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-158">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-159">Өңделген есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін ақы алынатын шот ұсынылмаған сатылымдардың нақты көрсеткіші және кері мәні болатын балама шот ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-160">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған мөлшер мен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-160">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4b6cf-161">Бұрын есеп-шот ұсынылған ақы транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-161">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-162">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-162">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-163">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-163">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4b6cf-164">Бұрын есеп-шот ұсынылған ақы транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-164">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-165">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-165">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-166">Мөлшер бойынша және өңделген түзетуші есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-166">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="4b6cf-167">Бұрын есеп-шот ұсынылған аралық кезеңнің толық кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-167">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-168">Аралық кезең үшін бастапқы есеп-шот жолы мәліметіндегі сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-168">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="4b6cf-169">Аралық кезеңдегі есеп-шот күйі <b>Тұтынушы есеп-шоты жарияланды</b> күйінен <b>Есеп-шот ұсынуға дайын</b> күйіне жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-169">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="4b6cf-170">Бұрын есеп-шот ұсынылған аралық кезеңнің жартылай кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-170">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-171">Қолдау көрсетілмейді</span><span class="sxs-lookup"><span data-stu-id="4b6cf-171">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="4b6cf-172">Бұрын есеп-шот ұсынылған өнімге негізделген келісім-шарт жолының кредиттері мен түзетулері.</span><span class="sxs-lookup"><span data-stu-id="4b6cf-172">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4b6cf-173">Қолдау көрсетілмейді</span><span class="sxs-lookup"><span data-stu-id="4b6cf-173">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
