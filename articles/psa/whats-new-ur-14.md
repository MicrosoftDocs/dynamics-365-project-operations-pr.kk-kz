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
ms.openlocfilehash: b811bf7ccfb626e6944801dffa943d2afab0c5e8
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124825"
---
# <a name="project-service-automation-update-release-14-v3"></a><span data-ttu-id="6a4d3-103">Project Service Automation 14 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="6a4d3-103">Project Service Automation Update Release 14, V3</span></span>
<span data-ttu-id="6a4d3-104">Dynamics 365 Project Service Automation (PSA) бағдарламасының ең соңғы жаңартуын қуана хабарлаймыз.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="6a4d3-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="6a4d3-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="6a4d3-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына кіріп, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="6a4d3-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="6a4d3-109">Бұл бөлімде PSA бағдарламасының 14-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="6a4d3-110">Бұл нұсқа V3.10.4.21 құрылым нөміріне ие және келесі кестеде қолжетімді:</span><span class="sxs-lookup"><span data-stu-id="6a4d3-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="6a4d3-111">**Жалпы қолжетімділік (өзін-өзі жаңарту):** қаңтар, 2020 ж</span><span class="sxs-lookup"><span data-stu-id="6a4d3-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="6a4d3-112">**Автоматты жаңарту:** ақпан, 2020 ж</span><span class="sxs-lookup"><span data-stu-id="6a4d3-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="6a4d3-113">14-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="6a4d3-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="6a4d3-114">Кеңейтімдер</span><span class="sxs-lookup"><span data-stu-id="6a4d3-114">Enhancements</span></span>

- <span data-ttu-id="6a4d3-115">Sales</span><span class="sxs-lookup"><span data-stu-id="6a4d3-115">Sales</span></span>

     - <span data-ttu-id="6a4d3-116">Баға ұсынысы **"Сәтті" ретінде жабылған** күйіне жаңартылғанда, **Баға ұсыну жолының мәліметтері** өрісіндегі мәндер **Жобалық келісім-шарт жолы мәліметтері** өрісіне көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="6a4d3-117">Расталған жобалар **"Сәтсіз" ретінде жабылған** күйінде болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="6a4d3-118">Ресурсты басқару</span><span class="sxs-lookup"><span data-stu-id="6a4d3-118">Resource Management</span></span>

     - <span data-ttu-id="6a4d3-119">Тапсырыстарды кеңейту кезінде, пайдаланушыларға тапсырыс нәтижелерін қорытындылау және "Тапсырыстарды жүргізу" сілтемесін беру үшін растау диалогтық терезесі ұсынылады.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="6a4d3-120">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="6a4d3-120">Bug fixes</span></span>

- <span data-ttu-id="6a4d3-121">Уақыт және шығыс</span><span class="sxs-lookup"><span data-stu-id="6a4d3-121">Time and Expense</span></span>

     - <span data-ttu-id="6a4d3-122">Түзетілді: пайдаланушы түзетуге арналған жазбаларды таңдамаған кезде, пайдаланушы тәжірибесі жақсарды.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="6a4d3-123">Ресурсты басқару</span><span class="sxs-lookup"><span data-stu-id="6a4d3-123">Resource Management</span></span>

     - <span data-ttu-id="6a4d3-124">Түзетілді: ресурсқа бірнеше рет тапсырыс беру тапсырыс беруге болатын ресурс атауының толып кетуіне әкеледі.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="6a4d3-125">Sales</span><span class="sxs-lookup"><span data-stu-id="6a4d3-125">Sales</span></span>

     - <span data-ttu-id="6a4d3-126">Түзетілді: жалпы сату бағасы пайдаланушы жоба бойынша шығындар сметасының өзіндік құнын енгізгенге дейін есептелмейді.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="6a4d3-127">Түзетілді: егер байланысты жобалық келісім-шарт **Жоба** күйінде болмаса, баға ұсынысы **Сәтті** ретінде жабылмайды.</span><span class="sxs-lookup"><span data-stu-id="6a4d3-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>

