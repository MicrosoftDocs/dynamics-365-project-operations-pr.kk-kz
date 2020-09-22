---
title: Өзіндік бетті жаңарту
description: Бұл тақырыпта Dynamics 365 Project Service Automation ішіндегі жаңа және өзгертілген мүмкіндіктері және ең жаңа нұсқаны жаңартуға арналған процесс туралы маңызды ақпаратты қайдан табуға болатыны көрсетілген.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 05/30/2019
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 for Project Service 3.x
author: rumant
ms.assetid: c92d0849-e40c-4a56-9719-34030fbf5991
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 55f544636f39fc4faae06fdd512f859800bb7b44
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753101"
---
# <a name="upgrade-home-page"></a><span data-ttu-id="89c75-103">Өзіндік бетті жаңарту</span><span class="sxs-lookup"><span data-stu-id="89c75-103">Upgrade home page</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a><span data-ttu-id="89c75-104">PSA 2.x немесе 1.x нұсқасын 3.x нұсқасына жаңарту</span><span class="sxs-lookup"><span data-stu-id="89c75-104">Upgrade from PSA version 2.x or 1.x to version 3.x</span></span>

### <a name="new-instances"></a><span data-ttu-id="89c75-105">Жаңа даналар</span><span class="sxs-lookup"><span data-stu-id="89c75-105">New instances</span></span>

<span data-ttu-id="89c75-106">2019 жылдың 17 мамырынан бастап жаңа дана ұсыну кезінде Project Service Automation таңдалғанда, 3.x нұсқасы әдепкі бойынша орнатылады.</span><span class="sxs-lookup"><span data-stu-id="89c75-106">As of May 17, 2019, when Project Service Automation is selected during the provisioning of a new instance, version 3.x is installed by default.</span></span>

### <a name="existing-instances"></a><span data-ttu-id="89c75-107">Қолданыстағы даналар</span><span class="sxs-lookup"><span data-stu-id="89c75-107">Existing instances</span></span>

<span data-ttu-id="89c75-108">Бұдан бұрын, PSA 2.x нұсқасының данасы бар және PSA бірыңғай клиенттік интерфейске негізделген (UCI) нұсқасы болып табылатын 3.x нұсқасына жаңартуды қажет ететін тұтынушылар Microsoft қолдау қызметіне хабарласып, 3.x нұсқасына жаңарту үшін қолдау қызметі дананы іске қоса алуы үшін дана туралы мәліметтерді беруі керек.</span><span class="sxs-lookup"><span data-stu-id="89c75-108">Previously, customers who have an instance of PSA version 2.x and needed to upgrade to version 3.x, which is the Unified client interface-based (UCI) version of PSA , had to contact Microsoft Support and provide the details of thier instance so that support could enable the instance for upgrade to version 3.x.</span></span> <span data-ttu-id="89c75-109">2020 жылдың 1 наурызынан бастап PSA 2.x нұсқасы бар және 3.x нұсқасына жаңартуды қажет ететін тұтынушылар Microsoft қолдау қызметіне жүгінбестен тікелей әкімші порталынан даналарын жаңарта алады.</span><span class="sxs-lookup"><span data-stu-id="89c75-109">As of March 1st, 2020, customers who have an instance of PSA version 2.x and need to upgrade to version 3.x, will able to upgrade their instances directly from the Admin portal without having to contact Microsoft Support.</span></span>  

> [!NOTE]
> <span data-ttu-id="89c75-110">PSA 3.x нұсқасында айтарлықтай өзгерістер бар.</span><span class="sxs-lookup"><span data-stu-id="89c75-110">PSA version 3.x includes significant changes.</span></span> <span data-ttu-id="89c75-111">Ол жақсартылған пайдаланушы тәжірибесін қамтамасыз етуге көмектесу үшін Бірыңғай интерфейс инфрақұрылымында жасалды.</span><span class="sxs-lookup"><span data-stu-id="89c75-111">It has been built on the Unified Interface framework to help provide an improved user experience.</span></span> <span data-ttu-id="89c75-112">Қайта құрастырылған бағдарлама тиісті, бірыңғай пайдаланушы интерфейсті (UI) жібереді және кез келген экран өлшемінде және құрылғыда оңтайлы көру үшін жауапты жоба қағидаларына сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="89c75-112">The redesigned app delivers a consistent, uniform user interface (UI), and it follows responsive design principles for optimal viewing on any screen size or device.</span></span> <span data-ttu-id="89c75-113">Бағдарлама бойынша басқа да өзгерістер болды.</span><span class="sxs-lookup"><span data-stu-id="89c75-113">There have been other changes throughout the application.</span></span> <span data-ttu-id="89c75-114">Өзгертілген кейбір аймақтар баға, тапсырыс беру және тағайындау ресурстары, уақыт, шығыстар және бекітулерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="89c75-114">Some of the areas that have been changed include pricing, booking and assigning resources, time, expenses, and approvals.</span></span>

<span data-ttu-id="89c75-115">Жаңарту процесін бастамас бұрын, келесі тапсырмаларды орындауға кеңес береміз:</span><span class="sxs-lookup"><span data-stu-id="89c75-115">Before you begin the upgrade process, we recommend that you complete the following tasks:</span></span>

- <span data-ttu-id="89c75-116">Dynamics 365 Field Service және Project Service Automation белгіленген данада орнатылғанына көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="89c75-116">Verify whether both Dynamics 365 Field Service and Project Service Automation are installed on the identified instance.</span></span> <span data-ttu-id="89c75-117">Егер екі шешім де орнатылған болса, дананы тұрақты пайдалануды жалғастырмас бұрын, екеуін де жаңартуды жоспарлау керек.</span><span class="sxs-lookup"><span data-stu-id="89c75-117">If both solutions are installed, you should plan to upgrade both before you resume regular use of the instance.</span></span>
- <span data-ttu-id="89c75-118">Келесі тақырыптарды мұқият қарап шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="89c75-118">Carefully review the following topics.</span></span> <span data-ttu-id="89c75-119">Нұсқалар арасындағы өзгерістер туралы хабардар болу және түсіну сізге жаңарту процесінде көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="89c75-119">Awareness and understanding of the changes between versions will help you with the upgrade process.</span></span> <span data-ttu-id="89c75-120">Бұл тақырыптарда PSА шешіміндегі негізгі өзгерістер туралы ақпарат, сонымен бірге 3.x нұсқасына жаңартуды жоспарлау бойынша ұсыныстар мен пікірлер берілген.</span><span class="sxs-lookup"><span data-stu-id="89c75-120">These topics provide information about the major changes in PSA, together with considerations and recommendations for planning your upgrade to version 3.x.</span></span>

    - [<span data-ttu-id="89c75-121">Project Service Automation бағдарламасының 3 нұсқасындағы жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="89c75-121">What's new or changed in Project Service Automation version 3</span></span>](whats-new-changed-v3.md)
    - [<span data-ttu-id="89c75-122">Ұсыныстарды жаңарту - Project Service Automation 2.x немесе 1.x нұсқасынан 3 нұсқасына</span><span class="sxs-lookup"><span data-stu-id="89c75-122">Upgrade considerations - Project Service Automation version 2.x or 1.x to version 3</span></span>](upgrade-v3.md)

- <span data-ttu-id="89c75-123">Өндіріс данасын жаңарту алдында іске асырудағы өзгерістерді бағалау үшін сынақ дананы жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="89c75-123">Upgrade your sandbox instance to evaluate the changes in your implementation before you upgrade your production instance.</span></span>

<span data-ttu-id="89c75-124">Жоғарыда айтылған тақырыптарды қарап шыққаннан кейін және PSA 3.x нұсқасына немесе UCI негізіндегі нұсқаға жаңартуға дайын болғаннан кейін, жаңартуды әкімші орталығынан қолжетімді ету үшін Microsoft қолдау қызметіне сұрау жіберіңіз.</span><span class="sxs-lookup"><span data-stu-id="89c75-124">After you've reviewed the topics that were mentioned earlier and are ready to upgrade to PSA version 3.x or the UCI-based version, submit a request to Microsoft support to make the upgrade available from Admin center.</span></span> <span data-ttu-id="89c75-125">Сұрауыңызда данаңыздың мәліметтерін көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="89c75-125">In your request, provide the details of your instance.</span></span>

## <a name="older-versions-of-psa-psa-version-2x-in-a-newly-created-instance"></a><span data-ttu-id="89c75-126">Жаңадан жасалған данадағы ескі PSA нұсқалары (PSA 2.x нұсқасы)</span><span class="sxs-lookup"><span data-stu-id="89c75-126">Older versions of PSA (PSA version 2.x) in a newly created instance</span></span>

<span data-ttu-id="89c75-127">2019 жылдың 17 мамырынан бастап барлық жаңа даналарда UCI әдепкі клиент ретінде болады.</span><span class="sxs-lookup"><span data-stu-id="89c75-127">As of May 17, 2019, all new instances will have UCI as the default client.</span></span> <span data-ttu-id="89c75-128">Осы өзгеріспен туралау үшін PSA 3.x және Field Service 8.x нұсқасы әдепкі бойынша қамтамасыз етіледі, өйткені бұл нұсқалар UCI клиентімен жұмыс істеуге арналған.</span><span class="sxs-lookup"><span data-stu-id="89c75-128">For alignment with this change, PSA version 3.x and Field Service version 8.x will be provisioned by default, because these versions are designed to work with the UCI client.</span></span>

<span data-ttu-id="89c75-129">2020 жылдың 1-наурызынан бастап Dynamics PSA тұтынушылары бұдан әрі PSA жүйесінің 2.х немесе одан төменгі нұсқалары секілді PSA жүйесінің ескі нұсқаларымен жаңа орталар жасай алмайды.</span><span class="sxs-lookup"><span data-stu-id="89c75-129">Starting March 1st 2020, customers of Dynamics PSA will no longer be able to create a new environments with older versions of PSA, for example PSA version 2.x or lower.</span></span> <span data-ttu-id="89c75-130">Кез-келген жаңа ортада тек PSA жүйесінің 3.x нұсқасы болады.</span><span class="sxs-lookup"><span data-stu-id="89c75-130">Any new environment will be to get only version 3.x of PSA.</span></span>

> [!NOTE]
> <span data-ttu-id="89c75-131">Field Service және PSA қосымшаларының ескі нұсқаларының бар мүмкіндіктерін пайдалану үшін **Жүйе параметрлері** бетіне өтіңіз және **Жаңа бірыңғай интерфейсті ғана пайдалану (ұсынылған)** өрісі үшін **Жоқ** параметрін таңдаңыз, өйткені бұл нұсқалар UCI ішіне дұрыс жүктелмейді.</span><span class="sxs-lookup"><span data-stu-id="89c75-131">For the best experience when you use older versions of the Field Service and PSA applications, go to the **System settings** page and for the field, **Use the new Unified Interface only (recommended)** field, select **No** as these versions aren't designed to be correctly loaded in UCI.</span></span> <span data-ttu-id="89c75-132">UCI интерфейсін өшіргеннен кейін, осы Field Service және PSA нұсқаларын ескі веб-клиенттің көмегімен ашуға және іске қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="89c75-132">After you have turned off UCI, you can open and run these versions of Field Service and PSA by using the old web client.</span></span> <span data-ttu-id="89c75-133">UCI клиентін өшіру жолы туралы нұсқауларды [Тек бірыңғай интерфейсті қосу](../admin/enable-unified-interface-only.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="89c75-133">For instructions about how to turn off the UCI client, see [Enable unified interface only](../admin/enable-unified-interface-only.md).</span></span>
