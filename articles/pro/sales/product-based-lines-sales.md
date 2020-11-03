---
title: Өнімге негізделген мүмкіндік жолдары
description: Бұл тақырыпта Project Operations бағдарламасындағы өнімге негізделген мүмкіндік жолдарының элементтері туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 17ffcf8dc94d42102115281d281d6b553cf1fa17
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079586"
---
# <a name="product-based-opportunity-lines"></a><span data-ttu-id="c953e-103">Өнімге негізделген мүмкіндік жолдары</span><span class="sxs-lookup"><span data-stu-id="c953e-103">Product-based opportunity lines</span></span>

<span data-ttu-id="c953e-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="c953e-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c953e-105">Өнімге негізделген мүмкіндіктер жолдары - бұл Мүмкіндіктегі жол элементтері.</span><span class="sxs-lookup"><span data-stu-id="c953e-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="c953e-106">Бұл жолдар тұтынушыға басқа қосымша қызметтерсіз түпкілікті есеп-шотта нақты жол элементтері ретінде жеткізіледі.</span><span class="sxs-lookup"><span data-stu-id="c953e-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="c953e-107">Байланысқан шығындар мен тұтынулар байланысты жобалардың тапсырмалары бойынша бақыланбайды.</span><span class="sxs-lookup"><span data-stu-id="c953e-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="c953e-108">Өнімге негізделген жолдар каталог элементтері немесе енгізілген өнімдер болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="c953e-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="c953e-109">Мүмкіндік өніміне негізделген жолдардағы функционалды мүмкіндіктердің көпшілігі Dynamics 365 Sales бағдарламасы ұсынған функционалды мүмкіндіктерге сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="c953e-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="c953e-110">Өнімге негізделген мүмкіндік жолдары туралы қосымша ақпаратты келесі бөлімнен қараңыз: [Мүмкіндікке өнімдер қосу](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="c953e-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="c953e-111">Жобаға негізделген мүмкіндіктерге тән өнімге негізделген мүмкіндік жолдары туралы бір тұжырымдама — **Тұтынушы бюджеті**.</span><span class="sxs-lookup"><span data-stu-id="c953e-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="c953e-112">Бұл өрісті тұтынушы жол элементі үшін төлеуге дайын соманы бақылау үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="c953e-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="c953e-113">Егер Мүмкіндіктер жиынтығының табыс әдісі **Жүйе арқылы есептелген** күйге орнатылған болса, болжамды табысты есептеу үшін өнімге және жобаға негізделген жолдар бойынша тұтынушы бюджетінің мәндері жинақталады.</span><span class="sxs-lookup"><span data-stu-id="c953e-113">If the revenue method of the Opportunity summary is set to **System Calculated** , the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
