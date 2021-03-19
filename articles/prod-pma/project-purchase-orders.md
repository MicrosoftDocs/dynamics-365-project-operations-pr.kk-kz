---
title: Жобаға арналған сатып алуға тапсырыстар
description: Бұл мақалада жоба үшін сатып алуға тапсырыстарды жасау үшін пайдалануға болатын әр алуан әдістер сипатталған. Сіз пайдаланатын әдіс сатып алуға тапсырыс мақсатына және сатып алынған элементтердің жоба аясында қашан қолданылып, төленетініне байланысты болады.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5f3f5d196e0d7db4a6d8c4cfe834a335f4ef737c
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289196"
---
# <a name="purchase-orders-for-a-project"></a><span data-ttu-id="d5640-104">Жобаға арналған сатып алуға тапсырыстар</span><span class="sxs-lookup"><span data-stu-id="d5640-104">Purchase orders for a project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="d5640-105">Бұл мақалада жоба үшін сатып алуға тапсырыстарды жасау үшін пайдалануға болатын әр алуан әдістер сипатталған.</span><span class="sxs-lookup"><span data-stu-id="d5640-105">This article describes the various methods that you can use to create purchase orders for a project.</span></span> <span data-ttu-id="d5640-106">Сіз пайдаланатын әдіс сатып алуға тапсырыс мақсатына және сатып алынған элементтердің жоба аясында қашан қолданылып, төленетініне байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="d5640-106">The method that you use depends on the purpose of the purchase order, and when the purchased items are consumed and charged to a project.</span></span>

### <a name="methods-for-creating-a-purchase-order"></a><span data-ttu-id="d5640-107">Сатып алуға тапсырыстар жасау әдістері</span><span class="sxs-lookup"><span data-stu-id="d5640-107">Methods for creating a purchase order</span></span>

<span data-ttu-id="d5640-108">"Жобаны басқару және есеп" бөлімінде сатып алуға тапсырыс жасау үшін келесі әдістердің бірін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="d5640-108">You can use one of the following methods to create a purchase order in Project management and accounting.</span></span> <span data-ttu-id="d5640-109">Сатып алуға тапсырыс мақсаты жоба үшін сатып алуға тапсырыс қашан қолданылатынын және элементтердің қашан төленетінін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="d5640-109">The purpose of the purchase order determines when the purchase order is consumed and, therefore, when items are charged to a project.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="d5640-110">Әдіс</span><span class="sxs-lookup"><span data-stu-id="d5640-110">Method</span></span></th>
<th><span data-ttu-id="d5640-111">Мақсат</span><span class="sxs-lookup"><span data-stu-id="d5640-111">Purpose</span></span></th>
<th><span data-ttu-id="d5640-112">Элементтерді тұтыну</span><span class="sxs-lookup"><span data-stu-id="d5640-112">Consumption of items</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="d5640-113">Сатып алуға тапсырысты тікелей жобадан жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="d5640-113">Create a purchase order directly from a project.</span></span></td>
<td><span data-ttu-id="d5640-114">Бұл әдісті жобада тұтыну үшін сыртқы жеткізушіден элементтерді сатып алу үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5640-114">Use this method to purchase items from an external vendor for consumption on a project.</span></span> <span data-ttu-id="d5640-115">Сатып алуға тапсырысты екі жолмен жасауға болады:</span><span class="sxs-lookup"><span data-stu-id="d5640-115">You can create the purchase order in two ways:</span></span>
<ul>
<li><span data-ttu-id="d5640-116">Жобаның өзінен.</span><span class="sxs-lookup"><span data-stu-id="d5640-116">From the project itself.</span></span> <span data-ttu-id="d5640-117">Бұл жағдайда, жоба сатып алуға тапсырыс үшін әлдеқашан анықталады.</span><span class="sxs-lookup"><span data-stu-id="d5640-117">In this case, the project is already defined for the purchase order.</span></span></li>
<li><span data-ttu-id="d5640-118">Жобаның сатып алуға тапсырысына өту арқылы.</span><span class="sxs-lookup"><span data-stu-id="d5640-118">By navigating to the project purchase order.</span></span> <span data-ttu-id="d5640-119">Сатып алуға тапсырыс жасау үшін жеткізушіні де, жобаны да таңдау керек.</span><span class="sxs-lookup"><span data-stu-id="d5640-119">You must select both the vendor and the project to create the purchase order for.</span></span></li>
</ul></td>
<td><span data-ttu-id="d5640-120">Элементтер жеткізуші есеп-шоты жаңартылған кезде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="d5640-120">Items are consumed when the vendor invoice is updated.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="d5640-121">Сатып алуға тапсырысты сату тапсырысынан жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="d5640-121">Create a purchase order from a sales order.</span></span></td>
<td><span data-ttu-id="d5640-122">Бұл әдісті жобадан сату тапсырысын жасаған кезде элементтерді сатып алу үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5640-122">Use this method to purchase items when you create a sales order from a project.</span></span></td>
<td><span data-ttu-id="d5640-123">Элементтер сату тапсырысы тұтынушыға есеп-шот бойынша ұсынылған кезде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="d5640-123">Items are consumed when the sales order is invoiced to the customer.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="d5640-124">Сатып алуға тапсырысты элемент талабы бөлімінен жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="d5640-124">Create a purchase order from an item requirement.</span></span></td>
<td><span data-ttu-id="d5640-125">Бұл әдісті жобадан элемент талабын жасаған кезде элементтерді сатып алу үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5640-125">Use this method to purchase items when you create an item requirement from a project.</span></span></td>
<td><span data-ttu-id="d5640-126">Элементтер элемент талабының тауар жөнелтпе құжаты жаңартылған кезде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="d5640-126">Items are consumed when the item requirement packing slip is updated.</span></span></td>
</tr>
</tbody>
</table>

> [!NOTE] 
> <span data-ttu-id="d5640-127">Жеткізуші есеп-шотын немесе тауар жөнелтпе құжатын жаңартқан кезде, сізден элемент талабы бойынша тауар жөнелтпе құжатын жаңарту сұралады.</span><span class="sxs-lookup"><span data-stu-id="d5640-127">When you update the vendor invoice or packing slip, you're prompted to update the packing slip on the item requirement.</span></span>

<span data-ttu-id="d5640-128">Қосымша ақпарат алу үшін [Элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу](tasks/receive-items-purchase-order-item-requirement.md) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="d5640-128">For more information, see [Receive items on purchase order from item requirement](tasks/receive-items-purchase-order-item-requirement.md).</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]