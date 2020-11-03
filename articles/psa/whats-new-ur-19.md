---
title: Project Service Automation бағдарламасының 19 жаңарту шығарылымы, Hotfix, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation 19 жаңарту шығарылымының 3-нұсқасында қолжетімді мүмкіндіктер мен түзетпелер көрсетілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: ecc923cccfad21985025ab9d8006aaff16afc25f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079613"
---
# <a name="project-service-automation-update-release-19-v3"></a><span data-ttu-id="a4720-103">Project Service Automation 19 жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="a4720-103">Project Service Automation Update Release 19, V3</span></span>

<span data-ttu-id="a4720-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="a4720-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a4720-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="a4720-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a4720-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="a4720-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a4720-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="a4720-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="a4720-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="a4720-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a4720-109">Бұл тақырыпта PSA 3-нұсқасы, 19 жаңарту шығарылымы үшін қолжетімді мүмкіндіктер мен түзетпелер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="a4720-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 19.</span></span> <span data-ttu-id="a4720-110">Бұл нұсқаның V3.10.30.41 құрастыру нөмірі бар, сондай-ақ 2020 жылдыңң мамыр айында өзіндік жаңарту арқылы жалпы түрде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="a4720-110">This version has a build number of V3.10.30.41 and is generally available through a self-update in May 2020.</span></span>

## <a name="update-release-19"></a><span data-ttu-id="a4720-111">19-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="a4720-111">Update Release 19</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a4720-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="a4720-112">Bug fixes</span></span>

<span data-ttu-id="a4720-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="a4720-113">**Time and Expense**</span></span>

<span data-ttu-id="a4720-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="a4720-114">The following issues have been fixed:</span></span> 

- <span data-ttu-id="a4720-115">Уақыт жазбаларын импорттау нәтижесінде алынған қателер дұрыс анықталмайды.</span><span class="sxs-lookup"><span data-stu-id="a4720-115">Errors derived from time entry imports are not surfaced correctly.</span></span>
- <span data-ttu-id="a4720-116">Уақыт жазбасы торы **Тек күн** өрісі тәртібіне қолдау көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="a4720-116">Time Entry Grid does not support **Date Only** field behavior.</span></span>
- <span data-ttu-id="a4720-117">Жобаның ресурстары жобаның көмегімен шығыстарды жасай алмайды.</span><span class="sxs-lookup"><span data-stu-id="a4720-117">Project Resources are unable to create an expense with a project.</span></span>

<span data-ttu-id="a4720-118">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="a4720-118">**Project Management**</span></span>

<span data-ttu-id="a4720-119">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="a4720-119">The following issues have been fixed:</span></span> 

-  <span data-ttu-id="a4720-120">Басты еншілес тапсырмасы аяқталуды есептеу (EAC) барысында дұрыс емес талпыныс болжамына алып келеді.</span><span class="sxs-lookup"><span data-stu-id="a4720-120">Grandchild task causes an incorrect effort estimate during the Completion (EAC) Calculation.</span></span>

<span data-ttu-id="a4720-121">**Sales**</span><span class="sxs-lookup"><span data-stu-id="a4720-121">**Sales**</span></span>

<span data-ttu-id="a4720-122">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="a4720-122">The following issues have been fixed:</span></span> 

- <span data-ttu-id="a4720-123">**Қайта есептеу** әрекеті шығыс келісім-шарт жолы мәліметтерімен немесе баға ұсыну жолы мәліметтерімен жұмыс істемейді.</span><span class="sxs-lookup"><span data-stu-id="a4720-123">The **Recalculate** action does not work with expense contract line details or quote line details.</span></span>
- <span data-ttu-id="a4720-124">**Бағаларды жаңарту** шығыс болжамдарында жоқ.</span><span class="sxs-lookup"><span data-stu-id="a4720-124">**Update Prices** is missing for expense estimates.</span></span>
-  <span data-ttu-id="a4720-125">Тұтынушылар **Жоба келісім-шарты** бетінен жеке келісім-шарт күйлерін таңдай алмайды.</span><span class="sxs-lookup"><span data-stu-id="a4720-125">Customers are unable to select custom contract status reasons from the **Project Contract** page.</span></span>
- <span data-ttu-id="a4720-126">Тұтынушылар баға ұсынудан пайдаланушылық бағатізбені жасау кезінде төмендетілген өнімділіктен өтеді.</span><span class="sxs-lookup"><span data-stu-id="a4720-126">Customers experience degraded performance when creating a custom price list from a quote.</span></span>
- <span data-ttu-id="a4720-127">Тұтынушылар **Баға ұсыну жолы мәліметтері** және **Келісім-шарт жолы мәліметтері** беттерінде **бірлік** әдепкі мәндерімен сәйкессіздіктен өтеді.</span><span class="sxs-lookup"><span data-stu-id="a4720-127">Customers experience inconsistency with **unit** defaults on **Quote Line Details** and **Contract Line Details** pages.</span></span>
- <span data-ttu-id="a4720-128">Ақылы келісім-шарт жолына ақылы емес транзакция санаты элементтерін қосу транзакция санатының **Ақылы емес** шот ұсыну түріне сәйкес келмейді.</span><span class="sxs-lookup"><span data-stu-id="a4720-128">Adding non-chargeable transaction category items to a chargeable contract line will not respect the **Non-chargeable** billing type of the transaction category.</span></span>
- <span data-ttu-id="a4720-129">Тұтынушылар бұған дейін жасалған келісім-шарттарда жаңадан қосылған рөлдер мен санатты пайдалана алмайды.</span><span class="sxs-lookup"><span data-stu-id="a4720-129">Customers can't use the newly added roles and category on previously created contracts.</span></span>
- <span data-ttu-id="a4720-130">Тұтынушылар PreValidateProjectTeamMemberUpdate.cs ішінде төмендетілген өнімділікті қажетсіз алудан өтеді</span><span class="sxs-lookup"><span data-stu-id="a4720-130">Customers experience degraded performance Unnecessary retrieve in PreValidateProjectTeamMemberUpdate.cs</span></span>
- <span data-ttu-id="a4720-131">**Ресурс санаттары** тізімінде ақылы емес ретінде орнатылған рөлдер жобаның келісім-шарт жолында **Ақылы рөлдер** қойыншасына **Ақылы емес** ретінде қосылады.</span><span class="sxs-lookup"><span data-stu-id="a4720-131">Roles set up as non-chargeable in the **Resource Categories** list should be added to the **Chargeable Roles** tab as **Non0chargeable** on the contract line for a project.</span></span>
- <span data-ttu-id="a4720-132">Тұтынушылар жобаны жасау кезінде төмендетілген өнімділікке тап болады, себебі **GetBookableResourceIdFromUser** тек бастапқы идентификаторды шығарып алудың орнына тіркелетін ресурстардың барлық бағандарын шығарып алады.</span><span class="sxs-lookup"><span data-stu-id="a4720-132">Customers may experience degraded performance when creating a project because **GetBookableResourceIdFromUser** retrieves all columns of bookable resources instead of just the primary ID.</span></span>
- <span data-ttu-id="a4720-133">**Транзакция түрі** нысанында пайдаланушыларды транзакция түрлері үшін жарамды емес **Бірліктер** және **Бірлік топтары** параметрлеріне кіргізбеу үшін алдын ала тексеруді жаңарту қосылатын модулі болмайды.</span><span class="sxs-lookup"><span data-stu-id="a4720-133">**TransactionType** entity missing the pre-validation update plug-in to prevent users from entering **Units** and **UnitGroups** that are not valid for transaction types.</span></span>
- <span data-ttu-id="a4720-134">**Жою** қадамы уақыт жазбасы импорты үшін жұмыс істемейді.</span><span class="sxs-lookup"><span data-stu-id="a4720-134">The **Remove** step does not work for time entry import.</span></span>
