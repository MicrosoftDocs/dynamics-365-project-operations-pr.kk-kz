---
title: Project Service Automation бағдарламасының 18 жаңарту шығарылымының 3 нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 18 жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
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
ms.openlocfilehash: 1d7ea200531dd24d56a829f879e3a2532a9b38dc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079614"
---
# <a name="project-service-automation-update-release-18-v3"></a><span data-ttu-id="a8c7e-103">Project Service Automation 18 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="a8c7e-103">Project Service Automation Update Release 18, V3</span></span>

<span data-ttu-id="a8c7e-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a8c7e-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a8c7e-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a8c7e-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="a8c7e-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a8c7e-109">Бұл бөлімде Project Service Automation бағдарламасының 18 жаңарту шығарылымының 3 нұсқасындағы жаңа немесе өзгертілген мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 18.</span></span> <span data-ttu-id="a8c7e-110">Бұл нұсқа V3.10.8.12 жиынтық нөміріне ие және әдетте өзін-өзі жаңарту арқылы 2020 жылдың сәуірінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-110">This version has a build number of V3.10.8.12 and is generally available through a self-update in April 2020.</span></span>

## <a name="update-release-18"></a><span data-ttu-id="a8c7e-111">18-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="a8c7e-111">Update Release 18</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a8c7e-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="a8c7e-112">Bug fixes</span></span>

<span data-ttu-id="a8c7e-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="a8c7e-113">**Time and Expense**</span></span>

- <span data-ttu-id="a8c7e-114">Түзетілді: **Қайта шақыру** , **Сұрау** және **Мақұлдаудан бас тарту** ағындары түсініксіз қате туралы хабарлары ерекше жағдайларды шығарады.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-114">Fixed: **Recall** , **Request** , and **Cancel Approval** flows throw exceptions with unclear error messages.</span></span>
- <span data-ttu-id="a8c7e-115">Түзетілді: **Мақұлдаудан бас тарту** шығыс үшін сәтсіз болған жағдайда, қатысты ерекшелік қатесі шықпайды.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-115">Fixed: When **Cancel Approval** fails for an expense, a relevant exception error is not thrown.</span></span>
- <span data-ttu-id="a8c7e-116">Түзетілді: қазан айында күндізгі жарықты үнемдеу уақытына (DST) ауысқаннан кейін уақыт жазбасы торы Австралиядағы жұмыс істемейтін күндерді қате өңдейді.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-116">Fixed: The Time Entry grid incorrectly handles non-working days in Australia after the daylight savings time (DST) switch in October.</span></span>
- <span data-ttu-id="a8c7e-117">Түзетілді: қате әдепкі логикасы шығындарды жіберуге жол бермейді.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-117">Fixed: Incorrect defaulting logic prevents submission of expenses.</span></span>
- <span data-ttu-id="a8c7e-118">Түзетілді: уақыт жазбасын мақұлдау сәтсіз болған жағдайда, мақұлдау **Күтілуде** күйінде қалады.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-118">Fixed: When time entry approval fails, the approval remains in a state of **Pending**.</span></span>
- <span data-ttu-id="a8c7e-119">Түзетілді: жаппай мақұлдау кезіндегі SQL қателері (тығырық/күту уақыты).</span><span class="sxs-lookup"><span data-stu-id="a8c7e-119">Fixed: SQL Errors on bulk approvals (deadlock/timeout).</span></span>
- <span data-ttu-id="a8c7e-120">Түзетілді: уақыт жазбаларын мақұлдау кезінде топ мүшелерін жаңартудан туындаған пайдаланушы тәжірибесіндегі маңызды мәселелер.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-120">Fixed: Significant performance issues in the user experience caused by updating team members while approving time entries.</span></span>

<span data-ttu-id="a8c7e-121">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="a8c7e-121">**Project Management**</span></span>

- <span data-ttu-id="a8c7e-122">Түзетілді: уақыт белдеуі хабарландыруы **Біріктіру** көрінісінен **Жоба** негізгі пішініне көшірілді.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-122">Fixed: Time zone notification moved from the **Reconciliation** view to the **Project** main form.</span></span>
- <span data-ttu-id="a8c7e-123">Түзетілді: жаңа жоба пішіні ашылған кезде күнтізбе үлгісі әдепкі бойынша дұрыс орындалмайды.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-123">Fixed: Calendar template is not correctly defaulting when a new project form opens.</span></span>
- <span data-ttu-id="a8c7e-124">Түзетілді: хром негізіндегі шолғыштар үшін пайдаланушылар жоюға болатын алдыңғы тапсырмаларды оңай таңдай алмайды.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-124">Fixed: For chromium-based browsers, users are unable to easily select predecessor tasks to delete.</span></span>
- <span data-ttu-id="a8c7e-125">Түзетілді: **Жобаны бос үлгіден** жасау немесе көшіру байланысты емес тапсырмаларды таңдайды.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-125">Fixed: Creating or copying **Project from Empty template** fetches unrelated assignments.</span></span>
- <span data-ttu-id="a8c7e-126">Түзетілді: нақты жағдайларда тапсырмалар торынан жаңа тағайындау жасау қайталанатын жазбалардың пайда болуына әкеледі.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-126">Fixed: In specific edge cases, creating a new assignment from the task grid results in duplicate records being created.</span></span>
- <span data-ttu-id="a8c7e-127">Түзетілді: қолмен орындау күйінде пайдаланушылар тапсырманың басталу уақытын ағымдағы сақталған күннен кешірек болатындай жаңарта алмайды.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-127">Fixed: In manual mode, users are unable to update task start dates to be later than the current date saved.</span></span>

<span data-ttu-id="a8c7e-128">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="a8c7e-128">**Resource Management**</span></span>

- <span data-ttu-id="a8c7e-129">Түзетілді: **Біріктіру** көрінісінің аралық қорытынды қатары кеңейтілген тапсырыстардан кейін тапсырыстар айырмасын қате есептейді.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-129">Fixed: **Reconciliation** view subtotal row incorrectly calculates bookings variance after extending bookings.</span></span>
- <span data-ttu-id="a8c7e-130">Түзетілді: **Біріктіру** көрінісі тапсырыс беруге болатын ресурста жоба күнтізбесіне сәйкес келмейтін күнтізбе болған жағдайда ресурс тағайындауларын қате көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-130">Fixed: **Reconciliation** view incorrectly displays resource assignments when the bookable resource has a calendar that does not match the project calendar.</span></span>

<span data-ttu-id="a8c7e-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="a8c7e-131">**Sales**</span></span>

- <span data-ttu-id="a8c7e-132">Түзетілді: уақыт жазбалары қайта мақұлданған кезде ( **Мақұлдау > Бас тарту >** қайта мақұлдау) қайталанатын ақысыз нақты мән жасалады.</span><span class="sxs-lookup"><span data-stu-id="a8c7e-132">Fixed: When time entries are re-approved ( **Approve > Cancel >** approve again), a duplicate non-chargeable actual is created.</span></span>
