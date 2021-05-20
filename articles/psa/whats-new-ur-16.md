---
title: Project Service Automation бағдарламасының 16 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 16-жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/18/2020
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
ms.openlocfilehash: 33a711816e8cca34c4595aa0929de9a808a48b0f
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949396"
---
# <a name="project-service-automation-update-release-16-v3"></a><span data-ttu-id="1a408-103">Project Service Automation 16 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="1a408-103">Project Service Automation Update Release 16, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="1a408-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="1a408-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="1a408-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="1a408-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="1a408-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="1a408-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="1a408-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="1a408-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="1a408-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту](/dynamics365/project-service/upgrade-psa-home-page) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="1a408-108">For more information, see [Install, Update a Preferred Solution](/dynamics365/project-service/upgrade-psa-home-page).</span></span>
<span data-ttu-id="1a408-109">Бұл бөлімде PSA бағдарламасының 16-шы жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="1a408-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 16.</span></span> <span data-ttu-id="1a408-110">Бұл нұсқа V3.10.6.34 құрылым нөміріне ие және әдетте 2020 жылдың қаңтар айында шыққан өзін-өзі жаңарту мүмкіндігі арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="1a408-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in January 2020.</span></span>


## <a name="update-release-16"></a><span data-ttu-id="1a408-111">16-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="1a408-111">Update Release 16</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="1a408-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="1a408-112">Bug fixes</span></span>

-   <span data-ttu-id="1a408-113">Уақыт және шығыс</span><span class="sxs-lookup"><span data-stu-id="1a408-113">Time and Expense</span></span>

    -   <span data-ttu-id="1a408-114">Бекітілді: Растаулар үшін жойылған уақыт пен шығыстар туралы жазбаларды жіберуге тырысатын пайдаланушылар енді тиісті қате туралы хабарларды алады.</span><span class="sxs-lookup"><span data-stu-id="1a408-114">Fixed: Users attempting to submit deleted time and expense entries for approvals will now receive relevant error messages.</span></span>

-   <span data-ttu-id="1a408-115">Жоба басқармасы</span><span class="sxs-lookup"><span data-stu-id="1a408-115">Project Management</span></span>

    -   <span data-ttu-id="1a408-116">Бекітілді: Үлгілердегі топ мүшелері үшін үлгі бойынша анықталған ресурстық қамтамасыз ету бірліктері жаңа жобаға қолданылатын үлгілермен бірге сақталады.</span><span class="sxs-lookup"><span data-stu-id="1a408-116">Fixed: The resourcing units defined for team members in templates are respected with the templates are applied to a new project.</span></span>

    -   <span data-ttu-id="1a408-117">Бекітілді: Жазбаның меншік түрін қайта тағайындауды өңдеу жақсартылды.</span><span class="sxs-lookup"><span data-stu-id="1a408-117">Fixed: Improved handling of the re-assignment of record ownership.</span></span>

    -   <span data-ttu-id="1a408-118">Бекітілді: Көшіру процессіндегі жобаларды көшірудің барлық операциялары аяқталғанша көшіруге рұқсат етілмейді.</span><span class="sxs-lookup"><span data-stu-id="1a408-118">Fixed: Projects that are in the process of being copied will not be permitted to copied until all copy operations are complete.</span></span>

-   <span data-ttu-id="1a408-119">Ресурсты басқару</span><span class="sxs-lookup"><span data-stu-id="1a408-119">Resource Management</span></span>

    -   <span data-ttu-id="1a408-120">Бекітілді: Тапсырыс беруді кеңейту енді қысқа уақыт аралықтарын дұрыс басқарады және енді кеңейтілген тапсырыс беру жүйелері үшін нөлдік сағаттарды жасамайды.</span><span class="sxs-lookup"><span data-stu-id="1a408-120">Fixed: Extend bookings now handles short durations correctly and no longer creates zero hours for extended bookings.</span></span>

    -   <span data-ttu-id="1a408-121">Бекітілді: Енді жобаның уақыт белдеуі +5:30 GMT, ал пайдаланушының уақыт белдеуі басқа болған кезде салыстыру көрінісі пайда болады.</span><span class="sxs-lookup"><span data-stu-id="1a408-121">Fixed: The reconciliation view now renders when the project time zone is +5:30 GMT and the user’s time aone is different.</span></span>

-   <span data-ttu-id="1a408-122">Sales</span><span class="sxs-lookup"><span data-stu-id="1a408-122">Sales</span></span>

    -   <span data-ttu-id="1a408-123">Бекітілді: Келісім-шарт жолымен салыстырылған жоба жойылып, жаңа жоба салыстырылған кезде жаңа жобадағы нақты жазбалар келісім-шарт жолында анықталған есеп-шот ұсыну және бағалау ережелеріне негізделген қайта бағалауға ұшырамайды.</span><span class="sxs-lookup"><span data-stu-id="1a408-123">Fixed: When a project mapped to a contract line is removed and a new project is mapped, the actual records on the new project were not getting re-evaluated based on the billing and pricing rules defined on the contract line.</span></span> <span data-ttu-id="1a408-124">Бұл осы шығарылымда бекітілген.</span><span class="sxs-lookup"><span data-stu-id="1a408-124">This has been fixed in this release.</span></span> <span data-ttu-id="1a408-125">Жаңадан салыстырылған жобадағы бағалау және нақты жазбалар кері қайтарылып, келісім-шарт жолының бағалау және есеп-шот ұсыну ережелеріне негізделе отырып қайтадан тиісті түрде жасалады.</span><span class="sxs-lookup"><span data-stu-id="1a408-125">Pricing and actual records on the newly mapped project will get reversed and re-created correctly based on the pricing and billing rules of the contract line.</span></span> <span data-ttu-id="1a408-126">Салыстырылмаған жобаның нақты жазбалары қайтадан бағаланып, нәтижесінде қайта жасалады.</span><span class="sxs-lookup"><span data-stu-id="1a408-126">The actual records of the un-mapped project will also get re-evaluated and re-created as a consequence.</span></span>

    -   <span data-ttu-id="1a408-127">Бекітілді: Бос мәндердің сақталмағанын тексеру үшін бағалау жолының **Сомасы** өрісіне қосымша растау қосылады.</span><span class="sxs-lookup"><span data-stu-id="1a408-127">Fixed: Additional validation has been added to an estimate line’s **Amount** field to ensure that null values are not persisted.</span></span>

    -   <span data-ttu-id="1a408-128">Бекітілді: Жобада нақты деректер жаңартылғаннан кейін пайдаланушыларға нақты деректерді қайта синхрондауға мүмкіндік беру үшін жобаның негізгі пішініне жаңарту түймесі қосылды.</span><span class="sxs-lookup"><span data-stu-id="1a408-128">Fixed: When actuals have been updated on a project, a refresh button has been added to the project main form to allow users to re-sync the actuals.</span></span>

    -   <span data-ttu-id="1a408-129">Бекітілді: Пайдаланушылар 2.X нұсқасынан 3.X нұсқасына дейін жаңартылған кезде, жоба атауына арналған БОС мәні бар жобаларға рұқсат етіледі.</span><span class="sxs-lookup"><span data-stu-id="1a408-129">Fixed: When users upgrade from 2.X to 3.X, projects with a NULL value for project name will be permitted.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]