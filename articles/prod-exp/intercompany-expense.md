---
title: Компанияаралық шығыстар
description: Бұл тақырыпта жұмысшы шығындарын жұмыс орындалған заңды нысанға белгілеу үшін компанияаралық шығындарды пайдалану туралы ақпарат берілген.
author: ShylaThompson
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d2cdba8d5368a8b26bf4d98226bda76a58261cf0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005078"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="47000-103">Компанияаралық шығыстар</span><span class="sxs-lookup"><span data-stu-id="47000-103">Intercompany expenses</span></span>

<span data-ttu-id="47000-104">Ұйымдағы бір заңды нысанда жұмыс істейтін қызметкер сол ұйымдағы басқа заңды нысан үшін жұмысты орындай алады.</span><span class="sxs-lookup"><span data-stu-id="47000-104">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="47000-105">Компанияаралық шығындарды жұмысшы шығындарын жұмыс орындалған заңды нысанға белгілеу үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="47000-105">You can use intercompany expenses to assign the worker’s expenses to the legal entity for which the  work was performed.</span></span> <span data-ttu-id="47000-106">Қызметкерді жалдайтын заңды нысан несиелік заңды нысан деп аталады.</span><span class="sxs-lookup"><span data-stu-id="47000-106">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="47000-107">Қызметкер шығындар жасайтын заңды нысан қарыз беруші заңды нысан деп аталады.</span><span class="sxs-lookup"><span data-stu-id="47000-107">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="47000-108">Жұмысшы компанияаралық шығындарды жасап, ұсынбас бұрын, сізге компанияаралық шығындар желілерін қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="47000-108">Before a worker can create and submit intercompany expenses, you must enable intercompany expense lines.</span></span> <span data-ttu-id="47000-109">Қарыз беретін заңды нысанда, **Шығындарды басқару параметрлері** бетінде **Компанияаралық шығындар желілеріне рұқсат беру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="47000-109">In the loaning legal entity, on the **Expense management parameters** page, select **Allow intercompany expense lines**.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="47000-110">Компанияаралық шығыстарға салық салу</span><span class="sxs-lookup"><span data-stu-id="47000-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="47000-111">Шығындар туралы есепте қарыз алушы заңды нысанмен (жеткізу орны) емес, қарыз беруші заңды нысанмен (дереккөзбен) байланысты салық топтарын пайдаланбас бұрын, бұл функцияны бас кітап сатылымы салығының параметрінде қосу керек.</span><span class="sxs-lookup"><span data-stu-id="47000-111">Before you can use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you must enable the functionality in the General ledger sales tax setup.</span></span> <span data-ttu-id="47000-112">**Компанияаралық салықтарды жүргізуге арналған заңды нысан** параметрі **Бастапқы** күйіне, ал **Сату салығына салық салу ережелерін қолдану** параметрі **Жоқ** күйіне орнатылса, қарыз беруші заңды нысан үшін салық тіркесімі пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="47000-112">When the **Legal entity for intercompany tax posting** parameter is set to **Source** and **Apply sales tax taxation rules** is set to **No**, the tax combination for the loaning legal entity is used.</span></span> <span data-ttu-id="47000-113">Сол параметр **Межелі орын** мәніне орнатылған кезде, қарыз беруші заңды нысан үшін салық комбинациясы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="47000-113">When the same parameter is set to **Destination**, the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="47000-114">АҚШ-тағы заңды нысандар үшін параметр **Дереккөз** мәніне орнатылған кезде, **Дебиторлық сатылым салығы** өрісі жаңа **Бас кітапқа енгізу топтары** бетіне конфигурациялануы тиіс.</span><span class="sxs-lookup"><span data-stu-id="47000-114">For legal entities in the United States, when the parameter is set to **Source**, the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="47000-115">Есепке алу жүйесі осы өрістегі ақпаратты есепке алу нысанына қатысты салық салу үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="47000-115">The accounting engine will use the information from this field for tax-related accounting entry.</span></span>   
<span data-ttu-id="47000-116">Бұл әрекет жобамен немесе жобасыз орналастырылған шығыс жолдарына сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="47000-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  


[!INCLUDE[footer-include](../includes/footer-banner.md)]