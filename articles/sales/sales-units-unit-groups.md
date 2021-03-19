---
title: Бірліктер мен бірлік топтары
description: Бұл тақырыпта Dynamics 365 Project Operations бағдарламасында бірліктер мен бірлік топтарын жасау жолдары туралы ақпарат берілген.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 162366f4b7aa678b4e39d9745a657037bf36cbe0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5277345"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="45fc2-103">Бірліктер мен бірлік топтары</span><span class="sxs-lookup"><span data-stu-id="45fc2-103">Units and unit groups</span></span>

<span data-ttu-id="45fc2-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="45fc2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="45fc2-105">Бірліктер - өнімдер не қызметтер сатылатын сандар немесе өлшемдер.</span><span class="sxs-lookup"><span data-stu-id="45fc2-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="45fc2-106">Мысалы, бақша жабдықтары сатылса, дәндерді бумаларда, қораптарда және тұғырларда сатуға болады.</span><span class="sxs-lookup"><span data-stu-id="45fc2-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="45fc2-107">Бірлік тобы - осы әр түрлі бірліктер топтамасы.</span><span class="sxs-lookup"><span data-stu-id="45fc2-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="45fc2-108">Осы тақырыптағы қадамдарды орындау үшін жүйе әкімшісі немесе Sales Professional менеджер рөліне тағайындалғаныңызға немесе балама рұқсаттарыңыз бар екеніне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="45fc2-109">Бірлік тобын жасау</span><span class="sxs-lookup"><span data-stu-id="45fc2-109">Create a unit group</span></span>

1. <span data-ttu-id="45fc2-110">Торап картасынан **Бірліктер** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="45fc2-111">**Жаңа** түймешігін таңдаңыз және **Бірлік тобын жасау** диалогтық терезесінде бірлік атын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-111">Select **New**, and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="45fc2-112">**Басты бірлік** өрісінде, өнім сатылатын ең төменгі жалпы өлшем бірлігін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="45fc2-113">Мысалы, "бөлік" немесе "унция" енгізе аласыз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="45fc2-114">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="45fc2-115">Бірліктер тобына бірліктер қосу</span><span class="sxs-lookup"><span data-stu-id="45fc2-115">Add units to a unit group</span></span>

1. <span data-ttu-id="45fc2-116">Бірліктер тобын ашып, **Қатысты** қойыншасында **Бірліктер** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="45fc2-117">Әлдеқашан қосылған басты бірлікті көресіз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="45fc2-118">**Жаңа бірлік қосу** түймешігін таңдаңыз және **Жылдам жасау: Бірлік** бетіндегі **Аты** өрісінде бірлік атын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-118">Select **Add New Unit**, and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="45fc2-119">**Мөлшер** өрісінде бірлік қамтитын мөлшерді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="45fc2-120">Мысалы, өрісте екі бөлік қамтылса, "2" деп енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="45fc2-121">**Негізгі бірлік** өрісінде, бірлік үшін ең төменгі өлшем бірлігін орнату үшін негізгі бірлікті таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="45fc2-122">Мысалы, "Бөлік" нұсқасын таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="45fc2-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="45fc2-123">**Сақтау** пәрменін таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="45fc2-123">Select **Save**:</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]