---
title: Компанияаралық шығыстар
description: Ұйымдағы бір заңды нысанда жұмыс істейтін қызметкер сол ұйымдағы басқа заңды нысан үшін жұмысты орындай алады. Мұндай жағдайда, қызметкерлердің шығындарын жұмысы орындалған заңды нысанға тағайындау үшін компанияаралық шығыстарды пайдалана аласыз.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079811"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="893d5-104">Компанияаралық шығыстар</span><span class="sxs-lookup"><span data-stu-id="893d5-104">Intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="893d5-105">Ұйымдағы бір заңды нысанда жұмыс істейтін қызметкер сол ұйымдағы басқа заңды нысан үшін жұмысты орындай алады.</span><span class="sxs-lookup"><span data-stu-id="893d5-105">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="893d5-106">Мұндай жағдайда, қызметкерлердің шығындарын жұмысы орындалған заңды нысанға тағайындау үшін компанияаралық шығыстарды пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="893d5-106">In this situation, you can use the intercompany expense feature to assign the worker’s expenses to the legal entity for which the work was performed.</span></span> <span data-ttu-id="893d5-107">Қызметкерді жалдайтын заңды нысан несиелік заңды нысан деп аталады.</span><span class="sxs-lookup"><span data-stu-id="893d5-107">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="893d5-108">Қызметкер шығындар жасайтын заңды нысан қарыз беруші заңды нысан деп аталады.</span><span class="sxs-lookup"><span data-stu-id="893d5-108">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="893d5-109">Қызметкер басқа заңды нысан үшін орындалатын жұмысқа шығындарды құрып, ұсынбас бұрын, **Шығысты басқару параметрлері** бетіндегі несие беретін заңды нысанда **Компанияаралық шығыс жолдарына рұқсат ету** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="893d5-109">Before a worker can create and submit expenses for work that is performed for a different legal entity, in the loaning legal entity, on the **Expense management parameters** page, select the **Allow intercompany expense lines** option.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="893d5-110">Компанияаралық шығыстарға салық салу</span><span class="sxs-lookup"><span data-stu-id="893d5-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="893d5-111">Егер сіз шығыс туралы есепте қарыз беруші (межелі орын) заңды нысанның орнына несие беруші (қайнар көз) заңды нысанға байланысты салық топтарын пайдалану керек болса, мұны жалпы сатылым салығы бойынша орнатылған Бас кітапта конфигурациялауыңыз қажет.</span><span class="sxs-lookup"><span data-stu-id="893d5-111">If you want to use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you will need to configure this in the General ledger sales tax set up.</span></span> <span data-ttu-id="893d5-112">Бас кітап параметрі болған кезде, **Компанияаралық салық салуға арналған заңды нысан** параметрі **Дереккөз** мәніне орнатылады және **Сатылым салығы бойынша салық салу ережелерін қолдану** параметрі **Жоқ** мәніне орнатылады, несие беруші заңды нысан үшін салық комбинациясы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="893d5-112">When the General ledger parameter, **Legal entity for intercompany tax posting** is set to **Source** and **Apply sales tax taxation rules** is set to **No** , the tax combination for the loaning legal entity will be used.</span></span> <span data-ttu-id="893d5-113">Сол параметр **Межелі орын** мәніне орнатылған кезде, қарыз беруші заңды нысан үшін салық комбинациясы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="893d5-113">When the same parameter is set to **Destination** , the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="893d5-114">АҚШ-тағы заңды нысандар үшін параметр **Дереккөз** мәніне орнатылған кезде, **Дебиторлық сатылым салығы** өрісі жаңа **Бас кітапқа енгізу топтары** бетіне конфигурациялануы тиіс.</span><span class="sxs-lookup"><span data-stu-id="893d5-114">For legal entities in the United States, when the parameter is set to **Source** , the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="893d5-115">Есепке алу жүйесі осы өрістегі ақпаратты есепке алу нысанына қатысты салық салу үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="893d5-115">The accounting engine will use the information from this field for tax related accounting entry.</span></span>   
<span data-ttu-id="893d5-116">Бұл әрекет жобамен немесе жобасыз орналастырылған шығыс жолдарына сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="893d5-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
