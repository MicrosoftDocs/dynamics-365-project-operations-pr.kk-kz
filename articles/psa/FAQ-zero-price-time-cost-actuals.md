---
title: Уақыт құнының нақты мәндері бойынша неліктен әдепкі баға нөлге тең емес?
description: Уақыт құнының нақты мәндері бойынша әдепкі бағаны 0-ге теңестіріңіз.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 44d4952b77ac0a541cdf8e3e55f202c9209efdf4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079679"
---
# <a name="why-is-the-price-defaulting-to-zero-on-time-cost-actuals"></a><span data-ttu-id="eda54-103">Уақыт құнының нақты мәндері бойынша неліктен әдепкі баға нөлге тең емес?</span><span class="sxs-lookup"><span data-stu-id="eda54-103">Why is the price defaulting to zero on time cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="eda54-104">Бұл ЖҚС нақты мәндерге қолданылады, мұндағы транзакция класы Уақыт күйіне, ал транзакция түрі Құн күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="eda54-104">This FAQ applies to actuals where the transaction class is set to Time and transaction type is Cost.</span></span> <span data-ttu-id="eda54-105">Келесі үш тексеріс уақыт құны нақты мәндерінде бағаны әдепкі бойынша 0-ге орнатуға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="eda54-105">The following three checks will help you troubleshoot why the price is defaulting to 0 on time cost actuals.</span></span>
 
## <a name="check-1-identify-the-cost-price-list-for-the-project"></a><span data-ttu-id="eda54-106">Тексеру 1: жобаның құн бағатізбесін анықтау</span><span class="sxs-lookup"><span data-stu-id="eda54-106">Check 1: Identify the cost price list for the project</span></span>

<span data-ttu-id="eda54-107">Нақты мәннің жоба өрісінен жобаны тауып, жоба бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-107">Find the project from the project field of the actual and then go to the project page.</span></span> <span data-ttu-id="eda54-108">Өрістегі келісім-шарт бірлігі сілтемесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="eda54-108">Click on the contracting unit link in the field.</span></span> <span data-ttu-id="eda54-109">Келісім-шарт бірлігі бетінен келісім-шарт бірлігінде Құн бағатізбелері торындағы бағатізбе бар-жоғын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-109">On the Contracting Unit page, check if the contracting unit has a price list in the Cost Price Lists grid.</span></span>

<span data-ttu-id="eda54-110">Бірнеше бағатізбе болса, мәселе оқшауланды.</span><span class="sxs-lookup"><span data-stu-id="eda54-110">If there is more than one price list, you have isolated the problem.</span></span> <span data-ttu-id="eda54-111">Жоба қызметінде әрбір ұйымдық бірліктің бір бағатізбесіне ғана қолдау көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="eda54-111">Project Service only supports one price list per organizational unit.</span></span> <span data-ttu-id="eda54-112">Ұйымдық бірліктің құн бағатізбелеріне тек бір бағатізбе тіркелгенше осы нысаннан барлық бағатізбелерді жойыңыз.</span><span class="sxs-lookup"><span data-stu-id="eda54-112">Remove all prices lists from this entity until there is only one price list attached in the Cost Price Lists grid of the Organizational Unit.</span></span>

<span data-ttu-id="eda54-113">Ұйымдық бірлікке ешбір бағатізбе тіркелмесе, ұйымдық бірлік валютасын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-113">If there are no price lists attached to the Organizational Unit, make a note of the currency of the Organizational unit.</span></span> <span data-ttu-id="eda54-114">Жоба қызметі және Параметрлер тармағына өтіп, Бағатізбелер қойыншасын ашыңыз. Мәтінмәні Құн күйіне орнатылған бағатізбелер және ұйымдық бірлік валютасына сәйкес валюта бар-жоғын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-114">Go to the Project Service and then Parameters and open the Price Lists tab. Check if there are any price lists with context set to Cost and currency that matches the currency of the Organizational Unit.</span></span>
 
<span data-ttu-id="eda54-115">Шарттарға сәйкес бағатізбелер болмаса, мәселе оқшауланды.</span><span class="sxs-lookup"><span data-stu-id="eda54-115">If there are no price lists that match that criteria, you have isolated the problem.</span></span> <span data-ttu-id="eda54-116">Мәтінмән Құн күйіне орнатылған кемінде бір бағатізбе және ұйымдық бірліктің валютасына сәйкес валюта бар-жоғын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-116">Make sure to have at least one price list whose context is set to Cost and whose currency matches the currency of the Organizational Unit.</span></span>

<span data-ttu-id="eda54-117">Осы шарттарға сәйкес бірнеше бағатізбе болса, қосымша тексерістер жасау үшін осы құжатты оқуды жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="eda54-117">If there is more than one price list that match that criteria, continue reading this document to make more checks.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-cost-actual"></a><span data-ttu-id="eda54-118">Тексеру 2: жоғарыда анықталған бағатізбелер уақытылы құн нақты мәнінің көрсетілген күніне қолданылады ма?</span><span class="sxs-lookup"><span data-stu-id="eda54-118">Check 2: Are any of the price lists identified above valid for the specific date of the time cost actual?</span></span>

<span data-ttu-id="eda54-119">Жоба қызметі үшін әдепкі бағалардың бағатізбесін қарастыру үшін, бағатізбе уақытылы құн нақты мәніндегі күнге қолданылуы керек.</span><span class="sxs-lookup"><span data-stu-id="eda54-119">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the time cost actual.</span></span> <span data-ttu-id="eda54-120">Жоғарыда анықталған бағатізбе(лер) қолданылатынын көру үшін келесілерді тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="eda54-120">Check the following to see if the price list(s) identified above are applicable:</span></span>

- <span data-ttu-id="eda54-121">Тіркелген бағатізбелердің жалпы қойыншасындағы басталу және аяқталу күндері бос еместігін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-121">Check if the start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="eda54-122">Жоғарыда анықталған бағатізбелердің басталу және аяқталу күндері бос болса, мәселе оқшауланды.</span><span class="sxs-lookup"><span data-stu-id="eda54-122">If the start and end dates on price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="eda54-123">Уақытылы құн нақты мәніндегі басталу күні өрісін ескеріңіз және анықталған бағатізбелер осы күні қолданылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-123">Make a note of the start date field on your time cost actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="eda54-124">Мысалы, уақытылы құн нақты мәні күні бағатізбедегі басталу және аяқталу күні арасында болуы керек.</span><span class="sxs-lookup"><span data-stu-id="eda54-124">For example, the date of the time cost actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="eda54-125">Уақытылы құн нақты мәніндегі осы күнді қамтитын бағатізбе болмаса, мәселені оқшауладыңыз.</span><span class="sxs-lookup"><span data-stu-id="eda54-125">If there is no price list that covers that date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="eda54-126">Бағатізбеде уақытылы құн нақты мәнінің күні қамту үшін бағатізбенің басталу және аяқталу күндерін өзгертіңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-126">Modify the start and end dates of the price list to ensure that the price list covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="eda54-127">Уақытылы құн нақты мәніндегі күнді қамтитын бірнеше бағатізбе болса, мәселені оқшауладыңыз.</span><span class="sxs-lookup"><span data-stu-id="eda54-127">If there is more than one price list that covers the date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="eda54-128">Уақытылы құн нақты мәні күнін қамтитын тек бір бағатізбе болуы үшін, бағатізбе(лер) басталу және аяқталу күндерін өңдеу арқылы осыны түзете аласыз.</span><span class="sxs-lookup"><span data-stu-id="eda54-128">You can fix this by editing the start and end dates of the price list(s) so that there is only one price list that covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="eda54-129">Уақытылы құн нақты мәнінің күнін қамтитын тек бір бағатізбе болса, құжаттағы келесі тексеріске өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-129">If there is only one price list that covers that date of the time cost actual, move to the next check in the document.</span></span>
<span data-ttu-id="eda54-130">Талап етілетін түзету жұмыстарын жасағаннан кейін уақыт жазбасын қайта жасап, оны растап, уақытылы құн нақты мәнінде жарамды баға көрсетілгенін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-130">Once you’ve done made the required fixes, recreate a time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-cost-actual"></a><span data-ttu-id="eda54-131">Тексеру 3: уақытылы құн нақты мәніндегі бағалар өлшемдерінің бағатізбесінде баға бар ма?</span><span class="sxs-lookup"><span data-stu-id="eda54-131">Check 3: Is there a price in the price list for the pricing dimensions on the time cost actual?</span></span>

<span data-ttu-id="eda54-132">1-тексеріс пен 2-тексеріс сәтті аяқталса, уақытылы құн нақты мәні күніне қолданылатын тек бір бағатізбе болуы керек.</span><span class="sxs-lookup"><span data-stu-id="eda54-132">If you have successfully completed Check 1 and Check 2, you should now have only one price list that is applicable for the date of the time cost actual.</span></span> <span data-ttu-id="eda54-133">Осы бағатізбені ашып, Рөл бағалары қойыншасына өтіңіз. Уақытылы құн нақты мәніндегі бағалар өлшемдерінің торында қатар бар-жоғына көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-133">Open this Price List and go to the Role Prices tab. Make sure that there is a row in the grid for the pricing dimensions on the time cost actual.</span></span>

<span data-ttu-id="eda54-134">Уақытылы құн нақты мәніндегі бағалар өлшемдерінің рөл бағатізбесінде қатар болмаса, мәселе оқшауланды.</span><span class="sxs-lookup"><span data-stu-id="eda54-134">If there is no row in the role price grid for the pricing dimensions on the time cost actual, then you have isolated the problem.</span></span> <span data-ttu-id="eda54-135">Уақытылы құн нақты мәніндегі бағалар өлшемдерінің Рөл бағалары торында қатар жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="eda54-135">Create a row in the Role prices grid for the pricing dimensions on your time cost actual.</span></span> <span data-ttu-id="eda54-136">Осы орындалса, уақыт жазбасын қайта жасап, оны растап, уақытылы құн нақты мәнінде жарамды баға көрсетілгенін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-136">Once this is done, recreate time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>
 
<span data-ttu-id="eda54-137">Жоғарыдағы үш тексерістен кейін уақытылы құн нақты мәнінде жарамды баға көрінбесе, қолдау билетін тіркеңіз.</span><span class="sxs-lookup"><span data-stu-id="eda54-137">If you still don't see a valid price on your time cost actual after you’ve done the three checks above, please log a support ticket.</span></span>


