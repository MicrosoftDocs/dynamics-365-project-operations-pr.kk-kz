---
title: Уақыт және материалдық жобаларға арналған жобаның сату тапсырыстары
description: Бұл тақырыпта уақыт және материалдық жобалар үшін жобаның сату тапсырыстарын құру жолы түсіндірілген.
author: Yowelle
manager: AnnBe
ms.date: 04/05/2019
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
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: 3653a6869dab323be88f1fd0f9fd0f2cb35c456f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079645"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="ba241-103">Уақыт және материалдық жобаларға арналған жобаның сату тапсырыстары</span><span class="sxs-lookup"><span data-stu-id="ba241-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="ba241-104">Бұл тақырыпта жоба үшін сату тапсырысын жасау жолы сипатталған.</span><span class="sxs-lookup"><span data-stu-id="ba241-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="ba241-105">Сату тапсырыстарын тек **уақыт және материал** түріндені жобалар үшін жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="ba241-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="ba241-106">Егер уақыт пен материалдық жоба келісім-шартында бірнеше қаржыландыру көзіне ие болса, **Жобаны басқару және есепке алу параметрлері** бетінде **Бірнеше қаржыландыру көздері бар жобалар үшін сату тапсырыстарына рұқсат беру** параметрін қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="ba241-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="ba241-107">Бірнеше қаржыландырудың көздері бар жобаның сату тапсырыстарын қолдау 10.0.2 және одан жоғары бағдарлама шығарылғаннан бастап қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="ba241-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="ba241-108">Бірнеше қаржыландыру көздері бар жобаның сату тапсырыстарын қолдауға мүмкіндік беретін параметр 2020 жылдың сәуірінде шығарылады, содан кейін функция әрдайым қосулы болады.</span><span class="sxs-lookup"><span data-stu-id="ba241-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="ba241-109">Жобаға негізделген сату тапсырыстарын екі жолмен жасауға болады:</span><span class="sxs-lookup"><span data-stu-id="ba241-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="ba241-110">Жобаның өзіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="ba241-110">Go to the project itself.</span></span> <span data-ttu-id="ba241-111">"Әрекеттер" тақтасында, **Басқару > Элемент тапсырмалары > Сату тапсырысы** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ba241-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="ba241-112">Жоба туралы ақпарат жобадағы сату тапсырысы бойынша әдепкі болады.</span><span class="sxs-lookup"><span data-stu-id="ba241-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="ba241-113">Егер жоба келісім-шарты бірнеше қаржыландыру көзіне ие болса, тұтынушыны сату тапсырысына белгілеу үшін қаржыландыру көзін таңдауыңыз қажет.</span><span class="sxs-lookup"><span data-stu-id="ba241-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="ba241-114">Егер жобаның бір ғана қаржыландыру көзі болса, тұтынушы автоматты түрде белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="ba241-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="ba241-115">**Барлық сату тапсырысы** тізімі бетіне өтіп, жаңа сату тапсырысын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="ba241-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="ba241-116">Сізге сату тапсырысы үшін жобаны таңдау қажет болады.</span><span class="sxs-lookup"><span data-stu-id="ba241-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="ba241-117">Жоба таңдалғаннан кейін, тұтынушы қаржыландыру көзінен белгіленеді немесе жоба келісім-шарты бірнеше қаржыландыру көзіне ие болса, қаржыландыру көзін таңдау қажет болады.</span><span class="sxs-lookup"><span data-stu-id="ba241-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>

