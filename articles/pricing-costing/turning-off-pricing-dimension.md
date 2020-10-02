---
title: Бағалау өлшемін өшіру
description: Осы тақырып бағалау өлшемдерін өшіру әдісі туралы ақпаратты ұсынады.
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
ms.openlocfilehash: 54e02726138f7306481ca50d5204ee29a3b68549
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896513"
---
# <a name="turning-off-a-pricing-dimension"></a><span data-ttu-id="b473b-103">Бағалау өлшемін өшіру</span><span class="sxs-lookup"><span data-stu-id="b473b-103">Turning off a pricing dimension</span></span>

<span data-ttu-id="b473b-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="b473b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b473b-105">Баға стратегиясын бірнеше жылда бір рет қарап, жаңартып отыру қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="b473b-105">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="b473b-106">Сіз жасаған кез келген жаңартулар қолданыстағы бағалар өлшемін өшіруді және жаңасын жасауды талап етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="b473b-106">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="b473b-107">Мысалы, сіз бұрын **Рөл** арқылы бағалаған болуыңыз мүмкін, бірақ қазір **Жұмыс тәжірибесі** арқылы бағалау туралы шешім қабылдадыңыз.</span><span class="sxs-lookup"><span data-stu-id="b473b-107">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="b473b-108">Бұл **Рөл** опциясын бағалау өлшемі ретінде өшіруді және **Жұмыс тәжірибесі** опциясын жаңа бағалау өлшемі ретінде жасауды қажет етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="b473b-108">This may require you to turn off **Role** as a pricing dimension and create **Work Experience** as a new pricing dimension.</span></span> 

<span data-ttu-id="b473b-109">Бағалар өлшемін кірістірілгеніне немесе реттелетініне қарамастан өшіру бағалар өлшемінің **Құнға қолданылатын** және **Сатылымға қолданылатын** өрістерін **Жоқ** параметріне орнату арқылы жүзеге асырылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="b473b-109">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="b473b-110">Алайда бұлай жасаған кезде, **Байланыстырылған баға жазбалары болса, бағалау өлшемін жаңарту немесе жою мүмкін емес** қате туралы хабарын алуыңыз мүмкін.</span><span class="sxs-lookup"><span data-stu-id="b473b-110">However, when you do this, you might receive the error message, **Pricing dimension cannot be updated or deleted if there are associated price records.**</span></span>

<span data-ttu-id="b473b-111">Бұл қате туралы хабар өшірілетін өлшем үшін алдын ала орнатылған баға жазбалары бар екенін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="b473b-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="b473b-112">Барлық өлшемге қатысты **Рөл бағасы** және **Рөлдің үстеме бағасы** жазбалары өлшем қолданысын **Жоқ** параметріне орнату алдында жойылуы керек.</span><span class="sxs-lookup"><span data-stu-id="b473b-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="b473b-113">Бұл ереже сіз жасаған кірістірілген бағалар өлшемдеріне де, кез келген реттелетін бағалар өлшемдеріне де қолданылады.</span><span class="sxs-lookup"><span data-stu-id="b473b-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="b473b-114">Бұл тексерудің себебі - әрбір **Рөл бағасы** жазбасы өлшемдердің бірегей тіркесімін қамтуы керек.</span><span class="sxs-lookup"><span data-stu-id="b473b-114">The reason for this validation is because each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="b473b-115">Мысалы, **АҚШ құн мөлшерлемелері, 2018** деп аталатын бағатізбеде келесідей **Рөл бағасы** жолдары бар.</span><span class="sxs-lookup"><span data-stu-id="b473b-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="b473b-116">Стандартты тақырып</span><span class="sxs-lookup"><span data-stu-id="b473b-116">Standard Title</span></span>         | <span data-ttu-id="b473b-117">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="b473b-117">Org Unit</span></span>    |<span data-ttu-id="b473b-118">Бірлік</span><span class="sxs-lookup"><span data-stu-id="b473b-118">Unit</span></span>   |<span data-ttu-id="b473b-119">Баға</span><span class="sxs-lookup"><span data-stu-id="b473b-119">Price</span></span>  |<span data-ttu-id="b473b-120">Валюта</span><span class="sxs-lookup"><span data-stu-id="b473b-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="b473b-121">Жүйелер инженері</span><span class="sxs-lookup"><span data-stu-id="b473b-121">Systems Engineer</span></span>|<span data-ttu-id="b473b-122">Contoso АҚШ</span><span class="sxs-lookup"><span data-stu-id="b473b-122">Contoso US</span></span>|<span data-ttu-id="b473b-123">Hour</span><span class="sxs-lookup"><span data-stu-id="b473b-123">Hour</span></span>| <span data-ttu-id="b473b-124">100</span><span class="sxs-lookup"><span data-stu-id="b473b-124">100</span></span>|<span data-ttu-id="b473b-125">USD</span><span class="sxs-lookup"><span data-stu-id="b473b-125">USD</span></span>|
| <span data-ttu-id="b473b-126">Жоғарғы жүйелер инженері</span><span class="sxs-lookup"><span data-stu-id="b473b-126">Senior Systems Engineer</span></span>|<span data-ttu-id="b473b-127">Contoso АҚШ</span><span class="sxs-lookup"><span data-stu-id="b473b-127">Contoso US</span></span>|<span data-ttu-id="b473b-128">Hour</span><span class="sxs-lookup"><span data-stu-id="b473b-128">Hour</span></span>| <span data-ttu-id="b473b-129">150</span><span class="sxs-lookup"><span data-stu-id="b473b-129">150</span></span>| <span data-ttu-id="b473b-130">USD</span><span class="sxs-lookup"><span data-stu-id="b473b-130">USD</span></span>|


<span data-ttu-id="b473b-131">**Стандартты тақырып** нысанын бағалау өлшемі ретінде өшірсеңіз және бағалау механизмі бағаны іздейтін болса, ол енгізу контекстіндегі **Ұйымдық бірлік** мәнін ғана пайдаланатын болады.</span><span class="sxs-lookup"><span data-stu-id="b473b-131">When you turn off **Standard Title** as the pricing dimension, and the pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="b473b-132">Егер енгізу мәтінмәнінің **Ұйымдық бөлімшесі** "Contoso US" болса, нәтиже анық болмайды, себебі екі жол да сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="b473b-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="b473b-133">Бұл сценарийді болдырмау үшін **Рөл бағасы** жазбаларын жасаған кезде жүйе өлшемдер тіркесімінің бірегей екендігін тексереді.</span><span class="sxs-lookup"><span data-stu-id="b473b-133">To avoid this scenario, when you create **Role Price** records, the system validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="b473b-134">Өлшем **Рөл бағасы** жазбалары жасалғаннан кейін өшірілсе, бұл шектеуді бұзуға болады.</span><span class="sxs-lookup"><span data-stu-id="b473b-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="b473b-135">Сондықтан өлшемді өшірмес бұрын, осы өлшем мәні толтырылған барлық **Рөл бағасы** және **Рөлдің үстеме бағасы** жолдарын жою керек.</span><span class="sxs-lookup"><span data-stu-id="b473b-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>
