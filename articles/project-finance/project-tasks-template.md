---
title: Жоба тапсырмаларын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына синхрондаңыз
description: Бұл тақырыпта жоба тапсырмаларын тікелей Microsoft Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance бағдарламасына синхрондау үшін пайдаланылатын үлгі және негізгі тапсырма сипатталған.
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
ms.assetid: d7f32327-33c4-43ab-b799-786210e93277
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 66a255346727c7ee4fbbf2920d2ef437ded03308
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753130"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="f6f44-103">Жоба тапсырмаларын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына синхрондаңыз</span><span class="sxs-lookup"><span data-stu-id="f6f44-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="f6f44-104">Бұл тақырыпта жоба тапсырмаларын тікелей Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance бағдарламасына синхрондау үшін пайдаланылатын үлгі және негізгі тапсырма сипатталған.</span><span class="sxs-lookup"><span data-stu-id="f6f44-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="f6f44-105">Жоба тапсырмаларын біріктіру, шығындар транзакциясының санаттары, сағаттық болжамдар, шығын болжамдары және функционалды құлыптау 8.0 нұсқасында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="f6f44-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="f6f44-106">Егер Enterprise Edition 7.3.0 нұсқасын пайдалансаңыз, 4132657 білім қоры мен 4132660 білім қорын орнатқаннан кейін, үлгілерді жоба тапсырмаларын, шығыс транзакция санаттарын, сағаттық болжамдарды, шығын болжамдарын және нақты көрсеткіштерді біріктіру және функционалды құлыптауды конфигурациялау үшін пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="f6f44-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="f6f44-107">Бухгалтерлік шоттар бойынша таратуды қалпына келтіру керек болса, онда сізге 4131710 білім қорын орнатуды ұсынамыз.</span><span class="sxs-lookup"><span data-stu-id="f6f44-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="f6f44-108">Нақты көрсеткіштерді біріктіру 8.0.1 немесе одан кейінгі нұсқада қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="f6f44-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="f6f44-109">Project Service Automation және Finance бағдарламасындағы деректер ағыны</span><span class="sxs-lookup"><span data-stu-id="f6f44-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="f6f44-110">Project Service Automation және Finance бағдарламасын біріктіру шешімі деректерді біріктіру мүмкіндігін Project Service Automation және Finance мысалдары бойынша деректерді синхрондау үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="f6f44-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="f6f44-111">Деректерді біріктіру мүмкіндігімен бірге қолжетімді біріктіру үлгісі Project Service Automation бағдарламасынан Finance бағдарламасына жоба тапсырмалары туралы деректер ағынына мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="f6f44-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f6f44-112">Келесі суретте деректердің Project Service Automation және Finance арасында синхрондалу жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="f6f44-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="f6f44-113">[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіруге арналған деректер ағыны](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="f6f44-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="f6f44-114">Үлгі және тапсырма</span><span class="sxs-lookup"><span data-stu-id="f6f44-114">Template and task</span></span>

<span data-ttu-id="f6f44-115">Үлгіге қатынасу мақсатында, жалпы үлгілерді таңдау үшін Microsoft Power Apps басқару орталығында **Жобалар**, содан кейін оң жақ жоғарғы бұрышта **Жаңа жоба** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f6f44-115">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="f6f44-116">Жоба тапсырмаларын Project Service Automation бағдарламасынан Finance бағдарламасына синхрондау үшін келесі үлгі және негізгі тапсырма пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="f6f44-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="f6f44-117">**Деректерді біріктірудегі үлгі атауы:** Жоба тапсырмалары (Fin және Ops арналған PSA)</span><span class="sxs-lookup"><span data-stu-id="f6f44-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="f6f44-118">**Жобадағы тапсырманың атауы:** Жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="f6f44-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="f6f44-119">Жоба тапсырмаларын синхрондау орын алмас бұрын, жоба келісім-шарттары мен жобаларды синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="f6f44-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="f6f44-120">Нысан жиынтығы</span><span class="sxs-lookup"><span data-stu-id="f6f44-120">Entity set</span></span>

| <span data-ttu-id="f6f44-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f6f44-121">Project Service Automation</span></span> | <span data-ttu-id="f6f44-122">Қаржы</span><span class="sxs-lookup"><span data-stu-id="f6f44-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="f6f44-123">Жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="f6f44-123">Project Tasks</span></span>              | <span data-ttu-id="f6f44-124">Жоба тапсырмасы үшін нысанды біріктіру</span><span class="sxs-lookup"><span data-stu-id="f6f44-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="f6f44-125">Нысан ағыны</span><span class="sxs-lookup"><span data-stu-id="f6f44-125">Entity flow</span></span>

<span data-ttu-id="f6f44-126">Жоба тапсырмалары Project Service Automation бағдарламасында басқарылады және олар жоба әрекеттері ретінде Finance бағдарламасына синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="f6f44-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="f6f44-127">Алғышарттар және салыстыру параметрі</span><span class="sxs-lookup"><span data-stu-id="f6f44-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="f6f44-128">Жоба тапсырмаларын синхрондау орын алмас бұрын, жоба келісім-шарттары мен жобаларды синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="f6f44-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="f6f44-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="f6f44-129">Power Query</span></span>

<span data-ttu-id="f6f44-130">Егер бұл шарт орындалса, деректерді сүзгілеу үшін Microsoft Power Query for Excel бағдарламасын пайдалану қажет:</span><span class="sxs-lookup"><span data-stu-id="f6f44-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="f6f44-131">Жоба тапсырмасында ресурстарға қатысты жазбалар бар.</span><span class="sxs-lookup"><span data-stu-id="f6f44-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="f6f44-132">Егер Power Query қолдану қажет болса, келесі нұсқаулықты орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="f6f44-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="f6f44-133">Жоба тапсырмаларының (Fin және Ops арналған PSA) үлгісінде **IsLineTask** сүзгісін **Жалған** мәніне орнату арқылы жоба тапсырмасынан ресурстарға қатысты жазбаларды шығаратын әдепкі сүзгі бар.</span><span class="sxs-lookup"><span data-stu-id="f6f44-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="f6f44-134">Егер өз үлгіңізді жасасаңыз, онда осы сүзгіні қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="f6f44-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="f6f44-135">Деректерді біріктіруде үлгіні салыстыру</span><span class="sxs-lookup"><span data-stu-id="f6f44-135">Template mapping in Data integration</span></span>

<span data-ttu-id="f6f44-136">Келесі суретте деректерді біріктіру кезіндегі үлгі тапсырмаларын салыстыру әрекеттерінің мысалы келтірілген.</span><span class="sxs-lookup"><span data-stu-id="f6f44-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="f6f44-137">Картада Project Service Automation бағдарламасынан Finance бағдарламасына синхрондалатын өріс туралы ақпарат көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="f6f44-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f6f44-138">[![Үлгіні салыстыру](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="f6f44-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>
