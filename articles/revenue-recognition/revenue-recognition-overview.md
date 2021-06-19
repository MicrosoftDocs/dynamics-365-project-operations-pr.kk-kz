---
title: Табысты тануға шолу
description: Бұл тақырыпта Project Operations бағдарламасындағы табысты тану туралы ақпарат берілген.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: f5f962572c6ec0298d2d91d33f83e4120a498a6f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013763"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="e12ad-103">Табысты тануға шолу</span><span class="sxs-lookup"><span data-stu-id="e12ad-103">Revenue recognition overview</span></span>

<span data-ttu-id="e12ad-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="e12ad-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e12ad-105">Dynamics 365 Project Operations бағдарламасында табысты тану қағидалары жоба немесе жоба бөлігі үшін таңдалған есептеу әдісі негізінде өзгереді.</span><span class="sxs-lookup"><span data-stu-id="e12ad-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="e12ad-106">Бұл тақырыпта Project Operations бағдарламасындағы табысты тану туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="e12ad-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="e12ad-107">Уақыт пен материалдарды есепке алу әдісін пайдалана отырып есепке алынатын транзакциялар</span><span class="sxs-lookup"><span data-stu-id="e12ad-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="e12ad-108">Шығындар мен табысты тану бір-бірімен байланысты.</span><span class="sxs-lookup"><span data-stu-id="e12ad-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="e12ad-109">Транзакция құны және шот ұсынылмаған сатылымдар [Project Operations Integration журналы](../project-accounting/project-operations-integration-journal.md) арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="e12ad-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="e12ad-110">Жоба құны мен табыс профилі шот ұсынылмаған сатылым транзакциялары бас кітапқа орналастырылғанын анықтайды.</span><span class="sxs-lookup"><span data-stu-id="e12ad-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="e12ad-111">Егер **Есептелген табыс** таңдалса жүйе орналастыру кезінде **WIP сатылым мәні** және **Есептелген табыс сатылымының құны** есеп-шоттарын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e12ad-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="e12ad-112">Келесі суретте осы әдістің мысалы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="e12ad-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="e12ad-113">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="e12ad-113">Transaction type</span></span> | <span data-ttu-id="e12ad-114">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="e12ad-114">Debit/Credit</span></span> | <span data-ttu-id="e12ad-115">Сомасы</span><span class="sxs-lookup"><span data-stu-id="e12ad-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="e12ad-116">WIP сатылым құны</span><span class="sxs-lookup"><span data-stu-id="e12ad-116">WIP Sales value</span></span> | <span data-ttu-id="e12ad-117">Дебет</span><span class="sxs-lookup"><span data-stu-id="e12ad-117">Debit</span></span> | <span data-ttu-id="e12ad-118">100-көше</span><span class="sxs-lookup"><span data-stu-id="e12ad-118">100</span></span> |
  | <span data-ttu-id="e12ad-119">Есептелген табыс сатылымының құны</span><span class="sxs-lookup"><span data-stu-id="e12ad-119">Accrued revenue sales value</span></span> | <span data-ttu-id="e12ad-120">Несие</span><span class="sxs-lookup"><span data-stu-id="e12ad-120">Credit</span></span> | <span data-ttu-id="e12ad-121">100-көше</span><span class="sxs-lookup"><span data-stu-id="e12ad-121">100</span></span> |

- <span data-ttu-id="e12ad-122">Есеп-шот ұсыну кезінде табыс танылды.</span><span class="sxs-lookup"><span data-stu-id="e12ad-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="e12ad-123">Орналастыру кезінде жүйе **Есеп-шот ұсынылған табыс** пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e12ad-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="e12ad-124">Келесі суретте осы әдістің мысалы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="e12ad-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="e12ad-125">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="e12ad-125">Transaction type</span></span> | <span data-ttu-id="e12ad-126">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="e12ad-126">Debit/Credit</span></span> | <span data-ttu-id="e12ad-127">Сомасы</span><span class="sxs-lookup"><span data-stu-id="e12ad-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="e12ad-128">Тұтынушы қалдығы</span><span class="sxs-lookup"><span data-stu-id="e12ad-128">Customer balance</span></span> | <span data-ttu-id="e12ad-129">Дебет</span><span class="sxs-lookup"><span data-stu-id="e12ad-129">Debit</span></span> | <span data-ttu-id="e12ad-130">120</span><span class="sxs-lookup"><span data-stu-id="e12ad-130">120</span></span> |
  | <span data-ttu-id="e12ad-131">Төлену керек сатылым салығы</span><span class="sxs-lookup"><span data-stu-id="e12ad-131">Sales tax payable</span></span> | <span data-ttu-id="e12ad-132">Несие</span><span class="sxs-lookup"><span data-stu-id="e12ad-132">Credit</span></span> | <span data-ttu-id="e12ad-133">20</span><span class="sxs-lookup"><span data-stu-id="e12ad-133">20</span></span> |
  | <span data-ttu-id="e12ad-134">Шот-фактура бойынша табыс</span><span class="sxs-lookup"><span data-stu-id="e12ad-134">Invoiced Revenue</span></span> | <span data-ttu-id="e12ad-135">Несие</span><span class="sxs-lookup"><span data-stu-id="e12ad-135">Credit</span></span> | <span data-ttu-id="e12ad-136">100-көше</span><span class="sxs-lookup"><span data-stu-id="e12ad-136">100</span></span> |

- <span data-ttu-id="e12ad-137">Егер кіріс есептелмеген сатылымдар орналастырылған кезде есептелген болса, онда жүйе есептелген кірісті есеп-шот ұсыну кезінде қалпына келтіреді.</span><span class="sxs-lookup"><span data-stu-id="e12ad-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="e12ad-138">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="e12ad-138">Transaction type</span></span> | <span data-ttu-id="e12ad-139">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="e12ad-139">Debit/Credit</span></span> | <span data-ttu-id="e12ad-140">Сомасы</span><span class="sxs-lookup"><span data-stu-id="e12ad-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="e12ad-141">WIP сатылым құны</span><span class="sxs-lookup"><span data-stu-id="e12ad-141">WIP Sales value</span></span> | <span data-ttu-id="e12ad-142">Несие</span><span class="sxs-lookup"><span data-stu-id="e12ad-142">Credit</span></span> | <span data-ttu-id="e12ad-143">100-көше</span><span class="sxs-lookup"><span data-stu-id="e12ad-143">100</span></span> |
  | <span data-ttu-id="e12ad-144">Есептелген табыс сатылымының құны</span><span class="sxs-lookup"><span data-stu-id="e12ad-144">Accrued revenue sales value</span></span> | <span data-ttu-id="e12ad-145">Дебет</span><span class="sxs-lookup"><span data-stu-id="e12ad-145">Debit</span></span> | <span data-ttu-id="e12ad-146">100-көше</span><span class="sxs-lookup"><span data-stu-id="e12ad-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="e12ad-147">Бекітілген бағаны есептеу әдісін пайдалана отырып есепке алынатын транзакциялар</span><span class="sxs-lookup"><span data-stu-id="e12ad-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="e12ad-148">Шығындар мен табысты тану бөлек.</span><span class="sxs-lookup"><span data-stu-id="e12ad-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="e12ad-149">Транзакция құны [Project Operations Integration журналы](../project-accounting/project-operations-integration-journal.md) арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="e12ad-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="e12ad-150">Шот ұсынылмаған сатылым транзакциялары жасалмайды.</span><span class="sxs-lookup"><span data-stu-id="e12ad-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="e12ad-151">Жоба құны мен табыс профилінде **WIP жоқ** күйіне орнатылған **Жобаны аяқтау есептеулері үшін пайдаланылатын қағида** параметрі болса, есеп-шот ұсыну кезінде табыс танылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e12ad-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="e12ad-152">Бұл әдісті қысқа мерзімді, қарапайым жобаларға ғана пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="e12ad-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="e12ad-153">**Аяқталған келісім-шарт** немесе **Аяқтау пайызының табысын тану** әдісімен бекітілген баға табысының болжамдарын пайдалана отырып табысты тануға болады.</span><span class="sxs-lookup"><span data-stu-id="e12ad-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="e12ad-154">Қосымша ресурстар</span><span class="sxs-lookup"><span data-stu-id="e12ad-154">Additional resources</span></span>
[<span data-ttu-id="e12ad-155">Есеп-шот ұсынылатын жобалар мақаласы үшін есепті конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="e12ad-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="e12ad-156">Бекітілген бағадағы табыс болжамы жобалары</span><span class="sxs-lookup"><span data-stu-id="e12ad-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="e12ad-157">Табыс болжамдарын басқару</span><span class="sxs-lookup"><span data-stu-id="e12ad-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="e12ad-158">Әдістерді аяқтау құны</span><span class="sxs-lookup"><span data-stu-id="e12ad-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]