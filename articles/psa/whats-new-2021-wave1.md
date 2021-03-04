---
title: Project Service Automation бағдарламасының 2021 жылғы ерте қатынасу шығарылымның 1-толқыны, V3 нұсқасындағы жаңалықтар мен өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 2021 жылғы ерте қатынасу шығарылымның 1-толқыны, V3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/29/2021
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
ms.openlocfilehash: 3895f06c6a401f200cf832940ef85eaa8d66fbb2
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5151170"
---
# <a name="whats-new-or-changed-in-project-service-automation-early-access-wave-1-2021-v3"></a><span data-ttu-id="08eda-103">Project Service Automation бағдарламасының 2021 жылғы ерте қатынасу шығарылымның 1-толқыны, V3 нұсқасындағы жаңалықтар мен өзгерістер</span><span class="sxs-lookup"><span data-stu-id="08eda-103">What's new or changed in Project Service Automation Early Access Wave 1 2021, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

## <a name="project-service-automation-early-access-wave-1-2021-v3"></a><span data-ttu-id="08eda-104">Project Service Automation бағдарламасының 2021 жылғы ерте қатынасу шығарылымның 1-толқыны, V3 нұсқасы</span><span class="sxs-lookup"><span data-stu-id="08eda-104">Project Service Automation Early Access Wave 1 2021, V3</span></span>

<span data-ttu-id="08eda-105">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="08eda-105">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="08eda-106">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="08eda-106">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="08eda-107">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="08eda-107">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="08eda-108">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="08eda-108">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="08eda-109">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="08eda-109">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="08eda-110">Бұл тақырыпта жаңа немесе Project Service Automation бағдарламасының 2021 жылғы ерте қатынасу шығарылымның 1-толқыны, V3 нұсқасына өзгертілген қолжетімді мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="08eda-110">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Early Access Wave 1 2021.</span></span> <span data-ttu-id="08eda-111">Бұл нұсқаның құрастыру нөмірі — V3.10.49.3 және бұл нұсқа әдетте 2021 жылдың ақпан айында дербес жаңарту арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="08eda-111">This version has a build number of V3.10.49.3 and is generally available through a self-update in February 2021.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="08eda-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="08eda-112">Bug fixes</span></span>

<span data-ttu-id="08eda-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="08eda-113">**Time and Expense**</span></span>

<span data-ttu-id="08eda-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="08eda-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="08eda-115">Ұзақтық нөлге тең болғанда уақыт жазбасы жасалған кезде, аяқталу күндері автоматты түрде толтырылады.</span><span class="sxs-lookup"><span data-stu-id="08eda-115">End dates auto-populate when a time entry is created if the duration is null.</span></span>
- <span data-ttu-id="08eda-116">Пайдаланушылар тапсырманы бекітілген немесе жіберілген уақыт жазбасы бойынша өзгерте алады.</span><span class="sxs-lookup"><span data-stu-id="08eda-116">Users can change the task on a time entry that has been approved or submitted.</span></span>
