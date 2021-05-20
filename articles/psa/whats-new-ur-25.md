---
title: Project Service Automation бағдарламасының 25-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 25-жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 3aa10e1d4b23fbe6c2743d71497bdef840776008
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948878"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a><span data-ttu-id="faf69-103">Project Service Automation бағдарламасының 25-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="faf69-103">What's new or changed in Project Service Automation Update Release 25, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="faf69-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="faf69-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="faf69-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="faf69-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="faf69-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="faf69-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="faf69-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="faf69-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="faf69-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="faf69-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="faf69-109">Бұл тақырыпта Project Service Automation бағдарламасының 25-жаңарту шығарылымының 3 нұсқасы үшін жаңартылған немесе өзгертілген мүмкіндіктер мен түзетулер көрсетілген. Бұл нұсқада 3.10.43.76 нұсқасының құрылым нөмірі бар және ол 2020 жылдың қазан айындағы өзін-өзі жаңартуы арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="faf69-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 25 This version has a build number of V 3.10.43.76 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-25"></a><span data-ttu-id="faf69-110">25-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="faf69-110">Update Release 25</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="faf69-111">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="faf69-111">Bug fixes</span></span>

<span data-ttu-id="faf69-112">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="faf69-112">**Time and Expense**</span></span>

<span data-ttu-id="faf69-113">Келесі мәселе түзетілді:</span><span class="sxs-lookup"><span data-stu-id="faf69-113">The following issue has been fixed:</span></span>

- <span data-ttu-id="faf69-114">Тым үлкен аралыққа негізделген қосымша деректерді көрсететін уақыт жазбасы шығарылды.</span><span class="sxs-lookup"><span data-stu-id="faf69-114">Time entry chart showing additional data based on too large of an interval being retrieved.</span></span>

<span data-ttu-id="faf69-115">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="faf69-115">**Resource Management**</span></span>

<span data-ttu-id="faf69-116">Келесі мәселе түзетілді:</span><span class="sxs-lookup"><span data-stu-id="faf69-116">The following issue has been fixed:</span></span>

- <span data-ttu-id="faf69-117">Universal Resource Scheduling түзетуінің импортын, жоғары нұсқалы түзету бұрыннан бар болса, өткізіп жіберу үшін Package deployer құралының коды қосылды.</span><span class="sxs-lookup"><span data-stu-id="faf69-117">Added package deployer code to skip the Universal Resource Scheduling patch import if a higher version patch already exists.</span></span>

<span data-ttu-id="faf69-118">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="faf69-118">**Project Management**</span></span>

<span data-ttu-id="faf69-119">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="faf69-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="faf69-120">Жобаны бақылау торында дұрыс емес жоспарлы құнға әкелетін айырбас бағамының дөңгелектенуі мен сәйкессіздіктері түзетілді.</span><span class="sxs-lookup"><span data-stu-id="faf69-120">Corrected rounding and exchange rate discrepancies resulting in incorrect planned cost in the project tracking grid.</span></span>
- <span data-ttu-id="faf69-121">**Жоба** пішінінде екі немесе одан да көп реакция торларын көрсету мүмкіндігіне қолдау көрсетілді.</span><span class="sxs-lookup"><span data-stu-id="faf69-121">Support the ability to display two or more react grids on the **Project** form.</span></span>
- <span data-ttu-id="faf69-122">Тапсырманы күнтізбелік аяқталу күнінен бұрын тағайындау мүмкіндігін шешу үшін тексеру ұсынылды, бұл ресурстың сәтсіз тағайындалуына әкеледі.</span><span class="sxs-lookup"><span data-stu-id="faf69-122">Provided validation to address the ability to assign a task past the calendar end date, which results in a failed resource assignment.</span></span>
- <span data-ttu-id="faf69-123">Төменде келтірілгеннен құрылған Null Reference Exception мүмкіндігін шешу үшін қателерді өңдеу жақсартылды:</span><span class="sxs-lookup"><span data-stu-id="faf69-123">Improved error handling to address Null Reference Exception generated from the following:</span></span>

    - <span data-ttu-id="faf69-124">**PreValidateProjectTeamMemberCreate** қосылатын модулі</span><span class="sxs-lookup"><span data-stu-id="faf69-124">**PreValidateProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="faf69-125">**PreValidateProjectTaskCreate** жоба тапсырмасы байланысты жобасыз жасалған кезде</span><span class="sxs-lookup"><span data-stu-id="faf69-125">**PreValidateProjectTaskCreate** when a project task is created without an associated project</span></span>
    - <span data-ttu-id="faf69-126">**PreProjectTeamMemberCreate** қосылатын модулі</span><span class="sxs-lookup"><span data-stu-id="faf69-126">**PreProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="faf69-127">**PostProjectTeamMemberDelete** қосылатын модулі</span><span class="sxs-lookup"><span data-stu-id="faf69-127">**PostProjectTeamMemberDelete** plug-in</span></span>
    - <span data-ttu-id="faf69-128">**PreValidateProjectTaskDelete** қосылатын модулі</span><span class="sxs-lookup"><span data-stu-id="faf69-128">**PreValidateProjectTaskDelete** plug-in</span></span>

<span data-ttu-id="faf69-129">**Sales**</span><span class="sxs-lookup"><span data-stu-id="faf69-129">**Sales**</span></span>

<span data-ttu-id="faf69-130">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="faf69-130">The following issues have been fixed:</span></span>

- <span data-ttu-id="faf69-131">**Жобаны көшіру: HelperResource болжамдарын басқару** мүмкіндігінен құрылған Null Reference Exception мүмкіндігін шешу үшін қателерді өңдеу жақсартылды.</span><span class="sxs-lookup"><span data-stu-id="faf69-131">Improved error handling to address Null Reference Exceptions generated from **Copy Project: Estimates HelperResource Management**.</span></span>
- <span data-ttu-id="faf69-132">**Уақыт және материалдық шоттың орындалмаған әрекеттері** тармағындағы **Есеп-шот ұсынуға дайын емес** төлем күйін өшірмейді.</span><span class="sxs-lookup"><span data-stu-id="faf69-132">**Not ready to Invoice** on a **Time and Material Billing Backlog** doesn't clear the billing status.</span></span>
- <span data-ttu-id="faf69-133">**Рөл бағасы** және **Каталог элементтері** қойыншасындағы қате белгіленген **Бағалар** түймешігі түзетілді.</span><span class="sxs-lookup"><span data-stu-id="faf69-133">Corrected mislabeled **Prices** buttons on the **Role Price** and **Catalog Items** tab.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]