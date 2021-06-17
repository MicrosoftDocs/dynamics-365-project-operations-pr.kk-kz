---
title: Өнімге негізделген баға ұсыну жолдарына шолу - жеңілдетілген
description: Бұл тақырыпта өнімге негізделген баға ұсынысы жолдарымен жұмыс істеу туралы ақпарат берілген.
author: rumant
ms.date: 10/30/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5cc3a97194e01b14de054a93a6268c1f0c24bc25
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994458"
---
# <a name="product-based-quote-lines-overview---lite"></a><span data-ttu-id="4ddc0-103">Өнімге негізделген баға ұсыну жолдарына шолу - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="4ddc0-103">Product-based quote lines overview - lite</span></span>

<span data-ttu-id="4ddc0-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="4ddc0-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4ddc0-105">Dynamics 365 Project Operations бағдарламасында өнімге негізделген баға ұсыну жолдарын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-105">You can create product-based quote lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="4ddc0-106">Өнімге негізделген баға ұсыну жолдарын қолмен қосуға болады немесе олар өнім каталогындағы элементтер болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-106">Product-based quote lines can be manually added, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="4ddc0-107">Өнім каталогы</span><span class="sxs-lookup"><span data-stu-id="4ddc0-107">Product catalog</span></span>

<span data-ttu-id="4ddc0-108">Өнім каталогындағы әрбір өнімнің әдепкі бірлігі мен бірлік тобы бар.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-108">Each product in the product catalog has a default unit and unit group.</span></span> <span data-ttu-id="4ddc0-109">Егер бірнеше өнім бірдей атрибуттар жиынтығын ортақ пайдаланса, сол төлсипаттарды ортақ пайдаланатын өнім тобын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-109">If multiple products share the same set of attributes, you can create a product family that share those attributes.</span></span> 

<span data-ttu-id="4ddc0-110">Мысалы, компания түрлі бағдарламалық жасақтамаға жазылым лицензияларын сатады.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-110">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="4ddc0-111">Барлық жазылым бағдарламалық жасақтамасында келесі екі атрибут бар:</span><span class="sxs-lookup"><span data-stu-id="4ddc0-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="4ddc0-112">Пайдаланушылар саны</span><span class="sxs-lookup"><span data-stu-id="4ddc0-112">Number of users</span></span>
- <span data-ttu-id="4ddc0-113">Аймен өлшенетін жазылым ұзақтығы</span><span class="sxs-lookup"><span data-stu-id="4ddc0-113">A subscription duration measured in months</span></span>

<span data-ttu-id="4ddc0-114">Каталогтың бұл түрін сақтау үшін **Жазылым бағдарламалық жасақтамасы** деп аталатын өнім тобын жасап, төлсипаттар ретінде пайдаланушылар санын және жазылым ұзақтығын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-114">To maintain this type of catalog, create a product family named **Subscription Software** and add the number of users and the subscription duration as attributes.</span></span> <span data-ttu-id="4ddc0-115">Әрі қарай, **Жазылым бағдарламалық жасақтамасы** өнім тобына жеке өнімдерді қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-115">Next, you can add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="4ddc0-116">Жобалық баға ұсыну жолына өнім каталогының элементтерін қосу</span><span class="sxs-lookup"><span data-stu-id="4ddc0-116">Add product catalog items to a project quote</span></span>

<span data-ttu-id="4ddc0-117">**Жобалық баға ұсынысы** және **Жобалық келісім-шарт** беттерінде жобаға негізделген жолдар мен өнімге негізделген жолдарға арналған бөлімдер бар.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-117">The **Project Quote** and **Project Contract** pages have sections for project-based lines and product-based lines.</span></span> <span data-ttu-id="4ddc0-118">Өнімге негізделген жолдарда баға ұсыну жолындағы немесе жоба келісім-шартының жолындағы ашылмалы тізімге өнім бойынша бағатізбедегі барлық өнімдер мен бірліктер кіреді.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-118">For product-based lines, the drop-down list on the quote line or project contract line includes all the products and units in the product price list.</span></span> <span data-ttu-id="4ddc0-119">Сондай-ақ өнім бағатізбесіне кірмейтін өнімдерді қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-119">You can also add products that aren't part of the product price list.</span></span>

<span data-ttu-id="4ddc0-120">Сонымен қатар өнімдерді басқа бағатізбелерден немесе тікелей өнім каталогынан қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-120">Additionally, you can select products from other price lists or directly from the product catalog.</span></span> <span data-ttu-id="4ddc0-121">Өнімдерді тікелей өнім каталогынан таңдаған кезде, өнімнің сатылым бағасын алу үшін сол өнімнің бағатізбесі пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-121">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="4ddc0-122">Әдепкі бағатізбе орнатылмаған болса, баға нөл (0) мәніне тең болады.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-122">If a default price list isn't set, the price is set to zero (0).</span></span>

<span data-ttu-id="4ddc0-123">Баға ұсыну жолы өнім каталогына негізделгенде, сатылым бағасын тікелей баға ұсыну жолында алдын ала анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-123">When a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="4ddc0-124">Екі қолжетімді мәні бар **Баға** өрісіндегі баға ұсыну жолы:</span><span class="sxs-lookup"><span data-stu-id="4ddc0-124">A quote line in **Pricing** field with two available values:</span></span>

- <span data-ttu-id="4ddc0-125">**Бағаны алдын ала анықтау**</span><span class="sxs-lookup"><span data-stu-id="4ddc0-125">**Override Pricing**</span></span>
- <span data-ttu-id="4ddc0-126">**Әдепкіні пайдалану**</span><span class="sxs-lookup"><span data-stu-id="4ddc0-126">**Use Default**</span></span>

<span data-ttu-id="4ddc0-127">Егер **Бағаны алдын ала анықтау** опциясын таңдасаңыз, әдепкі баға орнатылмайды.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-127">If you select **Override Pricing**, the default price isn't set.</span></span> <span data-ttu-id="4ddc0-128">Оның орнына, баға ұсыну жолындағы өнім бағасын енгізу керек.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-128">Instead, you must enter a price for the product on the quote line.</span></span> <span data-ttu-id="4ddc0-129">**Әдепкі параметрді пайдалану** опциясын таңдасаңыз, әдепкі сату бағасы пайдаланылады және өріс өңдеуге құлыпталады.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-129">If you select **Use Default**, the default sales price is used and the field is locked for editing.</span></span>

<span data-ttu-id="4ddc0-130">Әдепкі сатылым бағасы баға ұсыну жолының өнімге негізделген жолдарына енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-130">Default sales prices are entered on the product-based lines of a quote.</span></span> <span data-ttu-id="4ddc0-131">Содан кейін **Баға белгілеу** өрісі **Бағаны алдын ала анықтау** параметріне орнатылады, сонда баға ұсыну жолдарында әдепкі бағаны өңдей аласыз.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-131">The **Pricing** field is then set to **Override Pricing** so that you can edit the default price on the quote lines.</span></span> <span data-ttu-id="4ddc0-132">Бұл – Project Operations жүйесіне арналған Dynamics 365 Sales жүйесіндегі өнімге негізделген жолдар тәртібін алдын ала анықтау.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-132">This is a Project Operations-specific override to the product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]