---
title: Проформа есеп-шотын растау
description: Бұл тақырыпта Project Operations бағдарламасындағы алдын ала жазылатын есеп-шоттарды растау туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4b67ee6848efdcb85cf732c1eaa3e40cdc51a2e2
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079568"
---
# <a name="confirming-a-proforma-invoice"></a><span data-ttu-id="c22bb-103">Проформа есеп-шотын растау</span><span class="sxs-lookup"><span data-stu-id="c22bb-103">Confirming a proforma invoice</span></span>

<span data-ttu-id="c22bb-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="c22bb-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c22bb-105">Алдын ала жазылатын есеп-шот расталғаннан кейін, жоба есеп-шотының күйі **Расталған** күйге жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="c22bb-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="c22bb-106">Есеп-шот расталған кезде, ол тек оқуға арналған күйде болады.</span><span class="sxs-lookup"><span data-stu-id="c22bb-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="c22bb-107">Әрі қарай, есеп-шотты тұтынушы арқылы басталған түзетулер немесе несиелер болған жағдайда немесе есеп-шот төленген деп белгіленген жағдайда ғана түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="c22bb-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, of if the invoice is marked as paid.</span></span>

<span data-ttu-id="c22bb-108">Келесі кестеде жүйе арқылы жасалған нақты көрсеткіштер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="c22bb-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="c22bb-109">Бұл нақты көрсеткіштер жоба есеп-шотында ол расталмай тұрып белгілі бір операциялар жасалған кезде жасалады.</span><span class="sxs-lookup"><span data-stu-id="c22bb-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="c22bb-110">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c22bb-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="c22bb-111">
                    <strong>Растау бойынша жасалған нақты көрсеткіштер</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c22bb-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c22bb-112">Аванс немесе қаламақы есеп-шотын ұсыну</span><span class="sxs-lookup"><span data-stu-id="c22bb-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-113"><strong>Қаламақы</strong> түріндегі ұсынылған сатылым нақты көрсеткіші аванстағы немесе қаламақыдағы сомаға жасалады.</span><span class="sxs-lookup"><span data-stu-id="c22bb-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-114">Салыстыру үшін пайдаланылатын қаламақының немесе аванстың теріс мөлшеріндегі есеп-қисапсыз сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="c22bb-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c22bb-115">Есеп-шот бойынша қаламақыны немесе авансты толық тексергеннен кейін.</span><span class="sxs-lookup"><span data-stu-id="c22bb-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-116">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="c22bb-117">Бұл сома оң болып табылады, өйткені ол қаламақы немесе аванстық төлем кезінде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="c22bb-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-118">Осы есеп-шот бойынша ұсынылған нақты сатылым көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="c22bb-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c22bb-119">Есеп-шот бойынша қаламақыны немесе авансты жартылай тексергеннен кейін.</span><span class="sxs-lookup"><span data-stu-id="c22bb-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-120">Салыстыру үшін жасалған қаламақы немесе аванс есебінсіз сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="c22bb-121">Бұл сома оң болып табылады, өйткені ол қаламақы немесе аванстық төлем кезінде жасалған теріс соманы жоюға арналған.</span><span class="sxs-lookup"><span data-stu-id="c22bb-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-122">Осы есеп-шот бойынша ұсынылған нақты сатылым көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="c22bb-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-123">Алдағы есеп-шоттарда салыстыру үшін пайдаланылатын қаламақы немесе аванс сомасының ұсынылмаған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="c22bb-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c22bb-124">Есеп-шот жобасы бойынша ешқандай түзетулерсіз уақыт операциялары бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c22bb-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-125">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-126">Бастапқы уақыт келісімінде сағат пен сомаға ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="c22bb-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c22bb-127">Санын азайту үшін өңделген уақыт операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c22bb-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-128">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-129">Сағат бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c22bb-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-130">Есеп-шоттың редакцияланатын жолында түзетілген сандарды шегергеннен кейін қалған сағаттар мен сомаға төленбейтін жаңа төленбеген нақты сату көлемі, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c22bb-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c22bb-131">Санын арттыру үшін өңделген уақыт операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c22bb-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-132">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-133">Сағат бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c22bb-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c22bb-134">Есеп-шот жобасы бойынша ешқандай түзетулерсіз шығыс операциялары бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c22bb-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-135">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-136">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылған сатылымның нақты көрсеткіші</span><span class="sxs-lookup"><span data-stu-id="c22bb-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c22bb-137">Санын азайту үшін өңделген шығыс операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c22bb-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-138">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-139">Саны бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c22bb-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-140">Есеп-шоттың редакцияланатын жолында түзетілген сандарды шегергеннен кейін қалған сан мен сомаға төленбейтін жаңа төленбеген нақты сату көлемі, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c22bb-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c22bb-141">Санын арттыру үшін өңделген шығыс операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c22bb-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-142">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-143">Саны бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="c22bb-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c22bb-144">Төлемге арналған есеп-шот.</span><span class="sxs-lookup"><span data-stu-id="c22bb-144">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-145">Бастапқы журнал жолында төлем сомасын есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="c22bb-145">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-146">Бастапқы төлем журнал жолы бойынша саны мен сомасы бойынша ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="c22bb-146">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="c22bb-147">Кезең үшін есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c22bb-147">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-148">Жобаның келісім-шарт жолындағы бастапқы кезеңдегі маңызды кезең үшін ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="c22bb-148">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="c22bb-149">Өнімге негізделген келісім-шарт жолының есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="c22bb-149">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c22bb-150">Өнімге негізделген келісім-шарт жолынан түсетін мөлшер мен соманы көрсете отырып, нақты төлемдер сатылымы.</span><span class="sxs-lookup"><span data-stu-id="c22bb-150">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
