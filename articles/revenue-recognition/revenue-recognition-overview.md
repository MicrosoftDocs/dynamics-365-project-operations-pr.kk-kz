---
title: Табысты тануға шолу
description: Бұл тақырыпта Project Operations бағдарламасындағы табысты тану туралы ақпарат берілген.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5e77a0442f634a50f8099fadec42ff400fee0e81
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278875"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="8a6b6-103">Табысты тануға шолу</span><span class="sxs-lookup"><span data-stu-id="8a6b6-103">Revenue recognition overview</span></span>

<span data-ttu-id="8a6b6-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="8a6b6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8a6b6-105">Dynamics 365 Project Operations бағдарламасында табысты тану қағидалары жоба немесе жоба бөлігі үшін таңдалған есептеу әдісі негізінде өзгереді.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="8a6b6-106">Бұл тақырыпта Project Operations бағдарламасындағы табысты тану туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="8a6b6-107">Уақыт пен материалдарды есепке алу әдісін пайдалана отырып есепке алынатын транзакциялар</span><span class="sxs-lookup"><span data-stu-id="8a6b6-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="8a6b6-108">Шығындар мен табысты тану бір-бірімен байланысты.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="8a6b6-109">Транзакция құны және шот ұсынылмаған сатылымдар [Project Operations Integration журналы](../project-accounting/project-operations-integration-journal.md) арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="8a6b6-110">Жоба құны мен табыс профилі шот ұсынылмаған сатылым транзакциялары бас кітапқа орналастырылғанын анықтайды.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="8a6b6-111">Егер **Есептелген табыс** таңдалса жүйе орналастыру кезінде **WIP сатылым мәні** және **Есептелген табыс сатылымының құны** есеп-шоттарын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="8a6b6-112">Келесі суретте осы әдістің мысалы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="8a6b6-113">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="8a6b6-113">Transaction type</span></span> | <span data-ttu-id="8a6b6-114">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="8a6b6-114">Debit/Credit</span></span> | <span data-ttu-id="8a6b6-115">Сомасы</span><span class="sxs-lookup"><span data-stu-id="8a6b6-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8a6b6-116">WIP сатылым құны</span><span class="sxs-lookup"><span data-stu-id="8a6b6-116">WIP Sales value</span></span> | <span data-ttu-id="8a6b6-117">Дебет</span><span class="sxs-lookup"><span data-stu-id="8a6b6-117">Debit</span></span> | <span data-ttu-id="8a6b6-118">100-көше</span><span class="sxs-lookup"><span data-stu-id="8a6b6-118">100</span></span> |
  | <span data-ttu-id="8a6b6-119">Есептелген табыс сатылымының құны</span><span class="sxs-lookup"><span data-stu-id="8a6b6-119">Accrued revenue sales value</span></span> | <span data-ttu-id="8a6b6-120">Несие</span><span class="sxs-lookup"><span data-stu-id="8a6b6-120">Credit</span></span> | <span data-ttu-id="8a6b6-121">100-көше</span><span class="sxs-lookup"><span data-stu-id="8a6b6-121">100</span></span> |

- <span data-ttu-id="8a6b6-122">Есеп-шот ұсыну кезінде табыс танылды.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="8a6b6-123">Орналастыру кезінде жүйе **Есеп-шот ұсынылған табыс** пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="8a6b6-124">Келесі суретте осы әдістің мысалы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="8a6b6-125">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="8a6b6-125">Transaction type</span></span> | <span data-ttu-id="8a6b6-126">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="8a6b6-126">Debit/Credit</span></span> | <span data-ttu-id="8a6b6-127">Сомасы</span><span class="sxs-lookup"><span data-stu-id="8a6b6-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8a6b6-128">Тұтынушы қалдығы</span><span class="sxs-lookup"><span data-stu-id="8a6b6-128">Customer balance</span></span> | <span data-ttu-id="8a6b6-129">Дебет</span><span class="sxs-lookup"><span data-stu-id="8a6b6-129">Debit</span></span> | <span data-ttu-id="8a6b6-130">120</span><span class="sxs-lookup"><span data-stu-id="8a6b6-130">120</span></span> |
  | <span data-ttu-id="8a6b6-131">Төлену керек сатылым салығы</span><span class="sxs-lookup"><span data-stu-id="8a6b6-131">Sales tax payable</span></span> | <span data-ttu-id="8a6b6-132">Несие</span><span class="sxs-lookup"><span data-stu-id="8a6b6-132">Credit</span></span> | <span data-ttu-id="8a6b6-133">20</span><span class="sxs-lookup"><span data-stu-id="8a6b6-133">20</span></span> |
  | <span data-ttu-id="8a6b6-134">Шот-фактура бойынша табыс</span><span class="sxs-lookup"><span data-stu-id="8a6b6-134">Invoiced Revenue</span></span> | <span data-ttu-id="8a6b6-135">Несие</span><span class="sxs-lookup"><span data-stu-id="8a6b6-135">Credit</span></span> | <span data-ttu-id="8a6b6-136">100-көше</span><span class="sxs-lookup"><span data-stu-id="8a6b6-136">100</span></span> |

- <span data-ttu-id="8a6b6-137">Егер кіріс есептелмеген сатылымдар орналастырылған кезде есептелген болса, онда жүйе есептелген кірісті есеп-шот ұсыну кезінде қалпына келтіреді.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="8a6b6-138">Транзакция түрі</span><span class="sxs-lookup"><span data-stu-id="8a6b6-138">Transaction type</span></span> | <span data-ttu-id="8a6b6-139">Дебет/несие</span><span class="sxs-lookup"><span data-stu-id="8a6b6-139">Debit/Credit</span></span> | <span data-ttu-id="8a6b6-140">Сомасы</span><span class="sxs-lookup"><span data-stu-id="8a6b6-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8a6b6-141">WIP сатылым құны</span><span class="sxs-lookup"><span data-stu-id="8a6b6-141">WIP Sales value</span></span> | <span data-ttu-id="8a6b6-142">Несие</span><span class="sxs-lookup"><span data-stu-id="8a6b6-142">Credit</span></span> | <span data-ttu-id="8a6b6-143">100-көше</span><span class="sxs-lookup"><span data-stu-id="8a6b6-143">100</span></span> |
  | <span data-ttu-id="8a6b6-144">Есептелген табыс сатылымының құны</span><span class="sxs-lookup"><span data-stu-id="8a6b6-144">Accrued revenue sales value</span></span> | <span data-ttu-id="8a6b6-145">Дебет</span><span class="sxs-lookup"><span data-stu-id="8a6b6-145">Debit</span></span> | <span data-ttu-id="8a6b6-146">100-көше</span><span class="sxs-lookup"><span data-stu-id="8a6b6-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="8a6b6-147">Бекітілген бағаны есептеу әдісін пайдалана отырып есепке алынатын транзакциялар</span><span class="sxs-lookup"><span data-stu-id="8a6b6-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="8a6b6-148">Шығындар мен табысты тану бөлек.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="8a6b6-149">Транзакция құны [Project Operations Integration журналы](../project-accounting/project-operations-integration-journal.md) арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="8a6b6-150">Шот ұсынылмаған сатылым транзакциялары жасалмайды.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="8a6b6-151">Жоба құны мен табыс профилінде **WIP жоқ** күйіне орнатылған **Жобаны аяқтау есептеулері үшін пайдаланылатын қағида** параметрі болса, есеп-шот ұсыну кезінде табыс танылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="8a6b6-152">Бұл әдісті қысқа мерзімді, қарапайым жобаларға ғана пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="8a6b6-153">**Аяқталған келісім-шарт** немесе **Аяқтау пайызының табысын тану** әдісімен бекітілген баға табысының болжамдарын пайдалана отырып табысты тануға болады.</span><span class="sxs-lookup"><span data-stu-id="8a6b6-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="8a6b6-154">Қосымша ресурстар</span><span class="sxs-lookup"><span data-stu-id="8a6b6-154">Additional resources</span></span>
[<span data-ttu-id="8a6b6-155">Есеп-шот ұсынылатын жобалар мақаласы үшін есепті конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="8a6b6-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="8a6b6-156">Бекітілген бағадағы табыс болжамы жобалары</span><span class="sxs-lookup"><span data-stu-id="8a6b6-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="8a6b6-157">Табыс болжамдарын басқару</span><span class="sxs-lookup"><span data-stu-id="8a6b6-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="8a6b6-158">Әдістерді аяқтау құны</span><span class="sxs-lookup"><span data-stu-id="8a6b6-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]