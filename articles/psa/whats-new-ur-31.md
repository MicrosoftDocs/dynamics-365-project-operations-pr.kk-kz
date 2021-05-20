---
title: Project Service Automation бағдарламасының 31-жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 31-ші жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: a595c0a129ac35d3416984e57908e73e1eaef2fd
ms.sourcegitcommit: 6e1498502461e86cff722ccaf8795ff11c7c47ad
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5945542"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="56c0a-103">Project Service Automation бағдарламасының 31-жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="56c0a-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="56c0a-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="56c0a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="56c0a-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="56c0a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="56c0a-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="56c0a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="56c0a-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="56c0a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="56c0a-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="56c0a-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="56c0a-109">Бұл бөлімде Project Service Automation бағдарламасының 31-жаңарту шығарылымының 3-нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="56c0a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="56c0a-110">Бұл нұсқаның V3.10.52.77 құрастыру нөмірі бар, сондай-ақ 2021 жылдыңң мамыр айында өзіндік жаңарту арқылы жалпы түрде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="56c0a-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="56c0a-111">31-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="56c0a-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="56c0a-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="56c0a-112">Bug fixes</span></span>

<span data-ttu-id="56c0a-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="56c0a-113">**Time and Expense**</span></span>

<span data-ttu-id="56c0a-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="56c0a-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="56c0a-115">**Тапсырыс беруге болатын ресурс** бетіндегі уақытты енгізуді басқару пәрменінің түймелері шатастырылды.</span><span class="sxs-lookup"><span data-stu-id="56c0a-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="56c0a-116">Уақыт жазбасын бекіту кезінде **Project.SetTrackingFields** нысанында жарамсыз сілтеме ерекшелігі жасалды.</span><span class="sxs-lookup"><span data-stu-id="56c0a-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="56c0a-117">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="56c0a-117">**Resource Management**</span></span>

<span data-ttu-id="56c0a-118">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="56c0a-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="56c0a-119">**Топ мүшесін жасау** мүмкіндігі **Орындалған тапсырыстың әдепкі күйі** үшін тапсырыс беру параметрі метадеректерінің параметрін дұрыс көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="56c0a-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="56c0a-120">PSA 1.X нұсқасынан 3.X нұсқасына дейін жаңарту кезінде жаңарту процесі **UpgradeResourceRequirements** күйінде сәтсіз аяқталады.</span><span class="sxs-lookup"><span data-stu-id="56c0a-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="56c0a-121">**Сатылым**</span><span class="sxs-lookup"><span data-stu-id="56c0a-121">**Sales**</span></span>

<span data-ttu-id="56c0a-122">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="56c0a-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="56c0a-123">Нақты кіріс бақылау торындағы соманы жоба валютасына айналдырады.</span><span class="sxs-lookup"><span data-stu-id="56c0a-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="56c0a-124">Ұйымның базалық валютасы жобаның валютасынан өзгеше болатын сценарийлерде журнал жолдарын, баға ұсыну жолдары мен келісімшарттар жолдарын жасау кезінде әдепкі валюта анық емес.</span><span class="sxs-lookup"><span data-stu-id="56c0a-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="56c0a-125">**Күту режиміндегі түзету журналын тексеру** сұранысы жоба бойынша сүзгіленбейді.</span><span class="sxs-lookup"><span data-stu-id="56c0a-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="56c0a-126">Қалған сатылымдар жоба бойынша дұрыс есептелмеген.</span><span class="sxs-lookup"><span data-stu-id="56c0a-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="56c0a-127">Контактіге негізделген баға ұсыныстары бағатізбесіз жасалған кезде сәтсіздікке ұшырайды.</span><span class="sxs-lookup"><span data-stu-id="56c0a-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="56c0a-128">**Шот-фактураны растау** опциясы таңдалғанда өңдеу санағышы көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="56c0a-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="56c0a-129">**Шот-фактураны жасау** опциясы таңдалғанда өңдеу санағышы көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="56c0a-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="56c0a-130">Баға ұсынысын ұтылған ретінде жабу тапсырыстарды тоқтатпайды.</span><span class="sxs-lookup"><span data-stu-id="56c0a-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







