---
title: Элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу
description: Бұл тақырыпта элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу жолы түсіндіріледі.
author: KimANelson
manager: AnnBe
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.assetid: c61e3a5e-da3d-4f4c-87fa-03dea19f6936
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c5ed287aa24aff647ef1dc625f9e9f5f086ee662
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753001"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="c8813-103">Элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу</span><span class="sxs-lookup"><span data-stu-id="c8813-103">Receive items on purchase order from item requirement</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="c8813-104">Бұл тақырыпта элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу жолы түсіндіріледі.</span><span class="sxs-lookup"><span data-stu-id="c8813-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="c8813-105">Элемент транзакциясының орнына элемент талабын пайдалану арқылы, элементті нақты пайдаланбас бұрын жеткізуді жоспарлауға, сатып алуға тапсырысты, сауда келісімінің құрылымындағы элементті, өндірісті жоспарлаудағы элемент талабымен қоса жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="c8813-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="c8813-106">Бұл тапсырмада USSI деректер жиынтығы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="c8813-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="c8813-107">Шарлау аумағында, **Модульдер > жобаны басқару және есеп > Жобалар > Барлық жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="c8813-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="c8813-108">Тізімнен, қажетті жолдағы сілтемені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="c8813-109">Әрекеттер тақтасынан, **Жоспар** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="c8813-110">**Элемент талаптары** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="c8813-111">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-111">Select **New**.</span></span>
6. <span data-ttu-id="c8813-112">Жаңа жолда, **Элемент нөмірі** өрісіне мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="c8813-113">**Саны** өрісіне, нөмірді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="c8813-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="c8813-114">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-114">Select **Save**.</span></span>
9. <span data-ttu-id="c8813-115">Әрекеттер тақтасынан, **Басқару** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="c8813-116">**Функциялар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-116">Select **Functions**.</span></span>
11. <span data-ttu-id="c8813-117">**Сатып алуға тапсырысты жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="c8813-118">**Барлығын қамту** құсбелгісін қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="c8813-119">**Жеткізуші тіркелгісі** өрісіне, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="c8813-120">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-120">Select **OK**.</span></span>
15. <span data-ttu-id="c8813-121">Шарлау аумағында, **Модульдер > Несие берушілер > Сатып алуға тапсырыстар > Барлық сатып алуға тапсырыстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="c8813-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="c8813-122">Тізімнен, қажетті жолдағы сілтемені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="c8813-123">Әрекеттер тақтасында, **Сатып алу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="c8813-124">**Растау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="c8813-125">Әрекеттер тақтасында, **Алу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="c8813-126">**Өнім түбіртегі** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="c8813-127">**Өнім түбіртегі** өрісінде, мәнді теріңіз.</span><span class="sxs-lookup"><span data-stu-id="c8813-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="c8813-128">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c8813-128">Select **OK**.</span></span>

