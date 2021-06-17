---
title: Project Service Automation бағдарламасының 29.5 жаңарту шығарылымы, Hotfix, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 29.5 жаңарту шығарылымы, Hotfix, 3-нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/26/2021
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
ms.openlocfilehash: d5050945c4ab7c1da61b07ec08bed20f32e166b9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999183"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-295-v3"></a><span data-ttu-id="48a9d-103">Project Service Automation бағдарламасының 29.5 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="48a9d-103">What's new or changed in Project Service Automation Update Release 29.5, V3</span></span>

<span data-ttu-id="48a9d-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="48a9d-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="48a9d-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="48a9d-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="48a9d-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="48a9d-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="48a9d-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="48a9d-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="48a9d-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution.md) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="48a9d-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution.md).</span></span>

<span data-ttu-id="48a9d-109">Бұл бөлімде Project Service Automation бағдарламасының 29.5 жаңарту шығарылымының 3-нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="48a9d-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.5.</span></span> <span data-ttu-id="48a9d-110">Бұл нұсқа V3.10.47.150 құрылым нөміріне ие және әдетте 2021 жылдың қаңтар айында шыққан өзін-өзі жаңарту мүмкіндігі арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="48a9d-110">This version has a build number of V3.10.47.150 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-295"></a><span data-ttu-id="48a9d-111">29.5-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="48a9d-111">Update Release 29.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="48a9d-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="48a9d-112">Bug fixes</span></span>


<span data-ttu-id="48a9d-113">**Сатылым**</span><span class="sxs-lookup"><span data-stu-id="48a9d-113">**Sales**</span></span>

<span data-ttu-id="48a9d-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="48a9d-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="48a9d-115">Баға ұсынысын "ұтқан" ретінде жапқанда және баға ұсынысының бағатізбесі болмаған кезде **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** өрісінде жарамсыз сілтеменің ерекше жағдайы туындауы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="48a9d-115">A possible null reference exception occurs in **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** when you close a quote as won and the quote has no price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
