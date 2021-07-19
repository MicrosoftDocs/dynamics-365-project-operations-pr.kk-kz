---
title: Project Service Automation бағдарламасының 33 жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 33 жаңарту шығарылымының 3‑нұсқасында қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334563"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a><span data-ttu-id="138bb-103">Project Service Automation бағдарламасының 33 жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="138bb-103">What's new or changed in Project Service Automation Update Release 33, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="138bb-104">Біз Microsoft Dynamics 365 Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="138bb-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="138bb-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="138bb-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="138bb-106">Бұл Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="138bb-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="138bb-107">Осы шығарылымға жаңарту үшін Dynamics 365 онлайн шешімдері бетінің әкімші орталығына кіріп, жаңартуды орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="138bb-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="138bb-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="138bb-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="138bb-109">Бұл бөлімде Project Service Automation бағдарламасының 33 жаңарту шығарылымының 3 нұсқасындағы жаңа немесе өзгертілген мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="138bb-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 33.</span></span> <span data-ttu-id="138bb-110">Бұл нұсқада V3.10.54.98 құрастыру нөмірі бар және әдетте 2021 жылдың шілде айындағы өзін-өзі жаңарту арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="138bb-110">This version has a build number of V3.10.54.98 and is generally available through a self-update in July 2021.</span></span>

## <a name="update-release-33"></a><span data-ttu-id="138bb-111">33-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="138bb-111">Update Release 33</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="138bb-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="138bb-112">Bug fixes</span></span>

<span data-ttu-id="138bb-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="138bb-113">**Time and Expense**</span></span>

<span data-ttu-id="138bb-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="138bb-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="138bb-115">**msdyn_description** және **msdyn_externaldescription** екі құлыпталған өрісі жіберілгеннен кейін өңделеді.</span><span class="sxs-lookup"><span data-stu-id="138bb-115">Two locked fields, **msdyn_description** and **msdyn_externaldescription** are editable after submission.</span></span>
- <span data-ttu-id="138bb-116">Жобаға қатысы жоқ шығын жасалса, қате туралы хабар пайда болады.</span><span class="sxs-lookup"><span data-stu-id="138bb-116">An error message occurs if an expense is created that isn't related to a project.</span></span>
- <span data-ttu-id="138bb-117">Уақыт жазбасы жасалған кезде ресурс рөлі әдетте белсенді емес рөл болады.</span><span class="sxs-lookup"><span data-stu-id="138bb-117">When a time entry is created, the resource role defaults to an inactive role.</span></span>
- <span data-ttu-id="138bb-118">Қайта шақырылған және жойылған шығындармен байланысты журнал жолдары жойылмайды.</span><span class="sxs-lookup"><span data-stu-id="138bb-118">Journal lines associated with a recalled and deleted expense aren't deleted.</span></span>
- <span data-ttu-id="138bb-119">**Уақыт жазбасын жылдам жасау пішіні** бетінде **Жобаның тапсырмалар тізімі** көрінісін әдепкі бойынша көрсетілген күнді тапсырманың басталу күніне өзгерту үшін жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="138bb-119">On the **Time entry Quick Create Form**, update the **Project Task List** view to change the date displayed by default to the start date of the task.</span></span>
- <span data-ttu-id="138bb-120">Тапсырыс беруге болатын ресурстың **Қатысты** қойыншасынан уақыт жазбасын жасаған кезде, уақыт жазбасы басты тапсырыс беруге болатын ресурс орнына жүйеге кірген пайдаланушы үшін қате жасалады.</span><span class="sxs-lookup"><span data-stu-id="138bb-120">When you create a time entry from the **Related** tab of the bookable resource, the time entry is incorrectly created for the signed-in user instead of the parent bookable resource.</span></span>
- <span data-ttu-id="138bb-121">Жаңа өрістер **MDD жаппай растау** диалогтық терезесіне қосылады.</span><span class="sxs-lookup"><span data-stu-id="138bb-121">New fields are added to the **Bulk approval MDD** dialog box.</span></span>

<span data-ttu-id="138bb-122">**Жобаны жоспарлау**</span><span class="sxs-lookup"><span data-stu-id="138bb-122">**Project planning**</span></span>

<span data-ttu-id="138bb-123">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="138bb-123">The following issues have been fixed:</span></span>
- <span data-ttu-id="138bb-124">Жобаның жұмыс уақытының үлгілері күрделі күнтізбелермен қолданылған кезде, жобаны құрудың баяу өнімділігі.</span><span class="sxs-lookup"><span data-stu-id="138bb-124">Slow project creation performance when project work hour templates are applied with complex calendars.</span></span>
- <span data-ttu-id="138bb-125">Басталу күні аяқталу күнінен үлкен болған кезде, әр өрістің уақыт құрамдасындағы айырмашылықтарға байланысты жобаны көшіру үлгісінде қате көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="138bb-125">When the start date is greater than the end date, an error displays on the copy project template because of differences in the time component of each field.</span></span>

<span data-ttu-id="138bb-126">**Ресурстарды басқару**</span><span class="sxs-lookup"><span data-stu-id="138bb-126">**Resource management**</span></span>

<span data-ttu-id="138bb-127">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="138bb-127">The following issues have been fixed:</span></span>
- <span data-ttu-id="138bb-128">Ресурстарды пайдалану сұрауында қате параметр қолданылған және XML файлы **Ресурстарды пайдалану** торында қате сүзгі нәтижелеріне әкеледі.</span><span class="sxs-lookup"><span data-stu-id="138bb-128">An incorrect parameter is used in the resource utilization query and the XML leads to incorrect filter results on the **Resource Utilization** grid.</span></span>
- <span data-ttu-id="138bb-129">**Тапсырыстарды кеңейту** растауы тапсырыстар үшін аяқталу күнін дұрыс көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="138bb-129">The **Extend Bookings** confirmation displays incorrect end date for bookings.</span></span>

<span data-ttu-id="138bb-130">**Сатылым**</span><span class="sxs-lookup"><span data-stu-id="138bb-130">**Sales**</span></span>

<span data-ttu-id="138bb-131">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="138bb-131">The following issues have been fixed:</span></span>
- <span data-ttu-id="138bb-132">Егер санат бағасы жоқ мәндермен жасалса, қате туралы хабар пайда болады.</span><span class="sxs-lookup"><span data-stu-id="138bb-132">An error message occurs if a category price is created with missing values.</span></span>
- <span data-ttu-id="138bb-133">Егер келісім‑шарт жолының кезеңі тапсырыс жолынсыз жасалса қате туралы хабар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="138bb-133">An error message occurs if a contract line milestone is created without an order line.</span></span>
