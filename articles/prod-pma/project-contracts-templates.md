---
title: Жоба келісім-шарттары мен жобаларын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына тікелей синхрондау
description: Бұл тақырыпта үлгі мен жобаның келісім-шарттары мен жобаларын Microsoft Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance жүйесіне синхрондау үшін пайдаланылатын негізгі тапсырмалар сипатталады.
author: Yowelle
manager: AnnBe
ms.date: 09/09/2019
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
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 9e4f11ec0bb88ed0971a3d082e7ca7823fcf8453
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079794"
---
# <a name="synchronize-project-contracts-and-projects-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="91084-103">Жоба келісім-шарттары мен жобаларын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына тікелей синхрондау</span><span class="sxs-lookup"><span data-stu-id="91084-103">Synchronize project contracts and projects directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="91084-104">Бұл тақырыпта үлгі мен жобаның келісім-шарттары мен жобаларын Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance жүйесіне синхрондау үшін пайдаланылатын негізгі тапсырмалар сипатталады.</span><span class="sxs-lookup"><span data-stu-id="91084-104">This topic describes the template and underlying tasks that are used to synchronize project contracts and projects directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE] 
> <span data-ttu-id="91084-105">Enterprise Edition 7.3.0 бағдарламасын пайдаланатын болсаңыз 4074835 білім қорын орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="91084-105">If you're using Enterprise edition 7.3.0, you must install KB 4074835.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="91084-106">Project Service Automation және Finance бағдарламасындағы деректер ағыны</span><span class="sxs-lookup"><span data-stu-id="91084-106">Data flow for Project Service Automation to Finance</span></span>

> [!NOTE]
> <span data-ttu-id="91084-107">Project Service Automation бағдарламасын Finance біріктіру шешіміне пайдаланудан бұрын, Dynamics 365 деректерді біріктіру мүмкіндігімен таныс болуыңыз қажет.</span><span class="sxs-lookup"><span data-stu-id="91084-107">Before you can use the Project Service Automation to Finance integration solution, you should be familiar with the Dynamics 365 Data integration feature.</span></span>

<span data-ttu-id="91084-108">Project Service Automation және Finance бағдарламасын біріктіру шешімі деректерді біріктіру мүмкіндігін Project Service Automation және Finance мысалдары бойынша деректерді синхрондау үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="91084-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="91084-109">Деректерді біріктіру мүмкіндігімен қолжетімді біріктіру үлгісі жобаның келісім-шарттары, жобалар, жобаның келісім-шарт жолдары және жобаның келісім-шарт жолының кезеңдері туралы деректер ағынын Project Service Automation бағдарламасынан Finance бағдарламасына қосады.</span><span class="sxs-lookup"><span data-stu-id="91084-109">The integration template that is available with the Data integration feature enables the flow of data about project contracts, projects, project contract lines, and project contract line milestones from Project Service Automation to Finance.</span></span>

<span data-ttu-id="91084-110">Келесі суретте деректердің Project Service Automation және Finance арасында синхрондалу жолы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="91084-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="91084-111">[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіруге арналған деректер ағыны](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)</span><span class="sxs-lookup"><span data-stu-id="91084-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)</span></span>

## <a name="templates-and-tasks"></a><span data-ttu-id="91084-112">Үлгілер және тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="91084-112">Templates and tasks</span></span>

<span data-ttu-id="91084-113">Қолжетімді үлгілерге қатынасу үшін Microsoft Power Apps басқару орталығында **Жобалар** опциясын таңдап, содан соң жоғарғы оң жақтағы бұрышта жалпы үлгілерді таңдау үшін **Жаңа жоба** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="91084-113">To access the available templates, in the Microsoft Power Apps admin center, select **Projects** , and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="91084-114">Келесі үлгілер және негізгі тапсырмалар жобаның келісім-шарттарын және жобаларын Project Service Automation бағдарламасынан Finance бағдарламасына синхрондау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="91084-114">The following templates and underlying tasks are used to synchronize project contracts and projects from Project Service Automation to Finance:</span></span>

### <a name="integrating-with-dynamics-365-project-service-automation-v2x"></a><span data-ttu-id="91084-115">Dynamics 365 Project Service Automation v2.x қызметімен біріктіру</span><span class="sxs-lookup"><span data-stu-id="91084-115">Integrating with Dynamics 365 Project Service Automation v2.x</span></span>
- <span data-ttu-id="91084-116">**Деректерді біріктіру функциясындағы үлгі атауы:** Жобалар және келісім-шарттар (PSA бағдарламасынан Fin және Ops бағдарламасына)</span><span class="sxs-lookup"><span data-stu-id="91084-116">**Name of the template in Data integration:** Projects and contracts (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="91084-117">**Жобадағы тапсырмалардың атауы**</span><span class="sxs-lookup"><span data-stu-id="91084-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="91084-118">Жобалық келісім-шарттар PSA бағдарламасынан Fin және Ops бағдарламасына</span><span class="sxs-lookup"><span data-stu-id="91084-118">Project contracts PSA to Fin and Ops</span></span>
    - <span data-ttu-id="91084-119">Жобалар PSA бағдарламасынан Fin және Ops бағдарламасына</span><span class="sxs-lookup"><span data-stu-id="91084-119">Projects PSA to Fin and Ops</span></span>
    - <span data-ttu-id="91084-120">Жобалық келісім-шарттар жолдары PSA бағдарламасынан Fin және Ops бағдарламасына</span><span class="sxs-lookup"><span data-stu-id="91084-120">Project contract lines PSA to Fin and Ops</span></span>
    - <span data-ttu-id="91084-121">Жобалық келісім-шарт жолының кезеңдері PSA бағдарламасынан Fin және Ops бағдарламасына</span><span class="sxs-lookup"><span data-stu-id="91084-121">Project contract line milestones PSA to Fin and Ops</span></span>
  
### <a name="integrating-with-dynamics-365-project-service-automation-v3x"></a><span data-ttu-id="91084-122">Dynamics 365 Project Service Automation v3.x қызметімен біріктіру</span><span class="sxs-lookup"><span data-stu-id="91084-122">Integrating with Dynamics 365 Project Service Automation v3.x</span></span>
<span data-ttu-id="91084-123">Жобаның келісім-шарттық жолы кезеңінің үлгісіне әсер ететін Project Service Automation бағдарламасындағы схема өзгерісі бар, сондай-ақ v2 нұсқасын пайдалану Dynamics 365 бағдарламасымен Project Service Automation v3.x біріктіру үшін қажет.</span><span class="sxs-lookup"><span data-stu-id="91084-123">There is a schema change in Project Service Automation that impacts the Project contract line milestone template and use of the v2 version of the template is required to integrate Project Service Automation v3.x with Dynamics 365.</span></span>

- <span data-ttu-id="91084-124">**Деректерді біріктіру функциясындағы үлгі атауы:** Жобалар және келісім-шарттар (PSA 3.x бағдарламасынан Fin және Ops бағдарламасына) - v2</span><span class="sxs-lookup"><span data-stu-id="91084-124">**Name of the template in Data integration:** Projects and Contracts (PSA 3.x to Fin and Ops) - v2</span></span>
- <span data-ttu-id="91084-125">**Жобадағы тапсырмалардың атауы**</span><span class="sxs-lookup"><span data-stu-id="91084-125">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="91084-126">Жобалық келісім-шарттар PSA бағдарламасынан Fin және Ops бағдарламасына</span><span class="sxs-lookup"><span data-stu-id="91084-126">Project contracts PSA to Fin and Ops</span></span>
    - <span data-ttu-id="91084-127">Жобалар PSA бағдарламасынан Fin және Ops бағдарламасына</span><span class="sxs-lookup"><span data-stu-id="91084-127">Projects PSA to Fin and Ops</span></span>
    - <span data-ttu-id="91084-128">Жобалық келісім-шарттар жолдары PSA бағдарламасынан Fin және Ops бағдарламасына</span><span class="sxs-lookup"><span data-stu-id="91084-128">Project contract lines PSA to Fin and Ops</span></span>
    - <span data-ttu-id="91084-129">Жобалық келісім-шарт жолының кезеңдері PSA бағдарламасынан Fin және Ops бағдарламасына</span><span class="sxs-lookup"><span data-stu-id="91084-129">Project contract line milestones PSA to Fin and Ops</span></span>

<span data-ttu-id="91084-130">Жобаның келісім-шарттары мен жобаларын синхрондау орындалмас бұрын, тіркелгілерді синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="91084-130">Before synchronization of project contracts and projects can occur, you must synchronize accounts.</span></span>

## <a name="entity-set"></a><span data-ttu-id="91084-131">Нысан жиынтығы</span><span class="sxs-lookup"><span data-stu-id="91084-131">Entity set</span></span>

| <span data-ttu-id="91084-132">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="91084-132">Project Service Automation</span></span>       | <span data-ttu-id="91084-133">Қаржы</span><span class="sxs-lookup"><span data-stu-id="91084-133">Finance</span></span>                                                |
|----------------------------------|--------------------------------------------------------|
| <span data-ttu-id="91084-134">Тапсырыстар</span><span class="sxs-lookup"><span data-stu-id="91084-134">Orders</span></span>                           | <span data-ttu-id="91084-135">Жобаның келісім-шартына арналған біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="91084-135">Integration entity for project contract</span></span>                |
| <span data-ttu-id="91084-136">Жобалар</span><span class="sxs-lookup"><span data-stu-id="91084-136">Projects</span></span>                         | <span data-ttu-id="91084-137">Жобаға арналған біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="91084-137">Integration entity for project</span></span>                         |
| <span data-ttu-id="91084-138">Тапсырыс жолдары</span><span class="sxs-lookup"><span data-stu-id="91084-138">Order lines</span></span>                      | <span data-ttu-id="91084-139">Жобаның келісім-шарт жолына арналған біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="91084-139">Integration entity for project contract line</span></span>           |
| <span data-ttu-id="91084-140">Жобаның келісім-шарт жолының кезеңдері</span><span class="sxs-lookup"><span data-stu-id="91084-140">Project contract line milestones</span></span> | <span data-ttu-id="91084-141">Жобаның келісім-шарт жолының кезеңіне арналған біріктіру нысаны</span><span class="sxs-lookup"><span data-stu-id="91084-141">Integration entity for project contract line milestone</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="91084-142">Нысан ағыны</span><span class="sxs-lookup"><span data-stu-id="91084-142">Entity flow</span></span>

<span data-ttu-id="91084-143">Жобаның келісім-шарттары Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жобаның келісім-шарттары ретінде синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="91084-143">Project contracts are managed in Project Service Automation, and they are synchronized to Finance as project contracts.</span></span> <span data-ttu-id="91084-144">Біріктіру үлгісінің бөлігі ретінде жобаның келісім-шартына арналған Finance жүйесіндегі бастапқы біріктіруді орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="91084-144">As part of the integration template, you can set the integration source in Finance for the project contract.</span></span>

<span data-ttu-id="91084-145">Уақыт және материалдық жоба мен бекітіліген баға жобалары Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жобалар ретінде синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="91084-145">Time and material project and Fixed price projects are managed in Project Service Automation, and they are synchronized to Finance as projects.</span></span> <span data-ttu-id="91084-146">Үлгі интеграциясын біріктіру бөлігі ретінде жоба үшін Finance бағдарламасында бастапқы біріктіруді орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="91084-146">As part of the template integration, you can set the integration source in Finance for the project.</span></span>

<span data-ttu-id="91084-147">Жобаның келісім-шарт жолдары Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жоба келісім-шартының шот ұсыну ережелері ретінде синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="91084-147">Project contract lines are managed in Project Service Automation, and they are synchronized to Finance as project contract billing rules.</span></span> <span data-ttu-id="91084-148">Егер шот ұсыну әдісі әдепкі жобасы түрінен өзгеше болса, синхрондау келісім-шарт жолының жобасы мен жоба тобына арналған жоба түрін жаңартады.</span><span class="sxs-lookup"><span data-stu-id="91084-148">If the billing method differs from the default project type, the synchronization updates the project type for the contract line project and project group.</span></span>

<span data-ttu-id="91084-149">Жобаның келісім-шарт жолының кезеңдері Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жоба келісім-шартының шот ұсыну ережесінің кезеңдері ретінде синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="91084-149">Project contract line milestones are managed in Project Service Automation, and they are synchronized to Finance as project contract billing rule milestones.</span></span>

## <a name="project-service-automation-to-finance-integration-solution"></a><span data-ttu-id="91084-150">Project Service Automation бағдарламасынан Finance бағдарламасына біріктіру шешімі</span><span class="sxs-lookup"><span data-stu-id="91084-150">Project Service Automation to Finance integration solution</span></span>

<span data-ttu-id="91084-151">**Жоба келісім-шартының идентификаторы** өрісі **Жоба келісім-шарттары** бетінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="91084-151">The **Project contract ID** field is available on the **Project contracts** page.</span></span> <span data-ttu-id="91084-152">Бұл өріс біріктіруге қолдау көрсету үшін қалыпты және бірегей кілт ретінде жасалған.</span><span class="sxs-lookup"><span data-stu-id="91084-152">This field has been made a natural and unique key to support the integration.</span></span>

<span data-ttu-id="91084-153">Жаңа жобалық келісім-шарт жасалған кезде, егер **Жоба келісім-шартының идентификаторы** мәні әлі де болмаса, ол нөмір реттілігін пайдалану арқылы автоматты түрде құрылады.</span><span class="sxs-lookup"><span data-stu-id="91084-153">When a new project contract is created, if a **Project contract ID** value doesn't already exist, it's automatically generated by using a number sequence.</span></span> <span data-ttu-id="91084-154">Мән өсу нөмірі реттілігінің алдында келетін **ORD** мәнінен, содан соң алты таңбалық жұрнақтан тұрады.</span><span class="sxs-lookup"><span data-stu-id="91084-154">The value consists of **ORD** followed by an incrementing number sequence and then a suffix of six characters.</span></span> <span data-ttu-id="91084-155">Мұнда мысал берілген: **ORD-01022-Z4M9Q0**.</span><span class="sxs-lookup"><span data-stu-id="91084-155">Here is an example: **ORD-01022-Z4M9Q0**.</span></span>

<span data-ttu-id="91084-156">**Жоба нөмірі** өрісі **Жобалар** бетінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="91084-156">The **Project Number** field is available on the **Projects** page.</span></span> <span data-ttu-id="91084-157">Бұл өріс біріктіруге қолдау көрсету үшін қалыпты және бірегей кілт ретінде жасалған.</span><span class="sxs-lookup"><span data-stu-id="91084-157">This field has been made a natural and unique key to support the integration.</span></span>

<span data-ttu-id="91084-158">Жаңа жобалық келісім-шарт жасалған кезде, егер **Жоба нөмірі** мәні әлі де болмаса, ол нөмір реттілігін пайдалану арқылы автоматты түрде құрылады.</span><span class="sxs-lookup"><span data-stu-id="91084-158">When a new project is created, if a **Project Number** value doesn't already exist, it's automatically generated by using a number sequence.</span></span> <span data-ttu-id="91084-159">Мән өсу нөмірі реттілігінің алдында келетін **PRJ** мәнінен, содан соң алты таңбалық жұрнақтан тұрады.</span><span class="sxs-lookup"><span data-stu-id="91084-159">The value consists of **PRJ** followed by an incrementing number sequence and then a suffix of six characters.</span></span> <span data-ttu-id="91084-160">Мұнда мысал берілген: **PRJ-01049-CCNID0**.</span><span class="sxs-lookup"><span data-stu-id="91084-160">Here is an example: **PRJ-01049-CCNID0**.</span></span>

<span data-ttu-id="91084-161">Project Service Automation бағдарламасынан Finance бағдарламасына біріктіру шешімі қолданылған кезде жаңарту сценарийін **Жобаның келісім-шарт идентификаторы** өрісін қолданыстағы жобалық келісім-шарттарына, ал **Жоба нөмірі** өрісін Project Service Automation бағдарламасындағы қолданыстағы жобаларға орнатады.</span><span class="sxs-lookup"><span data-stu-id="91084-161">When the Project Service Automation to Finance integration solution is applied, an upgrade script sets the **Project contract ID** field for existing project contracts and the **Project Number** field for existing projects in Project Service Automation.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="91084-162">Алғышарттар және салыстыру параметрі</span><span class="sxs-lookup"><span data-stu-id="91084-162">Prerequisites and mapping setup</span></span>

- <span data-ttu-id="91084-163">Жобаның келісім-шарттары мен жобаларын синхрондау орындалмас бұрын, тіркелгілерді синхрондау қажет.</span><span class="sxs-lookup"><span data-stu-id="91084-163">Before synchronization of project contracts and projects can occur, you must synchronize accounts.</span></span>
- <span data-ttu-id="91084-164">Байланыс жинағында **msdyn\_organizationalunits** - **msdyn\_name \[Name\]** үшін біріктіру кілтінің өрісін салыстыруды қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="91084-164">In your connection set, add an integration key field mapping for **msdyn\_organizationalunits** to **msdyn\_name \[Name\]**.</span></span> <span data-ttu-id="91084-165">Алдымен байланыс жинағына жобаны қосу қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="91084-165">You might first need to add a project to the connection set.</span></span> <span data-ttu-id="91084-166">Қосымша ақпаратты [Деректерді бағдарламаларға арналған Common Data Service қызметіне біріктіру](https://docs.microsoft.com/powerapps/administrator/data-integrator) тақырыбынан қараңыз.</span><span class="sxs-lookup"><span data-stu-id="91084-166">For more information, see [Integrate data into Common Data Service for Apps](https://docs.microsoft.com/powerapps/administrator/data-integrator).</span></span>
- <span data-ttu-id="91084-167">Байланыс жинағында **msdyn\_projects** - **msdynce\_projectnumber \[Project Number\]** үшін біріктіру кілтінің өрісін салыстыруды қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="91084-167">In your connection set, add an integration key field mapping for **msdyn\_projects** to **msdynce\_projectnumber \[Project Number\]**.</span></span> <span data-ttu-id="91084-168">Алдымен байланыс жинағына жобаны қосу қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="91084-168">You might first need to add a project to the connection set.</span></span> <span data-ttu-id="91084-169">Қосымша ақпаратты [Деректерді бағдарламаларға арналған Common Data Service қызметіне біріктіру](https://docs.microsoft.com/powerapps/administrator/data-integrator) тақырыбынан қараңыз.</span><span class="sxs-lookup"><span data-stu-id="91084-169">For more information, see [Integrate data into Common Data Service for Apps](https://docs.microsoft.com/powerapps/administrator/data-integrator).</span></span>
- <span data-ttu-id="91084-170">Жобалық келісім-шарттарға арналған **SourceDataID** және жобалар басқа мәнге жаңартылуы мүмкін немесе салыстырудан алынып тасталынуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="91084-170">**SourceDataID** for project contracts and projects can be updated to a different value or removed from the mapping.</span></span> <span data-ttu-id="91084-171">Әдепкі үлгі мәні – **Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="91084-171">The default template value is **Project Service Automation**.</span></span>
- <span data-ttu-id="91084-172">**PaymentTerms** салыстырылуы ол Finance жүйесіндегі жарамды төлем шарттарын көрсететіндей жаңартылуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="91084-172">The **PaymentTerms** mapping must be updated so that it reflects valid terms of payment in Finance.</span></span> <span data-ttu-id="91084-173">Жоба тапсырмасынан салыстыруды алып тастауға болады.</span><span class="sxs-lookup"><span data-stu-id="91084-173">You can also remove the mapping from the project task.</span></span> <span data-ttu-id="91084-174">Әдепкі мәнді салыстырудың демо-деректер үшін әдепкі мәндері бар.</span><span class="sxs-lookup"><span data-stu-id="91084-174">The default value map has default values for demo data.</span></span> <span data-ttu-id="91084-175">Келесі кестеде Project Service Automation бағдарламасындағы мәндер көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="91084-175">The following table shows the values in Project Service Automation.</span></span>

    | <span data-ttu-id="91084-176">Мәні</span><span class="sxs-lookup"><span data-stu-id="91084-176">Value</span></span> | <span data-ttu-id="91084-177">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="91084-177">Description</span></span>   |
    |-------|---------------|
    | <span data-ttu-id="91084-178">1</span><span class="sxs-lookup"><span data-stu-id="91084-178">1</span></span>     | <span data-ttu-id="91084-179">Есеп-шотты алған соң 30 күннен кейін төлеу</span><span class="sxs-lookup"><span data-stu-id="91084-179">Net 30</span></span>        |
    | <span data-ttu-id="91084-180">2</span><span class="sxs-lookup"><span data-stu-id="91084-180">2</span></span>     | <span data-ttu-id="91084-181">2% 10, Нетто 30</span><span class="sxs-lookup"><span data-stu-id="91084-181">2% 10, Net 30</span></span> |
    | <span data-ttu-id="91084-182">3</span><span class="sxs-lookup"><span data-stu-id="91084-182">3</span></span>     | <span data-ttu-id="91084-183">Есеп-шотты алған соң 45 күннен кейін төлеу</span><span class="sxs-lookup"><span data-stu-id="91084-183">Net 45</span></span>        |
    | <span data-ttu-id="91084-184">4</span><span class="sxs-lookup"><span data-stu-id="91084-184">4</span></span>     | <span data-ttu-id="91084-185">Есеп-шотты алған соң 60 күннен кейін төлеу</span><span class="sxs-lookup"><span data-stu-id="91084-185">Net 60</span></span>        |

## <a name="power-query"></a><span data-ttu-id="91084-186">Power Query</span><span class="sxs-lookup"><span data-stu-id="91084-186">Power Query</span></span>

<span data-ttu-id="91084-187">Келесі шарттар орындалса, деректерді сүзгілеу үшін Excel бағдарламасына арналған Microsoft Power Query бағдарламасын пайдалану қажет:</span><span class="sxs-lookup"><span data-stu-id="91084-187">You must use Microsoft Power Query for Excel to filter data if the following conditions are met:</span></span>

- <span data-ttu-id="91084-188">Dynamics 365 Sales бағдарламасында сатылым тапсырыстарыңыз бар.</span><span class="sxs-lookup"><span data-stu-id="91084-188">You have sales orders in Dynamics 365 Sales.</span></span>
- <span data-ttu-id="91084-189">Project Service Automation бағдарламасында бірнеше ұйым бөлімшелері бар, сондай-ақ ұйым бөлімшелері Finance жүйесіндегі бірнеше заңды тұлғаларға салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="91084-189">You have multiple organizational units in Project Service Automation, and these organizational units will be mapped to multiple legal entities in Finance.</span></span>

<span data-ttu-id="91084-190">Power Query бағдарламасын пайдалану қажет болса, мына нұсқауларды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="91084-190">If you must use Power Query, follow these guidelines:</span></span>

- <span data-ttu-id="91084-191">Жобалар және келісім-шарттар (PSA бағдарламасынан Fin және Ops бағдарламаларына) үлгісінің **Жұмыс элементі (msdyn\_ordertype = 192350001)** түрінің тек сатылым тапсырыстарын қамтитын әдепкі сүзгілері бар.</span><span class="sxs-lookup"><span data-stu-id="91084-191">The Projects and contracts (PSA to Fin and Ops) template has a default filter that includes only sales orders of the **Work item (msdyn\_ordertype = 192350001)** type.</span></span> <span data-ttu-id="91084-192">Бұл сүзгі жоба келісім-шарттарының Finance жүйесіндегі сатылым тапсырыстары үшін жасалмайтынына кепілдік береді.</span><span class="sxs-lookup"><span data-stu-id="91084-192">This filter helps guarantee that project contracts aren't created for sales orders in Finance.</span></span> <span data-ttu-id="91084-193">Егер өз үлгіңізді жасасаңыз, онда осы сүзгіні қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="91084-193">If you create your own template, you must add this filter.</span></span>
- <span data-ttu-id="91084-194">Біріктіру байланыс жинағының заңды нысанына синхрондалуы қажет келісім-шарт ұйымдарын қамтитын Power Query сүзісін жасауыңыз қажет.</span><span class="sxs-lookup"><span data-stu-id="91084-194">You must create a Power Query filter that includes only the contract organizations that should be synchronized to the legal entity of the integration connection set.</span></span> <span data-ttu-id="91084-195">Мысалы, Contoso US келісім-шартының ұйым бөлімшесімен болатын жобалық келісім-шарттар USSI заңды нысаны үшін синхрондалуы қажет, бірақ Contoso US келісім-шартының ұйым бөлімшесімен болатын жобалық келісім-шарттар USMF заңды нысаны үшін синхрондалуы қажет.</span><span class="sxs-lookup"><span data-stu-id="91084-195">For example, project contracts that you have with the contract organizational unit of Contoso US should be synchronized to the USSI legal entity, but project contracts that you have with the contract organizational unit of Contoso Global should be synchronized to the USMF legal entity.</span></span> <span data-ttu-id="91084-196">Егер сіз бұл сүзгіні тапсырманы салыстыруға қоспасаңыз, барлық жобалық келісім-шарттар келісім-шарттың ұйым бөлімшесіне тәуелсіз түрде байланыс жинағы үшін анықталған заңды нысанға синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="91084-196">If you don't add this filter to your task mapping, all project contracts will be synchronized to the legal entity that is defined for the connection set, regardless of the contract organizational unit.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="91084-197">Деректерді біріктіруде үлгіні салыстыру</span><span class="sxs-lookup"><span data-stu-id="91084-197">Template mapping in Data integration</span></span>

> [!NOTE] 
> <span data-ttu-id="91084-198">**CustomerReference** , **AddressCity** , **AddressCountryRegionID** , **AddressDescription** , **AddressLine1** , **AddressLine2** , **AddressState** және **AddressZipCode** өрістері жобалық келісім-шарттарға арналған әдепкі салыстыруда қамтылмаған.</span><span class="sxs-lookup"><span data-stu-id="91084-198">The **CustomerReference** , **AddressCity** , **AddressCountryRegionID** , **AddressDescription** , **AddressLine1** , **AddressLine2** , **AddressState** , and **AddressZipCode** fields aren't included in the default mapping for project contracts.</span></span> <span data-ttu-id="91084-199">Осы деректердің жобалық келісім-шарттар үшін синхрондалуы қажет болса, салыстыруларды қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="91084-199">You can add the mappings if you require that this data be synchronized for project contracts.</span></span>
>
> <span data-ttu-id="91084-200">**Description** , **ParentID** , **ProjectGroup** , **ProjectManagerPersonnelNumber** және **ProjectType** өрістері жобаларға арналған әдепкі салыстыруда қамтылмайды.</span><span class="sxs-lookup"><span data-stu-id="91084-200">The **Description** , **ParentID** , **ProjectGroup** , **ProjectManagerPersonnelNumber** , and **ProjectType** fields aren't included in the default mapping for projects.</span></span> <span data-ttu-id="91084-201">Осы деректердің жобалар үшін синхрондалуы қажет болса, салыстыруларды қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="91084-201">You can add the mappings if you require that this data be synchronized for projects.</span></span>

<span data-ttu-id="91084-202">Келесі суреттер деректерді біріктіру қызметіндегі үлгі тапсырмасын салыстырулар мысалдарын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="91084-202">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="91084-203">Картада Project Service Automation бағдарламасынан Finance бағдарламасына синхрондалатын өріс туралы ақпарат көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="91084-203">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="91084-204">[![Жоба келісім-шартының үлгісін салыстыру](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)</span><span class="sxs-lookup"><span data-stu-id="91084-204">[![Project contract template mapping](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)</span></span>

<span data-ttu-id="91084-205">[![Жоба үлгісін салыстыру](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)</span><span class="sxs-lookup"><span data-stu-id="91084-205">[![Project template mapping](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)</span></span>

<span data-ttu-id="91084-206">[![Жоба келісім-шарт жолдары үлгісін салыстыру](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)</span><span class="sxs-lookup"><span data-stu-id="91084-206">[![Project contract lines template mapping](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)</span></span>

<span data-ttu-id="91084-207">[![Жоба келісім-шарт жолы кезеңінің үлгісін салыстыру](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)</span><span class="sxs-lookup"><span data-stu-id="91084-207">[![Project contract line milestone template mapping](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)</span></span>

#### <a name="project-contract-line-milestone-mapping-in-the-projects-and-contracts-psa-3x-to-dynamics---v2-template"></a><span data-ttu-id="91084-208">Жобалар және келісім-шарттар (Dynamics PSA 3.x) - v2 үлгісіндегі жобалық келісім-шарты жолы кезеңін салыстыруы:</span><span class="sxs-lookup"><span data-stu-id="91084-208">Project contract line milestone mapping in the Projects and Contracts (PSA 3.x to Dynamics) - v2 template:</span></span>

<span data-ttu-id="91084-209">[![Екінші нұсқа үлгісі бар жоба келісім-шарт жолы кезеңін салыстыру](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)</span><span class="sxs-lookup"><span data-stu-id="91084-209">[![Project contract line milestone mapping with version two template](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)</span></span>