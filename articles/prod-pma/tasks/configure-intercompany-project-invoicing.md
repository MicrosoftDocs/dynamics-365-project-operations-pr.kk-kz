---
title: Компанияаралық жоба есеп-шоттарын конфигурациялау
description: Бұл тақырыпта ұйымыңыздағы екі компания арасында жоба есеп-шотын орнату жолы көрсетілген.
author: Yowelle
manager: AnnBe
ms.date: 07/29/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendTable, InterCompanyTradingRelationSetupVendor, SysDataAreaSelectLookup, ProjParameters, ProjPosting, ProjTransferPrice
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 1cb53cb63ee11082146455ec9f13790501dc3d1d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079719"
---
# <a name="configure-intercompany-project-invoicing"></a><span data-ttu-id="dcc8d-103">Компанияаралық жоба есеп-шоттарын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="dcc8d-103">Configure intercompany project invoicing</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="dcc8d-104">Бұл тақырыпта ұйымыңыздағы екі компания арасында жоба есеп-шотын орнату жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-104">This topic shows how to set up project invoicing between two companies in your organization.</span></span> <span data-ttu-id="dcc8d-105">Бұл тапсырмада USSI деректер жиынтығы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="dcc8d-106">Шарлау аумағында, **Модульдер > Несие берушілер > Жеткізушілер > Барлық жеткізушілер** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-106">In the navigation pane, go to **Modules > Accounts payable > Vendors > All vendors**.</span></span>
2. <span data-ttu-id="dcc8d-107">**Барлық жеткізушілер** тізімінде, қажетті жазбаны табыңыз және таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-107">In the **All vendors** list, find and select the desired record.</span></span>
3. <span data-ttu-id="dcc8d-108">"Әрекеттер" тақтасында, **Жалпы** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-108">On the Action Pane, select **General**.</span></span>
4. <span data-ttu-id="dcc8d-109">**Компанияаралық** таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-109">Select **Intercompany**.</span></span>
5. <span data-ttu-id="dcc8d-110">Компанияаралық сауданы қосу үшін **Белсенді** режимін **Иә** мәніне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-110">Set **Active** to **Yes** to enable intercompany trading.</span></span>
6. <span data-ttu-id="dcc8d-111">**Тұтынушы компаниясы** өрісінде, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-111">In the **Customer company** field, enter or select a value.</span></span>
7. <span data-ttu-id="dcc8d-112">**Менің тіркелгім** өрісінде, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-112">In the **My account** field, enter or select a value.</span></span>
8. <span data-ttu-id="dcc8d-113">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-113">Select **Save**.</span></span>
9. <span data-ttu-id="dcc8d-114">Басты бетке оралу үшін беттерді жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-114">Close the pages to return to the home page.</span></span>
10. <span data-ttu-id="dcc8d-115">Шарлау аумағында, **Модульдер > Жобаларды басқару және есепке алу > Орнату > Жобаларды басқару және есепке алу параметрлері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-115">In the navigation pane, go to **Modules > Project management and accounting > Setup > Project management and accounting parameters**.</span></span>
11. <span data-ttu-id="dcc8d-116">**Компанияаралық** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-116">Select the **Intercompany** tab.</span></span>
12. <span data-ttu-id="dcc8d-117">Компанияаралық ресурстар жоспарын және уақыт кестесін қосу үшін жүгірткіні **Иә** мәніне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-117">Move the slider to **Yes** to enable intercompany resource scheduling and timesheets.</span></span>
13. <span data-ttu-id="dcc8d-118">Тізімде таңдалған жолды белгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-118">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="dcc8d-119">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-119">Select **New**.</span></span>
15. <span data-ttu-id="dcc8d-120">**Заңды нысанды қарызға алу** өрісінде, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-120">In the **Borrowing legal entity** field, enter or select a value.</span></span>
16. <span data-ttu-id="dcc8d-121">**Табысты есептеу** тұсына құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-121">Select the **Accrue revenue** check box.</span></span>
17. <span data-ttu-id="dcc8d-122">**Әдепкі уақыт кестесінің санаты** өрісінде, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-122">In the **Default timesheet category** field, enter or select a value.</span></span>
18. <span data-ttu-id="dcc8d-123">**Әдепкі шығын санаты** өрісінде, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-123">In the **Default expense category** field, enter or select a value.</span></span>
19. <span data-ttu-id="dcc8d-124">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-124">Select **Save**.</span></span>
20. <span data-ttu-id="dcc8d-125">Бетті жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-125">Close the page.</span></span>
21. <span data-ttu-id="dcc8d-126">Шарлау аумағында, **Модульдер > Жобаларды басқару және есепке алу > Орнату > Жариялау > Кітапты жариялау параметрі** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-126">In the navigation pane, go to **Modules > Project management and accounting > Setup > Posting > Ledger posting setup**.</span></span>
22. <span data-ttu-id="dcc8d-127">**Кітап тіркелгісінің түрлері** өрісінде опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-127">In the **Ledger account types** field, select an option.</span></span>
23. <span data-ttu-id="dcc8d-128">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-128">Select **New**.</span></span>
24. <span data-ttu-id="dcc8d-129">Жаңа жолдың **Негізгі тіркелгі** өрісінде қажетті мәндерді көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-129">In the **Main account** field of the new row, specify the desired values.</span></span>
25. <span data-ttu-id="dcc8d-130">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-130">Select **Save**.</span></span>
26. <span data-ttu-id="dcc8d-131">Бетті жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-131">Close the page.</span></span>
27. <span data-ttu-id="dcc8d-132">Шарлау аумағында, **Модульдер > Жобаларды басқару және есепке алу > Орнату > Бағалар > Тасымалдау бағасы** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-132">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Transfer price**.</span></span>
28. <span data-ttu-id="dcc8d-133">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-133">Select **New**.</span></span>
29. <span data-ttu-id="dcc8d-134">**Тиімді күн** өрісінде күнді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-134">In the **Effective date** field, enter a date.</span></span>
30. <span data-ttu-id="dcc8d-135">**Заңды нысанды қарызға алу** өрісінде, мәнді енгізіңіз немесе таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-135">In the **Borrowing legal entity** field, enter or select a value.</span></span>
31. <span data-ttu-id="dcc8d-136">**Тасымалдау бағасының үлгісі** өрісінде опцияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-136">In the **Transfer price model** field, select an option.</span></span>
32. <span data-ttu-id="dcc8d-137">**Баға белгілеу** өрісіне сан енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-137">In the **Pricing** field, enter a number.</span></span>
33. <span data-ttu-id="dcc8d-138">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="dcc8d-138">Select **Save**.</span></span>

