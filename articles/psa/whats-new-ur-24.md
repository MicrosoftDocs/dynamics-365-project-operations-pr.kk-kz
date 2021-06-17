---
title: Project Service Automation бағдарламасының 24 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 24 жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c95a9dcada4fbf6c462df29d450aaafab4e73aa5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000263"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="522ad-103">Project Service Automation 24 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="522ad-103">Project Service Automation Update Release 24, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="522ad-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="522ad-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="522ad-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="522ad-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="522ad-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="522ad-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="522ad-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="522ad-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="522ad-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="522ad-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="522ad-109">Бұл бөлімде Project Service Automation бағдарламасының 24-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="522ad-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="522ad-110">Бұл нұсқада V 3.10.42.43 құрылым нөмірі бар және әдетте 2020 жылдың қазан айында өзін-өзі жаңарту арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="522ad-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="522ad-111">24-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="522ad-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="522ad-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="522ad-112">Bug fixes</span></span>

<span data-ttu-id="522ad-113">**Sales**</span><span class="sxs-lookup"><span data-stu-id="522ad-113">**Sales**</span></span>

<span data-ttu-id="522ad-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="522ad-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="522ad-115">Өнімдердің әдепкі бағатізбесін орнату кезіндегі мәселе.</span><span class="sxs-lookup"><span data-stu-id="522ad-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="522ad-116">Баға ұсыну ұтысы енгізілген бағатізбесі мен рөлдік баға жазбаларының көшірмесіне байланысты баяу жүреді.</span><span class="sxs-lookup"><span data-stu-id="522ad-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="522ad-117">**Жоба келісім-шарты/сату орталығы** > **Өнім жолы элементі/Тапсырыс жолының саны** автоматты түрде ең жақын бүтін санға дейін дөңгелектенеді.</span><span class="sxs-lookup"><span data-stu-id="522ad-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="522ad-118">Бағатізбелерді оқу кезінде жүйенің артықшылықтарына қол жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="522ad-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="522ad-119">Тұтынушының мекенжай өрістерін, **address1_freighttermscode** және **address1_shippingmethodcode**, Баға ұсыну/ Тапсырыс өрісіне көшіріңіз.</span><span class="sxs-lookup"><span data-stu-id="522ad-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="522ad-120">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="522ad-120">**Time and Expense**</span></span>

<span data-ttu-id="522ad-121">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="522ad-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="522ad-122">**Уақыт жазбасының торы** **Тек күн** уақыт әрекетін қолдамайды.</span><span class="sxs-lookup"><span data-stu-id="522ad-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="522ad-123">**Уақыт жазбасы** автоматты түрде жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="522ad-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="522ad-124">Қолмен жаңарту қажет.</span><span class="sxs-lookup"><span data-stu-id="522ad-124">A manual refresh is required.</span></span>
- <span data-ttu-id="522ad-125">Ресурс тағайындауларында үзіліс болған кезде (0 сағат) уақыттағы жазбаларды тапсырмадан импорттау мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="522ad-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="522ad-126">Уақыт жазбасын жасаған кезде, басталу уақытын **msdyn_date** деп белгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="522ad-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="522ad-127">Уақыт жазбасы үшін жаппай өңдеуді қайта қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="522ad-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="522ad-128">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="522ad-128">**Resource Management**</span></span>

<span data-ttu-id="522ad-129">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="522ad-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="522ad-130">Тәулік аралық брондаудың күйін талапсыз жаңартуға тырысу сілтеменің бос болуына әкеледі.</span><span class="sxs-lookup"><span data-stu-id="522ad-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="522ad-131">**Салыстырып тексеру көрінісі** жүктеу кезінде қате орын алды.</span><span class="sxs-lookup"><span data-stu-id="522ad-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="522ad-132">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="522ad-132">**Project Management**</span></span>

<span data-ttu-id="522ad-133">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="522ad-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="522ad-134">**Жоба кестесі** бөлімінде, **Қолмен реттелетін** күйден **Автоматты** күйге ауысқан кезде, автоматты түрде сақтау орындалмайды.</span><span class="sxs-lookup"><span data-stu-id="522ad-134">In the **Project Schedule**, when changing from **Manual** to **Auto**, auto save is not completing.</span></span>
- <span data-ttu-id="522ad-135">Шығын құны **Жобаны бақылау торы** ауытқуына қарай есептелмейді.</span><span class="sxs-lookup"><span data-stu-id="522ad-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="522ad-136">Жүктеме кезіндегі **Болжамдар тегі** бағандары үшін сәйкес емес әрекет **Уақыт кезеңі** түрінің өзгеруіне қарсы.</span><span class="sxs-lookup"><span data-stu-id="522ad-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="522ad-137">Жобаның нақты құны **Нақты көрсеткіштер** қорытындыларын көрсетпеуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="522ad-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="522ad-138">**Қысқаша мазмұны** қойыншасындағы **Болжалды аяқталу күні** **WBS кестесі** сәйкес келмейді.</span><span class="sxs-lookup"><span data-stu-id="522ad-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="522ad-139">Тапсырманы шығару кезінде **Нақты сағаттарды жаңарту** дұрыс жұмыс істемейді.</span><span class="sxs-lookup"><span data-stu-id="522ad-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="522ad-140">**BU** түбірінен тыс жоба менеджері жоба жасай алмайды.</span><span class="sxs-lookup"><span data-stu-id="522ad-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="522ad-141">**Шығыс болжамдары** тармағындағы тапсырмаға немесе санатқа енгізілген өзгерістер сақталмайды.</span><span class="sxs-lookup"><span data-stu-id="522ad-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="522ad-142">**Келісім-шарт көшірмесі** есеп-шот кестелерін және сеанс күйін көшіреді.</span><span class="sxs-lookup"><span data-stu-id="522ad-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="522ad-143">**Нақты көрсеткіштерді жаңарту** түймесі жиынтық тапсырмаларды дұрыс есептемейді.</span><span class="sxs-lookup"><span data-stu-id="522ad-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="522ad-144">Microsoft Project қондырмасы: кез келген топ мүшесінде бос ресурс бірлігі болса, бос сілтеме қатесін түзетіңіз.</span><span class="sxs-lookup"><span data-stu-id="522ad-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]