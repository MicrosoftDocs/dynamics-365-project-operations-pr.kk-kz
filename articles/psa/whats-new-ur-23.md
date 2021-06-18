---
title: Project Service Automation бағдарламасының 23 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 23-жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: adf893a0627ae59f2132bb46686110dafda01d3d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006473"
---
# <a name="project-service-automation-update-release-23-v3"></a><span data-ttu-id="af21e-103">Project Service Automation 23-жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="af21e-103">Project Service Automation Update Release 23, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="af21e-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="af21e-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="af21e-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="af21e-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="af21e-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="af21e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="af21e-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="af21e-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="af21e-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="af21e-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="af21e-109">Бұл бөлімде Project Service Automation бағдарламасының 23-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="af21e-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 23.</span></span> <span data-ttu-id="af21e-110">Бұл нұсқада V 3.10.34.30 құрылым нөмірі бар және әдетте 2020 жылдың тамыз айында өзін-өзі жаңарту арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="af21e-110">This version has a build number of V 3.10.34.30 and is generally available through a self-update in August 2020.</span></span>

## <a name="update-release-23"></a><span data-ttu-id="af21e-111">23-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="af21e-111">Update Release 23</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="af21e-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="af21e-112">Bug fixes</span></span>

<span data-ttu-id="af21e-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="af21e-113">**Time and Expense**</span></span>

<span data-ttu-id="af21e-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="af21e-114">The following issues have been fixed:</span></span>
- <span data-ttu-id="af21e-115">Мәнді ерекшелікті қамтамасыз ету үшін **Жоба тобының мүшесін жою** терезесінде шеткі жағдайды басқарыңыз.</span><span class="sxs-lookup"><span data-stu-id="af21e-115">Handle edge case in **Project Team Member Delete** to provide a meaningful exception.</span></span>
- <span data-ttu-id="af21e-116">Тағайындауды импорттау бос жою экранына әкеледі.</span><span class="sxs-lookup"><span data-stu-id="af21e-116">Assignment import results in a blank remove screen.</span></span>

<span data-ttu-id="af21e-117">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="af21e-117">**Resource Management**</span></span>

<span data-ttu-id="af21e-118">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="af21e-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="af21e-119">**Ресурстарды пайдалану торының ресурстық картасы** уақыт шкаласы бес күннен асқанда дұрыс емес деректерді көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="af21e-119">The **Resource utilization grid resource card** shows incorrect data when the time scale is more than five days.</span></span>
- <span data-ttu-id="af21e-120">Тұтынушылар брондауға болатын ресурсты жасаған кезде, қосылатын модуль ресурсты Microsoft Office 365 тобына автоматты түрде қоса алмайды.</span><span class="sxs-lookup"><span data-stu-id="af21e-120">When customers create a bookable resource, the plug-in intermittently fails to automatically add the resource to a Microsoft Office 365 group.</span></span>
- <span data-ttu-id="af21e-121">**Салыстырып тексеру** көрінісі қолмен реттелетін контурларды **Апта** немесе **Ай** көрінісінде дұрыс көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="af21e-121">**Reconciliation** view displays manual contours incorrectly in the **Week** or **Month** view.</span></span>

<span data-ttu-id="af21e-122">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="af21e-122">**Project Management**</span></span>

<span data-ttu-id="af21e-123">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="af21e-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="af21e-124">**Пайдаланушы параметрлеріне арналған RetrieveMultiple** нысандарының шамадан тыс саны жобаны мақұлдау және басқа операциялар үшін өнімділіктің нашарлауын тудырады.</span><span class="sxs-lookup"><span data-stu-id="af21e-124">An excessive number of **RetrieveMultiple for usersettings** entities are causing degraded performance for project approvals and other operations.</span></span>
- <span data-ttu-id="af21e-125">**Тапсырманы жоспарлау** торының ресурсын іздеу жоба тобынан тек бес топ мүшесін көрсетумен шектеледі.</span><span class="sxs-lookup"><span data-stu-id="af21e-125">The **Task Planning** grid resource lookup is limited to only show up to five team members from the project team.</span></span> 
- <span data-ttu-id="af21e-126">**Тапсырманы жоспарлау** торының ресурсын іздеу белсенді емес ресурстарды сүзгіден өткізбейді.</span><span class="sxs-lookup"><span data-stu-id="af21e-126">The **Task Planning** grid resource lookup does not filter inactive resources.</span></span>
- <span data-ttu-id="af21e-127">Қолмен орындау режимі жобаны жоспарындағы жұмыс декомпозициясының құрылымында күткендей жұмыс істемейді.</span><span class="sxs-lookup"><span data-stu-id="af21e-127">Manual mode is not working as expected in the project planning work breakdown structure.</span></span>
- <span data-ttu-id="af21e-128">**Тапсырманы жоспарлау** торы **Белсенді емес транзакция санаттарын** көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="af21e-128">The **Task Planning** grid shows **Inactive Transaction Categories**.</span></span>
- <span data-ttu-id="af21e-129">**Ресурсты тағайындау** торы тапсырма бірнеше тағайындауға ие болған тор дұрыс емес дөңгелектенеді.</span><span class="sxs-lookup"><span data-stu-id="af21e-129">The **Resource Assignment** grid rounds incorrectly when a task has multiple assignments.</span></span>
- <span data-ttu-id="af21e-130">Дөңгелектеу мәндері жоспарланған құн мен бір тапсырмаға арналған нақты құн арасында ерекшеленеді.</span><span class="sxs-lookup"><span data-stu-id="af21e-130">Rounding values are different between planned cost and actual cost for a single task.</span></span>

<span data-ttu-id="af21e-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="af21e-131">**Sales**</span></span>

<span data-ttu-id="af21e-132">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="af21e-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="af21e-133">**Барлық транзакция санаттарын алу** пәрменін екі рет шерту арқылы бірнеше жолдар жасалады.</span><span class="sxs-lookup"><span data-stu-id="af21e-133">**Fetch All Transaction Categories** double-click creates multiple lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]