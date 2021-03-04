---
title: Project Service Automation бағдарламасының 17.5 жаңарту шығарылымы, Hotfix, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 17.5 жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/13/2020
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
ms.openlocfilehash: cd4142176258820f4718f457ca8610f19f584a32
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143736"
---
# <a name="project-service-automation-update-release-175-v3"></a><span data-ttu-id="b2d3b-103">Project Service Automation 17.5 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="b2d3b-103">Project Service Automation Update Release 17.5, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b2d3b-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b2d3b-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="b2d3b-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b2d3b-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="b2d3b-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b2d3b-109">Бұл бөлімде 17.5 жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-109">This topic lists the features and fixes that are new or changed for V3, Update Release 17.5.</span></span> <span data-ttu-id="b2d3b-110">Бұл нұсқа V3.10.7.32 құрылым нөміріне ие және әдетте 2020 жылдың наурыз айында шыққан өзін-өзі жаңарту мүмкіндігі арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-110">This version has a build number of V3.10.7.32 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-175"></a><span data-ttu-id="b2d3b-111">17.5-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="b2d3b-111">Update Release 17.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b2d3b-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="b2d3b-112">Bug fixes</span></span>


<span data-ttu-id="b2d3b-113">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="b2d3b-113">**Project Management**</span></span>

- <span data-ttu-id="b2d3b-114">Бекітілді: Ұзақ уақытқа созылатын тапсырмаларды орындау кезінде пайда болатын сервер тарапынан синхрондау мәселелері қарастырылды.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-114">Fixed: Addressed server-side synchronization issues that occur with long duration tasks.</span></span>
- <span data-ttu-id="b2d3b-115">Бекітілді: Тапсырмаларға жүйесіз түрде қосымша күн қосатын 24 сағаттық жұмыс сағаты үлгілері қарастырылды.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-115">Fixed: Addressed 24-hour work hour templates inaccurately adding an additional day to tasks.</span></span>
- <span data-ttu-id="b2d3b-116">Бекітілді: Тапсырмаларды жүйесіз түрде бір күн алға жылжытатын + 13 GMT жұмыс сағаты үлгілері қарастырылды.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-116">Fixed: Addressed +13 GMT work hour templates inaccurately shifting tasks one day ahead.</span></span>

