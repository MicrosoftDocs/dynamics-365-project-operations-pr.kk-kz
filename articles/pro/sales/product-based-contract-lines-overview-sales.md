---
title: Өнімге негізделген келісім-шарт жолдарын шолу
description: Бұл тақырыпта өнімге негізделген келісім-шарт жолдары туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 794a80b0dd6b8717b43e712b96b9ac077517c226
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079587"
---
# <a name="product-based-contract-lines-overview"></a><span data-ttu-id="f255a-103">Өнімге негізделген келісім-шарт жолдарын шолу</span><span class="sxs-lookup"><span data-stu-id="f255a-103">Product-based contract lines overview</span></span>

<span data-ttu-id="f255a-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="f255a-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f255a-105">Dynamics 365 Project Operations бағдарламасында өнімге негізделген келісім-шарт жолдарын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="f255a-105">You can create product-based contract lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="f255a-106">Өнімге негізделген келісім-шарт жолдары қолмен жасалған жолдар немесе олар өнім каталогындағы элементтер болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f255a-106">Product-based contract lines can be manually created lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="f255a-107">Өнім каталогы</span><span class="sxs-lookup"><span data-stu-id="f255a-107">Product catalog</span></span>

<span data-ttu-id="f255a-108">Өнім каталогындағы өнімдер әдепкі бірлік пен бірлік тобына ие.</span><span class="sxs-lookup"><span data-stu-id="f255a-108">The products in the product catalog have a default unit and unit group.</span></span> <span data-ttu-id="f255a-109">Егер бірнеше өнім бірдей атрибуттар жиынтығын ортақ пайдаланса, сол атрибуттарға ие өнім тобын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="f255a-109">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="f255a-110">Бір өнім тобындағы барлық өнімдер бірдей атрибуттар жиынтығын иеленеді.</span><span class="sxs-lookup"><span data-stu-id="f255a-110">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="f255a-111">Мысалы, компания түрлі бағдарламалық жасақтамаға жазылым лицензияларын сатады.</span><span class="sxs-lookup"><span data-stu-id="f255a-111">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="f255a-112">Барлық жазылым бағдарламалық жасақтамасында келесі екі атрибут бар:</span><span class="sxs-lookup"><span data-stu-id="f255a-112">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="f255a-113">Пайдаланушылар саны</span><span class="sxs-lookup"><span data-stu-id="f255a-113">Number of users</span></span>
- <span data-ttu-id="f255a-114">Жазылым ұзақтығы (айлар бойынша)</span><span class="sxs-lookup"><span data-stu-id="f255a-114">Subscription duration (in months)</span></span>

<span data-ttu-id="f255a-115">Каталогтың осы түрін сақтау үшін **Жазылым бағдарламалық жасақтамасы** деп аталатын өнімдер топтамасын құрыңыз.</span><span class="sxs-lookup"><span data-stu-id="f255a-115">To maintain this type of catalog, create a product family that is named **Subscription Software**.</span></span> <span data-ttu-id="f255a-116">Өнімдер топтамасына төлсипаттар, **Пайдаланушылар саны** және **Жазылым ұзақтығы** параметрлерін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f255a-116">Add the attributes, **Number of users** and **Subscription duration** to the product family.</span></span> <span data-ttu-id="f255a-117">Содан кейін **Жазылым бағдарламалық жасақтамасы** өнімдер топтамасына жеке өнімдерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f255a-117">Then, add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-contract"></a><span data-ttu-id="f255a-118">Жоба келісім-шартына өнім каталогының элементтерін қосу</span><span class="sxs-lookup"><span data-stu-id="f255a-118">Add product catalog items to a project Contract</span></span>

<span data-ttu-id="f255a-119">Жоба келісім-шарттары жолдың екі түріне арналған, жобаға және өнімге негізделген жолдар, бөлімдерге ие.</span><span class="sxs-lookup"><span data-stu-id="f255a-119">Project contracts have sections for two types of lines, project-based and product-based.</span></span> <span data-ttu-id="f255a-120">Өнімге негізделген жолдар келісім-шарттағы өнімнің бағатізбесіндегі барлық өнімдер мен бірліктерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="f255a-120">Product-based lines include all of the products and units in the product price list on the contract.</span></span> <span data-ttu-id="f255a-121">Келісім-шарт өнімінің бағатізбесіне кірмейтін өнімдерді қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="f255a-121">Products that aren't part of contract's product price list can be added.</span></span>

<span data-ttu-id="f255a-122">Сіз өнімдерді басқа бағатізбелерден немесе тікелей өнім каталогынан таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="f255a-122">You can select products from other price lists, or directly from the product catalog.</span></span> <span data-ttu-id="f255a-123">Өнімдерді тікелей өнім каталогынан таңдаған кезде, өнімнің сатылым бағасы үшін сол өнімнің бағатізбесі пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="f255a-123">When you select products directly from a product catalog, the default price list of that product is used for the product's sales price.</span></span> <span data-ttu-id="f255a-124">Әдепкі бағатізбе орнатылмаған болса, баға 0 (нөл) мәніне тең болады.</span><span class="sxs-lookup"><span data-stu-id="f255a-124">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="f255a-125">Егер келісім-шарт жолы өнім каталогына негізделсе, сатылым бағасын тікелей жолда алдын ала анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="f255a-125">If a contract line is based on a product catalog, you can override the sales price directly on the line.</span></span> <span data-ttu-id="f255a-126">Келісім-шарт жолы екі мәні бар **Бағалау** өрісіне ие:</span><span class="sxs-lookup"><span data-stu-id="f255a-126">A contract line has the **Pricing** field with the two values:</span></span>

- <span data-ttu-id="f255a-127">**Бағаны алдын ала анықтау**</span><span class="sxs-lookup"><span data-stu-id="f255a-127">**Override pricing**</span></span>
- <span data-ttu-id="f255a-128">**Әдепкіні пайдалану**</span><span class="sxs-lookup"><span data-stu-id="f255a-128">**Use default**</span></span>

<span data-ttu-id="f255a-129">Егер **Бағалау** өрісін **Бағаны алдын ала анықтау** параметріне орнатсаңыз, әдепкі баға орнатылмайды.</span><span class="sxs-lookup"><span data-stu-id="f255a-129">If you set the **Pricing** field to **Override pricing** , the default price isn't set.</span></span> <span data-ttu-id="f255a-130">Келісім-шарт жолындағы өнім үшін баға енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f255a-130">Enter a price for the product on the contract line.</span></span> <span data-ttu-id="f255a-131">Егер өрісті **Әдепкі бойынша пайдалану** мәніне орнатсаңыз, әдепкі сатылым бағасы пайдаланылады және өрісті өңдеу мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="f255a-131">If you set the field to **Use default** , the default sales price is used and the field can't be edited.</span></span>

<span data-ttu-id="f255a-132">Project Operations бағдарламасын орнатқаннан кейін, әдепкі сатылым бағасы келісім-шарттағы өнімге негізделген жолдарға енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="f255a-132">After you install Project Operations, default sales prices are entered on the product-based lines on a contract.</span></span> <span data-ttu-id="f255a-133">**Бағалау** өрісі **Бағаны алдын ала анықтау** параметріне орнатылады, сонда келісім-шарт жолдарында әдепкі бағаны өңдей аласыз.</span><span class="sxs-lookup"><span data-stu-id="f255a-133">The **Pricing** field is set to **Override pricing** so that you can edit the default price on the contract lines.</span></span> <span data-ttu-id="f255a-134">Бұл Dynamics 365 Sales бағдарламасындағы өнімге негізделген жолдар әрекетіне арналған Project Operations бағдарламасына тән алдын ала анықтау.</span><span class="sxs-lookup"><span data-stu-id="f255a-134">This is a Project Operations-specific override to product-based lines behavior in Dynamics 365 Sales.</span></span>
