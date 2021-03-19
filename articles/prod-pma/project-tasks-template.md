---
title: Жоба тапсырмаларын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына синхрондаңыз
description: Бұл тақырыпта жоба тапсырмаларын тікелей Microsoft Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance бағдарламасына синхрондау үшін пайдаланылатын үлгі және негізгі тапсырма сипатталған.
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
ms.openlocfilehash: 7cc9ee9de576549c132e14c333a1000c22a55236
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288926"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="0b360-103">Жоба тапсырмаларын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына синхрондаңыз</span><span class="sxs-lookup"><span data-stu-id="0b360-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="0b360-104">Бұл тақырыпта жоба тапсырмаларын тікелей Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance бағдарламасына синхрондау үшін пайдаланылатын үлгі және негізгі тапсырма сипатталған.</span><span class="sxs-lookup"><span data-stu-id="0b360-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="0b360-105">Жоба тапсырмаларын біріктіру, шығындар транзакциясының санаттары, сағаттық болжамдар, шығын болжамдары және функционалды құлыптау 8.0 нұсқасында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="0b360-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="0b360-106">Егер Enterprise Edition 7.3.0 нұсқасын пайдалансаңыз, 4132657 білім қоры мен 4132660 білім қорын орнатқаннан кейін, үлгілерді жоба тапсырмаларын, шығыс транзакция санаттарын, сағаттық болжамдарды, шығын болжамдарын және нақты көрсеткіштерді біріктіру және функционалды құлыптауды конфигурациялау үшін пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="0b360-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="0b360-107">Бухгалтерлік шоттар бойынша таратуды қалпына келтіру керек болса, онда сізге 4131710 білім қорын орнатуды ұсынамыз.</span><span class="sxs-lookup"><span data-stu-id="0b360-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="0b360-108">Нақты көрсеткіштерді біріктіру 8.0.1 немесе одан кейінгі нұсқада қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="0b360-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="0b360-109">Project Service Automation және Finance бағдарламасындағы деректер ағыны</span><span class="sxs-lookup"><span data-stu-id="0b360-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="0b360-110">Project Service Automation және Finance бағдарламасын біріктіру шешімі деректерді біріктіру мүмкіндігін Project Service Automation және Finance мысалдары бойынша деректерді синхрондау үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="0b360-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="0b360-111">Деректерді біріктіру мүмкіндігімен бірге қолжетімді біріктіру үлгісі Project Service Automation бағдарламасынан Finance бағдарламасына жоба тапсырмалары туралы деректер ағынына мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="0b360-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="0b360-112">Келесі суретте деректердің Project Service Automation және Finance арасында синхрондалу жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="0b360-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="0b360-113">[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіруге арналған деректер ағыны](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="0b360-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="0b360-114">Үлгі және тапсырма</span><span class="sxs-lookup"><span data-stu-id="0b360-114">Template and task</span></span>

<span data-ttu-id="0b360-115">Үлгіге қатынасу мақсатында, жалпы үлгілерді таңдау үшін Microsoft Power Apps басқару орталығында **Жобалар**, содан кейін оң жақ жоғарғы бұрышта **Жаңа жоба** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b360-115">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="0b360-116">Жоба тапсырмаларын Project Service Automation бағдарламасынан Finance бағдарламасына синхрондау үшін келесі үлгі және негізгі тапсырма пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="0b360-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="0b360-117">**Деректерді біріктірудегі үлгі атауы:** Жоба тапсырмалары (Fin және Ops арналған PSA)</span><span class="sxs-lookup"><span data-stu-id="0b360-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="0b360-118">**Жобадағы тапсырманың атауы:** Жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="0b360-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="0b360-119">Жоба тапсырмаларын синхрондау орын алмас бұрын, жоба келісім-шарттары мен жобаларды синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="0b360-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="0b360-120">Нысан жиынтығы</span><span class="sxs-lookup"><span data-stu-id="0b360-120">Entity set</span></span>

| <span data-ttu-id="0b360-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="0b360-121">Project Service Automation</span></span> | <span data-ttu-id="0b360-122">Қаржы</span><span class="sxs-lookup"><span data-stu-id="0b360-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="0b360-123">Жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="0b360-123">Project Tasks</span></span>              | <span data-ttu-id="0b360-124">Жоба тапсырмасы үшін нысанды біріктіру</span><span class="sxs-lookup"><span data-stu-id="0b360-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="0b360-125">Нысан ағыны</span><span class="sxs-lookup"><span data-stu-id="0b360-125">Entity flow</span></span>

<span data-ttu-id="0b360-126">Жоба тапсырмалары Project Service Automation бағдарламасында басқарылады және олар жоба әрекеттері ретінде Finance бағдарламасына синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="0b360-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="0b360-127">Алғышарттар және салыстыру параметрі</span><span class="sxs-lookup"><span data-stu-id="0b360-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="0b360-128">Жоба тапсырмаларын синхрондау орын алмас бұрын, жоба келісім-шарттары мен жобаларды синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="0b360-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="0b360-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="0b360-129">Power Query</span></span>

<span data-ttu-id="0b360-130">Егер бұл шарт орындалса, деректерді сүзгілеу үшін Microsoft Power Query for Excel бағдарламасын пайдалану қажет:</span><span class="sxs-lookup"><span data-stu-id="0b360-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="0b360-131">Жоба тапсырмасында ресурстарға қатысты жазбалар бар.</span><span class="sxs-lookup"><span data-stu-id="0b360-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="0b360-132">Егер Power Query қолдану қажет болса, келесі нұсқаулықты орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="0b360-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="0b360-133">Жоба тапсырмаларының (Fin және Ops арналған PSA) үлгісінде **IsLineTask** сүзгісін **Жалған** мәніне орнату арқылы жоба тапсырмасынан ресурстарға қатысты жазбаларды шығаратын әдепкі сүзгі бар.</span><span class="sxs-lookup"><span data-stu-id="0b360-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="0b360-134">Егер өз үлгіңізді жасасаңыз, онда осы сүзгіні қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="0b360-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="0b360-135">Деректерді біріктіруде үлгіні салыстыру</span><span class="sxs-lookup"><span data-stu-id="0b360-135">Template mapping in Data integration</span></span>

<span data-ttu-id="0b360-136">Келесі суретте деректерді біріктіру кезіндегі үлгі тапсырмаларын салыстыру әрекеттерінің мысалы келтірілген.</span><span class="sxs-lookup"><span data-stu-id="0b360-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="0b360-137">Картада Project Service Automation бағдарламасынан Finance бағдарламасына синхрондалатын өріс туралы ақпарат көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="0b360-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="0b360-138">[![Үлгіні салыстыру](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="0b360-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]