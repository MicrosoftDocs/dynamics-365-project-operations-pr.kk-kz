---
title: Project Service Automation бағдарламасының 13 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 13-жаңарту шығарылымының 3 нұсқасындағы жаңалықтар туралы ақпарат беріледі.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: dbdcb811bfeacf17e841d679f097c591c16cd4c0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281035"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="d683f-103">Project Service Automation 13 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="d683f-103">Project Service Automation Update Release 13, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="d683f-104">Dynamics 365 Project Service Automation (PSA) бағдарламасының ең соңғы жаңартуын қуана хабарлаймыз.</span><span class="sxs-lookup"><span data-stu-id="d683f-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="d683f-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="d683f-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="d683f-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="d683f-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="d683f-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына кіріп, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="d683f-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="d683f-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="d683f-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="d683f-109">Бұл бөлімде Project Service Automation бағдарламасының 13-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="d683f-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="d683f-110">Бұл нұсқа V3.10.3.18 құрылым нөміріне ие және келесі кестеде қолжетімді:</span><span class="sxs-lookup"><span data-stu-id="d683f-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="d683f-111">**Жалпы қолжетімділік (өзін-өзі жаңарту):** қараша, 2019 ж</span><span class="sxs-lookup"><span data-stu-id="d683f-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="d683f-112">**Автоматты жаңарту:** желтоқсан, 2019 ж</span><span class="sxs-lookup"><span data-stu-id="d683f-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="d683f-113">13-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="d683f-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="d683f-114">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="d683f-114">Bug fixes</span></span>

- <span data-ttu-id="d683f-115">Уақыт және шығыс</span><span class="sxs-lookup"><span data-stu-id="d683f-115">Time and Expense</span></span>

     - <span data-ttu-id="d683f-116">Түзетілді: **Шығысты растау** бетіндегі іздеу функциясы шығыс мақсаты бойынша іздеу кезінде жұмыс істемейді.</span><span class="sxs-lookup"><span data-stu-id="d683f-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="d683f-117">Ресурсты басқару</span><span class="sxs-lookup"><span data-stu-id="d683f-117">Resource Management</span></span>

     - <span data-ttu-id="d683f-118">Түзетілді: салыстыру нөмірлері дұрыстық үшін жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="d683f-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="d683f-119">Түзетілді: аталған ресурстарды тапсырмаларға **Кесте** қойыншасы арқылы тағайындауға болмайды.</span><span class="sxs-lookup"><span data-stu-id="d683f-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="d683f-120">Жоба басқармасы</span><span class="sxs-lookup"><span data-stu-id="d683f-120">Project Management</span></span>

     - <span data-ttu-id="d683f-121">Түзетілді: топ мүшесін **TransactionType** өрісінде **Бөлім** және **DefaultGroup** үшін реттеу туралы ақпарат жоқ болғанда тағайындағанда ерекшелік сілтемесінің бос болуы.</span><span class="sxs-lookup"><span data-stu-id="d683f-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="d683f-122">Sales</span><span class="sxs-lookup"><span data-stu-id="d683f-122">Sales</span></span>

     - <span data-ttu-id="d683f-123">Түзетілді: қайталанатын транзакция түріндегі жазбалар рөл бағаларының жазбаларын жасау кезінде қатені қайтарады.</span><span class="sxs-lookup"><span data-stu-id="d683f-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="d683f-124">Бекітілген: **Жаңа мүмкіндік**, **Баға ұсыну**, **Тапсырыс жолы** және **Өнімді қосу** үшін қосымша түймелер Мүмкіндіктер, Баға ұсыныстары, Тапсырыс өнімдері және жобаға негізделген жолдар қосалқы торының командаларында көрінеді.</span><span class="sxs-lookup"><span data-stu-id="d683f-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines subgrid.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]