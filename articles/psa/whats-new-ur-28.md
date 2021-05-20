---
title: Project Service Automation бағдарламасының 28-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 28-жаңарту шығарылымының 3-нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 2d5e8c629f8108ed039948ca70842c9d8afebfa6
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948695"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a><span data-ttu-id="53266-103">Project Service Automation бағдарламасының 28-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="53266-103">What's new or changed in Project Service Automation Update Release 28, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="53266-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="53266-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="53266-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="53266-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="53266-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="53266-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="53266-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="53266-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="53266-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="53266-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="53266-109">Бұл тақырыпта Project Service Automation бағдарламасының 28-жаңарту шығарылымының 3-нұсқасы үшін жаңартылған немесе өзгертілген мүмкіндіктер мен түзетулер көрсетілген. Бұл нұсқада 3.10.46.32 нұсқасының құрылым нөмірі бар және ол 2021 жылдың қаңтар айындағы өзіндік жаңартылу арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="53266-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 28 This version has a build number of V3.10.46.32 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-28"></a><span data-ttu-id="53266-110">28-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="53266-110">Update Release 28</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="53266-111">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="53266-111">Bug fixes</span></span>

<span data-ttu-id="53266-112">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="53266-112">**Time and Expense**</span></span>

<span data-ttu-id="53266-113">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="53266-113">The following issues have been fixed:</span></span>

- <span data-ttu-id="53266-114">Пайдаланушылар бекітілген және ұсынылған уақыт жазбаларын жаңарту үшін **Топтық өңдеу** мүмкіндігін пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="53266-114">Users can use **Bulk Edit** to update time entries that have been approved and submitted.</span></span>

<span data-ttu-id="53266-115">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="53266-115">**Project Management**</span></span>

<span data-ttu-id="53266-116">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="53266-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="53266-117">GUID тапсырмасы сан ретінде түсіндірілетін жағдайларда, тапсырмаларды өңдеу үшін **Жұмыс декомпозициясының құрылымы** бетінің таспасындағы **Тапсырманы өңдеу** мүмкіндігі арқылы ашу мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="53266-117">In cases where the task GUID is interpreted as a number, tasks can't be opened for edit using **Edit Task** in the ribbon on the **Work Breakdown Structure** page.</span></span>

<span data-ttu-id="53266-118">**Sales**</span><span class="sxs-lookup"><span data-stu-id="53266-118">**Sales**</span></span>

<span data-ttu-id="53266-119">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="53266-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="53266-120">**GetEstimatesForProject** қосылатын модулі шақырылғанда бос сілтеме ерекшелігі құрылады.</span><span class="sxs-lookup"><span data-stu-id="53266-120">A null reference exception is generated when the **GetEstimatesForProject** plug-in is invoked.</span></span>
- <span data-ttu-id="53266-121">Кезең торындағы **Шақыруға дайын ретінде белгілеу** жүйесі тек жаңартылатын **Есеп-шот күйі** төлсипатынан басқа төлсипаттарды жартылай жаңартады.</span><span class="sxs-lookup"><span data-stu-id="53266-121">**Mark ready to invoice** on the milestone grid only partially updates attributes, except for the **InvoiceStatus** attribute, which is updated.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]