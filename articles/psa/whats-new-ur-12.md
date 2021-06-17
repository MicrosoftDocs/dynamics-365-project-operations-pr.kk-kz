---
title: Project Service Automation бағдарламасының 12 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 12-жаңарту шығарылымының 3 нұсқасындағы жаңалықтар туралы ақпарат беріледі.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: f29eaf7c471104ad3e319d8f4e1cbc70e44fc1ca
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000353"
---
# <a name="project-service-automation-update-release-12-v3"></a><span data-ttu-id="fbc42-103">Project Service Automation 12 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="fbc42-103">Project Service Automation Update Release 12, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="fbc42-104">Dynamics 365 Project Service Automation (PSA) бағдарламасының ең соңғы жаңартуын қуана хабарлаймыз.</span><span class="sxs-lookup"><span data-stu-id="fbc42-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="fbc42-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="fbc42-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="fbc42-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="fbc42-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="fbc42-107">Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына кіріп, жаңартуды орнату үшін шешімдер бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="fbc42-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="fbc42-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="fbc42-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="fbc42-109">Бұл бөлімде Project Service Automation бағдарламасының 12-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="fbc42-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 12.</span></span> <span data-ttu-id="fbc42-110">Бұл нұсқа V3.10.2.34 құрылым нөміріне ие және әдетте 2019 жылдың қазан айында шыққан өзін-өзі жаңарту мүмкіндігі арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="fbc42-110">This version has a build number of V3.10.2.34 and is generally available through a self-update in October 2019.</span></span>

## <a name="update-release-12"></a><span data-ttu-id="fbc42-111">12-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="fbc42-111">Update Release 12</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="fbc42-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="fbc42-112">Bug fixes</span></span>

- <span data-ttu-id="fbc42-113">Уақыт және шығыс</span><span class="sxs-lookup"><span data-stu-id="fbc42-113">Time and Expense</span></span>

    - <span data-ttu-id="fbc42-114">Түзетілді: уақытты енгізу қатесі туралы хабарлама өзектірек контекспен жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="fbc42-114">Fixed: Time entry error messaging has been updated with more relevant context.</span></span>
    - <span data-ttu-id="fbc42-115">Түзетілді: уақыт жазбасы торы және кесте қажет болған жағдайда тік жылжыту жолағын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="fbc42-115">Fixed: Time entry grid and schedule correctly displays the vertical scrollbar when required.</span></span>
    - <span data-ttu-id="fbc42-116">Түзетілді: жіберілген шығыс пен уақыт жазбаларын мақұлдауға болады.</span><span class="sxs-lookup"><span data-stu-id="fbc42-116">Fixed: Submitted expense and time entries can be approved.</span></span>
    - <span data-ttu-id="fbc42-117">Түзетілді: "Мақұлдаудан бас тарту әрекетін растау" диалогтік хабары мақұлдау күйін көрсету үшін **Расталған** күйінен **Жіберілді** күйіне түзетілді.</span><span class="sxs-lookup"><span data-stu-id="fbc42-117">Fixed: Cancel approval confirmation dialog message has been corrected to reflect the status of the approval when changed from **Approved** to **Submitted**.</span></span>
    - <span data-ttu-id="fbc42-118">Түзетілді: **Бағасы**, **Бөлім** және **Саны** өрістері енді ол мақұлданғаннан кейін "Шығыс" жазбасында құлыпталған.</span><span class="sxs-lookup"><span data-stu-id="fbc42-118">Fixed: **Price**, **Unit**, and **Quantity** fields are now locked on the Expense record after it is has been approved.</span></span>

- <span data-ttu-id="fbc42-119">Жоба басқармасы</span><span class="sxs-lookup"><span data-stu-id="fbc42-119">Project Management</span></span>

    - <span data-ttu-id="fbc42-120">Түзетілді: **Топ мүшесі** негізгі пішініндегі **Жаңа** әрекеті алынып тасталды.</span><span class="sxs-lookup"><span data-stu-id="fbc42-120">Fixed: **New** action on **Team member** main form has been removed.</span></span>
    - <span data-ttu-id="fbc42-121">Түзетілді: ресурс тағайындаулары қате дөңгелектеу қателерін есепке алу үшін жаңартылды, бұл тапсырманың аяқталу күнінің ауысуына әкеледі.</span><span class="sxs-lookup"><span data-stu-id="fbc42-121">Fixed: Resource assignments have been updated to account for inaccurate rounding errors, which lead to a shift in a task’s end date.</span></span>
    - <span data-ttu-id="fbc42-122">Түзетілді: тапсырмалар торында серверге қатысты қателер пайдаланушыға жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="fbc42-122">Fixed: In the task grid, relevant server-side errors will be surfaced to the user.</span></span>
    - <span data-ttu-id="fbc42-123">Түзетілді: енді топ мүшесінің атауы лауазым атауының орнына адамды таңдау құралында көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fbc42-123">Fixed: The team member’s name now renders in the task people picker instead of the position name.</span></span>

- <span data-ttu-id="fbc42-124">Ресурсты басқару</span><span class="sxs-lookup"><span data-stu-id="fbc42-124">Resource Management</span></span>

    - <span data-ttu-id="fbc42-125">Түзетілді: үлгіден жасалған жобаларға арналған ресурс талабы туралы мәліметтер енді жобаның күнтізбесін қолданады.</span><span class="sxs-lookup"><span data-stu-id="fbc42-125">Fixed: Resource requirement details for projects created from a template now use the project calendar.</span></span>
    - <span data-ttu-id="fbc42-126">Түзетілді: дағдылар мен құзыреттер енді рөлдің басты деректерінен бастап осы рөл үшін жасалған ресурс талабына дейін әдепкі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="fbc42-126">Fixed: Skills and competencies now default from role master data to the resource requirement created for that role.</span></span>

- <span data-ttu-id="fbc42-127">Sales</span><span class="sxs-lookup"><span data-stu-id="fbc42-127">Sales</span></span>

    - <span data-ttu-id="fbc42-128">Түзетілді: **Негізгі келісім-шарт** формасында табылған көшірме нысан идентификаторлары.</span><span class="sxs-lookup"><span data-stu-id="fbc42-128">Fixed: Duplicate object IDs found on the **Contract main** form.</span></span>
    - <span data-ttu-id="fbc42-129">Түзетілді: логика **Баға ұсыну талдауы** қойыншасы метадеректер параметрлерін көрсетіп көрінетіндей жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="fbc42-129">Fixed: Logic has been updated to make the **Quote Analysis** tab visible so that it displays the metadata setup of the tab.</span></span>
    - <span data-ttu-id="fbc42-130">Түзетілді: нақты жазбадағы есеп беру күні бекітілген күннен емес, уақыт/шығыстың енгізілген күнінен басталады.</span><span class="sxs-lookup"><span data-stu-id="fbc42-130">Fixed: Accounting date on the actual record now comes from the date of the time/expense entry date and not the date of the approval.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]