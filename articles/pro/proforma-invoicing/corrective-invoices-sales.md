---
title: Кредиттер және түзетілген есеп-шоттар
description: Бұл тақырыпта Project Operations бағдарламасындағы түзетілген есеп-шоттар туралы ақпарат берілген
author: rumant
manager: Annbe
ms.date: 10/15/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d2187627439d42b37222dce0a491c62dafc358d5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079771"
---
# <a name="credits-and-corrected-invoices"></a><span data-ttu-id="c9cc7-103">Кредиттер және түзетілген есеп-шоттар</span><span class="sxs-lookup"><span data-stu-id="c9cc7-103">Credits and corrected invoices</span></span>

<span data-ttu-id="c9cc7-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="c9cc7-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c9cc7-105">Тұтынушымен және жоба менеджерімен келісілген өзгертулерді немесе кредиттерді өңдеу үшін расталған жоба есеп-шоттарын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="c9cc7-106">Расталған есеп-шотқа түзетулер енгізу үшін расталған есеп-шотты ашып, **Осы есеп-шотты түзету** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="c9cc7-107">Жоба есеп-шоты расталмайынша, бұл таңдау қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="c9cc7-108">Расталған есеп-шоттан жаңа жоба есеп-шоты жасалады.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="c9cc7-109">Алдында расталған есеп-шоттағы барлық есеп-шот жолы туралы мәліметтер жаңа жобаға көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="c9cc7-110">Төменде жаңа түзетілген есеп-шоттағы жол мәліметтері туралы түсінуге болатын бірнеше маңызды жағдайлар келтірілген:</span><span class="sxs-lookup"><span data-stu-id="c9cc7-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="c9cc7-111">Барлық шамалар нөлге дейін жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-111">All quantities are updated to zero.</span></span> <span data-ttu-id="c9cc7-112">Бағдарлама барлық есеп-шот ұсынылған элементтер толығымен жазылады деп болжайды.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="c9cc7-113">Қажет болса, бұл шамаларды есепке алынған соманы емес, есеп-шотты көрсететін мөлшерде қолмен жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="c9cc7-114">Енгізілген санға сүйене отырып, бағдарлама жазылған соманы есептейді.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="c9cc7-115">Бұл сома түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштерде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="c9cc7-116">Егер сіз салық мөлшеріне өзгертулер енгізсеңіз, онда сіз есептелетін салық мөлшерін емес, дұрыс салық мөлшерін енгізуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="c9cc7-117">Бұрын расталған өнімге негізделген келісім-шарт жолдары көшірілмейді.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="c9cc7-118">Өнімге негізделген жоба есеп-шотында түзетулерді өңдеуге қолдау көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="c9cc7-119">Аралық кезең түзетулері әрдайым толық кредиттер ретінде өңделеді.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="c9cc7-120">Егер клиент дұрыс емес сома үшін есеп-шот жасаған болса, онда қаламақы немесе аванс сомасы түзетілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="c9cc7-121">Бұрын расталған есеп-шот бойынша төлемдермен салыстыру үшін дұрыс емес сома қолданылған жағдайда, қаламақы мен аванстардың салыстыруларын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c9cc7-122">Басқа есеп-шоттар бойынша түзетулер болып табылатын есеп-шот жолы мәліметтерінде **Түзету** **Иә** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="c9cc7-123">Түзетілген есеп-шот жолы мәліметтері бар есеп-шоттарда **Түзетулері бар** өрісі **Иә** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="c9cc7-124">Түзетуші есеп-шотты растау бойынша жасалған нақты көрсеткіштер:</span><span class="sxs-lookup"><span data-stu-id="c9cc7-124">Actuals created on Confirmation of a corrective invoice:</span></span>

<span data-ttu-id="c9cc7-125">Төменде түзетуші есеп-шот жобасы бойынша расталғанға дейін орындалған операциялар негізінде түзетуді растауға арналған бағдарлама арқылы жасалған нақты көрсеткіштер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-125">Below are the actuals created by the application on confirmation of a corrective based on the operations performed on the draft corrective invoice before confirmation.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="c9cc7-126">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c9cc7-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="c9cc7-127">
                    <strong>Растау бойынша жасалған нақты көрсеткіштер</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c9cc7-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="c9cc7-128">Есеп-шот ұсынылған аванс немесе қаламақы түзетілуін растаңыз.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c9cc7-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-129">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="c9cc7-130">Бұл сома оң болып табылады, себебі ол қаламақы немесе аванстық төлем кезінде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-131">Шот ұсынылған нақты сатылымның кері бағыттау мәні бастапқы шот ұсынылған сатылымды кері бағыттау үшін қаламақы немесе аванстағы сома үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-132">Жаңа шот ұсынылған сатылымның нақты мәні қаламақыға немесе авансқа негізделген түзетілген есеп-шот жолындағы түзетілген сома үшін жасалған.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-133">Салыстыру үшін пайдаланылатын қаламақы немесе авансқа негізделген түзетілген есеп-шот жолындағы теріс соманың шот ұсынылмаған сатылымының нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="c9cc7-134">Бұрын салыстырылған қаламақы немесе аванстың түзетілуін растау.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-135">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="c9cc7-136">Бұл сома оң болып табылады, ол алдыңғы салыстыру орын алған кезде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-137">Алдыңғы есеп-шоттағы сома бойынша шот ұсынылған нақты сатылымның кері бағыттау мәні.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-138">Түзетілген қаламақы сомасы үшін жаңа шот ұсынылған сатылымның нақты мәні түзетілген есеп-шотта қолданылады.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-139">Кейінгі есеп-шоттарда салыстыру үшін пайдаланылатын қалған түзетілген қаламақының немесе аванстың теріс сомасымен шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9cc7-140">Бұрын есеп-шот ұсынылған уақыт транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-141">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-142">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c9cc7-143">Уақыт транзакциясы бойынша жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-144">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-145">Сағаттар мен сома бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-146">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған сағат пен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9cc7-147">Бұрын есеп-шот ұсынылған шығыс транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-148">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-149">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c9cc7-150">Бұрын есеп-шот ұсынылған шығыс транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-151">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-152">Мөлшер бойынша және түзетілген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-153">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған мөлшер мен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9cc7-154">Бұрын есеп-шот ұсынылған ақы транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-154">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-155">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-155">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-156">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9cc7-157">Бұрын есеп-шот ұсынылған ақы транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-157">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-158">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-159">Мөлшер бойынша және өңделген түзетуші есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="c9cc7-160">Бұрын есеп-шот ұсынылған аралық кезеңнің толық кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-160">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-161">Аралық кезең үшін бастапқы есеп-шот жолы мәліметіндегі сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-161">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="c9cc7-162">Жоба келісім-шарты жолындағы аралық кезең есеп-шоты немесе төлем күйі **Есеп-шот ұсынуға дайын** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-162">The milestone invoice or billing status on the project contract line is updated to **Ready to Invoice**.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="c9cc7-163">Бұрын есеп-шот ұсынылған аралық кезеңнің жартылай кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-163">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-164">Қолдау көрсетілмейді</span><span class="sxs-lookup"><span data-stu-id="c9cc7-164">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="c9cc7-165">Бұрын есеп-шот ұсынылған өнімге негізделген келісім-шарт жолының кредиттері мен түзетулері.</span><span class="sxs-lookup"><span data-stu-id="c9cc7-165">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9cc7-166">Қолдау көрсетілмейді</span><span class="sxs-lookup"><span data-stu-id="c9cc7-166">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>
