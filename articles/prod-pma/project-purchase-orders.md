---
title: Жобаға арналған сатып алуға тапсырыстар
description: Бұл мақалада жоба үшін сатып алуға тапсырыстарды жасау үшін пайдалануға болатын әр алуан әдістер сипатталған. Сіз пайдаланатын әдіс сатып алуға тапсырыс мақсатына және сатып алынған элементтердің жоба аясында қашан қолданылып, төленетініне байланысты болады.
author: Yowelle
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 3c3ce2d0c0fb3cecf22157db5cb37eb744027d0f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999363"
---
# <a name="purchase-orders-for-a-project"></a><span data-ttu-id="25141-104">Жобаға арналған сатып алуға тапсырыстар</span><span class="sxs-lookup"><span data-stu-id="25141-104">Purchase orders for a project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="25141-105">Бұл мақалада жоба үшін сатып алуға тапсырыстарды жасау үшін пайдалануға болатын әр алуан әдістер сипатталған.</span><span class="sxs-lookup"><span data-stu-id="25141-105">This article describes the various methods that you can use to create purchase orders for a project.</span></span> <span data-ttu-id="25141-106">Сіз пайдаланатын әдіс сатып алуға тапсырыс мақсатына және сатып алынған элементтердің жоба аясында қашан қолданылып, төленетініне байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="25141-106">The method that you use depends on the purpose of the purchase order, and when the purchased items are consumed and charged to a project.</span></span>

### <a name="methods-for-creating-a-purchase-order"></a><span data-ttu-id="25141-107">Сатып алуға тапсырыстар жасау әдістері</span><span class="sxs-lookup"><span data-stu-id="25141-107">Methods for creating a purchase order</span></span>

<span data-ttu-id="25141-108">"Жобаны басқару және есеп" бөлімінде сатып алуға тапсырыс жасау үшін келесі әдістердің бірін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="25141-108">You can use one of the following methods to create a purchase order in Project management and accounting.</span></span> <span data-ttu-id="25141-109">Сатып алуға тапсырыс мақсаты жоба үшін сатып алуға тапсырыс қашан қолданылатынын және элементтердің қашан төленетінін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="25141-109">The purpose of the purchase order determines when the purchase order is consumed and, therefore, when items are charged to a project.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="25141-110">Әдіс</span><span class="sxs-lookup"><span data-stu-id="25141-110">Method</span></span></th>
<th><span data-ttu-id="25141-111">Мақсат</span><span class="sxs-lookup"><span data-stu-id="25141-111">Purpose</span></span></th>
<th><span data-ttu-id="25141-112">Элементтерді тұтыну</span><span class="sxs-lookup"><span data-stu-id="25141-112">Consumption of items</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="25141-113">Сатып алуға тапсырысты тікелей жобадан жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="25141-113">Create a purchase order directly from a project.</span></span></td>
<td><span data-ttu-id="25141-114">Бұл әдісті жобада тұтыну үшін сыртқы жеткізушіден элементтерді сатып алу үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="25141-114">Use this method to purchase items from an external vendor for consumption on a project.</span></span> <span data-ttu-id="25141-115">Сатып алуға тапсырысты екі жолмен жасауға болады:</span><span class="sxs-lookup"><span data-stu-id="25141-115">You can create the purchase order in two ways:</span></span>
<ul>
<li><span data-ttu-id="25141-116">Жобаның өзінен.</span><span class="sxs-lookup"><span data-stu-id="25141-116">From the project itself.</span></span> <span data-ttu-id="25141-117">Бұл жағдайда, жоба сатып алуға тапсырыс үшін әлдеқашан анықталады.</span><span class="sxs-lookup"><span data-stu-id="25141-117">In this case, the project is already defined for the purchase order.</span></span></li>
<li><span data-ttu-id="25141-118">Жобаның сатып алуға тапсырысына өту арқылы.</span><span class="sxs-lookup"><span data-stu-id="25141-118">By navigating to the project purchase order.</span></span> <span data-ttu-id="25141-119">Сатып алуға тапсырыс жасау үшін жеткізушіні де, жобаны да таңдау керек.</span><span class="sxs-lookup"><span data-stu-id="25141-119">You must select both the vendor and the project to create the purchase order for.</span></span></li>
</ul></td>
<td><span data-ttu-id="25141-120">Элементтер жеткізуші есеп-шоты жаңартылған кезде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="25141-120">Items are consumed when the vendor invoice is updated.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="25141-121">Сатып алуға тапсырысты сату тапсырысынан жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="25141-121">Create a purchase order from a sales order.</span></span></td>
<td><span data-ttu-id="25141-122">Бұл әдісті жобадан сату тапсырысын жасаған кезде элементтерді сатып алу үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="25141-122">Use this method to purchase items when you create a sales order from a project.</span></span></td>
<td><span data-ttu-id="25141-123">Элементтер сату тапсырысы тұтынушыға есеп-шот бойынша ұсынылған кезде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="25141-123">Items are consumed when the sales order is invoiced to the customer.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="25141-124">Сатып алуға тапсырысты элемент талабы бөлімінен жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="25141-124">Create a purchase order from an item requirement.</span></span></td>
<td><span data-ttu-id="25141-125">Бұл әдісті жобадан элемент талабын жасаған кезде элементтерді сатып алу үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="25141-125">Use this method to purchase items when you create an item requirement from a project.</span></span></td>
<td><span data-ttu-id="25141-126">Элементтер элемент талабының тауар жөнелтпе құжаты жаңартылған кезде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="25141-126">Items are consumed when the item requirement packing slip is updated.</span></span></td>
</tr>
</tbody>
</table>

> [!NOTE] 
> <span data-ttu-id="25141-127">Жеткізуші есеп-шотын немесе тауар жөнелтпе құжатын жаңартқан кезде, сізден элемент талабы бойынша тауар жөнелтпе құжатын жаңарту сұралады.</span><span class="sxs-lookup"><span data-stu-id="25141-127">When you update the vendor invoice or packing slip, you're prompted to update the packing slip on the item requirement.</span></span>

<span data-ttu-id="25141-128">Қосымша ақпарат алу үшін [Элемент талабынан сатып алуға тапсырыс бойынша элементтерді алу](tasks/receive-items-purchase-order-item-requirement.md) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="25141-128">For more information, see [Receive items on purchase order from item requirement](tasks/receive-items-purchase-order-item-requirement.md).</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]