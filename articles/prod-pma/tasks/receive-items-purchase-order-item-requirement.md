---
title: Элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу
description: Бұл тақырыпта элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу жолы түсіндіріледі.
author: Yowelle
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 0e0c4a75f1d86538cc773af1f7c0ae3c83ef0ad5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6011693"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="892cc-103">Элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу</span><span class="sxs-lookup"><span data-stu-id="892cc-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="892cc-104">Бұл тақырыпта элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу жолы түсіндіріледі.</span><span class="sxs-lookup"><span data-stu-id="892cc-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="892cc-105">Элемент транзакциясының орнына элемент талабын пайдалану арқылы, элементті нақты пайдаланбас бұрын жеткізуді жоспарлауға, сатып алуға тапсырысты, сауда келісімінің құрылымындағы элементті, өндірісті жоспарлаудағы элемент талабымен қоса жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="892cc-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="892cc-106">Бұл тапсырмада USSI деректер жиынтығы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="892cc-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="892cc-107">Шарлау аумағында, **Модульдер > жобаны басқару және есеп > Жобалар > Барлық жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="892cc-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="892cc-108">Тізімнен, қажетті жолдағы сілтемені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="892cc-109">Әрекеттер тақтасынан, **Жоспар** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="892cc-110">**Элемент талаптары** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="892cc-111">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-111">Select **New**.</span></span>
6. <span data-ttu-id="892cc-112">Жаңа жолда, **Элемент нөмірі** өрісіне мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="892cc-113">**Саны** өрісіне, нөмірді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="892cc-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="892cc-114">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-114">Select **Save**.</span></span>
9. <span data-ttu-id="892cc-115">Әрекеттер тақтасынан, **Басқару** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="892cc-116">**Функциялар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-116">Select **Functions**.</span></span>
11. <span data-ttu-id="892cc-117">**Сатып алуға тапсырысты жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="892cc-118">**Барлығын қамту** құсбелгісін қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="892cc-119">**Жеткізуші тіркелгісі** өрісіне, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="892cc-120">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-120">Select **OK**.</span></span>
15. <span data-ttu-id="892cc-121">Шарлау аумағында, **Модульдер > Несие берушілер > Сатып алуға тапсырыстар > Барлық сатып алуға тапсырыстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="892cc-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="892cc-122">Тізімнен, қажетті жолдағы сілтемені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="892cc-123">Әрекеттер тақтасында, **Сатып алу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="892cc-124">**Растау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="892cc-125">Әрекеттер тақтасында, **Алу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="892cc-126">**Өнім түбіртегі** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="892cc-127">**Өнім түбіртегі** өрісінде, мәнді теріңіз.</span><span class="sxs-lookup"><span data-stu-id="892cc-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="892cc-128">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="892cc-128">Select **OK**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]