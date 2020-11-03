---
title: Project Service Automation бағдарламасының 22 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 22-жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 07/28/2020
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
ms.openlocfilehash: badd87a276d68d9959e9cca4220daf61ed570638
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079608"
---
# <a name="project-service-automation-update-release-22-v3"></a><span data-ttu-id="b9e9e-103">Project Service Automation 22 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="b9e9e-103">Project Service Automation Update Release 22, V3</span></span>

<span data-ttu-id="b9e9e-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b9e9e-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b9e9e-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b9e9e-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="b9e9e-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b9e9e-109">Бұл бөлімде Project Service Automation бағдарламасының 22-жаңарту шығарылымының 3 нұсқасындағы жаңа немесе өзгертілен мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 22.</span></span> <span data-ttu-id="b9e9e-110">Бұл нұсқаның V 3.10.33.48 құрастыру нөмірі бар, сондай-ақ 2020 жылдыңң маусым айында өзіндік жаңарту арқылы жалпы түрде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-110">This version has a build number of V 3.10.33.48 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-22"></a><span data-ttu-id="b9e9e-111">22-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="b9e9e-111">Update Release 22</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b9e9e-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="b9e9e-112">Bug fixes</span></span>



<span data-ttu-id="b9e9e-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="b9e9e-113">**Time and Expense**</span></span>

<span data-ttu-id="b9e9e-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="b9e9e-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="b9e9e-115">**Уақыт жазбалары** импортталғаннан кейін уақыт жазбалары кестесіне автоматты түрде қосылмайды.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-115">**Time entries** are not automatically added in the Time entries schedule after import.</span></span>
- <span data-ttu-id="b9e9e-116">**Уақытты жазбасы** тор күнді таңдау құралы пайдаланушының аймақтық параметрлерін танымайды.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-116">The **Time Entry** grid date picker does not recognize a user's regional settings.</span></span>

<span data-ttu-id="b9e9e-117">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="b9e9e-117">**Resource Management**</span></span>

<span data-ttu-id="b9e9e-118">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="b9e9e-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="b9e9e-119">Қолмен басқару режимде **Ресурсты тағайындау** контурларына енгізілген өзгерістер **Ресурстарға қойылатын талаптарды** жасау кезінде танылмайды.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-119">In manual mode, changes to **Resource Assignment** contours are not recognized when generating **Resource Requirements**.</span></span>
- <span data-ttu-id="b9e9e-120">**Ресурстар сұраулары** реттелетін сұрау күйлерін қолдамайды.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-120">**Resource Requests** do not support custom request statuses.</span></span>

<span data-ttu-id="b9e9e-121">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="b9e9e-121">**Project Management**</span></span>

<span data-ttu-id="b9e9e-122">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="b9e9e-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="b9e9e-123">EstimateGridControl түймесін екі рет басқанда голландиялық форматтағы сандар дұрыс талданбайды.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-123">Using double-click on EstimateGridControl will not correctly parse Dutch format numbers.</span></span>
- <span data-ttu-id="b9e9e-124">Тағайындалған сағаттар тағайындаулар Microsoft Project жұмыс үстелінің клиенттік қондырмасы арқылы өзгертілгенде дұрыс жаңартылмайды.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-124">Assigned hours do not update correctly when assignments are changed using the Microsoft Project desktop client add-in.</span></span>
- <span data-ttu-id="b9e9e-125">Жобаны бақылау және бағалау торлары келісімшарт валютасы тұтынушы валютасынан өзгеше болған кезде сатылымның валюталық кодын дұрыс көрсетпейді және ұйым валюталық белгілердің орнына валюталық кодтарды көрсететін етіп конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-125">Project Tracking and Estimates grids display incorrect sales currency code when contract currency is different than customer currency and organization is configured to display currency codes instead of currency symbols.</span></span>
- <span data-ttu-id="b9e9e-126">Топ мүшесінің аяқтау күні, егер жұмыс кестесі тәулігіне 24 сағат болса, бір күнді қосады.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-126">A Team member's finish date will add one day if the work hour schedule is 24-hours per day.</span></span>
- <span data-ttu-id="b9e9e-127">Жоба кестесінде тапсырмаға транзакция санатын қосу автоматты түрде сақтауға әкелмейді.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-127">On the Project Schedule, adding a Transaction Category to a task does not trigger auto save.</span></span>
- <span data-ttu-id="b9e9e-128">Жоба үлгісіне топ мүшесін қосу кезінде келесі қате пайда болады: "Ресурстар талаптарын жоба үлгілерімен байланыстыру мүмкін емес".</span><span class="sxs-lookup"><span data-stu-id="b9e9e-128">The following error is displayed when adding a team member to the Project Template: "Resource requirements cannot be associated with project templates".</span></span> 
- <span data-ttu-id="b9e9e-129">"msdyn.Approval.CanApproveOrReject" таспа ережесінің сценарийі күту уақыты қатесін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-129">Ribbon rule script "msdyn.Approval.CanApproveOrReject" displays a timeout error.</span></span>

<span data-ttu-id="b9e9e-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="b9e9e-130">**Sales**</span></span>

<span data-ttu-id="b9e9e-131">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="b9e9e-131">The following issues have been fixed:</span></span>

- <span data-ttu-id="b9e9e-132">'Жаңа баға ұсыну жобасының бағатізбесі' пішіні/нысанында бағатізбені іздеуде шығын тізбесі таңдалған кезде қате туралы хабарлама көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-132">Validation error message not displayed when a Cost Price List is selected in Price List lookup on 'New Quote Project Price List' form/entity.</span></span>
- <span data-ttu-id="b9e9e-133">Баға ұсынысын ұтқан ретінде жапқанда баға ұсынысына тіркелген BPF соңғы сатыда болса, ол жасалған келісім-шартқа өтпейді.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-133">Closing the quote as won does not navigate to the created contract if a BPF attached to the quote is in the final stage.</span></span>
- <span data-ttu-id="b9e9e-134">**Шот ұсынылмаған сатылымын** кері бағыттау уақыт жазбасын қайтарып алу кезінде бастапқы құнға байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-134">Reversing **Unbilled Sales** is linked to original cost when a time entry is recalled.</span></span>
- <span data-ttu-id="b9e9e-135">**Растау** түймесін басқаннан кейін, есеп-шот күйі жаңартылмаса **Расталған** күйіне өзгермейді.</span><span class="sxs-lookup"><span data-stu-id="b9e9e-135">After selecting the **Confirm** button, the invoice status doesn't change to **Confirmed** unless the invoice is refreshed.</span></span>