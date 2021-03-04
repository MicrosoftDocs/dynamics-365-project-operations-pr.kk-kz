---
title: Project Service Automation бағдарламасының 15 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 15-жаңарту шығарылымының 3 нұсқасындағы жаңалықтар туралы ақпарат беріледі.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/27/2020
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
ms.openlocfilehash: 0ec6746c0d3a1a03ee56440c73d044df844046f8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143970"
---
# <a name="project-service-automation-update-release-15-v3"></a><span data-ttu-id="80305-103">Project Service Automation 15 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="80305-103">Project Service Automation Update Release 15, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="80305-104">Dynamics 365 Project Service Automation (PSA) бағдарламасының ең соңғы жаңартуын қуана хабарлаймыз.</span><span class="sxs-lookup"><span data-stu-id="80305-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="80305-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="80305-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="80305-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="80305-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="80305-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына кіріп, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="80305-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="80305-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="80305-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="80305-109">Бұл бөлімде PSA бағдарламасының 15-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="80305-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 15.</span></span> <span data-ttu-id="80305-110">Бұл нұсқа V3.10.5.28 құрылым нөміріне ие және әдетте 2020 жылдың қаңтар айында шыққан өзін-өзі жаңарту мүмкіндігі арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="80305-110">This version has a build number of V3.10.5.28 and is generally available through a self-update in January 2020.</span></span>

## <a name="update-release-15"></a><span data-ttu-id="80305-111">15-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="80305-111">Update Release 15</span></span> 

### <a name="enhancements"></a><span data-ttu-id="80305-112">Кеңейтімдер</span><span class="sxs-lookup"><span data-stu-id="80305-112">Enhancements</span></span>

- <span data-ttu-id="80305-113">Жоба басқармасы</span><span class="sxs-lookup"><span data-stu-id="80305-113">Project Management</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="80305-114">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="80305-114">Bug fixes</span></span>

- <span data-ttu-id="80305-115">Уақыт және шығыс</span><span class="sxs-lookup"><span data-stu-id="80305-115">Time and Expense</span></span>

  - <span data-ttu-id="80305-116">Түзетілді: салыстыру көрінісінде жүктеу кезінде қателерді өңдеуді қосу.</span><span class="sxs-lookup"><span data-stu-id="80305-116">Fixed: Add on-load error handling in the reconciliation view.</span></span>
  - <span data-ttu-id="80305-117">Түзетілді: Жоба ресурсының хабы: түсініксіздікті азайту үшін **Сома** атауын өзгерту.</span><span class="sxs-lookup"><span data-stu-id="80305-117">Fixed: Project Resource Hub: Rename **Amount** to reduce ambiguity.</span></span>
  - <span data-ttu-id="80305-118">Түзетілді: түрді қосу үшін **Уақыт жазбасы бағандарын көшіру** көрінісін реттеу.</span><span class="sxs-lookup"><span data-stu-id="80305-118">Fixed: Adjust the view **Copy Time Entry Columns** to include the type.</span></span>
  - <span data-ttu-id="80305-119">Түзетілді: ондық сандарды қолдана отырып, тордың көрінісінде уақыт жазбасының ұзақтығын өңдеу кейбір сандар үшін белгісіз қателікке әкеледі.</span><span class="sxs-lookup"><span data-stu-id="80305-119">Fixed: Editing time entry duration in the grid view using decimal numbers results in unknown error for some numbers.</span></span>

- <span data-ttu-id="80305-120">Жоба басқармасы</span><span class="sxs-lookup"><span data-stu-id="80305-120">Project Management</span></span>

  - <span data-ttu-id="80305-121">Түзетілді: **Бақылау көрінісінде пайдалану** ашылмалы мәзірі енді параметрлердің еніне қарай кеңейеді.</span><span class="sxs-lookup"><span data-stu-id="80305-121">Fixed: The drop-down menu for **Use in Tracking View** now expands based on the width of the options.</span></span>
  - <span data-ttu-id="80305-122">Түзетілді: жобаларды +13 уақыт белдеуінде басқару кезінде, тапсырмалардың есептеулері дұрыс емес нәтижелерді көрсетуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="80305-122">Fixed: When managing projects in the +13 time zone, tasks calculations can display inaccurate results.</span></span>
  - <span data-ttu-id="80305-123">Түзетілді: **Топ мүшесінің аяқталу уақыты** тәулік бойғы күнтізбені қолданған кезде түзетілді.</span><span class="sxs-lookup"><span data-stu-id="80305-123">Fixed: **Team Member End Time** has been corrected when using a 24-hour calendar.</span></span>
  - <span data-ttu-id="80305-124">Түзетілді: **BPF** параметрі **msdyn_жоба** негізгі формасында қайта іске қосылды.</span><span class="sxs-lookup"><span data-stu-id="80305-124">Fixed: Re-activated the **BPF** in **msdyn_project** main form.</span></span>
  - <span data-ttu-id="80305-125">Түзетілді: тапсырмалар есептеуі енді бір күнді елемейді.</span><span class="sxs-lookup"><span data-stu-id="80305-125">Fixed: Assignments calculation no longer ignores one day.</span></span>
  - <span data-ttu-id="80305-126">Түзетілді: уақыт белдеуі пайдаланушы мен жоба арасында әр түрлі болған кезде, жаңа хабарландыру баннері жоба нысанына қосылды.</span><span class="sxs-lookup"><span data-stu-id="80305-126">Fixed: A new notification banner has been added to the project form when the time zone differs between user and project.</span></span>

- <span data-ttu-id="80305-127">Sales</span><span class="sxs-lookup"><span data-stu-id="80305-127">Sales</span></span>

  - <span data-ttu-id="80305-128">Түзетілді: шығысты бағалау санатын іздеу параметрі көшірмелерді сүзгілеу үшін пайдаланылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="80305-128">Fixed: Expense estimate category lookup can be used to filter duplicates.</span></span>
  - <span data-ttu-id="80305-129">Түзетілді: **PluginDomain.ExecuteInTryCatchBlock(..)** ішіндегі код бұдан былай ерекшеліктің шығу тегін жасырмайды.</span><span class="sxs-lookup"><span data-stu-id="80305-129">Fixed: Code in **PluginDomain.ExecuteInTryCatchBlock(..)** no longer hides the origin of the exception.</span></span>
  - <span data-ttu-id="80305-130">Түзетілді: 1000-нан астам жоба болған кезде, **Баға ұсыну жолы** пішініндегі **Жобаны іздеу** өрісінде бұдан былай қате туралы хабар пайда болмайды.</span><span class="sxs-lookup"><span data-stu-id="80305-130">Fixed: No longer get an error message in **Project lookup** in the **Quote Line** form when there are more than 1000 projects.</span></span>
  - <span data-ttu-id="80305-131">Түзетілді: еңбекақы мен шығыс болжамдарына арналған **Болжамдар** торы енді дұрыс ақша белгісін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="80305-131">Fixed: **Estimates** grid for labor estimates and expense estimates now displays the correct currency symbol.</span></span>
  - <span data-ttu-id="80305-132">Түзетілді: ұйым PSA бағдарламасын 14-жаңарту шығарылымынан 15-шығарылымға дейін жаңартқан соң, **Кесте** қойыншасы бұдан былай **Жоба** пішінінде бос болып көрінбейді.</span><span class="sxs-lookup"><span data-stu-id="80305-132">Fixed: After an organization updates PSA from Update Release 14 to Update Release 15, the **Schedule** tab no longer appears as blank on the **Project** form.</span></span>
