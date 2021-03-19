---
title: Ресурс болжамдары
description: Бұл тақырыпта Project Operations бағдарламасындағы ресурс бағалауларының есептелу жолы туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 98a61746f172b50bf6fa29cb0d21462cd616f417
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286525"
---
# <a name="resource-estimates"></a><span data-ttu-id="bbde4-103">Ресурс болжамдары</span><span class="sxs-lookup"><span data-stu-id="bbde4-103">Resource estimates</span></span>

<span data-ttu-id="bbde4-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="bbde4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bbde4-105">Ресурстарды бағалау жұмыс бағасының қолданыстағы өлшемдерімен бірге жұмыс декомпозициясының құрылымында анықталған кезең-кезеңмен жүргізілетін күш-жігердің негізінде жүргізіледі.</span><span class="sxs-lookup"><span data-stu-id="bbde4-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="bbde4-106">Әдетте, есептеу **әр x сағат рөлі үшін баға/сағат** болып табылады.</span><span class="sxs-lookup"><span data-stu-id="bbde4-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="bbde4-107">Әрбір ресурсқа арналған кезең-кезеңмен бөлінген күш-жігер ресурстарды тағайындау жазбасында сақталады.</span><span class="sxs-lookup"><span data-stu-id="bbde4-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="bbde4-108">Бағаны белгілеу алдын ала анықталған бағатізбеде сақталады.</span><span class="sxs-lookup"><span data-stu-id="bbde4-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="bbde4-109">Бірлікті түрлендіру қолданыстағы бағатізбе негізінде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="bbde4-109">Unit conversion is applied based on the applicable price list.</span></span>

![Ресурс болжамдары](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="bbde4-111">Әдепкі өзіндік құны және құн валютасы</span><span class="sxs-lookup"><span data-stu-id="bbde4-111">Default cost price and cost currency</span></span>

<span data-ttu-id="bbde4-112">Өзіндік құн әдепкі бойынша ұйымдық бөлімшемен анықталады.</span><span class="sxs-lookup"><span data-stu-id="bbde4-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="bbde4-113">Әдепкі шығынның вексель мөлшерлемесі және сатылым валютасы</span><span class="sxs-lookup"><span data-stu-id="bbde4-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="bbde4-114">Сатылым бағалары әр мәмілеге бір рет қолданылады.</span><span class="sxs-lookup"><span data-stu-id="bbde4-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="bbde4-115">Әдепкі бойынша сатылым бағатізбесінің иерархиясы келесідей:</span><span class="sxs-lookup"><span data-stu-id="bbde4-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="bbde4-116">ұйым</span><span class="sxs-lookup"><span data-stu-id="bbde4-116">Organization</span></span>
2. <span data-ttu-id="bbde4-117">Тұтынушы</span><span class="sxs-lookup"><span data-stu-id="bbde4-117">Customer</span></span>
3. <span data-ttu-id="bbde4-118">Баға ұсыну/келісім-шарт</span><span class="sxs-lookup"><span data-stu-id="bbde4-118">Quote/contract</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]