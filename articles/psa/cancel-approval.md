---
title: Бұрын бекітілген уақыт пен шығындар туралы жазбалардан бас тарту
description: Бұл тақырыпта бекітілген жобаның уақыт пен шығындар транзакциясынан бас тарту жолы туралы ақпарат берілген.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
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
ms.openlocfilehash: bf3d146d2b07723b4d2e6e85eafd6f1b23b8b83f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014753"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a><span data-ttu-id="28b88-103">Бұрын бекітілген уақыт немесе шығындар туралы жазбалардан бас тарту</span><span class="sxs-lookup"><span data-stu-id="28b88-103">Cancel previously approved time or expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="28b88-104">Dynamics 365 Project Service Automation бағдарламасының соңғы нұсқасында бекітушілер бұрын бекіткен уақыт немесе шығындар туралы жазбалардан бас тарта алады.</span><span class="sxs-lookup"><span data-stu-id="28b88-104">In the latest version of Dynamics 365 Project Service Automation, approvers can cancel time or expense entries that they previously approved.</span></span>

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a><span data-ttu-id="28b88-105">Бұрын бекітілген уақыт немесе шығындар туралы жазбадан бас тарту</span><span class="sxs-lookup"><span data-stu-id="28b88-105">Cancel a previously approved time or expense entry</span></span>

<span data-ttu-id="28b88-106">Бұрын бекітілген уақыт немесе шығындар туралы жазбадан бас тарту үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="28b88-106">Follow these steps to cancel a time or expense entry that you previously approved.</span></span>

1. <span data-ttu-id="28b88-107">**Жобалар** \> **Менің жұмысым** \> **Бекітулер** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="28b88-107">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="28b88-108">**Бекітулер** тізім бетінде көріністі **Менің өткен бекітулерім** көрінісіне өзгертіңіз.</span><span class="sxs-lookup"><span data-stu-id="28b88-108">On the **Approvals** list page, change the view to **My past approvals**.</span></span> <span data-ttu-id="28b88-109">Осы кезде сіз бұрын бекіткен уақыт немесе шығындар туралы жазбалардың тізімі көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="28b88-109">A list of the time and expense entries that you previously approved is shown.</span></span>
3. <span data-ttu-id="28b88-110">Бір немесе бірнеше жазбаны таңдап, **Бекітуден бас тарту** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="28b88-110">Select one or more entries, and then select **Cancel approval**.</span></span> <span data-ttu-id="28b88-111">Сізге ескерту хабары көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="28b88-111">You receive a warning message.</span></span>
4. <span data-ttu-id="28b88-112">Бекітуден бас тарту үшін **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="28b88-112">Select **OK** to cancel the approval.</span></span>

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a><span data-ttu-id="28b88-113">Уақыт немесе шығындар туралы жазба бекітуінен бас тарту әсері туралы жалпы ақпарат</span><span class="sxs-lookup"><span data-stu-id="28b88-113">Understand the impact of canceling a time or expense entry approval</span></span>

<span data-ttu-id="28b88-114">Бекітуден бас тартылған кезде, бұл операциялық және қаржылық әсер тигізеді.</span><span class="sxs-lookup"><span data-stu-id="28b88-114">When an approval is canceled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="28b88-115">Операциялық әсер</span><span class="sxs-lookup"><span data-stu-id="28b88-115">Operational impact</span></span>

<span data-ttu-id="28b88-116">Операцияларда бекітуден бас тартылған кезде, жазбаның күйі **Жоба** күйіне қалпына келтіріледі және бекіту бұдан былай **Менің өткен бекітулерім** көрінісінде пайда болмайды.</span><span class="sxs-lookup"><span data-stu-id="28b88-116">On the operations side, when an approval is canceled, the status of the record is reset to **Draft**, and the approval no longer appears in the **My past approvals** view.</span></span> <span data-ttu-id="28b88-117">Оның орнына, бас тартылған бекіту уақыт жазбасы немесе шығын жазбасы екеніне байланысты, **Бекітілетін уақыт жазбалары** немесе **Бекітілетін шығын жазбалары** көріністерінің біреуінде пайда болады.</span><span class="sxs-lookup"><span data-stu-id="28b88-117">Instead, the canceled approval appears in either the **Time entries for approval** view or the **Expense entries for approval** view, depending on whether it was a time entry or an expense entry.</span></span> <span data-ttu-id="28b88-118">Сонымен қатар жазба **Жоба** күйіндегі бекітулерге сәйкес болуы үшін, қатысты уақыт немесе шығын жазбасының күйі **Жіберілді** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="28b88-118">Additionally, the status of the related time or expense entry is changed to **Submitted**, so that the related entry is consistent with approvals that have a status of **Draft**.</span></span>

<span data-ttu-id="28b88-119">Бекітуші ретінде, сіз **Жоба** күйіндегі бекітулердің кейбір өрістерін өңдей аласыз.</span><span class="sxs-lookup"><span data-stu-id="28b88-119">As an approver, you can edit some of the fields of an approval that has a status of **Draft**.</span></span> <span data-ttu-id="28b88-120">Бұл өрістер **Есеп-шот ұсыну түрі** және **Уақыт жазбалары есеп-шот ұсыну сағаттары** өрістерін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="28b88-120">These fields include **Billing Type** and **Billable Hours for Time Entries**.</span></span> <span data-ttu-id="28b88-121">Өзгерістер енгізгеннен кейін, жазбаны қайта бекітуге болады.</span><span class="sxs-lookup"><span data-stu-id="28b88-121">After you make changes, you can approve the record again.</span></span> <span data-ttu-id="28b88-122">Не болмаса, жазбадан бас тартуға болады.</span><span class="sxs-lookup"><span data-stu-id="28b88-122">Alternatively, you can reject the entry.</span></span> <span data-ttu-id="28b88-123">Егер уақыт жазбасын бекітуден бас тартсаңыз, жазбаның күйі **Қайтарылған** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="28b88-123">If you reject the approval of a time entry, the status of the entry is changed to **Returned**.</span></span> <span data-ttu-id="28b88-124">Егер шығын жазбасын бекітуден бас тартсаңыз, жазбаның күйі **Бас тарылған** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="28b88-124">If you reject the approval of an expense entry, the status is changed to **Rejected**.</span></span> <span data-ttu-id="28b88-125">Функционалды түрде, қайтарылған және бас тартылған жазбалар **Жоба** күйіндегі жазба сияқты бірдей әрекет етеді.</span><span class="sxs-lookup"><span data-stu-id="28b88-125">Functionally, both returned and rejected entries behave the same as an entry that has a status of **Draft**.</span></span> <span data-ttu-id="28b88-126">Жобалық топ мүшесі жазбаға қандай да бір қажетті өзгерістерді енгізіп, оны бекіту үшін қайта жібере алады немесе жазбаны толығымен жоя алады.</span><span class="sxs-lookup"><span data-stu-id="28b88-126">A project team member can either make any required changes to the entry and then resubmit it for approval, or delete the entry entirely.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="28b88-127">Қаржылық әсер</span><span class="sxs-lookup"><span data-stu-id="28b88-127">Financial impact</span></span>

<span data-ttu-id="28b88-128">Бекітуден бас тарту жобаға қаржылық жағынан да әсер етеді.</span><span class="sxs-lookup"><span data-stu-id="28b88-128">A project is also affected financially when an approval is canceled.</span></span> <span data-ttu-id="28b88-129">Алдымен, шығындар мен сатылымдардың тиісті нақты мәндері келесі жолмен жаңартылады:</span><span class="sxs-lookup"><span data-stu-id="28b88-129">First, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="28b88-130">Реттеу күйі **Реттелген** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="28b88-130">The adjustment status is set to **Adjusted**.</span></span>
- <span data-ttu-id="28b88-131">Есеп-шот ұсыну күйі **Бас тартылды** күйіне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="28b88-131">The billing status is set to **Canceled**.</span></span>

<span data-ttu-id="28b88-132">Содан кейін "Нақты мәндер" кестесінде кері бағытталған жазбалар жасалады.</span><span class="sxs-lookup"><span data-stu-id="28b88-132">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="28b88-133">Кері бағытталған жазбаларды жасау үшін, жүйе бастапқы нақты мәндерден өрістердің мәндерін көшіреді.</span><span class="sxs-lookup"><span data-stu-id="28b88-133">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="28b88-134">Көшірілмейтін жалғыз мәндер — сандық мәндер.</span><span class="sxs-lookup"><span data-stu-id="28b88-134">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="28b88-135">Оның орнына, бұл мәндер кері бағытталады.</span><span class="sxs-lookup"><span data-stu-id="28b88-135">These values are reversed instead.</span></span> <span data-ttu-id="28b88-136">Кері бағытталған нақты мәндер **Құн** және **Шот ұсынылмаған сатылым** нақты мәндері үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="28b88-136">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="28b88-137">Кері бағытталған нақты мәндердегі **Реттеу күйі** өрісі **Реттелмейді** күйіне және есеп-шот ұсыну күйі **Бас тартылды** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="28b88-137">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the billing status is set to **Canceled**.</span></span>

<span data-ttu-id="28b88-138">Осы өзгерістер енгізілгеннен кейін, жобаға жұмсалған сома ретінде есептелген сома мен жоба бойынша тапсырыстар қоржыны осы нақты мәндер көрсететін сомалар үшін ұзақ уақыт бойы есептеледі.</span><span class="sxs-lookup"><span data-stu-id="28b88-138">After these changes are made, the amount that is recorded as spent on the project and the revenue backlog on the project will longer account for the amounts that these actuals represent.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]