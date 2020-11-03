---
title: Ресурс болжамдары
description: Бұл тақырыпта Project Operations бағдарламасындағы ресурс бағалауларының есептелу жолы туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079580"
---
# <a name="resource-estimates"></a><span data-ttu-id="83eea-103">Ресурс болжамдары</span><span class="sxs-lookup"><span data-stu-id="83eea-103">Resource estimates</span></span>

<span data-ttu-id="83eea-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="83eea-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="83eea-105">Ресурстарды бағалау жұмыс бағасының қолданыстағы өлшемдерімен бірге жұмыс декомпозициясының құрылымында анықталған кезең-кезеңмен жүргізілетін күш-жігердің негізінде жүргізіледі.</span><span class="sxs-lookup"><span data-stu-id="83eea-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="83eea-106">Әдетте, есептеу **әр x сағат рөлі үшін баға/сағат** болып табылады.</span><span class="sxs-lookup"><span data-stu-id="83eea-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="83eea-107">Әрбір ресурсқа арналған кезең-кезеңмен бөлінген күш-жігер ресурстарды тағайындау жазбасында сақталады.</span><span class="sxs-lookup"><span data-stu-id="83eea-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="83eea-108">Бағаны белгілеу алдын ала анықталған бағатізбеде сақталады.</span><span class="sxs-lookup"><span data-stu-id="83eea-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="83eea-109">Бірлікті түрлендіру қолданыстағы бағатізбе негізінде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="83eea-109">Unit conversion is applied based on the applicable price list.</span></span>

![Ресурс болжамдары](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="83eea-111">Әдепкі өзіндік құны және құн валютасы</span><span class="sxs-lookup"><span data-stu-id="83eea-111">Default cost price and cost currency</span></span>

<span data-ttu-id="83eea-112">Өзіндік құн әдепкі бойынша ұйымдық бөлімшемен анықталады.</span><span class="sxs-lookup"><span data-stu-id="83eea-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="83eea-113">Әдепкі шығынның вексель мөлшерлемесі және сатылым валютасы</span><span class="sxs-lookup"><span data-stu-id="83eea-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="83eea-114">Сатылым бағалары әр мәмілеге бір рет қолданылады.</span><span class="sxs-lookup"><span data-stu-id="83eea-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="83eea-115">Әдепкі бойынша сатылым бағатізбесінің иерархиясы келесідей:</span><span class="sxs-lookup"><span data-stu-id="83eea-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="83eea-116">ұйым</span><span class="sxs-lookup"><span data-stu-id="83eea-116">Organization</span></span>
2. <span data-ttu-id="83eea-117">Тұтынушы</span><span class="sxs-lookup"><span data-stu-id="83eea-117">Customer</span></span>
3. <span data-ttu-id="83eea-118">Баға ұсыну/келісім-шарт</span><span class="sxs-lookup"><span data-stu-id="83eea-118">Quote/contract</span></span>
