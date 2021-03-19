---
title: Еңбек және шығындардың стандартты құнын конфигурациялау
description: Бұл тақырыпта жобаға арналған еңбек және шығындардың стандартты құнын орнату жолы түсіндірілген.
author: Yowelle
manager: AnnBe
ms.date: 08/02/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjCostPriceHour, ProjSalesPriceHour, ProjCostPriceExpense, ProjSalesPriceCost
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b16ed50584b2b4535d1c61fe7069708182a4820e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288341"
---
# <a name="configure-standard-costs-for-labor-and-expenses"></a><span data-ttu-id="40e52-103">Еңбек және шығындардың стандартты құнын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="40e52-103">Configure standard costs for labor and expenses</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="40e52-104">Бұл тақырыпта жобаға арналған еңбек және шығындардың стандартты құнын орнату жолы түсіндірілген.</span><span class="sxs-lookup"><span data-stu-id="40e52-104">This topic explains how to set up standard costs for labor and expenses for a project.</span></span> <span data-ttu-id="40e52-105">Бұл тапсырмада USSI деректер жиынтығы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="40e52-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="40e52-106">Шарлау аумағында, **Модульдер > Жобаларды басқару және есепке алу > Орнату > Бағалар > Шығын (сағат)** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-106">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (hour)**.</span></span>
2. <span data-ttu-id="40e52-107">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-107">Select **New**.</span></span>
3. <span data-ttu-id="40e52-108">**Тиімді күн** өрісінде күнді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-108">In the **Effective date** field, enter a date.</span></span>
4. <span data-ttu-id="40e52-109">**Шыған** өрісіне сан енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-109">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="40e52-110">Жоба санаты үшін стандартты шығынды орната аласыз немесе қызметкер нөмірі, жоба нөмірі, санат, күн немесе олардың кез-келген тіркесімі бойынша шығынды орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="40e52-110">You can set up a standard cost price for the project category, or you can set up a cost price by worker number, project number, category, date, or any combination of these.</span></span> <span data-ttu-id="40e52-111">Қолданылатын шығын – бұл мәліметтің ең жоғары деңгейіне ие шығын.</span><span class="sxs-lookup"><span data-stu-id="40e52-111">The cost price that is applied is the cost price with the highest level of detail.</span></span>  
5. <span data-ttu-id="40e52-112">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-112">Select **Save**.</span></span>
6. <span data-ttu-id="40e52-113">Шарлау аумағында, **Модульдер > Жобаларды басқару және есепке алу > Орнату > Бағалар > Сатылым бағасы (сағат)** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-113">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (hour)**.</span></span>
7. <span data-ttu-id="40e52-114">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-114">Select **New**.</span></span>
8. <span data-ttu-id="40e52-115">**Тиімді күн** өрісінде күнді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-115">In the **Effective date** field, enter a date.</span></span>
9. <span data-ttu-id="40e52-116">**Жарамды** өрісінде опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-116">In the **Valid for** field, select an option.</span></span>
10. <span data-ttu-id="40e52-117">**Баға белгілеу** өрісіне сан енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-117">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="40e52-118">Бір сағаттық транзакциялар үшін немесе жоба санаты үшін стандартты сатылым бағасын орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="40e52-118">You can set up a standard sales price for hour transactions or for a project category.</span></span> <span data-ttu-id="40e52-119">Сондай-ақ сатылым бағаларын қызметкер нөмірі, жоба нөмірі, санаты, транзакция күні немесе олардың кез-келген тіркесімі бойынша орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-119">You can also set up sales prices by worker number, project number, category, transaction date, or any combination of these.</span></span> <span data-ttu-id="40e52-120">Қызметкер сағат журналына транзакция енгізген кезде қолданылатын нақты сатылым бағасы – бұл мәліметтің ең жоғары деңгейіне ие сатылым бағасы.</span><span class="sxs-lookup"><span data-stu-id="40e52-120">The actual sales price, which is applied when a worker enters a transaction in the Hour journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="40e52-121">Мысалы, жалпы сатылым бағасы да, қызметкердің арнайы сатылым бағасы да орнатылса, қызметкердің арнайы сатылым бағасы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="40e52-121">For example, if both a general sales price and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
11. <span data-ttu-id="40e52-122">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-122">Select **Save**.</span></span>
12. <span data-ttu-id="40e52-123">Бетті жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-123">Close the page.</span></span>
13. <span data-ttu-id="40e52-124">Шарлау аумағында, **Модульдер > Жобаларды басқару және есепке алу > Орнату > Бағалар > Шығын (шығыс)** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-124">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (expense)**.</span></span>
14. <span data-ttu-id="40e52-125">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-125">Select **New**.</span></span>
15. <span data-ttu-id="40e52-126">**Тиімді күн** өрісінде күнді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-126">In the **Effective date** field, enter a date.</span></span>
16. <span data-ttu-id="40e52-127">**Шыған** өрісіне сан енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-127">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="40e52-128">Бірнеше өрісті толтыруға болады, бірақ бұл жазбаны сақтау үшін қажетті минимум.</span><span class="sxs-lookup"><span data-stu-id="40e52-128">Multiple fields can be filled in, but this is the minimum needed to save the record.</span></span>  
17. <span data-ttu-id="40e52-129">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-129">Select **Save**.</span></span>
18. <span data-ttu-id="40e52-130">Шарлау аумағында, **Модульдер > Жобаларды басқару және есепке алу > Орнату > Бағалар > Сатылым бағасы (шығыс)** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-130">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (expense)**.</span></span>
19. <span data-ttu-id="40e52-131">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-131">Select **New**.</span></span>
20. <span data-ttu-id="40e52-132">**Тиімді күн** өрісінде күнді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-132">In the **Effective date** field, enter a date.</span></span>
21. <span data-ttu-id="40e52-133">**Жарамды** өрісінде опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-133">In the **Valid for** field, select an option.</span></span>
22. <span data-ttu-id="40e52-134">**Баға белгілеу** өрісіне сан енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="40e52-134">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="40e52-135">Қызметкер шығындар журналына транзакциялар енгізген кезде қолданылатын нақты сатылым бағасы – бұл мәліметтің ең жоғары деңгейіне ие сатылым бағасы.</span><span class="sxs-lookup"><span data-stu-id="40e52-135">The actual sales price, which is applied when a worker enters transactions in an expense journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="40e52-136">Мысалы, жалпы және қызметкердің арнайы сатылым бағасы орнатылса, қызметкердің арнайы сатылым бағасы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="40e52-136">For example, if both a general and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
23. <span data-ttu-id="40e52-137">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="40e52-137">Select **Save**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]