---
title: Табысты тануға шолу
description: Бұл тақырыпта Project Operations бағдарламасындағы табысты тану туралы ақпарат берілген.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: ab9b36b71223b1bcfe48de5f9b68b6fb6a98f388
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368033"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="c4e5c-103">Табысты тануға шолу</span><span class="sxs-lookup"><span data-stu-id="c4e5c-103">Revenue recognition overview</span></span>

<span data-ttu-id="c4e5c-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="c4e5c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c4e5c-105">Dynamics 365 Project Operations бағдарламасында табысты тану қағидалары жоба немесе жоба бөлігі үшін таңдалған есептеу әдісі негізінде өзгереді.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="c4e5c-106">Бұл тақырыпта Project Operations бағдарламасындағы табысты тану туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="c4e5c-107">Уақыт пен материалдарды есепке алу әдісін пайдалана отырып есепке алынатын транзакциялар</span><span class="sxs-lookup"><span data-stu-id="c4e5c-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="c4e5c-108">Шығындар мен табысты тану бір-бірімен байланысты.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="c4e5c-109">Транзакция құны және шот ұсынылмаған сатылымдар [Project Operations Integration журналы](../project-accounting/project-operations-integration-journal.md) арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="c4e5c-110">Жоба құны мен табыс профилі шот ұсынылмаған сатылым транзакциялары бас кітапқа орналастырылғанын анықтайды.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="c4e5c-111">Егер **Есептелген табыс** таңдалса жүйе орналастыру кезінде **WIP сатылым мәні** және **Есептелген табыс сатылымының құны** есеп-шоттарын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="c4e5c-112">Келесі суретте осы әдістің мысалы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="c4e5c-113">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="c4e5c-113">Transaction type</span></span> | <span data-ttu-id="c4e5c-114">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="c4e5c-114">Debit/Credit</span></span> | <span data-ttu-id="c4e5c-115">Сомасы</span><span class="sxs-lookup"><span data-stu-id="c4e5c-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="c4e5c-116">WIP сатылым құны</span><span class="sxs-lookup"><span data-stu-id="c4e5c-116">WIP Sales value</span></span> | <span data-ttu-id="c4e5c-117">Дебет</span><span class="sxs-lookup"><span data-stu-id="c4e5c-117">Debit</span></span> | <span data-ttu-id="c4e5c-118">100-көше</span><span class="sxs-lookup"><span data-stu-id="c4e5c-118">100</span></span> |
  | <span data-ttu-id="c4e5c-119">Есептелген табыс сатылымының құны</span><span class="sxs-lookup"><span data-stu-id="c4e5c-119">Accrued revenue sales value</span></span> | <span data-ttu-id="c4e5c-120">Несие</span><span class="sxs-lookup"><span data-stu-id="c4e5c-120">Credit</span></span> | <span data-ttu-id="c4e5c-121">100-көше</span><span class="sxs-lookup"><span data-stu-id="c4e5c-121">100</span></span> |

- <span data-ttu-id="c4e5c-122">Есеп-шот ұсыну кезінде табыс танылды.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="c4e5c-123">Орналастыру кезінде жүйе **Есеп-шот ұсынылған табыс** пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="c4e5c-124">Келесі суретте осы әдістің мысалы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="c4e5c-125">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="c4e5c-125">Transaction type</span></span> | <span data-ttu-id="c4e5c-126">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="c4e5c-126">Debit/Credit</span></span> | <span data-ttu-id="c4e5c-127">Сомасы</span><span class="sxs-lookup"><span data-stu-id="c4e5c-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="c4e5c-128">Тұтынушы қалдығы</span><span class="sxs-lookup"><span data-stu-id="c4e5c-128">Customer balance</span></span> | <span data-ttu-id="c4e5c-129">Дебет</span><span class="sxs-lookup"><span data-stu-id="c4e5c-129">Debit</span></span> | <span data-ttu-id="c4e5c-130">120</span><span class="sxs-lookup"><span data-stu-id="c4e5c-130">120</span></span> |
  | <span data-ttu-id="c4e5c-131">Төлену керек сатылым салығы</span><span class="sxs-lookup"><span data-stu-id="c4e5c-131">Sales tax payable</span></span> | <span data-ttu-id="c4e5c-132">Несие</span><span class="sxs-lookup"><span data-stu-id="c4e5c-132">Credit</span></span> | <span data-ttu-id="c4e5c-133">20</span><span class="sxs-lookup"><span data-stu-id="c4e5c-133">20</span></span> |
  | <span data-ttu-id="c4e5c-134">Шот-фактура бойынша табыс</span><span class="sxs-lookup"><span data-stu-id="c4e5c-134">Invoiced Revenue</span></span> | <span data-ttu-id="c4e5c-135">Несие</span><span class="sxs-lookup"><span data-stu-id="c4e5c-135">Credit</span></span> | <span data-ttu-id="c4e5c-136">100-көше</span><span class="sxs-lookup"><span data-stu-id="c4e5c-136">100</span></span> |

- <span data-ttu-id="c4e5c-137">Егер кіріс есептелмеген сатылымдар орналастырылған кезде есептелген болса, онда жүйе есептелген кірісті есеп-шот ұсыну кезінде қалпына келтіреді.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="c4e5c-138">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="c4e5c-138">Transaction type</span></span> | <span data-ttu-id="c4e5c-139">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="c4e5c-139">Debit/Credit</span></span> | <span data-ttu-id="c4e5c-140">Сомасы</span><span class="sxs-lookup"><span data-stu-id="c4e5c-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="c4e5c-141">WIP сатылым құны</span><span class="sxs-lookup"><span data-stu-id="c4e5c-141">WIP Sales value</span></span> | <span data-ttu-id="c4e5c-142">Несие</span><span class="sxs-lookup"><span data-stu-id="c4e5c-142">Credit</span></span> | <span data-ttu-id="c4e5c-143">100-көше</span><span class="sxs-lookup"><span data-stu-id="c4e5c-143">100</span></span> |
  | <span data-ttu-id="c4e5c-144">Есептелген табыс сатылымының құны</span><span class="sxs-lookup"><span data-stu-id="c4e5c-144">Accrued revenue sales value</span></span> | <span data-ttu-id="c4e5c-145">Дебет</span><span class="sxs-lookup"><span data-stu-id="c4e5c-145">Debit</span></span> | <span data-ttu-id="c4e5c-146">100-көше</span><span class="sxs-lookup"><span data-stu-id="c4e5c-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="c4e5c-147">Бекітілген бағаны есептеу әдісін пайдалана отырып есепке алынатын транзакциялар</span><span class="sxs-lookup"><span data-stu-id="c4e5c-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="c4e5c-148">Шығындар мен табысты тану бөлек.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="c4e5c-149">Транзакция құны [Project Operations Integration журналы](../project-accounting/project-operations-integration-journal.md) арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="c4e5c-150">Шот ұсынылмаған сатылым транзакциялары жасалмайды.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="c4e5c-151">Жоба құны мен табыс профилінде **WIP жоқ** күйіне орнатылған **Жобаны аяқтау есептеулері үшін пайдаланылатын қағида** параметрі болса, есеп-шот ұсыну кезінде табыс танылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="c4e5c-152">Бұл әдісті қысқа мерзімді, қарапайым жобаларға ғана пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="c4e5c-153">**Аяқталған келісім-шарт** немесе **Аяқтау пайызының табысын тану** әдісімен бекітілген баға табысының болжамдарын пайдалана отырып табысты тануға болады.</span><span class="sxs-lookup"><span data-stu-id="c4e5c-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="c4e5c-154">Қосымша ресурстар</span><span class="sxs-lookup"><span data-stu-id="c4e5c-154">Additional resources</span></span>
[<span data-ttu-id="c4e5c-155">Есеп-шот ұсынылатын жобалар мақаласы үшін есепті конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="c4e5c-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="c4e5c-156">Бекітілген бағадағы табыс болжамы жобалары</span><span class="sxs-lookup"><span data-stu-id="c4e5c-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="c4e5c-157">Табыс болжамдарын басқару</span><span class="sxs-lookup"><span data-stu-id="c4e5c-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="c4e5c-158">Әдістерді аяқтау құны</span><span class="sxs-lookup"><span data-stu-id="c4e5c-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]