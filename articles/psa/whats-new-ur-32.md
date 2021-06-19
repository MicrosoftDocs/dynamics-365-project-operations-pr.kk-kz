---
title: Project Service Automation бағдарламасының 32-жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 32-жаңарту шығарылымының 3‑нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 11bf451ef4f24e2301ffde4f86a556a8a4fe30b0
ms.sourcegitcommit: 886102894244887d72e5a6213071e8d8a52c9d48
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/01/2021
ms.locfileid: "6129673"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a><span data-ttu-id="e5599-103">Project Service Automation бағдарламасының 32-жаңарту шығарылымының 3-нұсқасындағы жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="e5599-103">What's new or changed in Project Service Automation Update Release 32, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="e5599-104">Біз Microsoft Dynamics 365 Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="e5599-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="e5599-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="e5599-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="e5599-106">Бұл Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="e5599-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="e5599-107">Осы шығарылымға жаңарту үшін Dynamics 365 онлайн шешімдері бетінің әкімші орталығына кіріп, жаңартуды орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e5599-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="e5599-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="e5599-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="e5599-109">Бұл бөлімде Project Service Automation бағдарламасының 32-жаңарту шығарылымының 3-нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="e5599-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 32.</span></span> <span data-ttu-id="e5599-110">Бұл нұсқада V3.10.53.108 жинақ нөмірі бар және әдетте 2021 жылдың маусымында жеке жаңарту арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="e5599-110">This version has a build number of V3.10.53.108 and is generally available through a self-update in June 2021.</span></span>

## <a name="update-release-32"></a><span data-ttu-id="e5599-111">32-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="e5599-111">Update Release 32</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="e5599-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="e5599-112">Bug fixes</span></span>

#### <a name="general"></a><span data-ttu-id="e5599-113">Жалпы мәліметтер </span><span class="sxs-lookup"><span data-stu-id="e5599-113">General</span></span>

- <span data-ttu-id="e5599-114">Үлкен жаңарту сәтсіз аяқталған кезде, ортақ бағдарламаларға қолжетімділікті қамтамасыз ету үшін тек бағдарламаның негізгі кіру нүктелерін ғана бұғаттау керек.</span><span class="sxs-lookup"><span data-stu-id="e5599-114">When a major upgrade fails, only the main application entry points should be blocked, to ensure that shared entities are still accessible.</span></span>

#### <a name="time-and-expense"></a><span data-ttu-id="e5599-115">Уақыт және шығыс</span><span class="sxs-lookup"><span data-stu-id="e5599-115">Time and Expense</span></span>

<span data-ttu-id="e5599-116">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="e5599-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="e5599-117">**TimeEntriesImportFromResourceAssignment** ресурстарды тағайындау контурының басталу және аяқталу уақытын сақтамайды.</span><span class="sxs-lookup"><span data-stu-id="e5599-117">**TimeEntriesImportFromResourceAssignment** doesn't maintain the start and end times of the resource assignment contour slice.</span></span>
- <span data-ttu-id="e5599-118">**Уақыт жазбасы** торында **Жазбаны ашу** түймешігін таңдаған кезде, сізге басқа нысандарды таңдауға тыйым салынуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e5599-118">When you select **Open Entry** on the **Time Entry** grid, you might be prevented from selecting other forms.</span></span>
- <span data-ttu-id="e5599-119">Уақыт жазбаларына тағайындауларды импорттаған кезде, клиент кодының сұрауы сұраудың сәтсіз болуына әкелетін ұзын URL мекенжайын тудыруы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e5599-119">While you import assignments to time entries, the client code query could generate a long URL that fails the query.</span></span>
- <span data-ttu-id="e5599-120">**Уақыт жазбасы** торында мән ұяшықтан жойылғаннан кейін, фокус торда қалмайды.</span><span class="sxs-lookup"><span data-stu-id="e5599-120">In the **Time Entry** grid, after a value is deleted from a cell, the focus doesn't remain in the grid.</span></span>
- <span data-ttu-id="e5599-121">**Қабылдамау** түймешігі заманауи мақұлдау үшін **Мақұлдауды өңдеу** көрінісінен жойылды.</span><span class="sxs-lookup"><span data-stu-id="e5599-121">The **Reject** button has been removed from the **Processing approvals** view for modern approvals.</span></span>
- <span data-ttu-id="e5599-122">Уақыт жазбасын жаппай мақұлдаудың тұрақтылығы мен өнімділігіне тығырықтар және **Уақыт жазбасы** нысанына қатысты өзгертулерді тиісті түрде өңдемеу әсер етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e5599-122">The stability and performance of time entry bulk approval are affected by deadlocks and a failure to appropriately handle customizations that are related to the **Time Entry** entity.</span></span>

#### <a name="project-planning"></a><span data-ttu-id="e5599-123">Жобаны жоспарлау</span><span class="sxs-lookup"><span data-stu-id="e5599-123">Project Planning</span></span>

- <span data-ttu-id="e5599-124">**Келісімшарт бірлігі** өрісінде нөл мәні бар жобаны жаңартқанда нөлдік сілтеме ерекшелігі жасалады.</span><span class="sxs-lookup"><span data-stu-id="e5599-124">A null reference exception is generated when you update a project that has a null value in the **Contracting Unit** field.</span></span>
- <span data-ttu-id="e5599-125">**Жоба қорытындыларын жаңарту** қалған соманы және жобадағы қалған сатылым көлемін дұрыс есептемейді.</span><span class="sxs-lookup"><span data-stu-id="e5599-125">**Refresh Project Totals** incorrectly calculates the remaining cost and remaining sales on a project.</span></span>
- <span data-ttu-id="e5599-126">Артық баға есептеулері ресурстарды тағайындау контурындағы жаңартуларға байланысты өнімділікке әсер етеді.</span><span class="sxs-lookup"><span data-stu-id="e5599-126">Redundant pricing calculations affect performance that is related to updates on resource assignment contours.</span></span>

#### <a name="resource-management"></a><span data-ttu-id="e5599-127">Ресурсты басқару</span><span class="sxs-lookup"><span data-stu-id="e5599-127">Resource Management</span></span>

<span data-ttu-id="e5599-128">Келесі мәселе түзетілді:</span><span class="sxs-lookup"><span data-stu-id="e5599-128">The following issue has been fixed:</span></span>

- <span data-ttu-id="e5599-129">Тапсырыс беруге болатын ресурстың күнтізбе сыйымдылығы 1-ден көп болған кезде Project Service Automation бағдарламасы сыйымдылықты 0 (нөл) деп қате таниды.</span><span class="sxs-lookup"><span data-stu-id="e5599-129">When a bookable resource's calendar capacity is more than 1, Project Service Automation incorrectly recognizes the capacity as 0 (zero).</span></span> <span data-ttu-id="e5599-130">Сондықтан кесте көрінісінде шексіз цикл пайда болады.</span><span class="sxs-lookup"><span data-stu-id="e5599-130">Therefore, an infinite loop occurs in the schedule view.</span></span>

#### <a name="sales"></a><span data-ttu-id="e5599-131">Сатылым</span><span class="sxs-lookup"><span data-stu-id="e5599-131">Sales</span></span>

<span data-ttu-id="e5599-132">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="e5599-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="e5599-133">Реттелетін транзакция түрі бар журнал жолы жасалған кезде, келесі нөлдік сілтеме ерекшеліктері орын алады: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span><span class="sxs-lookup"><span data-stu-id="e5599-133">When a journal line is created that has a custom transaction type, the following null reference exception occurs: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span></span>
- <span data-ttu-id="e5599-134">Баға ұсыныстары көшірілгенге дейін белсенсіздендірілген рөлдер мен санаттар жаңадан көшірілген баға ұсынысының ақылы рөлдері мен санаттарына қосылмауы керек.</span><span class="sxs-lookup"><span data-stu-id="e5599-134">Roles and categories that are inactivated before a quotation is copied should not be added to chargeable roles and categories of the newly copied quotation.</span></span>
- <span data-ttu-id="e5599-135">Құжат күні мен есеп күні тікелей жоба шот-фактурасында жасалатын шот-фактура жолында берілген басталу күнімен сәйкес келмейді.</span><span class="sxs-lookup"><span data-stu-id="e5599-135">The document date and accounting date aren't aligned with the start date that is provided on an invoice line detail that is created directly on a draft invoice.</span></span>
- <span data-ttu-id="e5599-136">Нөлдік сілтеме ерекшеліктері баға ұсынысы көшірілгенге дейін рөлдер мен санаттарды белсенсіздендіруге байланысты сценарийлерде жасалады.</span><span class="sxs-lookup"><span data-stu-id="e5599-136">Null reference exceptions are generated in scenarios that are related to inactivation of roles and categories before a quotation is copied.</span></span>
- <span data-ttu-id="e5599-137">**Жобалар** бетіндегі **Бағаларды жаңарту** әрекеті шығындар болжамдары мен материал болжамдарын жаңартпайды.</span><span class="sxs-lookup"><span data-stu-id="e5599-137">The **Update Prices** action on the **Projects** page doesn't update expense estimates and material estimates.</span></span>
