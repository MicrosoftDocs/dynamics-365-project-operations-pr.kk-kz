---
title: Шығыс құнының нақты мәндері бойынша неліктен әдепкі баға нөлге тең емес?
description: Шығыс құнының нақты мәндері бойынша әдепкі бағаны нөлге теңестіріңіз.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
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
ms.openlocfilehash: 742b0b9c495b4b3ecb4705be3ece5656f0322ca9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285851"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="a1da0-103">Шығыс құнының нақты мәндері бойынша неліктен әдепкі баға нөлге тең емес</span><span class="sxs-lookup"><span data-stu-id="a1da0-103">Why is the price defaulting to zero on expense cost actuals</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a1da0-104">Бұл ЖҚС шығыс нақты мәндеріне қолданылады, мұндағы транзакция класы Шығыс күйіне, ал транзакция түрі Құн күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a1da0-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="a1da0-105">Шығыс құнының нақты мәндері бойынша құн мөлшерлемелерін шешу</span><span class="sxs-lookup"><span data-stu-id="a1da0-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="a1da0-106">Байланысты шығыс жазбасына өтіп, шығыс жазбасы өрісіндегі сома бар екендігіне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="a1da0-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="a1da0-107">Бастапқы шығыс жазбасында толтырылған сома өрісі болмаса, мәселені оқшаулауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="a1da0-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="a1da0-108">Осы мәселені шешу үшін, шығыс жазбасын жарамды сомамен қайта жасап растаңыз.</span><span class="sxs-lookup"><span data-stu-id="a1da0-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]