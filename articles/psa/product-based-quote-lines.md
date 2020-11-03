---
title: Өнімге негізделген баға ұсыну жолдары
description: Бұл тақырыпта өнімге негізделген баға ұсыну жолдары туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
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
ms.openlocfilehash: 55a5b5041a494892e6d96bf24e1bc132a26521dc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079840"
---
# <a name="product-based-quote-lines"></a><span data-ttu-id="2f6ea-103">Өнімге негізделген баға ұсыну жолдары</span><span class="sxs-lookup"><span data-stu-id="2f6ea-103">Product-based quote lines</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


<span data-ttu-id="2f6ea-104">Dynamics 365 Project Service Automation бағдарламасында өнімге негізделген баға ұсыну жолдарын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-104">You can create product-based quote lines in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="2f6ea-105">Өнімге негізделген баға ұсыну жолдары "енгізілген" жолдар немесе олар өнім каталогындағы элементтер болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-105">Product-based quote lines can be "write-in" lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="2f6ea-106">Өнім каталогы</span><span class="sxs-lookup"><span data-stu-id="2f6ea-106">Product catalog</span></span>

<span data-ttu-id="2f6ea-107">Dynamics 365 өнім каталогындағы өнімдер әдепкі бірлік пен бірлік тобына ие.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-107">The products in a Dynamics 365 product catalog have a default unit and unit group.</span></span> <span data-ttu-id="2f6ea-108">Егер бірнеше өнім бірдей атрибуттар жиынтығын ортақ пайдаланса, сол атрибуттарға ие өнім тобын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-108">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="2f6ea-109">Бір өнім тобындағы барлық өнімдер бірдей атрибуттар жиынтығын иеленеді.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-109">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="2f6ea-110">Мысалы, компания түрлі бағдарламалық жасақтамаға жазылым лицензияларын сатады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-110">For example, a company sells subscription licenses for a variety of software.</span></span> <span data-ttu-id="2f6ea-111">Барлық жазылым бағдарламалық жасақтамасында келесі екі атрибут бар:</span><span class="sxs-lookup"><span data-stu-id="2f6ea-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="2f6ea-112">Пайдаланушылар саны</span><span class="sxs-lookup"><span data-stu-id="2f6ea-112">Number of users</span></span> 
- <span data-ttu-id="2f6ea-113">Жазылым ұзақтығы (айлар бойынша)</span><span class="sxs-lookup"><span data-stu-id="2f6ea-113">Subscription duration (in months)</span></span>

<span data-ttu-id="2f6ea-114">Каталогтың бұл түрін сақтаудың жақсы тәсілі — **Жазылым бағдарламалық жасақтамасы** деп аталатын және атрибуттар ретінде **Пайдаланушылар саны** және **Жазылым ұзақтығы** бар өнім тобын құру.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-114">A good way to maintain this type of catalog is to create a product family that is named **Subscription Software** , and that has **Number of users** and **Subscription duration** as attributes.</span></span> <span data-ttu-id="2f6ea-115">Содан кейін **Жазылым бағдарламалық жасақтамасы** өнім тобына **Dynamics 365 Sales** немесе **Dynamics 365 Field Service** сияқты жеке өнімдерді қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-115">You can then add individual products, such as **Dynamics 365 Sales** or **Dynamics 365 Field Service** to the **Subscription Software** product family.</span></span>

## <a name="adding-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="2f6ea-116">Жобалық баға ұсыну жолына өнім каталогының элементтерін қосу</span><span class="sxs-lookup"><span data-stu-id="2f6ea-116">Adding product catalog items to a project quote</span></span>

<span data-ttu-id="2f6ea-117">Жобаның баға ұсыну жолы мен жоба келісім-шартының беттерінде жолдың екі түріне арналған бөлімдер бар: жобаға және өнімге негізделген жолдар.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-117">Project quote and project contract pages have sections for two types of lines: project-based lines and product-based lines.</span></span> <span data-ttu-id="2f6ea-118">Өнімге негізделген жолдар үшін Dynamics 365 жүйесі өнім каталогындағы элементтерді баға ұсыну жолына қосу үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-118">For product-based lines, Dynamics 365 is used to add items from a product catalog to a quote.</span></span> <span data-ttu-id="2f6ea-119">Баға ұсыну жолындағы немесе жоба келісім-шартының жолындағы ашылмалы тізімге баға ұсыну жолына немесе жоба келісім-шартына тіркелген өнім бойынша бағатізбедегі барлық өнімдер мен бірліктер кіреді.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-119">The drop-down list on the quote line or project contract line includes all the products and units in the product price list that is attached to the quote or project contract.</span></span> <span data-ttu-id="2f6ea-120">Сондай-ақ баға ұсыну жолының өнім бойынша бағатізбесіне кірмейтін өнімдерді қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-120">You can also add products that aren't part of quote's product price list.</span></span>

<span data-ttu-id="2f6ea-121">Сонымен қатар басқа бағатізбелерден өнімдерді таңдай аласыз немесе өнімдерді тікелей өнім каталогынан таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-121">Additionally, you can select products from other price lists, or you can select products directly from the product catalog.</span></span> <span data-ttu-id="2f6ea-122">Өнімдерді тікелей өнім каталогынан таңдаған кезде, өнімнің сатылым бағасын алу үшін сол өнімнің бағатізбесі пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-122">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="2f6ea-123">Әдепкі бағатізбе орнатылмаған болса, баға 0 (нөл) мәніне тең болады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-123">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="2f6ea-124">Егер баға ұсыну жолы өнім каталогына негізделсе, сатылым бағасын тікелей баға ұсыну жолында алдын ала анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-124">If a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="2f6ea-125">Dynamics 365 жүйесіндегі баға ұсыну жолында **Баға белгілеу** өрісінің барын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-125">Note that a quote line in Dynamics 365 has a **Pricing** field.</span></span> <span data-ttu-id="2f6ea-126">Екі мән қолжетімді:</span><span class="sxs-lookup"><span data-stu-id="2f6ea-126">Two values are available:</span></span>

- <span data-ttu-id="2f6ea-127">Бағаны алдын ала анықтау</span><span class="sxs-lookup"><span data-stu-id="2f6ea-127">Override pricing</span></span>  
- <span data-ttu-id="2f6ea-128">Әдепкіні пайдалану</span><span class="sxs-lookup"><span data-stu-id="2f6ea-128">Use default</span></span>

<span data-ttu-id="2f6ea-129">Егер осы өрісті **Бағаны алдын ала анықтау** параметріне орнатсаңыз, Dynamics 365 жүйесі әдепкі бағаны орнатпайды.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-129">If you set this field to **Override pricing** , Dynamics 365 doesn't set a default price.</span></span> <span data-ttu-id="2f6ea-130">Баға ұсыну жолындағы өнім бағасын енгізу керек.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-130">You must enter a price for the product on the quote line.</span></span> <span data-ttu-id="2f6ea-131">Егер осы өрісті **Әдепкіні пайдалану** параметріне орнатсаңыз, Dynamics 365 жүйесі әдепкі сатылым бағасын қолданады және өңдеуді болдырмау үшін өрісті құлыптайды.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-131">If you set this field to **Use default** , Dynamics 365 uses the default sales price and locks the field to prevent editing.</span></span>

<span data-ttu-id="2f6ea-132">PSA бағдарламасын орнатқаннан кейін, әдепкі сатылым бағасы баға ұсыну жолындағы өнімге негізделген жолдарға енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-132">After you install PSA, default sales prices are entered on the product-based lines on a quote.</span></span> <span data-ttu-id="2f6ea-133">Содан кейін **Баға белгілеу** өрісі **Бағаны алдын ала анықтау** параметріне орнатылады, сонда баға ұсыну жолдарында әдепкі бағаны өңдей аласыз.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-133">The **Pricing** field is then set to **Override pricing** so that you can edit the default price on the quote lines.</span></span>

> ![Бағаны алдын ала анықтауды орнату](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a><span data-ttu-id="2f6ea-135">Өнімдердің сандық факторлары</span><span class="sxs-lookup"><span data-stu-id="2f6ea-135">Quantity factors for products</span></span>

<span data-ttu-id="2f6ea-136">PSA бағдарламасы жазылымға негізделген өнімдерді сату мүмкіндігін қолдау үшін сандық факторларды қолданады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-136">PSA uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="2f6ea-137">Жазылымға негізделген өнімдер үшін баға ұсыну жолындағы сан немесе жоба келісім-шартының жолы пайдаланушы айларының санымен көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-137">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="2f6ea-138">Әдетте, жазылым бағдарламалық жасақтамасының бағасы каталогта бір айға берілетін бір пайдаланушыға арналған баға ретінде сақталады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-138">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="2f6ea-139">Алайда, оның орнына басқа уақыт сипаттамаларын қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-139">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="2f6ea-140">Сатылым процесінде баға ұсыну жолындағы баға, әдетте, бір пайдаланушыға арналған, АТ бөлімінің сатылым агенті арқылы келісілген және жеңілдікпен есептелген бір айлық баға болып табылады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-140">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="2f6ea-141">Әр мәміледе пайдаланушылар саны мен жазылу айлары әртүрлі болады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-141">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="2f6ea-142">Баға ұсыну жолының мөлшерін есептеу үшін пайдаланылатын сан пайдаланушылар саны мен жазылу айлары санының көбейтіндісі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-142">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="2f6ea-143">Сатылымның бұл түрін қолдау үшін, PSA бағдарламасы сандық факторлар ұғымын енгізді.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-143">To support this type of sale, PSA introduced the concept of quantity factors.</span></span> <span data-ttu-id="2f6ea-144">Сандық факторлар Dynamics 365 жүйесінде өнім атрибуттарына сүйенеді.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-144">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="2f6ea-145">Өнімнің белгілі бір сипаттарын конфигурациялаған кезде, PSA бағдарламасы сандық факторлар ретінде сол сипаттардың жиынтығын немесе барлық сипаттарды белгілеуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-145">When you configure specific properties for a product, PSA lets you flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="2f6ea-146">PSA бағдарламасы сандық деректер түрі бар сандық сипаттар немесе өнім сипаттарының сандық фактор ретінде белгіленетінін тексереді.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-146">PSA validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="2f6ea-147">Сандық факторлар конфигурацияланған өнім баға ұсыну жолына қосылғанда, баға ұсыну жолындағы **Саны** өрісі тек оқуға арналған өріске айналады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-147">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="2f6ea-148">Сандық фактор болып табылатын өнім сипаттарының мәндерін енгізгеннен кейін, PSA бағдарламасы баға ұсыну жолының санын есептейді.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-148">After you enter values for product properties that are quantity factors, PSA computes the quantity of the quote line.</span></span>

<span data-ttu-id="2f6ea-149">Мысалы, Dynamics 365 жүйесі келесі сипаттарға ие болуы мүмкін:</span><span class="sxs-lookup"><span data-stu-id="2f6ea-149">For example, Dynamics 365 might have the following properties:</span></span> 

- <span data-ttu-id="2f6ea-150">**Пайдаланушылар №** - пайдаланушылар саны</span><span class="sxs-lookup"><span data-stu-id="2f6ea-150">**No of users** - The number of users</span></span> 
- <span data-ttu-id="2f6ea-151">**Айлар №** - жазылу айларының саны</span><span class="sxs-lookup"><span data-stu-id="2f6ea-151">**No of Months** - The number of subscription months</span></span>
- <span data-ttu-id="2f6ea-152">**Өнімнің SKU нөмірі**</span><span class="sxs-lookup"><span data-stu-id="2f6ea-152">**Product SKU**</span></span> 

<span data-ttu-id="2f6ea-153">**Пайдаланушылар №** және **Айлар №** сипаттарын өнім жолын өңдеу арқылы сандық факторлар ретінде белгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="2f6ea-153">Tne **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 

> ![Пайдаланушылар және айлар санын сапа факторлары ретінде белгілеу](media/basic-guide-11.png)
 
