---
title: Project Service Automation бағдарламасының 30-жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 30-жаңарту шығарылымының 3-нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 3b6b7dba9c2a22587d27006b9972c950fbb454f2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010433"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a><span data-ttu-id="9473a-103">Project Service Automation бағдарламасының 30-жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="9473a-103">What's new or changed in Project Service Automation Update Release 30, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="9473a-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="9473a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="9473a-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="9473a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="9473a-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="9473a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="9473a-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="9473a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="9473a-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution.md) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="9473a-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution.md).</span></span>

<span data-ttu-id="9473a-109">Бұл бөлімде Project Service Automation бағдарламасының 30-жаңарту шығарылымының 3-нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="9473a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 30.</span></span> <span data-ttu-id="9473a-110">Бұл нұсқа V3.10.51.61 жиынтық нөміріне ие және әдетте өзін-өзі жаңарту арқылы 2021 жылдың сәуірінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="9473a-110">This version has a build number of V3.10.51.61 and is generally available through a self-update in April 2021.</span></span>

## <a name="update-release-30"></a><span data-ttu-id="9473a-111">30-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="9473a-111">Update Release 30</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="9473a-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="9473a-112">Bug fixes</span></span>

<span data-ttu-id="9473a-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="9473a-113">**Time and Expense**</span></span>

<span data-ttu-id="9473a-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="9473a-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="9473a-115">**Рөл** өрісі жойылған болса, **Жылдам жасау** бетіндегі уақыт жазбасын жасағанда және сақтағанда қате пайда болады.</span><span class="sxs-lookup"><span data-stu-id="9473a-115">An error occurs when you create and save a time entry on the **Quick Create** page if the **Role** field is removed.</span></span>
- <span data-ttu-id="9473a-116">"Уақыт жазбасы" сүзгісі қате сүзгі операторын қолданады.</span><span class="sxs-lookup"><span data-stu-id="9473a-116">The Time Entry filter applies the wrong filter operator.</span></span>
- <span data-ttu-id="9473a-117">Уақыт жазбасы басқару элементіндегі **Аптаны көшіру** опциясын таңдаған кезде көшірілген уақыт кестелері автоматты түрде көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="9473a-117">Copied timesheets aren't automatically displayed when you select **Copy Week** on the time entry control.</span></span>

<span data-ttu-id="9473a-118">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="9473a-118">**Resource Management**</span></span>

<span data-ttu-id="9473a-119">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="9473a-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="9473a-120">Тапсырысты ұзартқанда, қатты көшірмелеуге тағайындалған брондау күйі дұрыс емес.</span><span class="sxs-lookup"><span data-stu-id="9473a-120">When you extend a booking, the booking status assigned to the hard booking is incorrect.</span></span> <span data-ttu-id="9473a-121">Брондауды ұзарту брондауды орнату метадеректерінде **Бекітілген** ретінде анықталған күйге сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="9473a-121">Extending a booking respects the booking status defined as **Committed** in the booking setup metadata.</span></span>
- <span data-ttu-id="9473a-122">Брондаудың жарамды күйі көрсетілмеген кезде, қате туралы хабарлама дұрыс локализацияланбаған.</span><span class="sxs-lookup"><span data-stu-id="9473a-122">When a valid booking status isn't specified, the error message is not correctly localized.</span></span>

<span data-ttu-id="9473a-123">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="9473a-123">**Project Management**</span></span>

<span data-ttu-id="9473a-124">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="9473a-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="9473a-125">Жобаларды бір валютада жасау мүмкін емес және оған басқа валютада тиісті тапсырмалар кіреді.</span><span class="sxs-lookup"><span data-stu-id="9473a-125">Projects can't be created in one currency and include related tasks in another currency.</span></span>

<span data-ttu-id="9473a-126">**Сатылым**</span><span class="sxs-lookup"><span data-stu-id="9473a-126">**Sales**</span></span>

<span data-ttu-id="9473a-127">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="9473a-127">The following issues have been fixed:</span></span>

- <span data-ttu-id="9473a-128">Бағатізбе көшірілген кезде бағалар жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="9473a-128">When a price list is copied, prices aren't updated.</span></span>
- <span data-ttu-id="9473a-129">Баға мәліметтерінің шыққан жеріне сәйкес мәні болса, баға ұсыныстарын "ұтқан" ретінде жабу сәтсіз аяқталды.</span><span class="sxs-lookup"><span data-stu-id="9473a-129">Closing a quote as won fails when the cost detail has a value for origin.</span></span>
- <span data-ttu-id="9473a-130">**Жоба тапсырмасы** нысанында **Болжалды құны** атауы **Жоспарланған құны (негізгі)** атауына өзгертілді.</span><span class="sxs-lookup"><span data-stu-id="9473a-130">On the **Project Task** entity, **Estimated Cost** has been renamed to **Planned Cost (Base)**.</span></span>
- <span data-ttu-id="9473a-131">Жарамсыз сілтеме ерекшеліктері шот-фактуралар жасалған немесе жойылған кезде жасалады.</span><span class="sxs-lookup"><span data-stu-id="9473a-131">A null reference exception is generated when invoices are created or deleted.</span></span>
