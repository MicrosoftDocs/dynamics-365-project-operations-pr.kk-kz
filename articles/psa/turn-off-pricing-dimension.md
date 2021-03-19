---
title: Бағалар өлшемін өшіру
description: Бұл тақырыпта Project Service шешімінде бағалар өлшемдерін орнату жолы көрсетілген.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 6e4b80b9c4b1b0f57d04079c9d2f84051b451d29
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281845"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="e3ce4-103">Бағалар өлшемін өшіру</span><span class="sxs-lookup"><span data-stu-id="e3ce4-103">Turn off a pricing dimension</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="e3ce4-104">Баға стратегиясын бірнеше жылда бір рет қарап, жаңартып отыру қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="e3ce4-105">Сіз жасаған кез келген жаңартулар қолданыстағы бағалар өлшемін өшіруді және жаңасын жасауды талап етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="e3ce4-106">Мысалы, сіз бұрын **Рөл** арқылы бағалаған болуыңыз мүмкін, бірақ қазір **Жұмыс тәжірибесі** арқылы бағалау туралы шешім қабылдадыңыз.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-106">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="e3ce4-107">Бұл **Рөл** бағалар өлшемін өшіріп, жаңа **Жұмыс тәжірибесі** бағалар жаңа өлшемін жасауды талап етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="e3ce4-108">Бағалар өлшемін кірістірілгеніне немесе реттелетініне қарамастан өшіру бағалар өлшемінің **Құнға қолданылатын** және **Сатылымға қолданылатын** өрістерін **Жоқ** параметріне орнату арқылы жүзеге асырылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="e3ce4-109">Алайда мұны жасаған кезде келесі қате туралы хабарды алуыңыз мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-109">However, when you do this, you might receive the following error message.</span></span>

![Бағалар өлшемін өшіру кезінде бизнес процестің қатесі болуы мүмкін](media/Business-Process-Error.png)


<span data-ttu-id="e3ce4-111">Бұл қате туралы хабар өшірілетін өлшем үшін алдын ала орнатылған баға жазбалары бар екенін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="e3ce4-112">Барлық өлшемге қатысты **Рөл бағасы** және **Рөлдің үстеме бағасы** жазбалары өлшем қолданысын **Жоқ** параметріне орнату алдында жойылуы керек.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="e3ce4-113">Бұл ереже сіз жасаған кірістірілген бағалар өлшемдеріне де, кез келген реттелетін бағалар өлшемдеріне де қолданылады.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="e3ce4-114">Бұл тексерудің себебі Project Service бағдарламасында **Рөл бағасы** жазбасында өлшемдердің бірегей комбинациясы болуы керектігіне қатысты шектеудің болуына байланысты.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="e3ce4-115">Мысалы, **АҚШ құн мөлшерлемелері, 2018** деп аталатын бағатізбеде келесідей **Рөл бағасы** жолдары бар.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="e3ce4-116">Стандартты тақырып</span><span class="sxs-lookup"><span data-stu-id="e3ce4-116">Standard Title</span></span>         | <span data-ttu-id="e3ce4-117">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="e3ce4-117">Org Unit</span></span>    |<span data-ttu-id="e3ce4-118">Бірлік</span><span class="sxs-lookup"><span data-stu-id="e3ce4-118">Unit</span></span>   |<span data-ttu-id="e3ce4-119">Баға</span><span class="sxs-lookup"><span data-stu-id="e3ce4-119">Price</span></span>  |<span data-ttu-id="e3ce4-120">Валюта</span><span class="sxs-lookup"><span data-stu-id="e3ce4-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="e3ce4-121">Жүйелер инженері</span><span class="sxs-lookup"><span data-stu-id="e3ce4-121">Systems Engineer</span></span>|<span data-ttu-id="e3ce4-122">Contoso АҚШ</span><span class="sxs-lookup"><span data-stu-id="e3ce4-122">Contoso US</span></span>|<span data-ttu-id="e3ce4-123">Hour</span><span class="sxs-lookup"><span data-stu-id="e3ce4-123">Hour</span></span>| <span data-ttu-id="e3ce4-124">100</span><span class="sxs-lookup"><span data-stu-id="e3ce4-124">100</span></span>|<span data-ttu-id="e3ce4-125">USD</span><span class="sxs-lookup"><span data-stu-id="e3ce4-125">USD</span></span>|
| <span data-ttu-id="e3ce4-126">Жоғарғы жүйелер инженері</span><span class="sxs-lookup"><span data-stu-id="e3ce4-126">Senior Systems Engineer</span></span>|<span data-ttu-id="e3ce4-127">Contoso АҚШ</span><span class="sxs-lookup"><span data-stu-id="e3ce4-127">Contoso US</span></span>|<span data-ttu-id="e3ce4-128">Hour</span><span class="sxs-lookup"><span data-stu-id="e3ce4-128">Hour</span></span>| <span data-ttu-id="e3ce4-129">150</span><span class="sxs-lookup"><span data-stu-id="e3ce4-129">150</span></span>| <span data-ttu-id="e3ce4-130">USD</span><span class="sxs-lookup"><span data-stu-id="e3ce4-130">USD</span></span>|


<span data-ttu-id="e3ce4-131">**Стандартты тақырып** бағалар өлшемін өшіріп, Project Service бағалар жүйесі бағаны іздеген кезде, ол тек енгізу мәтінмәніндегі **Ұйымдық бөлімше** мәнін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="e3ce4-132">Егер енгізу мәтінмәнінің **Ұйымдық бөлімшесі** "Contoso US" болса, нәтиже анық болмайды, себебі екі жол да сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="e3ce4-133">Бұл сценарийді жасамау үшін **Рөл бағасы** жазбаларын жасаған кезде, Project Service өлшемдер тіркесімінің бірегей екенін растайды.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="e3ce4-134">Өлшем **Рөл бағасы** жазбалары жасалғаннан кейін өшірілсе, бұл шектеуді бұзуға болады.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="e3ce4-135">Сондықтан өлшемді өшірмес бұрын, осы өлшем мәні толтырылған барлық **Рөл бағасы** және **Рөлдің үстеме бағасы** жолдарын жою керек.</span><span class="sxs-lookup"><span data-stu-id="e3ce4-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]