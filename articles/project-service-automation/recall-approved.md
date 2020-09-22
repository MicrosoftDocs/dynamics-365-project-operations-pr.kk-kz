---
title: Бекітілген уақыт немесе шығындар туралы жазбаларды кері қайтару
description: Бұл тақырыпта бұрын бекітілген уақыт немесе шығындар транзакциясын кері қайтару жолы туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 03/08/2019
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 2.x and 3.x
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 74df6e196c9f060f957d79aebc9640a162fb2913
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753148"
---
# <a name="recall-approved-time-or-expense-entries"></a><span data-ttu-id="adaed-103">Бекітілген уақыт немесе шығындар туралы жазбаларды кері қайтару</span><span class="sxs-lookup"><span data-stu-id="adaed-103">Recall approved time or expense entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="adaed-104">Жоба тобының мүшесі немесе уақыт немесе шығындар туралы жазбаны ұсынатын басқа адам уақыт немесе шығындар туралы жазба мақұлданғаннан кейін оны кері қайтара алады.</span><span class="sxs-lookup"><span data-stu-id="adaed-104">A project team member or an other person who submits a time or expense entry can recall that time or expense entry after it has been approved.</span></span> <span data-ttu-id="adaed-105">Бекітілген уақыт немесе шығындар туралы жазбаны кері қайтару процесі екі қадамнан тұрады:</span><span class="sxs-lookup"><span data-stu-id="adaed-105">The process for recalling an approved time or expense entry has two steps:</span></span>

1. <span data-ttu-id="adaed-106">Өтініш беруші кері қайтару әрекетіне сұрау жасайды.</span><span class="sxs-lookup"><span data-stu-id="adaed-106">A submitter requests a recall.</span></span>
2. <span data-ttu-id="adaed-107">Бекітуші кері қайтару сұрауын мақұлдайды.</span><span class="sxs-lookup"><span data-stu-id="adaed-107">An approver approves the recall.</span></span>

## <a name="request-a-recall"></a><span data-ttu-id="adaed-108">Кері қайтару сұрауы</span><span class="sxs-lookup"><span data-stu-id="adaed-108">Request a recall</span></span>

<span data-ttu-id="adaed-109">Бекітілген уақыт немесе шығындар туралы жазбаны кері қайтару үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-109">Follow these steps to request a recall of an approved time or expense entry.</span></span>

1. <span data-ttu-id="adaed-110">Уақыт жазбалары үшін **Жобалар** \> **Менің жұмысым** \> **Уақыт жазбасы** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="adaed-110">For time entries, go to **Projects** \> **My Work** \> **Time Entry**.</span></span>

    <span data-ttu-id="adaed-111">-немесе-</span><span class="sxs-lookup"><span data-stu-id="adaed-111">–or–</span></span>

    <span data-ttu-id="adaed-112">Шығындар туралы жазбалар үшін **Жобалар** \> **Менің жұмысым** \> **Шығындар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="adaed-112">For expense entries, go to **Projects** \> **My Work** \> **Expenses**.</span></span>

2. <span data-ttu-id="adaed-113">Уақыт жазбалары үшін жоба мен тапсырманың нақты тіркесімі үшін барлық уақыт жазбаларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-113">For time entries, select all the time entries for a specific combination of a project and a task.</span></span> <span data-ttu-id="adaed-114">Не болмаса, торда, белгілі бір жобаның нақты күн бойынша уақыттың жеке ұяшықтарын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-114">Alternatively, in the grid, select the individual cells for time on a specific date for a specific project.</span></span>

    <span data-ttu-id="adaed-115">-немесе-</span><span class="sxs-lookup"><span data-stu-id="adaed-115">–or–</span></span>

    <span data-ttu-id="adaed-116">Шығындар туралы жазбалар үшін кері қайтарылатын шығындар туралы жазба жолын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-116">For expense entries, select the row for the expense entry to recall.</span></span>

3. <span data-ttu-id="adaed-117">**Кері қайтару** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-117">Select **Recall**.</span></span> <span data-ttu-id="adaed-118">Растау диалогтық терезесі көрінеді.</span><span class="sxs-lookup"><span data-stu-id="adaed-118">A confirmation dialog box appears.</span></span> <span data-ttu-id="adaed-119">Егер таңдалған уақыт пен шығындар туралы жазбалар бұрыннан мақұлданған болса, сізден кері қайтару себебін енгізу сұралады.</span><span class="sxs-lookup"><span data-stu-id="adaed-119">If the selected time and expense entries were already approved, you're prompted to enter a reason for the recall.</span></span>
4. <span data-ttu-id="adaed-120">Кері қайтару себебін енгізіп, операцияны растау үшін **OK** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-120">Enter a reason for the recall, and then select **OK** to confirm the operation.</span></span> <span data-ttu-id="adaed-121">Жүйе жазбаларды мақұлдаған адамға кері қайтару әрекетін мақұлдау туралы сұрау жібереді.</span><span class="sxs-lookup"><span data-stu-id="adaed-121">The system sends the person who approved the entries a request to approve the recall.</span></span>

> [!NOTE]
> <span data-ttu-id="adaed-122">Бекітілген уақыт пен шығындар туралы жазбаларды кері қайтаруға болатынына қарамастан, егер бекітілген уақыт немесе шығыстар бойынша есеп-шот тұтынушыға ұсынылған болса, кері қайтару сұрауын жасау мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="adaed-122">Although approved time and expense entries can be recalled, if an approved time or expense has already been invoiced to the customer, a recall request can't be created.</span></span> <span data-ttu-id="adaed-123">Кері қайтару сұрауын жасауға әрекет ететін пайдаланушы уақытты немесе шығындарды кері қайтаруға болмайтындығы туралы хабарлама алады, себебі оның есеп-шоты әлдеқашан ұсынылған.</span><span class="sxs-lookup"><span data-stu-id="adaed-123">A user who tries to create a recall request will receive a message that states that the time or expense can't be recalled because it was already invoiced.</span></span>

## <a name="approve-or-reject-a-recall-request"></a><span data-ttu-id="adaed-124">Кері қайтару сұрауын мақұлдау немесе қабылдамау</span><span class="sxs-lookup"><span data-stu-id="adaed-124">Approve or reject a recall request</span></span>

<span data-ttu-id="adaed-125">Кері қайтару сұрауын мақұлдау немесе қабылдамау үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-125">Follow these steps to approve or reject a recall request.</span></span>

1. <span data-ttu-id="adaed-126">**Жобалар** \> **Менің жұмысым** \> **Бекітулер** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="adaed-126">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="adaed-127">**Бекітулер** тізім бетінде көріністі **Мақұлдауға берілген кері қайтару сұраулары** көрінісіне өзгертіңіз.</span><span class="sxs-lookup"><span data-stu-id="adaed-127">On the **Approvals** list page, change the view to **Recall requests for approval**.</span></span> <span data-ttu-id="adaed-128">Жіберілген кері қайтару сұрауларының тізімі көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="adaed-128">A list of submitted recall requests is shown.</span></span>
3. <span data-ttu-id="adaed-129">Бір немесе бірнеше жазбаны таңдап, **Бекіту** немесе **Қабылдамау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-129">Select one or more entries, and then select either **Approve** or **Reject**.</span></span>
4. <span data-ttu-id="adaed-130">Егер **Бекіту** опциясын таңдасаңыз, мақұлдау әсері түсіндірілетін ескерту хабарламасын аласыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-130">If you selected **Approve**, you receive a warning message that explains the impact of the approval.</span></span> <span data-ttu-id="adaed-131">Операцияны растау үшін **OK** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="adaed-131">Select **OK** to confirm the operation.</span></span> <span data-ttu-id="adaed-132">Кері қайтару сұрауы мақұлданды.</span><span class="sxs-lookup"><span data-stu-id="adaed-132">The recall request is approved.</span></span>

    <span data-ttu-id="adaed-133">-немесе-</span><span class="sxs-lookup"><span data-stu-id="adaed-133">–or–</span></span>

    <span data-ttu-id="adaed-134">Егер **Қабылдамау** опциясын таңдасаңыз, кері қайтару сұрауы қабылданбайды.</span><span class="sxs-lookup"><span data-stu-id="adaed-134">If you selected **Reject**, the recall request is rejected.</span></span>

> [!NOTE]
> <span data-ttu-id="adaed-135">Кері қайтару әрекеті сұралған кезде, кері қайтару сұрауы мақұлданған кезде, жүйе уақыт немесе шығындар туралы жазбалар бойынша кез келген есеп-шот ұсыну әрекетінің бар-жоғын тексереді.</span><span class="sxs-lookup"><span data-stu-id="adaed-135">As when a recall is requested, when a recall is approved, the system checks for any invoicing activity on the time or expense entries.</span></span> <span data-ttu-id="adaed-136">Егер жазба бойынша есеп-шот ұсынылған болса немесе ол жобалық есеп-шотта болса, растаушы уақытты немесе шығысты кері қайтару үшін мақұлдау мүмкін еместігі туралы қате туралы хабарлама алады, себебі оның есеп-шоты әлдеқашан ұсынылған.</span><span class="sxs-lookup"><span data-stu-id="adaed-136">If an entry was already invoiced, or if it's on a draft invoice, the approver will receive an error message that states that the time or expense can't be approved for recall, because it was already invoiced.</span></span>

## <a name="impact-of-a-recall-request"></a><span data-ttu-id="adaed-137">Кері қайтару сұрауының әсері</span><span class="sxs-lookup"><span data-stu-id="adaed-137">Impact of a recall request</span></span>

<span data-ttu-id="adaed-138">Мақұлдау әрекеті кері қайтарылған кезде, бұл операциялық және қаржылық әсер тигізеді.</span><span class="sxs-lookup"><span data-stu-id="adaed-138">When an approval is recalled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="adaed-139">Операциялық әсер</span><span class="sxs-lookup"><span data-stu-id="adaed-139">Operational impact</span></span>

<span data-ttu-id="adaed-140">Егер кері қайтару сұрауы мақұлданса, мақұлдау жазбасы **Қабылданбады** ретінде белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="adaed-140">If a recall request is approved, the approval record is marked as **Rejected**.</span></span> <span data-ttu-id="adaed-141">Жазбаның күйі де **Қайтарылған** немесе **Қабылданбаған** күйінен өзгертіледі, бұл уақыт жазбасына немесе шығындар туралы жазбаға байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="adaed-141">The status of the entry is changed to either **Returned** or **Rejected**, depending on whether it's a time entry or an expense entry.</span></span>

<span data-ttu-id="adaed-142">Жоба тобының мүшесі жазбаларды көре алады, жазбаларды өңдеп, қайтадан жібере алады немесе жазбаларды толығымен жоя алады.</span><span class="sxs-lookup"><span data-stu-id="adaed-142">The project team member can view entries, edit and then resubmit entries, or delete entries entirely.</span></span>

<span data-ttu-id="adaed-143">Егер кері қайтару сұрауы қабылданбаса, жазбаның күйі **Бекітілген** күйінде қалады және жазбаны жоба тобының мүшесі немесе жоба мақұлдаушысы өңдей алмайды.</span><span class="sxs-lookup"><span data-stu-id="adaed-143">If a recall request is rejected, the status of the entry remains **Approved**, and the entry can't be edited by the project team member or the approver for the project.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="adaed-144">Қаржылық әсер</span><span class="sxs-lookup"><span data-stu-id="adaed-144">Financial impact</span></span>

<span data-ttu-id="adaed-145">Егер кері қайтару сұрауы мақұлданса, шығындар мен сатылымдардың тиісті нақты мәндері келесі жолмен жаңартылады:</span><span class="sxs-lookup"><span data-stu-id="adaed-145">If a recall request is approved, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="adaed-146">**Реттеу күйі** өрісі **Реттелген** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="adaed-146">The **Adjustment Status** field is updated to **Adjusted**.</span></span>
- <span data-ttu-id="adaed-147">**Шот күйі** өрісі **Бас тартылған** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="adaed-147">The **Billing Status** field is updated to **Canceled**.</span></span>

<span data-ttu-id="adaed-148">Содан кейін "Нақты мәндер" кестесінде кері бағытталған жазбалар жасалады.</span><span class="sxs-lookup"><span data-stu-id="adaed-148">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="adaed-149">Кері бағытталған жазбаларды жасау үшін, жүйе бастапқы нақты мәндерден өрістердің мәндерін көшіреді.</span><span class="sxs-lookup"><span data-stu-id="adaed-149">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="adaed-150">Көшірілмейтін жалғыз мәндер — сандық мәндер.</span><span class="sxs-lookup"><span data-stu-id="adaed-150">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="adaed-151">Оның орнына, бұл мәндер кері бағытталады.</span><span class="sxs-lookup"><span data-stu-id="adaed-151">These values are reversed instead.</span></span> <span data-ttu-id="adaed-152">Кері бағытталған нақты мәндер **Құн** және **Шот ұсынылмаған сатылым** нақты мәндері үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="adaed-152">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="adaed-153">Кері бағытталған нақты мәндердегі **Реттеу күйі** өрісі **Реттелмейді** күйіне және **Есеп-шот ұсыну күйі** өрісі **Бас тартылған** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="adaed-153">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the **Billing status** field is set to **Canceled**.</span></span> <span data-ttu-id="adaed-154">Осы өзгерістер себебінен, жазылған жұмсалған сома мен жоба бойынша тапсырыстар қоржыны осы нақты мәндер көрсететін сомалар үшін бұдан былай есептелмейді.</span><span class="sxs-lookup"><span data-stu-id="adaed-154">Because of these changes, the recorded spending and the revenue backlog on the project will no longer account for the amounts that these actuals represent.</span></span>

<span data-ttu-id="adaed-155">Егер кері қайтару сұрауы қабылданбаса, бұл жобаға ешқандай қаржылық әсер тигізбейді.</span><span class="sxs-lookup"><span data-stu-id="adaed-155">If a recall request is rejected, there is no financial impact on the project.</span></span>

## <a name="changes-to-time-entry-records"></a><span data-ttu-id="adaed-156">Уақыт жазбасының жазбаларына енгізілген өзгерістер</span><span class="sxs-lookup"><span data-stu-id="adaed-156">Changes to time entry records</span></span>

<span data-ttu-id="adaed-157">Төмендегі суретте кері қайтарылған кезде бекітілген уақыт жазбаларында болатын өзгерістер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="adaed-157">The following illustration shows the changes that occur for approved time entries when they are recalled.</span></span>

![Уақыт жазбасы күйінің ауысымдары](media/TimeEntryStateTransitions.png)

## <a name="changes-to-expense-entry-records"></a><span data-ttu-id="adaed-159">Шығындар жазбасы жазбаларына енгізілген өзгерістер</span><span class="sxs-lookup"><span data-stu-id="adaed-159">Changes to expense entry records</span></span>

<span data-ttu-id="adaed-160">Төмендегі суретте кері қайтарылған кезде бекітілген шығындар жазбаларында болатын өзгерістер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="adaed-160">The following illustration shows the changes that occur for approved expense entries when they are recalled.</span></span>

![Шығындар жазбасы күйінің ауысымдары](media/ExpenseEntryStateTransitions.png)
