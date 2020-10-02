---
title: Сатылым прайс-листін орнату
description: Осы тақырып жоба бағасын белгілеу үшін сатылым прайс-листтері туралы ақпаратты ұсынады.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2a66802adfcadab7b4d34149b146ca3cb27c903e
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896468"
---
# <a name="sales-price-list-setup"></a><span data-ttu-id="ac3f3-103">Сатылым прайс-листін орнату</span><span class="sxs-lookup"><span data-stu-id="ac3f3-103">Sales price list setup</span></span>

<span data-ttu-id="ac3f3-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="ac3f3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ac3f3-105">Жобаның баға ұсыныстары мен келісім-шарттары үшін, жобаның бағатізбесінде өнімнің бағатізбесінен өзгеше бағаны алдын ала анықтау үлгісі бар.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="ac3f3-106">Өнім каталогына негізделген баға ұсыну жолы үшін, рөлдер мен санаттарға бағаны тікелей баға ұсыну жолында алдын ала анықтауға болады, себебі әрбір баға ұсыну жолы нақты бір каталог элементіне нұсқайды.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="ac3f3-107">Дегенмен жобаға негізделген баға ұсыну жолында рөлдер мен санаттарға бағаны тікелей баға ұсыну жолында алдын ала анықтау мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="ac3f3-108">Жоба прайс-листін анықталған екі үлгімен жұмыс істеу үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="ac3f3-109">Бағаны алдын ала анықтау кезінде екеуінің арасындағы әрекеттер айырмашылығының себебінен, жоба ресурстары мен каталог элементтері үшін бөлек бағатізбенің болғаны жөн.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="ac3f3-110">Жобаның бағасын белгілеу үшін, келесі нысандардың әрқайсысы бір немесе бірнеше байланыстырылған сатылым бағатізбесіне ие бола алады:</span><span class="sxs-lookup"><span data-stu-id="ac3f3-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="ac3f3-111">Тұтынушы (тіркелгі)</span><span class="sxs-lookup"><span data-stu-id="ac3f3-111">Customer (account)</span></span> 
- <span data-ttu-id="ac3f3-112">Мүмкіндік</span><span class="sxs-lookup"><span data-stu-id="ac3f3-112">Opportunity</span></span> 
- <span data-ttu-id="ac3f3-113">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="ac3f3-113">Quote</span></span> 
- <span data-ttu-id="ac3f3-114">Жоба келісім-шарты</span><span class="sxs-lookup"><span data-stu-id="ac3f3-114">Project Contract</span></span>

<span data-ttu-id="ac3f3-115">Бұл нысандардың бағатізбемен байланысы жоба бағатізбелерімен анықталады.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="ac3f3-116">Тұтынушы, мүмкіндік, баға ұсыну және жоба келісім-шарты бойынша сатылымдар нысандарымен бір немесе бірнеше бағатізбені байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="ac3f3-117">Жобаның әдепкі бағатізбесі тұтынушы жазбасына автоматты түрде енгізілмейді.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="ac3f3-118">Дегенмен жобаның бағатізбесін тұтынушы жазбасына қолмен тіркеуге болады.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="ac3f3-119">Бұған қарамастан, жобаның бағатізбесін тұтынушымен реттелетін баға келісімі болған кезде ғана қолмен тіркеуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="ac3f3-120">Жоба прайс-листі сатылым нысанына бекітілген кезде, келесі ақпарат тексеріледі:</span><span class="sxs-lookup"><span data-stu-id="ac3f3-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="ac3f3-121">Прайс-листте **Сатылым** контексті бар.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="ac3f3-122">Бағатізбенің валютасы тұтынушы валютасына сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="ac3f3-123">Жоба келісім-шартында, жобаның қатысты прайс-листтерін автоматты түрде орнату үшін келесі кезектілік тәртібі пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="ac3f3-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="ac3f3-124">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="ac3f3-124">Quote</span></span>
2. <span data-ttu-id="ac3f3-125">Мүмкіндік</span><span class="sxs-lookup"><span data-stu-id="ac3f3-125">Opportunity</span></span>
3. <span data-ttu-id="ac3f3-126">Тұтынушы</span><span class="sxs-lookup"><span data-stu-id="ac3f3-126">Customer</span></span> 
4. <span data-ttu-id="ac3f3-127">Глобалдық параметрлер</span><span class="sxs-lookup"><span data-stu-id="ac3f3-127">Global settings</span></span> 

<span data-ttu-id="ac3f3-128">Жоба прайс-листі әдепкі бойынша енгізіледі, жүйе валютаның тұтынушы валютасына сәйкестігін және енгізілген әдепкі прайс-листтерде **Сатылым** контексті бар-жоғын тексереді.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="ac3f3-129">Тұтынушы, мүмкіндік, баға ұсыну және жоба келісім-шартының нысандарымен бірнеше бағатізбені байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="ac3f3-130">Бұл мүмкіндік құнсыздану себебінен орын алатын баға жаңартулары үшін тіркелгіге бірнеше бағатізбені қажет етуіңіз мүмкін ұзақ мерзімді жоба келісім-шарты үшін күн бойынша әдепкі бағаларды қолдайды.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="ac3f3-131">Дегенмен тұтынушы, мүмкіндік, баға ұсыну немесе жоба келісім-шартының нысанымен байланыстырылған бағатізбелердің жарамдылық мерзімі қабаттасқан болса, әдепкі бағалардың дұрыс болмауы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="ac3f3-132">Сондықтан жарамдылық мерзімі қабаттасқан жоба бағатізбелерінің осы нысандармен байланыстырылмағанына көз жеткізу қажет.</span><span class="sxs-lookup"><span data-stu-id="ac3f3-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>
