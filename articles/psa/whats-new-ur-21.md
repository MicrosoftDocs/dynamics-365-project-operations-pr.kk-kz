---
title: Project Service Automation бағдарламасының 21-жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 21-жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: e8a15d5f723da528640c62c1892bac0d801c2bee
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079611"
---
# <a name="project-service-automation-update-release-21-v3"></a><span data-ttu-id="4aea3-103">Project Service Automation 21 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="4aea3-103">Project Service Automation Update Release 21, V3</span></span>

<span data-ttu-id="4aea3-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="4aea3-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="4aea3-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="4aea3-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="4aea3-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="4aea3-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="4aea3-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="4aea3-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="4aea3-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="4aea3-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="4aea3-109">Бұл бөлімде Project Service Automation бағдарламасының 21-жаңарту шығарылымының 3 нұсқасындағы жаңа немесе өзгертілен мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="4aea3-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 21.</span></span> <span data-ttu-id="4aea3-110">Бұл нұсқаның V 3.10.32.50 құрастыру нөмірі бар, сондай-ақ 2020 жылдыңң маусым айында өзіндік жаңарту арқылы жалпы түрде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="4aea3-110">This version has a build number of V 3.10.32.50 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-21"></a><span data-ttu-id="4aea3-111">21-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="4aea3-111">Update Release 21</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="4aea3-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="4aea3-112">Bug fixes</span></span>

<span data-ttu-id="4aea3-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="4aea3-113">**Time and Expense**</span></span>

<span data-ttu-id="4aea3-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="4aea3-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="4aea3-115">**Уақыт жазбасы торын басқару элементін** бақылау тақталарында орналастыру кезінде тор бақылау тақтасындағы тор контейнерінің толық енін пайдаланбайды.</span><span class="sxs-lookup"><span data-stu-id="4aea3-115">When hosting the **Time Entry Grid Control** in Dashboards, the grid does not utilize the full width of the dashboard grid container.</span></span>
- <span data-ttu-id="4aea3-116">Нақты уақыт белдеулері үшін **Уақытты жазбасы** торды басқару элементінде жазбалар көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="4aea3-116">For specific time zones, the **Time Entry** grid control does not display records.</span></span>
- <span data-ttu-id="4aea3-117">Сағат 21:00-ден кейінгі уақыт жазбалары дұрыс емес күні пайда болады.</span><span class="sxs-lookup"><span data-stu-id="4aea3-117">Time entries that are after 9:00 PM appear on the wrong day.</span></span>
- <span data-ttu-id="4aea3-118">Егер **Шығыс түбіртегі қажет** шығыс санатының мәні жоқ болса, пайдаланушылар шығыстарды жібере алмайды.</span><span class="sxs-lookup"><span data-stu-id="4aea3-118">Users are unable to submit expenses if the expense category, **Expense receipt required** has no value.</span></span>

<span data-ttu-id="4aea3-119">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="4aea3-119">**Resource Management**</span></span>

<span data-ttu-id="4aea3-120">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="4aea3-120">The following issues have been fixed:</span></span>

- <span data-ttu-id="4aea3-121">**Біріктіру** көрінісінде белсенді емес тапсырыстар көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="4aea3-121">Inactive bookings are displayed in the **Reconciliation** view.</span></span>
- <span data-ttu-id="4aea3-122">Жалпы ресурстардың орындалуы жарамды тапсырыс беру күйінің бар екеніне көз жеткізу үшін тексеруден өтпеді.</span><span class="sxs-lookup"><span data-stu-id="4aea3-122">Generic resource fulfillment was missing validation to ensure that a valid booking status exists.</span></span>

<span data-ttu-id="4aea3-123">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="4aea3-123">**Project Management**</span></span>

<span data-ttu-id="4aea3-124">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="4aea3-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="4aea3-125">**Жоба** пішін торлары ( **Ресурсты тағайындау** , **Тапсырма** , **Біріктіру** көрінісі, **Шығын болжамдары** ) жоба белсенді болмаса да, өңделетін болады.</span><span class="sxs-lookup"><span data-stu-id="4aea3-125">The **Project** form grids ( **Resource Assignment** , **Task** , **Reconciliation** view, **Expense Estimates** ) remain editable even when a project is not active.</span></span>
- <span data-ttu-id="4aea3-126">Көшірме тұтынушыларды расталған жоба келісімшарттарымен байланысқан тұтынушылармен біріктіруге болмайды.</span><span class="sxs-lookup"><span data-stu-id="4aea3-126">Duplicate customers can't be merged with customers that are linked to confirmed project contracts.</span></span>
- <span data-ttu-id="4aea3-127">Жарамды күнтізбесі жоқ ресурс қосылған кезде, жүйе пайдаланушыға қатысты қате туралы хабарламаны қайтармайды.</span><span class="sxs-lookup"><span data-stu-id="4aea3-127">When a resource who does not have a valid calendar is added, the system does not return a user friendly-error message.</span></span>
- <span data-ttu-id="4aea3-128">Тапсырмалар торындағы **Тапсырма қосу** түймесі жоба **Microsoft Project қондырмасына** байланысқан кезде іске қосылады.</span><span class="sxs-lookup"><span data-stu-id="4aea3-128">The **Add Task** button on the task grid is enabled when the project is linked to **Microsoft Project add-in**.</span></span>
- <span data-ttu-id="4aea3-129">Санаты бар тапсырма шығыны белгіленген рөлі бар ресурсқа тағайындалған кезде талпыныс өрлейтін болады.</span><span class="sxs-lookup"><span data-stu-id="4aea3-129">Effort grows uncontrollably when a task with a category is assigned to a resource with a role for which there is a cost price defined.</span></span>

<span data-ttu-id="4aea3-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="4aea3-130">**Sales**</span></span>

<span data-ttu-id="4aea3-131">Мына жақсартуларды енгізілді:</span><span class="sxs-lookup"><span data-stu-id="4aea3-131">The following enhancements have been made:</span></span>

- <span data-ttu-id="4aea3-132">**Есеп-шот жиілігі** және **Шот ұсынуды бастау** параметрлері **Есеп-шот кестесі** қойыншасына көшірілді.</span><span class="sxs-lookup"><span data-stu-id="4aea3-132">**Invoice Frequency** and **Billing Start** have been moved to the **Invoice Schedule** tab.</span></span>

<span data-ttu-id="4aea3-133">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="4aea3-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="4aea3-134">**Рөл** параметрінің жалпы сатылым бағасы нөлге (0) тең болмаса да **Санат** үшін **Жалпы сатылым бағасы** нөлге тең.</span><span class="sxs-lookup"><span data-stu-id="4aea3-134">**Total Sales Price** is zero (0) for **Category** even though **Role** has a total sales price that is not zero.</span></span>
- <span data-ttu-id="4aea3-135">Басқа теңшелген процесс қосымша өрісті жаңартып жатқанда тұтынушылар **Есеп-шот күйі** өрісін **Есеп-шотқа дайын** мәніне өзгерте алмайды.</span><span class="sxs-lookup"><span data-stu-id="4aea3-135">Customers can't change the value of the **Invoice Status** field to **Ready for invoicing** when another customized process is updating an additional field.</span></span>
- <span data-ttu-id="4aea3-136">**Есеп-шот жолдарын жаңарту** түймесі бірнеше рет қайталанып таңдалса бірнеше көшірме жолдар жасай алады.</span><span class="sxs-lookup"><span data-stu-id="4aea3-136">The **Refresh Invoice Lines** button can create multiple duplicated lines if it is repeatedly selected.</span></span>
- <span data-ttu-id="4aea3-137">**Бағаларды жаңарту** түймесі **Жедел қарау** пішініндегі **Рөл бағалары** ішкі торында жұмыс істемейді.</span><span class="sxs-lookup"><span data-stu-id="4aea3-137">The **Update Prices** button doesn't work on the **Role Prices** sub-grid in the **Quick View** form.</span></span>
- <span data-ttu-id="4aea3-138">**Сату бағаларының шешімі** логикасы уақыт белдеулерін дұрыс қолданбайды, нәтижесінде бағатізбелері дұрыс таңдалмайды.</span><span class="sxs-lookup"><span data-stu-id="4aea3-138">The **Sales Price List Resolution** logic improperly handles time zones, resulting in the incorrect selection of price lists.</span></span>
- <span data-ttu-id="4aea3-139">Жобаның **Нақты жалпы құны** бір реттік жазбаны мақұлдағаннан кейін аз мөлшерде азайтылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="4aea3-139">A project’s **Total Actual Cost** can be off by a fractional amount after a single time entry is approved.</span></span>
- <span data-ttu-id="4aea3-140">Егер **Шығарып алынған рөл бағасының** **'Бастапқы бірлік'** және **'Негізгі бірліктегі баға'** өрістерінде мән болмаса, **Баға шешімі** логикасында түсінікті қате туралы хабар пайда болмайды.</span><span class="sxs-lookup"><span data-stu-id="4aea3-140">The **Price Resolution** logic does not provide a user-friendly error message if **Retrieved RolePrice** doesn't have values in **'Primary Unit'** and **'Price In Primary Unit'** fields.</span></span>