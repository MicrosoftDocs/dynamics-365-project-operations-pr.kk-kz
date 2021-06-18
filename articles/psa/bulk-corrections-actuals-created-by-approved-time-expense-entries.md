---
title: Бекітілген уақыт және шығыс жазбаларымен жасалған нақты деректерді жаппай түзетулер
description: Бұл бөлімде егер есеп-шот ұсыну аяқталмаған болса әкімшінің бұған дейін бекітілген уақыт немесе шығыс жазбаларына бірлі-жарым немесе жаппай түзетулер енгізуі жөнінде түсінік беріледі.
author: rumant
ms.date: 04/02/2020
ms.topic: article
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
search.app:
- ProjectOperations
ms.openlocfilehash: c6d849e4be9e3687396cd6a0c4158d92f25c7879
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012053"
---
# <a name="bulk-corrections-of-actuals-created-by-approved-time-and-expense-entries"></a><span data-ttu-id="5ccae-103">Бекітілген уақыт және шығыс жазбаларымен жасалған нақты деректерді жаппай түзетулер</span><span class="sxs-lookup"><span data-stu-id="5ccae-103">Bulk corrections of actuals created by approved time and expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="5ccae-104">Кей кезде уақыт немесе шығыс жазбасы дұрыс емес енгізілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="5ccae-104">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="5ccae-105">Мысалы, уақыт жазбасын жасау кезінде кеңесші қате күнді таңдауы мүмкін немесе шығысты енгізу кезінде сандарды ауыстыруы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="5ccae-105">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="5ccae-106">Егер кеңесші жіберілген жазбаларға жаңартулар енгізе алмаса, әкімші жоба жазбасын тікелей түзете алады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-106">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="5ccae-107">Осы тақырыптағы процедураларды аяқтау үшін сізге әкімшінің рұқсаты қажет.</span><span class="sxs-lookup"><span data-stu-id="5ccae-107">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="5ccae-108">Бекітілген уақыт жазбаларын түзету</span><span class="sxs-lookup"><span data-stu-id="5ccae-108">Correct approved time entries</span></span>     

<span data-ttu-id="5ccae-109">Жобаның бір немесе бірнеше уақыт жазбаларын түзету үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-109">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="5ccae-110">**Сатылым** аймағында **Транзакциялар**, содан соң **Бекітілген уақыт** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-110">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="5ccae-111">**Бекітілген уақыт** тізімінде түзету үшін бір немесе бірнеше бекітілген уақытты тауып, таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-111">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="5ccae-112">Тиісті жазбаларды табу үшін сүзгіні пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-112">You can use the filter to locate related entries.</span></span> <span data-ttu-id="5ccae-113">Мысалы, жоба идентификаторы бойынша сүзгілеп, сол жоба идентификаторы бар барлық бекітіліген уақыт жазбаларын таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-113">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="5ccae-114">**Дұрыс жазбалар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-114">Select **Correct entries**.</span></span> <span data-ttu-id="5ccae-115">Жаңа түзету журналы **Уақыт бойынша түзету** тағайындалған түрімен автоматты түрде жасалады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-115">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="5ccae-116">Сіз таңдаған жазбалар журналға қосылады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-116">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="5ccae-117">**Жаңа журнал** бетінде түзету журналына арналған **Сипаттама** параметрін енгізіп, содан соң **Уақыт жазбасының түзетулері** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-117">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  
5. <span data-ttu-id="5ccae-118">**Уақыт жазбаларының жаңа мәндері** бөлімінде қажетінше тиісті ақпараты бар өрістерді жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-118">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="5ccae-119">Мысалы, сіз тағайындалған жобаны немесе тапсырыс беруге болатын ресурстарды өзгерте аласыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-119">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="5ccae-120">**Алдын ала қарау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-120">Select **Preview**.</span></span> <span data-ttu-id="5ccae-121">Диалогтық терезеде **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-121">In the dialog box, select **OK**.</span></span> <span data-ttu-id="5ccae-122">**Журнал жолы** қойыншасында кері қайтарылған таңдалған уақыт жазбаларына және жасалған түзетілген тиісті жолдарға қатысты бастапқы нақты деректер тізімін қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-122">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="5ccae-123">Егер қосымша түзетулер жасау қажет болса, 5-ші және 6-шы қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-123">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="5ccae-124">Барлық түзетілген нақты деректерде сіздің **Уақыт жазбаларының жаңа мәндері** бөлімінде таңдаған мәндер болады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-124">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="5ccae-125">Егер түзетулер күтілгендей болса, **Растау** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-125">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="5ccae-126">Диалогтық терезеде **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-126">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="5ccae-127">**Сатылым** аймағына қайта оралып, **Жобалар** параметрін таңдаңыз, содан соң уақыт жазбаларын жаңартқан жобаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-127">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="5ccae-128">**Жобалар** бетіндегі **Нақты деректер** қойыншасында жасалған өзгерістерді қараңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-128">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="5ccae-129">Егер **Нақты деректер** қойыншасы көрінбесе **Қатысты** > **Нақты деректер** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-129">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="5ccae-130">**Нақты байланыстырылған көрініс** тізімінде кері қайтарылған бастапқы уақыт жазбаларының тиісті түзетілген уақыт жазбалары ретінде көрсетілетінін қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-130">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="5ccae-131">Мысалы, келесі сызбада «Сомасы» бағанында көрсетілетін дебеттерден тұратын 8,00 шамасы бар екі жол элементі бар.</span><span class="sxs-lookup"><span data-stu-id="5ccae-131">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="5ccae-132">Сонымен қатар «Сомасы» бағанында табысқа жазылатын соманы көрсететін -8,00 шамасы бар екі жол элементі бар.</span><span class="sxs-lookup"><span data-stu-id="5ccae-132">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="5ccae-133">Бұл түзетулер шаманы нөлге келтіреді.</span><span class="sxs-lookup"><span data-stu-id="5ccae-133">These corrections bring the quantity to zero.</span></span>

![Нақты байланыстырылған көрініс тізімі](https://github.com/MicrosoftDocs/dynamics-365-customer-engagement-pr/blob/bulk-corrections-actuals-created-by-approved-time-expense-entries.md/time-actuals.png)
 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="5ccae-135">Бекітілген шығыс жазбаларын түзету</span><span class="sxs-lookup"><span data-stu-id="5ccae-135">Correct approved expense entries</span></span>

<span data-ttu-id="5ccae-136">Бір немесе бірнеше шығыс жазбаларын түзету үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="5ccae-137">**Сатылым** аймағындағы сол жақ навигация тақтасында **Транзакциялар** бөлімінде **Бекітілген шығыстар** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="5ccae-138">**Бекітілген шығыстар** тізімінде түзету қажет жобаны таңдап, содан соң **Жазбаларды түзету** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="5ccae-139">Жаңа түзету журналы **Шығыс түзету** тағайындалған түрімен автоматты түрде жасалады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="5ccae-140">**Жаңа журнал** бетінде түзету үшін **Сипаттама** өрісін енгізіңіз, сондай-ақ **Шығысты түзету** қойыншасындағы **Шығыстардың жаңа мәндері** бөлімінде таңдалған шығыс жолдары үшін түзеткіңіз келетін деректер өрістерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="5ccae-141">Мысалы, шығысты басқа **Жоба** параметріне тағайындауға немесе **Шығыс санаты**, **Шығыс күні** немесе **Тапсырыс беруге болатын ресурс** параметрлерін түзетуге болады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="5ccae-142">**Алдын ала қарау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-142">Select **Preview**.</span></span> <span data-ttu-id="5ccae-143">Диалогтық терезеде **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="5ccae-144">**Журнал жолы** қойыншасындағы түзетулерді тексеріңіз. Кері қайтарылған таңдалған шығыс жазбаларына және жасалған түзетілген тиісті жолдарға қатысты бастапқы нақты деректер тізімін қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="5ccae-145">Егер түзетілген мәндер күтілгендей болса, **Растау** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="5ccae-146">Диалогтық терезеде **ОК** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="5ccae-147">Егер мәндер күтілгендей көрсетілмесе, **Бекітілген шығыстар** тізіміне оралу үшін **Болдырмау** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="5ccae-148">2-5 қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="5ccae-149">Түзетілген нақты деректерде сіздің **Шығыстардың жаңа мәндері** бөлімінде таңдаған мәндер болады.</span><span class="sxs-lookup"><span data-stu-id="5ccae-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="5ccae-150">Түзету журналын растағаннан кейін, өзгертулерді көру үшін жобаға немесе жаңартылған жобаларға қайта оралыңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="5ccae-151">Жоба бетіндегі **Нақты деректер** қойыншасында **Нақты байланыстырылған көрініс** бөлімін қарап шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="5ccae-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="5ccae-152">Бастапқы жазбалар мен түзетілген жазбалар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="5ccae-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="5ccae-153">Төмендегі сызбада шығыс жазбасының бастапқы сомалары және шығы жазбасының тиісті түзетілген сомалары көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="5ccae-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 

![Шығыстың нақты деректері](https://user-images.githubusercontent.com/60806505/77122219-4cd52900-69fa-11ea-8349-ccd2ffebf640.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]