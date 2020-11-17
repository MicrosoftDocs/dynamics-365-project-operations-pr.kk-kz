---
title: Проформа-шотын растау - жеңілдетілген
description: Бұл тақырыпта Project Operations бағдарламасындағы алдын ала жазылатын есеп-шоттарды растау туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 02b671e4ad327b2448529d7119211613f3a9cb27
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176528"
---
# <a name="confirm-a-proforma-invoice---lite"></a><span data-ttu-id="0cb95-103">Проформа-шотын растау - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="0cb95-103">Confirm a proforma invoice - lite</span></span>

<span data-ttu-id="0cb95-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="0cb95-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="0cb95-105">Алдын ала жазылатын есеп-шот расталғаннан кейін, жоба есеп-шотының күйі **Расталған** күйге жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="0cb95-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="0cb95-106">Есеп-шот расталған кезде, ол тек оқуға арналған күйде болады.</span><span class="sxs-lookup"><span data-stu-id="0cb95-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="0cb95-107">Әрі қарай, есеп-шотты тұтынушы арқылы басталған түзетулер немесе несиелер болған жағдайда немесе есеп-шот төленген деп белгіленген жағдайда ғана түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="0cb95-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, of if the invoice is marked as paid.</span></span>

<span data-ttu-id="0cb95-108">Келесі кестеде жүйе арқылы жасалған нақты көрсеткіштер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="0cb95-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="0cb95-109">Бұл нақты көрсеткіштер жоба есеп-шотында ол расталмай тұрып белгілі бір операциялар жасалған кезде жасалады.</span><span class="sxs-lookup"><span data-stu-id="0cb95-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="0cb95-110">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0cb95-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="0cb95-111">
                    <strong>Растау бойынша жасалған нақты көрсеткіштер</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0cb95-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0cb95-112">Аванс немесе қаламақы есеп-шотын ұсыну</span><span class="sxs-lookup"><span data-stu-id="0cb95-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-113"><strong>Қаламақы</strong> түріндегі ұсынылған сатылым нақты көрсеткіші аванстағы немесе қаламақыдағы сомаға жасалады.</span><span class="sxs-lookup"><span data-stu-id="0cb95-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-114">Салыстыру үшін пайдаланылатын қаламақының немесе аванстың теріс мөлшеріндегі есеп-қисапсыз сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="0cb95-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0cb95-115">Есеп-шот бойынша қаламақыны немесе авансты толық тексергеннен кейін.</span><span class="sxs-lookup"><span data-stu-id="0cb95-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-116">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="0cb95-117">Бұл сома оң болып табылады, өйткені ол қаламақы немесе аванстық төлем кезінде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="0cb95-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-118">Осы есеп-шот бойынша ұсынылған нақты сатылым көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="0cb95-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0cb95-119">Есеп-шот бойынша қаламақыны немесе авансты жартылай тексергеннен кейін.</span><span class="sxs-lookup"><span data-stu-id="0cb95-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-120">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="0cb95-121">Бұл сома оң болып табылады, өйткені ол қаламақы немесе аванстық төлем кезінде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="0cb95-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-122">Осы есеп-шот бойынша ұсынылған нақты сатылым көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="0cb95-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-123">Алдағы есеп-шоттарда салыстыру үшін пайдаланылатын қаламақы немесе аванс сомасының ұсынылмаған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="0cb95-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0cb95-124">Есеп-шот жобасы бойынша ешқандай түзетулерсіз уақыт операциялары бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="0cb95-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-125">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-126">Бастапқы уақыт келісімінде сағат пен сомаға ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="0cb95-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0cb95-127">Санын азайту үшін өңделген уақыт операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="0cb95-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-128">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-129">Сағат бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="0cb95-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-130">Есеп-шоттың редакцияланатын жолында түзетілген сандарды шегергеннен кейін қалған сағаттар мен сомаға төленбейтін жаңа төленбеген нақты сату көлемі, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="0cb95-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0cb95-131">Санын арттыру үшін өңделген уақыт операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="0cb95-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-132">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-133">Сағат бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="0cb95-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0cb95-134">Есеп-шот жобасы бойынша ешқандай түзетулерсіз шығыс операциялары бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="0cb95-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-135">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-136">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылған сатылымның нақты көрсеткіші</span><span class="sxs-lookup"><span data-stu-id="0cb95-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0cb95-137">Санын азайту үшін өңделген шығыс операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="0cb95-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-138">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-139">Саны бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="0cb95-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-140">Есеп-шоттың редакцияланатын жолында түзетілген сандарды шегергеннен кейін қалған сан мен сомаға төленбейтін жаңа төленбеген нақты сату көлемі, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="0cb95-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0cb95-141">Санын арттыру үшін өңделген шығыс операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="0cb95-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-142">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-143">Саны бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="0cb95-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0cb95-144">Төлемге арналған есеп-шот.</span><span class="sxs-lookup"><span data-stu-id="0cb95-144">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-145">Бастапқы журнал жолында төлем сомасын есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="0cb95-145">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-146">Бастапқы төлем журнал жолы бойынша саны мен сомасы бойынша ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="0cb95-146">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="0cb95-147">Кезең үшін есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="0cb95-147">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-148">Жобаның келісім-шарт жолындағы бастапқы кезеңдегі маңызды кезең үшін ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="0cb95-148">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="0cb95-149">Өнімге негізделген келісім-шарт жолының есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="0cb95-149">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0cb95-150">Өнімге негізделген келісім-шарт жолынан түсетін мөлшер мен соманы көрсете отырып, нақты төлемдер сатылымы.</span><span class="sxs-lookup"><span data-stu-id="0cb95-150">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
