---
title: Баға ұсынудың, баға белгілеудің және есеп-шот ұсынуға арналған негізгі нұсқаулық
description: Бұл тақырыпта Project Service Automation бағдарламасындағы негізгі баға ұсыну, баға белгілеу және шот ұсыну туралы ақпарат берілген.
author: kfend
ms.custom:
- dyn365-projectservice
ms.date: 2/14/2019
ms.topic: article
ms.author: kfend
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 7ec1170a7a703d181be4aa95daf7927bbe30b1b1
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6007463"
---
# <a name="basic-guide-to-quoting-pricing-and-billing"></a><span data-ttu-id="2b4a2-103">Баға ұсынудың, баға белгілеудің және есеп-шот ұсынуға арналған негізгі нұсқаулық</span><span class="sxs-lookup"><span data-stu-id="2b4a2-103">Basic guide to quoting, pricing and billing</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="2b4a2-104">Тиісті уақытта тиісті ресурстарды табу, сол ресурстарды жобада тіркеу және оларды пайдалану ұйымдарға табыс мақсаттары мен тұтынушы қанағаттанушылығы мақсаттарына жету үшін көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="2b4a2-104">The ability to find the right resources at the right time, book those resources on projects, and keep resources utilized helps organizations meet revenue targets and customer satisfaction goals.</span></span> 

<span data-ttu-id="2b4a2-105">Бұрын осы тақырыпта болған PDF сілтемесі жойылып, мазмұны келесі тақырыптарға ауыстырылды:</span><span class="sxs-lookup"><span data-stu-id="2b4a2-105">The PDF link that was previously in this topic has been removed and the content has been moved to the following topics:</span></span>

- [<span data-ttu-id="2b4a2-106">Баға белгілеу және есеп-шот ұсыну</span><span class="sxs-lookup"><span data-stu-id="2b4a2-106">Quoting, pricing, and billing</span></span>](../quote-bill-price.md)
- [<span data-ttu-id="2b4a2-107">Сатылым процестері</span><span class="sxs-lookup"><span data-stu-id="2b4a2-107">Sales processes</span></span>](../basic-sales-process.md)
- [<span data-ttu-id="2b4a2-108">Баға ұсыныстары және баға ұсыну жолдары</span><span class="sxs-lookup"><span data-stu-id="2b4a2-108">Quotes and quote lines</span></span>](../basic-quote-lines.md)
- [<span data-ttu-id="2b4a2-109">Өнімге негізделген баға ұсыну жолдары</span><span class="sxs-lookup"><span data-stu-id="2b4a2-109">Product-based quote lines</span></span>](../product-based-quote-lines.md)
- [<span data-ttu-id="2b4a2-110">Баға белгілеу</span><span class="sxs-lookup"><span data-stu-id="2b4a2-110">Pricing</span></span>](../basic-pricing.md)
- [<span data-ttu-id="2b4a2-111">Өнім каталогының баға белгілеуі</span><span class="sxs-lookup"><span data-stu-id="2b4a2-111">Product catalog pricing</span></span>](../product-catalog-pricing.md)
- [<span data-ttu-id="2b4a2-112">Бизнес транзакциялар</span><span class="sxs-lookup"><span data-stu-id="2b4a2-112">Business transactions</span></span>](../basic-business-transactions.md)
- [<span data-ttu-id="2b4a2-113">Болжамдар</span><span class="sxs-lookup"><span data-stu-id="2b4a2-113">Estimates</span></span>](../estimates.md)
- [<span data-ttu-id="2b4a2-114">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="2b4a2-114">Actuals</span></span>](../actuals.md)
- [<span data-ttu-id="2b4a2-115">Жобаның баға ұсыныстарын талдау</span><span class="sxs-lookup"><span data-stu-id="2b4a2-115">Analyzing project quotes</span></span>](../basic-analyzing-quotes.md)
- [<span data-ttu-id="2b4a2-116">Ұйымдық бөлімшелер</span><span class="sxs-lookup"><span data-stu-id="2b4a2-116">Organizational units</span></span>](../advanced-organizational.md)
- [<span data-ttu-id="2b4a2-117">Бірлік топтары және бірліктер</span><span class="sxs-lookup"><span data-stu-id="2b4a2-117">Unit groups and units</span></span>](../advanced-units.md)
- [<span data-ttu-id="2b4a2-118">Көпвалюталы сценарийлер</span><span class="sxs-lookup"><span data-stu-id="2b4a2-118">Multi-currency scenarios</span></span>](../advanced-currency.md)
- [<span data-ttu-id="2b4a2-119">Нақты көрсеткіштерді жазу</span><span class="sxs-lookup"><span data-stu-id="2b4a2-119">Recording actuals</span></span>](../advanced-actuals.md)

> [!NOTE]
> <span data-ttu-id="2b4a2-120">Бұл тақырып болашақтағы құжаттамалық жаңартудан жойылады.</span><span class="sxs-lookup"><span data-stu-id="2b4a2-120">This topic will be removed in a future documentation update.</span></span> 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]