---
title: Түзету журналдарын жасау және растау
description: Осы тақырып түзету журналын жасау және растау әдісі туралы ақпаратты ұсынады.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 274f99527804b0db81b26201a22eb5a8cbe86c9a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896963"
---
# <a name="create-and-confirm-correction-journals"></a><span data-ttu-id="ad651-103">Түзету журналдарын жасау және растау</span><span class="sxs-lookup"><span data-stu-id="ad651-103">Create and confirm Correction journals</span></span>

<span data-ttu-id="ad651-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="ad651-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ad651-105">Кей кезде уақыт немесе шығыс жазбасы дұрыс емес енгізілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="ad651-105">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="ad651-106">Мысалы, уақыт жазбасын жасау кезінде кеңесші қате күнді таңдауы мүмкін немесе шығысты енгізу кезінде сандарды ауыстыруы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="ad651-106">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="ad651-107">Егер кеңесші жіберілген жазбаларға жаңартулар енгізе алмаса, әкімші жоба жазбасын тікелей түзете алады.</span><span class="sxs-lookup"><span data-stu-id="ad651-107">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="ad651-108">Осы тақырыптағы процедураларды аяқтау үшін сізге әкімшінің рұқсаты қажет.</span><span class="sxs-lookup"><span data-stu-id="ad651-108">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="ad651-109">Бекітілген уақыт жазбаларын түзету</span><span class="sxs-lookup"><span data-stu-id="ad651-109">Correct approved time entries</span></span>     

<span data-ttu-id="ad651-110">Жобаның бір немесе бірнеше уақыт жазбаларын түзету үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-110">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="ad651-111">**Сатылым** аймағында **Транзакциялар**, содан соң **Бекітілген уақыт** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-111">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="ad651-112">**Бекітілген уақыт** тізімінде түзету үшін бір немесе бірнеше бекітілген уақытты тауып, таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-112">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="ad651-113">Тиісті жазбаларды табу үшін сүзгіні пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="ad651-113">You can use the filter to locate related entries.</span></span> <span data-ttu-id="ad651-114">Мысалы, жоба идентификаторы бойынша сүзгілеп, сол жоба идентификаторы бар барлық бекітіліген уақыт жазбаларын таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="ad651-114">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="ad651-115">**Дұрыс жазбалар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-115">Select **Correct entries**.</span></span> <span data-ttu-id="ad651-116">Жаңа түзету журналы **Уақыт бойынша түзету** тағайындалған түрімен автоматты түрде жасалады.</span><span class="sxs-lookup"><span data-stu-id="ad651-116">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="ad651-117">Сіз таңдаған жазбалар журналға қосылады.</span><span class="sxs-lookup"><span data-stu-id="ad651-117">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="ad651-118">**Жаңа журнал** бетінде түзету журналына арналған **Сипаттама** параметрін енгізіп, содан соң **Уақыт жазбасының түзетулері** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-118">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  

5. <span data-ttu-id="ad651-119">**Уақыт жазбаларының жаңа мәндері** бөлімінде қажетінше тиісті ақпараты бар өрістерді жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-119">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="ad651-120">Мысалы, сіз тағайындалған жобаны немесе тапсырыс беруге болатын ресурстарды өзгерте аласыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-120">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="ad651-121">**Алдын ала қарау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-121">Select **Preview**.</span></span> <span data-ttu-id="ad651-122">Диалогтық терезеде **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-122">In the dialog box, select **OK**.</span></span> <span data-ttu-id="ad651-123">**Журнал жолы** қойыншасында кері қайтарылған таңдалған уақыт жазбаларына және жасалған түзетілген тиісті жолдарға қатысты бастапқы нақты деректер тізімін қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="ad651-123">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="ad651-124">Егер қосымша түзетулер жасау қажет болса, 5-ші және 6-шы қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-124">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="ad651-125">Барлық түзетілген нақты деректерде сіздің **Уақыт жазбаларының жаңа мәндері** бөлімінде таңдаған мәндер болады.</span><span class="sxs-lookup"><span data-stu-id="ad651-125">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="ad651-126">Егер түзетулер күтілгендей болса, **Растау** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-126">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="ad651-127">Диалогтық терезеде **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-127">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="ad651-128">**Сатылым** аймағына қайта оралып, **Жобалар** параметрін таңдаңыз, содан соң уақыт жазбаларын жаңартқан жобаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-128">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="ad651-129">**Жобалар** бетіндегі **Нақты деректер** қойыншасында жасалған өзгерістерді қараңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-129">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="ad651-130">Егер **Нақты деректер** қойыншасы көрінбесе **Қатысты** > **Нақты деректер** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-130">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="ad651-131">**Нақты байланыстырылған көрініс** тізімінде кері қайтарылған бастапқы уақыт жазбаларының тиісті түзетілген уақыт жазбалары ретінде көрсетілетінін қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="ad651-131">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="ad651-132">Мысалы, келесі сызбада «Сомасы» бағанында көрсетілетін дебеттерден тұратын 8,00 шамасы бар екі жол элементі бар.</span><span class="sxs-lookup"><span data-stu-id="ad651-132">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="ad651-133">Сонымен қатар, «Сомасы» бағанында табысқа жазылатын соманы көрсететін -8,00 шамасы бар екі жол элементі бар.</span><span class="sxs-lookup"><span data-stu-id="ad651-133">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="ad651-134">Бұл түзетулер шаманы нөлге келтіреді.</span><span class="sxs-lookup"><span data-stu-id="ad651-134">These corrections bring the quantity to zero.</span></span>

 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="ad651-135">Бекітілген шығыс жазбаларын түзету</span><span class="sxs-lookup"><span data-stu-id="ad651-135">Correct approved expense entries</span></span>

<span data-ttu-id="ad651-136">Бір немесе бірнеше шығыс жазбаларын түзету үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="ad651-137">**Сатылым** аймағындағы сол жақ навигация тақтасында **Транзакциялар** бөлімінде **Бекітілген шығыстар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="ad651-138">**Бекітілген шығыстар** тізімінде түзету қажет жобаны таңдап, содан соң **Жазбаларды түзету** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="ad651-139">Жаңа түзету журналы **Шығыс түзету** тағайындалған түрімен автоматты түрде жасалады.</span><span class="sxs-lookup"><span data-stu-id="ad651-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="ad651-140">**Жаңа журнал** бетінде түзету үшін **Сипаттама** өрісін енгізіңіз, сондай-ақ **Шығысты түзету** қойыншасындағы **Шығыстардың жаңа мәндері** бөлімінде таңдалған шығыс жолдары үшін түзеткіңіз келетін деректер өрістерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="ad651-141">Мысалы, шығысты басқа **Жоба** параметріне тағайындауға немесе **Шығыс санаты**, **Шығыс күні** немесе **Тапсырыс беруге болатын ресурс** параметрлерін түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="ad651-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="ad651-142">**Алдын ала қарау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-142">Select **Preview**.</span></span> <span data-ttu-id="ad651-143">Диалогтық терезеде **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="ad651-144">**Журнал жолы** қойыншасындағы түзетулерді тексеріңіз. Кері қайтарылған таңдалған шығыс жазбаларына және жасалған түзетілген тиісті жолдарға қатысты бастапқы нақты деректер тізімін қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="ad651-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="ad651-145">Егер түзетілген мәндер күтілгендей болса, **Растау** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="ad651-146">Диалогтық терезеде **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="ad651-147">Егер мәндер күтілгендей көрсетілмесе, **Бекітілген шығыстар** тізіміне оралу үшін **Болдырмау** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="ad651-148">2-5 қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="ad651-149">Түзетілген нақты деректерде сіздің **Шығыстардың жаңа мәндері** бөлімінде таңдаған мәндер болады.</span><span class="sxs-lookup"><span data-stu-id="ad651-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="ad651-150">Түзету журналын растағаннан кейін, өзгертулерді көру үшін жобаға немесе жаңартылған жобаларға қайта оралыңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="ad651-151">Жоба бетіндегі **Нақты деректер** қойыншасында **Нақты байланыстырылған көрініс** бөлімін қарап шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="ad651-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="ad651-152">Бастапқы жазбалар мен түзетілген жазбалар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="ad651-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="ad651-153">Төмендегі сызбада шығыс жазбасының бастапқы сомалары және шығы жазбасының тиісті түзетілген сомалары көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="ad651-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 


