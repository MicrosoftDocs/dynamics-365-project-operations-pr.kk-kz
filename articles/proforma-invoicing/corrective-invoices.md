---
title: Жобаға негізделген түзетпе есеп-шоттары
description: Бұл тақырыпта Project Operations бағдарламасында жобаға негізделген түзетпе есеп-шоттарды жасау және растау туралы ақпарат берілген.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6b6670f823577bf7f784443f97f0b77e1e9a6aa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012278"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="6207d-103">Жобаға негізделген түзетпе есеп-шоттары</span><span class="sxs-lookup"><span data-stu-id="6207d-103">Corrective project-based invoices</span></span>

<span data-ttu-id="6207d-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="6207d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="6207d-105">Тұтынушымен және жоба менеджерімен келісілген өзгертулерді немесе кредиттерді өңдеу үшін расталған жоба есеп-шоттарын түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="6207d-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="6207d-106">Расталған есеп-шотқа түзетулер енгізу үшін расталған есеп-шотты ашып, **Осы есеп-шотты түзету** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="6207d-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="6207d-107">Егер жоба есеп-шоты расталмаса немесе жобаға негізделген есеп-шотта аванстар немесе қаламақылар немесе аванстар мен қаламақылар біріктірілмесе, бұл таңдау қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="6207d-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="6207d-108">Расталған есеп-шоттан жаңа жоба есеп-шоты жасалады.</span><span class="sxs-lookup"><span data-stu-id="6207d-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="6207d-109">Алдында расталған есеп-шоттағы барлық есеп-шот жолы туралы мәліметтер жаңа жобаға көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="6207d-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="6207d-110">Төменде жаңа түзетілген есеп-шоттағы жол мәліметтері туралы түсінуге болатын бірнеше маңызды жағдайлар келтірілген:</span><span class="sxs-lookup"><span data-stu-id="6207d-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="6207d-111">Барлық шамалар нөлге дейін жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="6207d-111">All quantities are updated to zero.</span></span> <span data-ttu-id="6207d-112">Dynamics 365 Project Operations барлық есеп-шоттар толығымен есептелген деп болжайды.</span><span class="sxs-lookup"><span data-stu-id="6207d-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="6207d-113">Қажет болса, бұл шамаларды есепке алынған соманы емес, есеп-шотты көрсететін мөлшерде қолмен жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="6207d-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="6207d-114">Енгізілген санға сүйене отырып, бағдарлама жазылған соманы есептейді.</span><span class="sxs-lookup"><span data-stu-id="6207d-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="6207d-115">Бұл сома түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштерде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="6207d-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="6207d-116">Егер сіз салық мөлшеріне өзгертулер енгізсеңіз, онда сіз есептелетін салық мөлшерін емес, дұрыс салық мөлшерін енгізуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="6207d-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="6207d-117">Аралық кезең түзетулері әрдайым толық кредиттер ретінде өңделеді.</span><span class="sxs-lookup"><span data-stu-id="6207d-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="6207d-118">Басқа шот ұсынылған төлемдер үшін түзетулер болып табылатын есеп-шоттар туралы мәліметтерде **Түзету** өрісі **Иә** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="6207d-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="6207d-119">Есеп-шоттар туралы мәліметтерді түзеткен есеп-шоттар үшін **Түзетулері бар** өрісі **Иә** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="6207d-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="6207d-120">Түзетуші есеп-шотты растау бойынша жасалған нақты көрсеткіштер</span><span class="sxs-lookup"><span data-stu-id="6207d-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="6207d-121">Төмендегі кестеде түзетілген есеп-шот расталған кезде жасалатын нақты көрсеткіштер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="6207d-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="6207d-122">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="6207d-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="6207d-123">
                    <strong>Растау бойынша жасалған нақты көрсеткіштер</strong>
                </span><span class="sxs-lookup"><span data-stu-id="6207d-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6207d-124">Бұрын есеп-шот ұсынылған уақыт транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-125">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-126">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі сағат және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6207d-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="6207d-127">Уақыт транзакциясы бойынша жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-128">Уақыт үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған сағат пен сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-129">Сағаттар мен сома бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="6207d-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-130">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған сағат пен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6207d-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6207d-131">Бұрын есеп-шот ұсынылған шығыс транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-132">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-133">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6207d-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="6207d-134">Бұрын есеп-шот ұсынылған шығыс транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-135">Шығыс үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-136">Мөлшер бойынша және түзетілген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="6207d-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-137">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған мөлшер мен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6207d-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6207d-138">Бұрын есеп-шот ұсынылған материалдық транзакцияның толық несиесіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-139">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-140">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін жаңа шот ұсынылмаған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="6207d-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="6207d-141">Материалдық транзакция бойынша ішінара несие бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-142">Материал үшін бастапқы есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-143">Өңделген есеп-шот жолы туралы мәлімет бойынша саны мен мөлшері үшін ақы алынатын шот ұсынылмаған сатылымдардың нақты көрсеткіші және кері мәні болатын балама шот ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="6207d-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-144">Есеп-шот жолы мәліметіндегі түзетілген сандарды шегергеннен кейін қалған мөлшер мен сома үшін ақылы жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6207d-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6207d-145">Бұрын есеп-шот ұсынылған ақы транзакциясының толық кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-146">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-147">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі мөлшер және сома үшін жаңа шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="6207d-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="6207d-148">Бұрын есеп-шот ұсынылған ақы транзакциясының жартылай кредитіне есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-149">Ақы үшін бастапқы есеп-шот жолы мәліметіндегі есеп-шот ұсынылған мөлшер және сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-150">Мөлшер бойынша және өңделген түзетуші есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="6207d-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="6207d-151">Бұрын есеп-шот ұсынылған аралық кезеңнің толық кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-152">Аралық кезең үшін бастапқы есеп-шот жолы мәліметіндегі сома үшін шот ұсынылған сатылымды кері бағыттау.</span><span class="sxs-lookup"><span data-stu-id="6207d-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="6207d-153">Аралық кезеңдегі есеп-шот күйі <b>Тұтынушы есеп-шоты жарияланды</b> күйінен <b>Есеп-шот ұсынуға дайын</b> күйіне жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="6207d-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="6207d-154">Бұрын есеп-шот ұсынылған аралық кезеңнің жартылай кредитіне есеп шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="6207d-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="6207d-155">Бұл сценарийге қолдау көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="6207d-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
