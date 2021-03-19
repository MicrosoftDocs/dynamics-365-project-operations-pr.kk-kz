---
title: Элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу
description: Бұл тақырыпта элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу жолы түсіндіріледі.
author: Yowelle
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
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c2083516ff929113fd6db377acfe5aeb104666dd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288235"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="1a512-103">Элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу</span><span class="sxs-lookup"><span data-stu-id="1a512-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="1a512-104">Бұл тақырыпта элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу жолы түсіндіріледі.</span><span class="sxs-lookup"><span data-stu-id="1a512-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="1a512-105">Элемент транзакциясының орнына элемент талабын пайдалану арқылы, элементті нақты пайдаланбас бұрын жеткізуді жоспарлауға, сатып алуға тапсырысты, сауда келісімінің құрылымындағы элементті, өндірісті жоспарлаудағы элемент талабымен қоса жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="1a512-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="1a512-106">Бұл тапсырмада USSI деректер жиынтығы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="1a512-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="1a512-107">Шарлау аумағында, **Модульдер > жобаны басқару және есеп > Жобалар > Барлық жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="1a512-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="1a512-108">Тізімнен, қажетті жолдағы сілтемені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="1a512-109">Әрекеттер тақтасынан, **Жоспар** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="1a512-110">**Элемент талаптары** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="1a512-111">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-111">Select **New**.</span></span>
6. <span data-ttu-id="1a512-112">Жаңа жолда, **Элемент нөмірі** өрісіне мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="1a512-113">**Саны** өрісіне, нөмірді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="1a512-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="1a512-114">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-114">Select **Save**.</span></span>
9. <span data-ttu-id="1a512-115">Әрекеттер тақтасынан, **Басқару** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="1a512-116">**Функциялар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-116">Select **Functions**.</span></span>
11. <span data-ttu-id="1a512-117">**Сатып алуға тапсырысты жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="1a512-118">**Барлығын қамту** құсбелгісін қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="1a512-119">**Жеткізуші тіркелгісі** өрісіне, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="1a512-120">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-120">Select **OK**.</span></span>
15. <span data-ttu-id="1a512-121">Шарлау аумағында, **Модульдер > Несие берушілер > Сатып алуға тапсырыстар > Барлық сатып алуға тапсырыстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="1a512-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="1a512-122">Тізімнен, қажетті жолдағы сілтемені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="1a512-123">Әрекеттер тақтасында, **Сатып алу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="1a512-124">**Растау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="1a512-125">Әрекеттер тақтасында, **Алу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="1a512-126">**Өнім түбіртегі** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="1a512-127">**Өнім түбіртегі** өрісінде, мәнді теріңіз.</span><span class="sxs-lookup"><span data-stu-id="1a512-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="1a512-128">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1a512-128">Select **OK**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]