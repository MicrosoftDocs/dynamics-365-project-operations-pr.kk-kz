---
title: Жоба болжамдарын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына тікелей синхрондау
description: Бұл тақырыпта үлгілер және жобаның сағаттық болжамдары мен жобаның шығыс болжамдарын Microsoft Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance жүйесіне тікелей синхрондау үшін пайдаланылатын негізгі тапсырмалар сипатталады.
author: Yowelle
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
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 58e204b2c1238e00ffb16533cc82dad69fbf77a9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289466"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="1cf46-103">Жоба болжамдарын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына тікелей синхрондау</span><span class="sxs-lookup"><span data-stu-id="1cf46-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="1cf46-104">Бұл тақырыпта үлгілер және жобаның сағаттық болжамдары мен жобаның шығыс болжамдарын Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance жүйесіне тікелей синхрондау үшін пайдаланылатын негізгі тапсырмалар сипатталады.</span><span class="sxs-lookup"><span data-stu-id="1cf46-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="1cf46-105">Жоба тапсырмасын біріктіру, шығыс транзакция санаттары, сағаттық болжамдар, шығыс болжамдар және функционалдылықты құлыптау 8.0. нұсқасында қолжетімді болады.</span><span class="sxs-lookup"><span data-stu-id="1cf46-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="1cf46-106">Нақты көрсеткіштерді біріктіру 8.0.1 немесе одан кейінгі нұсқада қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="1cf46-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="1cf46-107">Project Service Automation және Finance бағдарламасындағы деректер ағыны</span><span class="sxs-lookup"><span data-stu-id="1cf46-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="1cf46-108">Project Service Automation және Finance бағдарламасын біріктіру шешімі деректерді біріктіру мүмкіндігін Project Service Automation және Finance мысалдары бойынша деректерді синхрондау үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="1cf46-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="1cf46-109">Деректерді біріктіру функциясымен қолжетімді болатын біріктіру үлгілері жобаның сағаттық болжамдары мен жобаның шығыс болжамдары туралы деректер ағынын Project Service Automation бағдарламасынан Finance бағдарламасына жіберуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="1cf46-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="1cf46-110">Келесі суретте деректердің Project Service Automation және Finance арасында синхрондалу жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="1cf46-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="1cf46-111">[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіруге арналған деректер ағыны](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="1cf46-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="1cf46-112">Жобаның сағаттық болжамдары</span><span class="sxs-lookup"><span data-stu-id="1cf46-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="1cf46-113">Үлгі және тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="1cf46-113">Template and tasks</span></span>

<span data-ttu-id="1cf46-114">Қолжетімді үлгілерге қатынасу үшін Microsoft Power Apps басқару орталығында **Жобалар** опциясын таңдап, содан соң жоғарғы оң жақтағы бұрышта жалпы үлгілерді таңдау үшін **Жаңа жоба** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="1cf46-115">Келесі үлгілер және негізгі тапсырмалар жобаның сағаттық болжамдарын Project Service Automation бағдарламасынан Finance бағдарламасына синхрондау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="1cf46-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="1cf46-116">**Деректерді біріктіру функциясындағы үлгі атауы:** жобаның сағаттық болжамдары (PSA бағдарламасынан Fin және Ops бағдарламасына)</span><span class="sxs-lookup"><span data-stu-id="1cf46-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="1cf46-117">**Жобадағы тапсырмалардың атауы**</span><span class="sxs-lookup"><span data-stu-id="1cf46-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="1cf46-118">Транзакция қатынастары</span><span class="sxs-lookup"><span data-stu-id="1cf46-118">Transaction relationships</span></span>
    - <span data-ttu-id="1cf46-119">Шығыс болжамдары</span><span class="sxs-lookup"><span data-stu-id="1cf46-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="1cf46-120">Нысан жиынтығы</span><span class="sxs-lookup"><span data-stu-id="1cf46-120">Entity set</span></span>

| <span data-ttu-id="1cf46-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="1cf46-121">Project Service Automation</span></span> | <span data-ttu-id="1cf46-122">Қаржы</span><span class="sxs-lookup"><span data-stu-id="1cf46-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="1cf46-123">Жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="1cf46-123">Project tasks</span></span>              | <span data-ttu-id="1cf46-124">Жобаның сағаттық болжамдары үшін біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="1cf46-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="1cf46-125">Нысан ағыны</span><span class="sxs-lookup"><span data-stu-id="1cf46-125">Entity flow</span></span>

<span data-ttu-id="1cf46-126">Жобаның сағаттық болжамдары Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жобаның сағаттық болжамдары ретінде синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="1cf46-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="1cf46-127">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="1cf46-127">Prerequisites</span></span>

<span data-ttu-id="1cf46-128">Жобаның сағаттық болжамдарын синхрондау орындалмас бұрын, жобаларды, жоба тапсырмаларын және жобаның шығыс транзакциясының санаттарын синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="1cf46-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="1cf46-129">Power Query</span></span>

<span data-ttu-id="1cf46-130">Жобаның сағаттық болжамдары үлгісінде, осы тапсырмаларды орындау үшін Excel бағдарламасына арналған Microsoft Power Query қондырмасын пайдалану қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="1cf46-131">Біріктіру жаңа сағаттық болжамдарды жасаған кезде пайдаланылатын әдепкі болжам үлгісінің идентификаторын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="1cf46-132">Сағаттық болжамдарға біріге алмайтын тапсырмадағы кез келген ресурсқа арналған жазбаларды сүзгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="1cf46-133">Кез келген бос транзакция санатының жолдарын сүзгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="1cf46-134">Бұл тапсырманы орындамау қате сағаттық болжамдарға әкелуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="1cf46-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="1cf46-135">Әдепкі болжам үлгісінің идентификаторын орнату</span><span class="sxs-lookup"><span data-stu-id="1cf46-135">Set the default forecast model ID</span></span>

<span data-ttu-id="1cf46-136">Үлгідегі әдепкі болжам идентификаторын орнату үшін, **Карта** көрсеткісін салыстыруды ашу үшін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="1cf46-137">Содан кейін **Кеңейтілген сұрау және сүзгілеу** сілтемесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="1cf46-138">Егер әдепкі "Жобаның сағаттық болжамдары" (PSA бағдарламасынан Fin және Ops бағдарламасына) үлгісін пайдалансаңыз, **Қолданылған қадамдар** тізіміндегі **Енгізілген шарт** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="1cf46-139">**Функция** жазбасында, біріктірумен пайдаланылуы керек болжам үлгісінің идентификатор атауы бар **O\_болжам** бағанын ауыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="1cf46-140">Әдепкі үлгіде демо деректерінен алынған болжам үлгісінің идентификаторы бар.</span><span class="sxs-lookup"><span data-stu-id="1cf46-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="1cf46-141">Егер жаңа үлгі жасасаңыз, осы бағанды қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="1cf46-142">Power Query қондырмасында, **Шартты бағанды қосу** параметрін таңдап, **ModelID** сияқты жаңа бағанға арналған атау енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-142">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="1cf46-143">Бағанның шартын енгізіңіз, егер жоба тапсырмасы нөлге тең болмаса, онда \<enter the forecast model ID\>; басқасы нөл.</span><span class="sxs-lookup"><span data-stu-id="1cf46-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="1cf46-144">Ресурсқа арналған жазбаларды сүзгілеу</span><span class="sxs-lookup"><span data-stu-id="1cf46-144">Filter out resource-specific records</span></span>

<span data-ttu-id="1cf46-145">Жобаның сағаттық болжамдары (PSA бағдарламасынан Fin және Ops бағдарламасына) үлгісінде кез келген ресурсқа арналған жазбаларды жоятын әдепкі сүзгі бар.</span><span class="sxs-lookup"><span data-stu-id="1cf46-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="1cf46-146">Егер өз үлгіңізді жасасаңыз, онда осы сүзгіні қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="1cf46-147">Тек **Жалған** жазбалар қамтылатындай етіп **msdyn\_islinetask** бағанында сүзгілеу үшін **Кеңейтілген сұрау және сүзгілеу** сілтемесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="1cf46-148">Бос транзакция санатының жолдарын сүзгілеу</span><span class="sxs-lookup"><span data-stu-id="1cf46-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="1cf46-149">Бос транзакция санаттары бар кез келген жолдарды жою үшін сүзгі қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="1cf46-150">Бұл тапсырма әдепкі үлгіні пайдалануыңызға немесе жеке үлгіні жасауыңызға қарамастан қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="1cf46-151">Бұл сүзгі қорытынды жолдарды сағаттық болжамдардың Finance бағдарламасында қате болуына әкелуі мүмкін Project Service Automation бағдарламасынан жояды.</span><span class="sxs-lookup"><span data-stu-id="1cf46-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="1cf46-152">**Кеңейтілген сұрау және сүзгілеу** сілтемесін **msdyn\_transactioncategory\_value** бағанындаға бос жазбаларды сүзгілеу үшін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="1cf46-153">Деректерді біріктіруде үлгіні салыстыру</span><span class="sxs-lookup"><span data-stu-id="1cf46-153">Template mapping in Data integration</span></span>

<span data-ttu-id="1cf46-154">Келесі суретте деректерді біріктіру қызметіндегі үлгі тапсырмасын салыстыру мысалы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="1cf46-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="1cf46-155">Картада Project Service Automation бағдарламасынан Finance бағдарламасына синхрондалатын өріс туралы ақпарат көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="1cf46-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="1cf46-156">[![Деректерді біріктіруде үлгі тапсырманы салыстыру](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="1cf46-156">[![Template task mapping in data integration](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="1cf46-157">Жобаның шығыс болжамдары</span><span class="sxs-lookup"><span data-stu-id="1cf46-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="1cf46-158">Үлгі және тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="1cf46-158">Template and tasks</span></span>

<span data-ttu-id="1cf46-159">Келесі үлгі және негізгі тапсырмалар жобаның шығыс болжамдарын Project Service Automation бағдарламасынан Finance бағдарламасына синхрондау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="1cf46-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="1cf46-160">**Деректерді біріктіру функциясындағы үлгі атауы:** жобаның шығыс болжамдары (PSA бағдарламасынан Fin және Ops бағдарламасына)</span><span class="sxs-lookup"><span data-stu-id="1cf46-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="1cf46-161">**Жобадағы тапсырмалардың атауы**</span><span class="sxs-lookup"><span data-stu-id="1cf46-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="1cf46-162">Транзакция қатынастары</span><span class="sxs-lookup"><span data-stu-id="1cf46-162">Transaction relationships</span></span> 
    - <span data-ttu-id="1cf46-163">Шығыс болжамдары</span><span class="sxs-lookup"><span data-stu-id="1cf46-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="1cf46-164">Нысан жиынтығы</span><span class="sxs-lookup"><span data-stu-id="1cf46-164">Entity set</span></span>

| <span data-ttu-id="1cf46-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="1cf46-165">Project Service Automation</span></span> | <span data-ttu-id="1cf46-166">Қаржы</span><span class="sxs-lookup"><span data-stu-id="1cf46-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="1cf46-167">Транзакция байланыстары</span><span class="sxs-lookup"><span data-stu-id="1cf46-167">Transaction Connections</span></span>    | <span data-ttu-id="1cf46-168">Жобаның транзакция қатынастарына арналған біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="1cf46-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="1cf46-169">Болжам жолдары</span><span class="sxs-lookup"><span data-stu-id="1cf46-169">Estimate Lines</span></span>             | <span data-ttu-id="1cf46-170">Жобаның шығыс болжамдары үшін біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="1cf46-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="1cf46-171">Нысан ағыны</span><span class="sxs-lookup"><span data-stu-id="1cf46-171">Entity flow</span></span>

<span data-ttu-id="1cf46-172">Жобаның шығыс болжамдары Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жобаның шығыс болжамдары ретінде синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="1cf46-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="1cf46-173">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="1cf46-173">Prerequisites</span></span>

<span data-ttu-id="1cf46-174">Жобаның шығыс болжамдарын синхрондау орындалмас бұрын, жобаларды, жоба тапсырмаларын және жобаның шығыс транзакциясының санаттарын синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="1cf46-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="1cf46-175">Power Query</span></span>

<span data-ttu-id="1cf46-176">Жобаның шығыс болжамдары үлгісінде, келесі тапсырмаларды орындау үшін Excel бағдарламасына арналған Microsoft Power Query қондырмасын пайдалану қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="1cf46-177">Тек шығыс болжамының жол жазбаларын қамту үшін сүзгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="1cf46-178">Біріктіру жаңа сағаттық болжамдарды жасаған кезде пайдаланылатын әдепкі болжам үлгісінің идентификаторын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="1cf46-179">Есеп-шот түрлерін түрлендіріңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-179">Transform the billing types.</span></span>
- <span data-ttu-id="1cf46-180">Транзакция түрлерін түрлендіріңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="1cf46-181">Тек шығыс болжамының жолдарын қамту үшін сүзгілеу</span><span class="sxs-lookup"><span data-stu-id="1cf46-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="1cf46-182">Жобаның шығыс болжамдары (PSA бағдарламасынан Fin және Ops бағдарламасына) үлгісінде біріктірудегі шығыс жолдарды қамтитын әдепкі сүзгі бар.</span><span class="sxs-lookup"><span data-stu-id="1cf46-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="1cf46-183">Егер өз үлгіңізді жасасаңыз, онда осы сүзгіні қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="1cf46-184">**Транзакция қатынастары** тапсырмасын таңдаңыз, содан кейін салыстыруды ашу үшін **Карта** көрсеткісін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="1cf46-185">**Кеңейтілген сұрау және сүзгілеу** сілтемесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="1cf46-186">**msdyn\_transactiontype1** бағанын тек **msdyn\_estimateline** бағанын қамтитындай етіп сүзгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="1cf46-187">Әдепкі болжам үлгісінің идентификаторын орнату</span><span class="sxs-lookup"><span data-stu-id="1cf46-187">Set the default forecast model ID</span></span>

<span data-ttu-id="1cf46-188">Үлгідегі әдепкі болжам идентификаторын жаңарту үшін, **Шығыс болжамдары** тапсырмасын таңдаңыз, содан кейін салыстыруды ашу үшін **Карта** көрсеткісін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="1cf46-189">**Кеңейтілген сұрау және сүзгілеу** сілтемесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="1cf46-190">Егер әдепкі жобаның шығыс болжамдары (PSA бағдарламасынан Fin және Ops бағдарламасына) үлгісін пайдалансаңыз, Power Query қондырмасында, алдымен **Қолданылған қадамдар** бөлімінен **Енгізілген шарт** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="1cf46-191">**Функция** жазбасында, біріктірумен пайдаланылуы керек болжам үлгісінің идентификатор атауы бар **O\_болжам** бағанын ауыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="1cf46-192">Әдепкі үлгіде демо деректерінен алынған болжам үлгісінің идентификаторы бар.</span><span class="sxs-lookup"><span data-stu-id="1cf46-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="1cf46-193">Егер жаңа үлгі жасасаңыз, осы бағанды қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="1cf46-194">Power Query қондырмасында, **Шартты бағанды қосу** параметрін таңдап, **ModelID** сияқты жаңа бағанға арналған атау енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-194">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="1cf46-195">Бағанның шартын енгізіңіз, егер болжам жолының идентификаторы нөлге тең болмаса, онда \<enter the forecast model ID\>; басқасы нөл.</span><span class="sxs-lookup"><span data-stu-id="1cf46-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="1cf46-196">Есеп-шот түрлерін түрлендіру</span><span class="sxs-lookup"><span data-stu-id="1cf46-196">Transform the billing types</span></span>

<span data-ttu-id="1cf46-197">Жобаның шығыс болжамдары (PSA бағдарламасынан Fin және Ops бағдарламасына) үлгісі біріктіру кезінде Project Service Automation бағдарламасынан алынған есеп-шот түрлерін түрлендіру үшін пайдаланылатын шартты бағанды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="1cf46-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="1cf46-198">Егер жеке үлгіңізді жасасаңыз, шартты бағанды қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="1cf46-199">**Кеңейтілген сұрау және сүзгілеу** сілтемесін, содан кейін **Шартты бағанды қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="1cf46-200">Жаңа бағанға арналған **BillingType** сияқты атауды енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="1cf46-201">Содан кейін келесі шартты енгіңіз:</span><span class="sxs-lookup"><span data-stu-id="1cf46-201">Then enter the following condition:</span></span>

<span data-ttu-id="1cf46-202">Егер **msdyn\_billingtype** = 192350000 болса, онда **Ақысыз**</span><span class="sxs-lookup"><span data-stu-id="1cf46-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="1cf46-203">басқасы **msdyn\_billingtype** = 192350001 болса, онда **Ақылы**</span><span class="sxs-lookup"><span data-stu-id="1cf46-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="1cf46-204">басқасы **msdyn\_billingtype** = 192350002 болса, онда **Қосымша**</span><span class="sxs-lookup"><span data-stu-id="1cf46-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="1cf46-205">басқасы **Қолжетімді емес**</span><span class="sxs-lookup"><span data-stu-id="1cf46-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="1cf46-206">Транзакция түрлерін түрлендіру</span><span class="sxs-lookup"><span data-stu-id="1cf46-206">Transform the transaction types</span></span>

<span data-ttu-id="1cf46-207">Жобаның шығыс болжамдары (PSA бағдарламасынан Fin және Ops бағдарламасына) үлгісі біріктіру кезінде Project Service Automation бағдарламасынан алынған транзакция түрлерін түрлендіру үшін пайдаланылатын шартты бағанды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="1cf46-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="1cf46-208">Егер жеке үлгіңізді жасасаңыз, шартты бағанды қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="1cf46-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="1cf46-209">**Кеңейтілген сұрау және сүзгілеу** сілтемесін, содан кейін **Шартты бағанды қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="1cf46-210">Жаңа бағанға арналған **TransactionType** сияқты атауды енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="1cf46-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="1cf46-211">Содан кейін келесі шартты енгіңіз:</span><span class="sxs-lookup"><span data-stu-id="1cf46-211">Then enter the following condition:</span></span>

<span data-ttu-id="1cf46-212">Егер **msdyn\_transactiontypecode** = 192350000 болса, онда **Шығын**</span><span class="sxs-lookup"><span data-stu-id="1cf46-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="1cf46-213">басқасы **msdyn\_transactiontypecode** = 192350005 болса, онда **Сатылым**</span><span class="sxs-lookup"><span data-stu-id="1cf46-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="1cf46-214">басқасы **бос**</span><span class="sxs-lookup"><span data-stu-id="1cf46-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="1cf46-215">Деректерді біріктіруде үлгіні салыстыру</span><span class="sxs-lookup"><span data-stu-id="1cf46-215">Template mapping in Data integration</span></span>

<span data-ttu-id="1cf46-216">Келесі суреттер деректерді біріктіру қызметіндегі үлгі тапсырмасын салыстырулар мысалдарын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="1cf46-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="1cf46-217">Картада Project Service Automation бағдарламасынан Finance бағдарламасына синхрондалатын өріс туралы ақпарат көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="1cf46-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="1cf46-218">[![Шығысты болжау транзакцияларының үлгісін салыстыру](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="1cf46-218">[![Template mapping of expense estimate transactions](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="1cf46-219">[![Шығыс болжамдарының үлгісін салыстыру](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="1cf46-219">[![Template mapping of expense estimates](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]