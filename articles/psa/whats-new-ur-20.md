---
title: Project Service Automation бағдарламасының 20 жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation 20 жаңарту шығарылымының 3-нұсқасында қолжетімді мүмкіндіктер мен түзетпелер көрсетілген
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: 12edae76dbc6de63d3e2d36058c4092f80ede77d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079609"
---
# <a name="project-service-automation-update-release-20-v3"></a><span data-ttu-id="ed939-103">Project Service Automation 20 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="ed939-103">Project Service Automation Update Release 20, V3</span></span>

<span data-ttu-id="ed939-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="ed939-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="ed939-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="ed939-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="ed939-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="ed939-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="ed939-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="ed939-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="ed939-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="ed939-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="ed939-109">Бұл тақырыпта Project Service Automation 20 жаңарту шығарылымының 3-нұсқасында жаңа немесе өзгертілген мүмкіндіктер мен түзетпелер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="ed939-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 20.</span></span> <span data-ttu-id="ed939-110">Бұл нұсқаның V 3.10.31.37 құрастыру нөмірі бар, сондай-ақ 2020 жылдыңң маусым айында өзіндік жаңарту арқылы жалпы түрде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="ed939-110">This version has a build number of V 3.10.31.37 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-20"></a><span data-ttu-id="ed939-111">20-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="ed939-111">Update Release 20</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="ed939-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="ed939-112">Bug fixes</span></span>

<span data-ttu-id="ed939-113">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="ed939-113">**Project Management**</span></span>

<span data-ttu-id="ed939-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="ed939-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="ed939-115">Сағаттарды қажет ететінтағайындау әдісімен жобалық топ мүшелерін импорттау нәтижесінде көрсетілген сағаттар нөл болған кезде анық емес қате туралы хабар пайда болады.</span><span class="sxs-lookup"><span data-stu-id="ed939-115">Importing project team members with an allocation method that requires hours results in an unclear error message when the specified hours are zero.</span></span>
- <span data-ttu-id="ed939-116">Жоба тапсырмсы үшін **Сипаттама** өрісіне таңбалардың максималды саны енгізілген кезде, пайдаланушыларға дұрыс емес деген қате туралы хабар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="ed939-116">Users receive an incorrect error when the maximum number of characters have been entered into the **Description** field for a project task.</span></span>
- <span data-ttu-id="ed939-117">Пайдаланушының тіл параметрлері жапон тіліне орнатылған кезде, **Microsoft Dynamics 365 Project Service Automation қондырмасын жүктеп алу** беті ағылшын тіліндегі жүктеп алу бетіне бағыттайды.</span><span class="sxs-lookup"><span data-stu-id="ed939-117">The **Microsoft Dynamics 365 Project Service Automation add-in download** page redirects to the English download page when the user’s language settings are set to Japanese.</span></span>
- <span data-ttu-id="ed939-118">Сервер қатесі пайда болған кезде, кейде **Жобалар** пішінінің **Кесте** қойыншасындағы синхрондау белгісі сақталады.</span><span class="sxs-lookup"><span data-stu-id="ed939-118">When a server error occurs, the synchronization label on the **Schedule** tab of the **Projects** form sometimes remains.</span></span>
- <span data-ttu-id="ed939-119">Тапсырма өзгертілген кезде, артық тапсырма жаңартулары серверге жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="ed939-119">Redundant task updates are being sent to the server when a task is modified.</span></span>

<span data-ttu-id="ed939-120">**Sales**</span><span class="sxs-lookup"><span data-stu-id="ed939-120">**Sales**</span></span>

<span data-ttu-id="ed939-121">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="ed939-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="ed939-122">**Келісім-шарт** пішінінде **Есеп-шот жасау** опциясын екі рет басу жалғыз нақты көрсеткіштер жазбасы үшін екі есеп-шотты жасайды.</span><span class="sxs-lookup"><span data-stu-id="ed939-122">On the **Contract** form, double-clicking **Create Invoice** creates two invoices for a single actuals record.</span></span>
- <span data-ttu-id="ed939-123">Internet Explorer 11 браузерінде пайдаланушылар шығыс жазбаларын жасай алмайды.</span><span class="sxs-lookup"><span data-stu-id="ed939-123">In Internet Explorer 11, users are unable to create expense entries.</span></span>
- <span data-ttu-id="ed939-124">Шығын кері мәні мен шот ұсынылмаған сатылым нақты мәндерінің кері мәні өзара байланысты емес.</span><span class="sxs-lookup"><span data-stu-id="ed939-124">Reversal of Cost and reversal of Unbilled Sales Actuals are not linked.</span></span>
- <span data-ttu-id="ed939-125">**Жоба** пішініндегі **Нақты көрсеткіштерді жаңарту** түймешігі **Тапсырманың нақты сағаттары** мәнін жаңартпайды.</span><span class="sxs-lookup"><span data-stu-id="ed939-125">The **Refresh Actuals** button on the **Project** form does not refresh **Task Actual Hours**.</span></span>
- <span data-ttu-id="ed939-126">**PreValidateProjectTeamMemberCreate** қосылатын модулі **msdyn_isgenericresourceprojectscoped** төлсипаты **Жалған** мәніне орнатылған кезде көшірме жалпы тапсырыс берілетін ресурстарды жасай алады.</span><span class="sxs-lookup"><span data-stu-id="ed939-126">The **PreValidateProjectTeamMemberCreate** plug-in can create duplicate generic bookable resources when the attribute **msdyn_isgenericresourceprojectscoped** is set to **False**.</span></span>
- <span data-ttu-id="ed939-127">**Қайта есептеу** әрекеті өнімге негізделген баға ұсыну жолы мәліметтері мен келісім-шарт жолы мәліметтерінің ақылы құнын жояды.</span><span class="sxs-lookup"><span data-stu-id="ed939-127">**Recalculate** clears chargeable costs of product-based quote line details and contract line details.</span></span>
- <span data-ttu-id="ed939-128">Белгілі бір сценарийлерде **PostEstimateLineUpdate** қосылатын модулі бос анықтамалық ерекшелік қатесін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="ed939-128">In specific scenarios, the **PostEstimateLineUpdate** plug-in displays a null teference exception error.</span></span>
- <span data-ttu-id="ed939-129">**Табыстылық талдауының диаграммасы** ішіндегі уақыт фазасының ұзақтығы баға ұсынудың бекітілген баға ұсыну жолы мәліметіндегі шығындардың ұзақтығына сәйкес келмейді.</span><span class="sxs-lookup"><span data-stu-id="ed939-129">Time phase duration on the **Profitability Analysis Chart** does not match duration of the costs in the fixed-price quote line detail of the quote.</span></span>
- <span data-ttu-id="ed939-130">Бірлік пен бірлік тобының мәндері **Келісім-шарт жолы мәліметтері** және **Баға ұсыну жолы мәліметтері** пішіндеріндегі шығыс санаттары үшін әдепкі мән ретінде дұрыс орнатылмайды.</span><span class="sxs-lookup"><span data-stu-id="ed939-130">Unit and unit group values do not default correctly for expense categories on the **Contract Line Details** and **Quote Line Details** forms.</span></span>
- <span data-ttu-id="ed939-131">**Ұйымдық бірлік шығыны** тізімдері жарамдылық мерзімінің қабатталуына рұқсат береді.</span><span class="sxs-lookup"><span data-stu-id="ed939-131">**Org Unit Cost Price** lists permit overlaps in the date effectivity.</span></span>
- <span data-ttu-id="ed939-132">Тапсырыс түрі жұмысқа негізделмеген болса, бос анықтамалық ерекшелік қатесіне себеп болатындықтан, пайдаланушыларға **OrgUnit** мәнін өзгертуге рұқсат етілмейді.</span><span class="sxs-lookup"><span data-stu-id="ed939-132">Users are not permitted to change the **OrgUnit** when the order type is not work-based because it will lead to a null reference exception error.</span></span>
- <span data-ttu-id="ed939-133">**Баға ұсыну жолы мәліметтері** пішінінен **Баға ұсыну** қойыншасына кері шарлауға әрекеттенген кезде, пішін жаңартылып, **Баға ұсыну жолы мәліметтері** қойыншасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="ed939-133">When attempting to navigate from the **Quote Line Details** form, back to the **Quote** tab, the form refreshes and displays the **Summary** tab.</span></span>