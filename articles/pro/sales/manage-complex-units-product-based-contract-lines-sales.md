---
title: Өнімге негізделген келісім-шарт жолдары үшін күрделі бірліктерді басқару - жеңілдетілген
description: Бұл тақырып жазылымға негізделген өнімдерді сатуды қолдау туралы ақпарат береді.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 029d2aa4fd20fc036a34ae6136fe12454f3b7703
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273340"
---
# <a name="manage-complex-units-for-product-based-contract-lines---lite"></a><span data-ttu-id="08d2c-103">Өнімге негізделген келісім-шарт жолдары үшін күрделі бірліктерді басқару - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="08d2c-103">Manage complex units for product-based contract lines - lite</span></span>

<span data-ttu-id="08d2c-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="08d2c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="08d2c-105">Dynamics 365 Project Operations бағдарламасы жазылымға негізделген өнімдерді сату мүмкіндігін қолдау үшін сандық факторларды пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="08d2c-106">Жазылымға негізделген өнімдер үшін келісім-шарт жолындағы сан немесе жоба келісім-шартының жолы пайдаланушы айларының санымен көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="08d2c-106">For subscription-based products, the quantity on the contract or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="08d2c-107">Жазылым бағдарламалық жасақтамасының бағасы каталогта бір айға берілетін бір пайдаланушыға арналған баға ретінде сақталады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-107">The price of subscription software is stored in the catalog as the price per-user, per-month.</span></span> <span data-ttu-id="08d2c-108">Сатылым процесінде келісім-шарт жолындағы баға, әдетте, бір пайдаланушыға арналған, АТ бөлімінің сатылым агенті арқылы келісілген және жеңілдікпен есептелген бір айлық баға болып табылады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-108">During the sales process, the price on the contract line is usually the per-user, per-month price that was negotiated and discounted by the sales agent.</span></span> <span data-ttu-id="08d2c-109">Әр мәміледе пайдаланушылар саны мен жазылу айлары әртүрлі болады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="08d2c-110">Келісім-шарт жолының мөлшерін есептеу үшін пайдаланылатын сан — пайдаланушылар саны мен жазылу айлары санының көбейтіндісі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-110">The quantity used to calculate the amount of the contract line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="08d2c-111">Сатылымның бұл түрін қолдау үшін Project Operations бағдарламасы *сандық факторлар* ұғымына қолдау көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="08d2c-111">To support this type of sale, Project Operations supports the concept of *quantity factors*.</span></span> <span data-ttu-id="08d2c-112">Мөлшер коэффициенттері өнім төлсипаттарына тәуелді.</span><span class="sxs-lookup"><span data-stu-id="08d2c-112">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="08d2c-113">Өнім үшін арнайы сипаттарды конфигурациялаған кезде, сол сипаттардың жиынтығын немесе барлық сипаттарды мөлшер коэффициенттері ретінде белгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-113">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="08d2c-114">Project Operations бағдарламасы сандық деректер түрі бар сандық сипаттар немесе өнім сипаттарының сандық фактор ретінде белгіленетінін тексереді.</span><span class="sxs-lookup"><span data-stu-id="08d2c-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="08d2c-115">Конфигурацияланған мөлшер факторлары бар өнім келісім-шарт жолына қосылған кезде, **Саны** өрісі тек оқуға арналған түріне айналады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-115">When a product with configured quantity factors is added to a contract line, the **Quantity** field  becomes read-only.</span></span> <span data-ttu-id="08d2c-116">Сандық фактор болып табылатын өнім сипаттарының мәндерін енгізгеннен кейін, Project Operations бағдарламасы келісім-шарт жолының санын есептейді.</span><span class="sxs-lookup"><span data-stu-id="08d2c-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the contract line.</span></span>

<span data-ttu-id="08d2c-117">Мысалы, Dynamics 365 Sales жүйесі келесі сипаттарға ие болуы мүмкін:</span><span class="sxs-lookup"><span data-stu-id="08d2c-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="08d2c-118">**Пайдаланушылар саны**: пайдаланушылар саны.</span><span class="sxs-lookup"><span data-stu-id="08d2c-118">**No of users**: The number of users.</span></span>
- <span data-ttu-id="08d2c-119">**Айлар саны**: жазылым айларының саны.</span><span class="sxs-lookup"><span data-stu-id="08d2c-119">**No of Months**: The number of subscription months.</span></span>
- <span data-ttu-id="08d2c-120">**Өнім SKU**: өнім үшін қоймада сақтау бірлігі (SKU).</span><span class="sxs-lookup"><span data-stu-id="08d2c-120">**Product SKU**: The stock keeping unit (SKU) for the product.</span></span>

<span data-ttu-id="08d2c-121">**Пайдаланушылар саны** және **Айлар саны** сипаттарын өнім желісінің сипаттарын өңдеу арқылы мөлшер коэффициенттері ретінде белгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-121">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="08d2c-122">Өнім қасиеттерінен мөлшерлік факторларды құру үшін келесі әрекеттерді орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="08d2c-122">To create quantity factors from product properties, complete the following steps.</span></span>

1. <span data-ttu-id="08d2c-123">**Project Operations** бағдарламасында **Сатылым өнімдері** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="08d2c-123">On the **Project Operations**, select **Sales-Products**.</span></span>
2. <span data-ttu-id="08d2c-124">Сандық факторларды орнату үшін қажетті өнімді ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="08d2c-124">Open the product for which you need to set up quantity factors.</span></span> <span data-ttu-id="08d2c-125">Өнім қасиеттерінің орнатылғанына көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="08d2c-125">Make sure that the product has properties already set up.</span></span>
3. <span data-ttu-id="08d2c-126">**Жоба туралы ақпарат** бетінде **Сандық факторлар** қойындысын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="08d2c-126">On the **Project Information** page, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="08d2c-127">Қосалқы торда **+ Жаңа өріс есептеуі** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="08d2c-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="08d2c-128">**Сандық фактор** атауын енгізіп, өріс есептеуіне салыстырылатын сипат мәнін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="08d2c-128">Enter the name of the **Quantity Factor** and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="08d2c-129">Пішінді сақтау және жабу.</span><span class="sxs-lookup"><span data-stu-id="08d2c-129">Save and close the form.</span></span>
7. <span data-ttu-id="08d2c-130">Өнімге негізделген келісім-шарт жолының санын құрайтын барлық қасиеттер үшін 2-6 қадамдарын қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="08d2c-130">Repeat steps 2-6 for all the properties that together will make up the quantity for the product-based contract line.</span></span>

<span data-ttu-id="08d2c-131">Сандық факторлар орнатылған кезде, пайдаланушы осы өнім үшін келісім-шарт жолын жасаған кезде, келісім-шарт жолының саны бұғатталады.</span><span class="sxs-lookup"><span data-stu-id="08d2c-131">With quantity factors set up, when the user creates a contract line for this product, the quantity of the contract line is locked.</span></span> <span data-ttu-id="08d2c-132">Содан кейін ол сан осы келісім-шарт жолы үшін меншік мәндерінің көбейтіндісі ретінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="08d2c-132">The quantity is then calculated as a product of the property values for that contract line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]