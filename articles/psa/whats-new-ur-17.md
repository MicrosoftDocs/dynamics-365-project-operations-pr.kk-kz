---
title: Project Service Automation бағдарламасының 17 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 17 жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: f9fb941a95b0610dc546b1c12a87aa7faef4d676
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143737"
---
# <a name="project-service-automation-update-release-17-v3"></a><span data-ttu-id="f031d-103">Project Service Automation 17 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="f031d-103">Project Service Automation Update Release 17, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="f031d-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="f031d-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="f031d-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="f031d-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="f031d-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="f031d-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f031d-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f031d-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="f031d-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="f031d-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f031d-109">Бұл бөлімде PSA бағдарламасының 17 жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="f031d-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 17.</span></span> <span data-ttu-id="f031d-110">Бұл нұсқа V3.10.6.34 құрылым нөміріне ие және әдетте 2020 жылдың наурыз айында шыққан өзін-өзі жаңарту мүмкіндігі арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="f031d-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-17"></a><span data-ttu-id="f031d-111">17-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="f031d-111">Update Release 17</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="f031d-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="f031d-112">Bug fixes</span></span>

<span data-ttu-id="f031d-113">**Жалпы**</span><span class="sxs-lookup"><span data-stu-id="f031d-113">**General**</span></span>

- <span data-ttu-id="f031d-114">Бекітілді: Топ мүшелерінің лицензияларын қамтамасыз ету үшін Project Service Automation жаңартыңыз (Жоба ресурсының хабы топ мүшесі қызметінің 3.х метадеректерін қамтиды)</span><span class="sxs-lookup"><span data-stu-id="f031d-114">Fixed: Update Project Service Automation to enforce Team Member licenses (Project Resource Hub will include Team Member Service plan metadata 3.x)</span></span>
 
<span data-ttu-id="f031d-115">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="f031d-115">**Time and Expense**</span></span>

- <span data-ttu-id="f031d-116">Бекітілді: Шығыс бағалауын нөлдік емес бағадан нөлдік (0) бағаға өзгерту мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="f031d-116">Fixed: It is not possible to change an expense estimate from a non-zero price to zero (0).</span></span> <span data-ttu-id="f031d-117">Өзгеріс еленбеді.</span><span class="sxs-lookup"><span data-stu-id="f031d-117">The change is ignored.</span></span>

<span data-ttu-id="f031d-118">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="f031d-118">**Project Management**</span></span>

- <span data-ttu-id="f031d-119">Бекітілді: топ мүшелерінің лауазым атына бос мәндерді тексеру қосылды.</span><span class="sxs-lookup"><span data-stu-id="f031d-119">Fixed: A check for null values has been added on a team member's position name.</span></span>
- <span data-ttu-id="f031d-120">Бекітілді: **msdyn_userresourceid** өрісі **msdyn_resourceassignment** нысанында ескірген.</span><span class="sxs-lookup"><span data-stu-id="f031d-120">Fixed: **msdyn_userresourceid** field on the **msdyn_resourceassignment** entity has been deprecated.</span></span>
- <span data-ttu-id="f031d-121">Бекітілді: 2.x нұсқасынан 3.x нұсқасына жаңарту енді тапсырма тағайындауларындағы бос талпыныс контурларын өңдейді.</span><span class="sxs-lookup"><span data-stu-id="f031d-121">Fixed: Upgrade from 2.x to 3.x now handles empty effort contours on task assignments.</span></span>

<span data-ttu-id="f031d-122">**Sales**</span><span class="sxs-lookup"><span data-stu-id="f031d-122">**Sales**</span></span>

- <span data-ttu-id="f031d-123">Бекітілді: **Invoice.PreValidateInvoiceUpdate** енді жазба иелерін қайта тағайындау сценарийлерін дұрыс өңдейді.</span><span class="sxs-lookup"><span data-stu-id="f031d-123">Fixed: **Invoice.PreValidateInvoiceUpdate** now handles the scenario of reassigning record owners properly.</span></span>
- <span data-ttu-id="f031d-124">Бекітілді: транзакция класы **Уақыт** болғанда, **UnitGroup** нысаны **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, және **ContractLineDetails** нысандарын қоса алғанда барлық нысандар үшін өңделмейтін болады.</span><span class="sxs-lookup"><span data-stu-id="f031d-124">Fixed: When the transaction class is **Time**, **UnitGroup** is non-editable for all entities including, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, and **ContractLineDetails**.</span></span> <span data-ttu-id="f031d-125">Дегенмен **Бірлік** тек **JournalLine** және **InvoiceLineDetails** нысандары үшін өңделмейтін болады.</span><span class="sxs-lookup"><span data-stu-id="f031d-125">However, **Unit** is non-editable only for **JournalLine** and **InvoiceLineDetails**.</span></span>


