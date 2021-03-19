---
title: Проформа-шотын растау
description: Бұл тақырыпта проформа есеп-шотын растау туралы ақпарат берілген.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b2ed241509d2643d841ce55777e6e316612f70b8
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287875"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="a30ea-103">Проформа-шотын растау</span><span class="sxs-lookup"><span data-stu-id="a30ea-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="a30ea-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="a30ea-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a30ea-105">Алдын ала жазылатын есеп-шот расталғаннан кейін, жоба есеп-шотының күйі **Расталған** күйге жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="a30ea-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="a30ea-106">Есеп-шот расталған кезде, ол тек оқуға арналған күйде болады.</span><span class="sxs-lookup"><span data-stu-id="a30ea-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="a30ea-107">Әрі қарай, есеп-шотты тұтынушы арқылы басталған түзетулер немесе несиелер болған жағдайда немесе ол төленген деп белгіленген жағдайда ғана түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="a30ea-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="a30ea-108">Келесі кестеде жүйе арқылы жасалған нақты көрсеткіштер келтірілген.</span><span class="sxs-lookup"><span data-stu-id="a30ea-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="a30ea-109">Бұл нақты көрсеткіштер жоба есеп-шотында ол расталмай тұрып белгілі бір операциялар жасалған кезде жасалады.</span><span class="sxs-lookup"><span data-stu-id="a30ea-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="a30ea-110">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a30ea-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="a30ea-111">
                    <strong>Растау бойынша жасалған нақты көрсеткіштер</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a30ea-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a30ea-112">Есеп-шот жобасы бойынша ешқандай түзетулерсіз уақыт операциялары бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="a30ea-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-113">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="a30ea-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-114">Бастапқы уақыт келісімінде сағат пен сомаға ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="a30ea-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a30ea-115">Санын азайту үшін өңделген уақыт операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="a30ea-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-116">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="a30ea-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-117">Сағат бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="a30ea-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-118">Есеп-шоттың редакцияланатын жолында түзетілген сандарды шегергеннен кейін қалған сағат пен сомаға төленбейтін жаңа төленбеген нақты сату көлемі, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="a30ea-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a30ea-119">Санын арттыру үшін өңделген уақыт операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="a30ea-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-120">Бастапқы уақытты бекіту кезінде сағат пен соманы есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="a30ea-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-121">Сағат бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="a30ea-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a30ea-122">Есеп-шот жобасы бойынша ешқандай түзетулерсіз шығыс операциялары бойынша есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="a30ea-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-123">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="a30ea-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-124">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="a30ea-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a30ea-125">Санын азайту үшін өңделген шығыс операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="a30ea-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-126">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="a30ea-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-127">Саны бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="a30ea-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-128">Есеп-шоттың редакцияланатын жолында түзетілген сандарды шегергеннен кейін қалған сан мен сомаға төленбейтін жаңа төленбеген нақты сату көлемі, сатылымдық нақты көрсеткіштің түзетпесі және ұсынылған сатылымдық нақты көрсеткіштің баламасы.</span><span class="sxs-lookup"><span data-stu-id="a30ea-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a30ea-129">Санын арттыру үшін өңделген шығыс операциясы есеп-шотын ұсыну.</span><span class="sxs-lookup"><span data-stu-id="a30ea-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-130">Шығындардың бастапқы келісімі бойынша саны мен сомасы бойынша ұсынылмаған сатылымды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="a30ea-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-131">Саны бойынша және өңделген есеп-шот жолы мәліметтеріндегі сома бойынша ақылы жаңа сатылымның ұсынылмаған сатылымдық нақты көрсеткіші, өңделмеген сатылымдық нақты көрсеткіштің түзетпесі және баламалы ұсынылған сатылымдық нақты көрсеткіш.</span><span class="sxs-lookup"><span data-stu-id="a30ea-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a30ea-132">Төлемге арналған есеп-шот.</span><span class="sxs-lookup"><span data-stu-id="a30ea-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-133">Бастапқы журнал жолында төлем сомасын есептемей сатуды қалпына келтіру.</span><span class="sxs-lookup"><span data-stu-id="a30ea-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-134">Бастапқы төлем журнал жолы бойынша саны мен сомасы бойынша ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="a30ea-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="a30ea-135">Кезең үшін есеп-шот ұсыну.</span><span class="sxs-lookup"><span data-stu-id="a30ea-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a30ea-136">Жобаның келісім-шарт жолындағы бастапқы кезеңдегі маңызды кезең үшін ұсынылған сатылымның нақты көрсеткіші.</span><span class="sxs-lookup"><span data-stu-id="a30ea-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]