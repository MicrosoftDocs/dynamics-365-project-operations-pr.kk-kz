---
title: Жобаның шығыс санаттарын Finance and Operations және Project Service Automation арасында синхрондаңыз
description: Бұл тақырыпта жобаның шығыс санаттарын Microsoft Dynamics 365 Finance және Dynamics 365 Project Service Automation арасында синхрондау үшін пайдаланылатын үлгілер мен негізгі тапсырмалар сипатталады.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 7dd914dc-1913-45eb-8a67-e897b00089fa
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 757fe1dbc804b986fc3334ebae7254a3f0491f59
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753094"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="74462-103">Жобаның шығыс санаттарын Finance and Operations және Project Service Automation арасында синхрондаңыз</span><span class="sxs-lookup"><span data-stu-id="74462-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="74462-104">Бұл тақырыпта жобаның шығыс санаттарын Dynamics 365 Finance және Dynamics 365 Project Service Automation арасында синхрондау үшін пайдаланылатын үлгілер мен негізгі тапсырмалар сипатталады.</span><span class="sxs-lookup"><span data-stu-id="74462-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="74462-105">Жоба тапсырмаларын біріктіру, шығындар транзакциясының санаттары, сағаттық болжамдар, шығын болжамдары және функционалды құлыптау 8.0 нұсқасында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="74462-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="74462-106">Нақты көрсеткіштерді біріктіру 8.0.1 немесе одан кейінгі нұсқада қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="74462-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="74462-107">Егер Enterprise Edition 7.3.0 нұсқасын пайдалансаңыз, 4132657 білім қоры мен 4132660 білім қорын орнатқаннан кейін, үлгілерді жоба тапсырмаларын, шығыс транзакция санаттарын, сағаттық болжамдарды, шығын болжамдарын және нақты көрсеткіштерді біріктіру және функционалды құлыптауды конфигурациялау үшін пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="74462-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="74462-108">Бухгалтерлік шоттар бойынша таратуларды қалпына келтіру қажет, сондай-ақ 4131710 білім қорын орнатуды ұсынамыз.</span><span class="sxs-lookup"><span data-stu-id="74462-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="74462-109">Project Service Automation және Finance бағдарламасына арналған деректер ағыны</span><span class="sxs-lookup"><span data-stu-id="74462-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="74462-110">Project Service Automation және Finance біріктіру шешімі Project Service Automation және Finance даналары ішінде деректерді синхрондау үшін деректерді біріктіру мүмкіндігін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="74462-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="74462-111">Деректерді біріктіру функциясымен қолжетімді болатын біріктіру үлгілері жобаның шығыс транзакциясы санаттары туралы деректер ағынын Finance және Project Service Automation арасында қосады.</span><span class="sxs-lookup"><span data-stu-id="74462-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="74462-112">Егер жобаның шығыс санаттары Finance жүйесінде игерілсе, біріктіру ағыны Finance жүйесінен Project Service Automation бағдарламасына бірінші орында тұрады.</span><span class="sxs-lookup"><span data-stu-id="74462-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="74462-113">Жобаның шығыс санаттарының біріктіру идентификаторлары Project Service Automation бағдарламасынан Finance жүйесіге синхрондалу арқылы жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="74462-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="74462-114">Егер жобаның шығыс санаттары Project Service Automation бағдарламасында игерілсе, біріктіру ағыны Project Service Automation бағдарламасынан Finance жүйесіне бірінші орында тұрады.</span><span class="sxs-lookup"><span data-stu-id="74462-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="74462-115">Жоба санаттары Project Service Automation бағдарламасынан синхрондалудан бұрын Finance жүйесінде конфигурациялануы қажет.</span><span class="sxs-lookup"><span data-stu-id="74462-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="74462-116">Содан соң Finance жүйесінен қайтадан Project Service Automation бағдарламасына синхрондап, содан соң тағы да Project Service Automation бағдарламасынан Finance жүйесіне синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="74462-117">Осылайша, сіз санаттар бір-бірімен байланысты екеніне және ешқандай көшірмелер жасалмайтынына кепілдік бересіз.</span><span class="sxs-lookup"><span data-stu-id="74462-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="74462-118">Әдетте жобаның шығыс санаттары Finance жүйесінде игеріледі.</span><span class="sxs-lookup"><span data-stu-id="74462-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="74462-119">Дегенмен, егер олай болмаса немесе егер шығыс санаттары Project Service Automation бағдарламасында жасалса, жобаның шығыс транзакция санаттары (PSA бағдарламасынан Fin және Ops бағдарламасына) үлгісін пайдалану арқылы алдымен синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="74462-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="74462-120">Содан соң жобаның шығыс транзакция санаттарының (Fin және Ops бағдарламасынан PSA бағдарламасына) үлгісі арқылы синхрондаңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="74462-121">Содан кейін Project Service Automation бағдарламасынан Finance бағдарламасына тағы бір рет синхрондауды жүргізу қажет.</span><span class="sxs-lookup"><span data-stu-id="74462-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="74462-122">Егер алдымен Project Service Automation бағдарламасынан синхрондайтын болсаңыз, синхрондалу жүргізілмес бұрын Finance жүйесінде келесі талаптар орындалуы қажет:</span><span class="sxs-lookup"><span data-stu-id="74462-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="74462-123">Project Service Automation бағдарламасында орнатылған жоба санатына сәйкес келетін ортақ пайдаланылатын санат болуы қажет және ол **Жоба** үшін де, сондай-ақ **Шығыс** үшін де қосулы болуы қажет.</span><span class="sxs-lookup"><span data-stu-id="74462-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="74462-124">Біріктірілуі тиіс әрбір Finance заңды нысаны үшін келесі жоба санаттары болуы қажет:</span><span class="sxs-lookup"><span data-stu-id="74462-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="74462-125">**Жоба санаты** бар.</span><span class="sxs-lookup"><span data-stu-id="74462-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="74462-126">**Шығыста пайдалану** қосылған.</span><span class="sxs-lookup"><span data-stu-id="74462-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="74462-127">**Журналда белсенді** қосылған.</span><span class="sxs-lookup"><span data-stu-id="74462-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="74462-128">**Транзакция түрі** **Шығыс** параметріне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="74462-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="74462-129">Келесі суретте деректердің Project Service Automation және Finance арасында синхрондалу жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="74462-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="74462-130">[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіруге арналған деректер ағыны](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="74462-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="74462-131">Жобаның шығыс санатын Finance жүйесінен Project Service Automation бағдарламасына синхрондау</span><span class="sxs-lookup"><span data-stu-id="74462-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="74462-132">Үлгі және тапсырма</span><span class="sxs-lookup"><span data-stu-id="74462-132">Template and task</span></span>

<span data-ttu-id="74462-133">Үлгіге қатынасу мақсатында, жалпы үлгілерді таңдау үшін Microsoft Power Apps басқару орталығында **Жобалар**, содан кейін оң жақ жоғарғы бұрышта **Жаңа жоба** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-133">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="74462-134">Келесі үлгі және негізгі тапсырма жобаның шығыс санаттарын Finance жүйесінен Project Service Automation бағдарламасына синхрондау үшін пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="74462-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="74462-135">**Деректерді біріктіру функциясындағы үлгі атауы:** жобаның шығыс транзакция санаттары (Fin және Ops бағдарламасынан PSA бағдарламасына)</span><span class="sxs-lookup"><span data-stu-id="74462-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="74462-136">**Жобадағы тапсырма атауы:** PSA бағдарламасына синхрондау санаттары</span><span class="sxs-lookup"><span data-stu-id="74462-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="74462-137">Нысан жиынтығы</span><span class="sxs-lookup"><span data-stu-id="74462-137">Entity set</span></span>

| <span data-ttu-id="74462-138">Қаржы</span><span class="sxs-lookup"><span data-stu-id="74462-138">Finance</span></span>                           | <span data-ttu-id="74462-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="74462-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="74462-140">Санаттарға арналған біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="74462-140">Integration entity for categories</span></span> | <span data-ttu-id="74462-141">Транзакция санаттары</span><span class="sxs-lookup"><span data-stu-id="74462-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="74462-142">Нысан ағыны</span><span class="sxs-lookup"><span data-stu-id="74462-142">Entity flow</span></span>

<span data-ttu-id="74462-143">Жобаның шығыс санаттары Finance бағдарламасында басқарылады және олар Project Service Automation бағдарламасына транзакция санаттары ретінде синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="74462-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="74462-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="74462-144">Power Query</span></span>

<span data-ttu-id="74462-145">Project Service Automation бағдарламасына синхрондау кезінде транзакция санатында шот ұсыну түрін орнату үшін Excel бағдарламасына арналған Microsoft Power Query бағдарламасын пайдалану қажет.</span><span class="sxs-lookup"><span data-stu-id="74462-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="74462-146">Жобаның шығыс транзакция санаттары (Fin және Ops бағдарламасынан PSA бағдарламасына) үлгісі әдепкі баған мен салыстыруды қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="74462-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="74462-147">Егер жеке үлгіңізді жасасаңыз, Power Query бағдарламасында шартты бағанды қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="74462-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="74462-148">Осы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-148">Follow these steps.</span></span>

1. <span data-ttu-id="74462-149">Жобаның шығыс транзакция санаттарының (Fin және Ops бағдарламаларынан PSA бағдарламасына) үлгісінде жобаның шығыс санаттарыны салыстырылуын ашу үшін көрсеткіні басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="74462-150">Power Query бағдарламасын ашу үшін **Кеңейтілген сұрау және сүзгілеу** сілтемесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="74462-151">**Шартты бағанды қосу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="74462-152">Жаңа бағанға арналған **BillingType** сияқты атауды енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="74462-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="74462-153">Келесі шартты енгізіңіз: **егер САНАТ ИДЕНТИФИКАТОРЫ нөлге тең болмаса, онда 19235001, нөлге тең**.</span><span class="sxs-lookup"><span data-stu-id="74462-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="74462-154">Бағанда **ОК** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="74462-155">Осы жаңа бағанды салыстыру бетінде салыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="74462-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="74462-156">Келесі суретте деректерді біріктіру қызметіндегі үлгі тапсырмасын салыстыру мысалы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="74462-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="74462-157">Салыстыру Finance жүйесінен Project Service Automation жүйесіне синхрондалатын өріс ақпаратын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="74462-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="74462-158">[![Үлгіні салыстыру](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="74462-158">[![Template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="74462-159">Жобаның шығыс санатын Project Service Automation бағдарламасынан Finance жүйесіне синхрондау</span><span class="sxs-lookup"><span data-stu-id="74462-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="74462-160">Үлгі және тапсырма</span><span class="sxs-lookup"><span data-stu-id="74462-160">Template and task</span></span>

<span data-ttu-id="74462-161">Келесі үлгі және негізгі тапсырма жобаның шығыс санаттарын Project Service Automation бағдарламасынан Finance жүйесіне синхрондау үшін пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="74462-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="74462-162">**Деректерді біріктіру функциясындағы үлгі атауы:** жобаның шығыс транзакция санаттары (PSA бағдарламасынан Fin және Ops бағдарламасына)</span><span class="sxs-lookup"><span data-stu-id="74462-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="74462-163">**Жобадағы тапсырма атауы:** Fin Ops бағдарламасына синхрондау санаттары</span><span class="sxs-lookup"><span data-stu-id="74462-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="74462-164">Нысан жиынтығы</span><span class="sxs-lookup"><span data-stu-id="74462-164">Entity set</span></span>

| <span data-ttu-id="74462-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="74462-165">Project Service Automation</span></span> | <span data-ttu-id="74462-166">Қаржы</span><span class="sxs-lookup"><span data-stu-id="74462-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="74462-167">Транзакция санаттары</span><span class="sxs-lookup"><span data-stu-id="74462-167">Transaction categories</span></span>     | <span data-ttu-id="74462-168">Санаттарға арналған біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="74462-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="74462-169">Нысан ағыны</span><span class="sxs-lookup"><span data-stu-id="74462-169">Entity flow</span></span>

<span data-ttu-id="74462-170">Жобаның шығыс санаттары Finance бағдарламасында басқарылады және олар Project Service Automation бағдарламасына транзакция санаттары ретінде синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="74462-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="74462-171">Finance жүйесіне қайта синхрондау Project Service Automation бағдарламасының біріктіру идентификаторымен Finance жүйесінде жоба санатын жаңартады.</span><span class="sxs-lookup"><span data-stu-id="74462-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="74462-172">Деректерді біріктіруде үлгіні салыстыру</span><span class="sxs-lookup"><span data-stu-id="74462-172">Template mapping in Data integration</span></span>

<span data-ttu-id="74462-173">Келесі суретте деректерді біріктіру қызметіндегі үлгі тапсырмасын салыстыру мысалы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="74462-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="74462-174">Картада Project Service Automation бағдарламасынан Finance бағдарламасына синхрондалатын өріс туралы ақпарат көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="74462-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="74462-175">[![Үлгіні салыстыру](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="74462-175">[![Template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>
