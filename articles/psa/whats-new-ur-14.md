---
title: Project Service Automation бағдарламасының 14 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 14-жаңарту шығарылымының 3 нұсқасындағы жаңалықтар туралы ақпарат беріледі.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
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
ms.openlocfilehash: e19c8ffe7d92ab7ec9eb46aff8f944c62b0bb4bc
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280990"
---
# <a name="project-service-automation-update-release-14-v3"></a><span data-ttu-id="11422-103">Project Service Automation 14 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="11422-103">Project Service Automation Update Release 14, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="11422-104">Dynamics 365 Project Service Automation (PSA) бағдарламасының ең соңғы жаңартуын қуана хабарлаймыз.</span><span class="sxs-lookup"><span data-stu-id="11422-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="11422-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="11422-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="11422-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="11422-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="11422-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына кіріп, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="11422-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="11422-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="11422-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="11422-109">Бұл бөлімде PSA бағдарламасының 14-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="11422-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="11422-110">Бұл нұсқа V3.10.4.21 құрылым нөміріне ие және келесі кестеде қолжетімді:</span><span class="sxs-lookup"><span data-stu-id="11422-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="11422-111">**Жалпы қолжетімділік (өзін-өзі жаңарту):** қаңтар, 2020 ж</span><span class="sxs-lookup"><span data-stu-id="11422-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="11422-112">**Автоматты жаңарту:** ақпан, 2020 ж</span><span class="sxs-lookup"><span data-stu-id="11422-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="11422-113">14-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="11422-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="11422-114">Кеңейтімдер</span><span class="sxs-lookup"><span data-stu-id="11422-114">Enhancements</span></span>

- <span data-ttu-id="11422-115">Sales</span><span class="sxs-lookup"><span data-stu-id="11422-115">Sales</span></span>

     - <span data-ttu-id="11422-116">Баға ұсынысы **"Сәтті" ретінде жабылған** күйіне жаңартылғанда, **Баға ұсыну жолының мәліметтері** өрісіндегі мәндер **Жобалық келісім-шарт жолы мәліметтері** өрісіне көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="11422-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="11422-117">Расталған жобалар **"Сәтсіз" ретінде жабылған** күйінде болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="11422-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="11422-118">Ресурсты басқару</span><span class="sxs-lookup"><span data-stu-id="11422-118">Resource Management</span></span>

     - <span data-ttu-id="11422-119">Тапсырыстарды кеңейту кезінде, пайдаланушыларға тапсырыс нәтижелерін қорытындылау және "Тапсырыстарды жүргізу" сілтемесін беру үшін растау диалогтық терезесі ұсынылады.</span><span class="sxs-lookup"><span data-stu-id="11422-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="11422-120">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="11422-120">Bug fixes</span></span>

- <span data-ttu-id="11422-121">Уақыт және шығыс</span><span class="sxs-lookup"><span data-stu-id="11422-121">Time and Expense</span></span>

     - <span data-ttu-id="11422-122">Түзетілді: пайдаланушы түзетуге арналған жазбаларды таңдамаған кезде, пайдаланушы тәжірибесі жақсарды.</span><span class="sxs-lookup"><span data-stu-id="11422-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="11422-123">Ресурсты басқару</span><span class="sxs-lookup"><span data-stu-id="11422-123">Resource Management</span></span>

     - <span data-ttu-id="11422-124">Түзетілді: ресурсқа бірнеше рет тапсырыс беру тапсырыс беруге болатын ресурс атауының толып кетуіне әкеледі.</span><span class="sxs-lookup"><span data-stu-id="11422-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="11422-125">Sales</span><span class="sxs-lookup"><span data-stu-id="11422-125">Sales</span></span>

     - <span data-ttu-id="11422-126">Түзетілді: жалпы сату бағасы пайдаланушы жоба бойынша шығындар сметасының өзіндік құнын енгізгенге дейін есептелмейді.</span><span class="sxs-lookup"><span data-stu-id="11422-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="11422-127">Түзетілді: егер байланысты жобалық келісім-шарт **Жоба** күйінде болмаса, баға ұсынысы **Сәтті** ретінде жабылмайды.</span><span class="sxs-lookup"><span data-stu-id="11422-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]