---
title: Жобалар мен жоба келісім-шарттары бойынша есеп-шот ұсынудың орындалмаған әрекеттерін қарап шығу
description: Бұл тақырыпта уақытты, шығынды және өнімнің орындалмаған әрекеттерін қарап шығу және оларды есеп-шот ұсынуға дайын ретінде белгілеу жолы туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 03/11/2019
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 2.x and 3.x
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: db15ea136b9939c0a0631936bcadab538bf2dd4a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753115"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a><span data-ttu-id="27b88-103">Жобалар мен жоба келісім-шарттары бойынша есеп-шот ұсынудың орындалмаған әрекеттерін қарап шығу</span><span class="sxs-lookup"><span data-stu-id="27b88-103">Review the invoicing backlog on projects and project contracts</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="27b88-104">Транзакция есеп-шотты жасауға және өңдеуге дайын болған кезде, оны **Есеп-шот ұсынуға дайын** деп белгілеу керек.</span><span class="sxs-lookup"><span data-stu-id="27b88-104">When a transaction is ready to have an invoice created and processed, the transaction should be marked **Ready to invoice**.</span></span> <span data-ttu-id="27b88-105">Бұл тақырыпта жасауға болатын транзакциялар түрлері сипатталған.</span><span class="sxs-lookup"><span data-stu-id="27b88-105">This topic describes the types of transactions that can be created.</span></span>

## <a name="review-the-time-and-material-billing-backlog"></a><span data-ttu-id="27b88-106">Уақыт және материалдық шоттың орындалмаған әрекеттерін қарап шығу</span><span class="sxs-lookup"><span data-stu-id="27b88-106">Review the time and material billing backlog</span></span>

<span data-ttu-id="27b88-107">Жобаға уақыт пен шығыс жазбасы жіберілген және бекітілген кезде, PSA жобаның нақты мәнін жасайды.</span><span class="sxs-lookup"><span data-stu-id="27b88-107">When a time or expense entry is submitted and approved for a project, PSA creates a project actual.</span></span> <span data-ttu-id="27b88-108">Егер жоба мен транзакция класының тіркесімі уақыт және материалдар жобасының келісім-шарт жолына салыстырылған болса, жазба бекітілген кезде екі нақты мән жасалады:</span><span class="sxs-lookup"><span data-stu-id="27b88-108">If the combination of the project and the transaction class are mapped to a contract line for a time-and-materials project, two actuals are created when the entry is approved:</span></span>

- <span data-ttu-id="27b88-109">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="27b88-109">Cost actual</span></span> 
- <span data-ttu-id="27b88-110">Шот ұсынылмаған сатылымның нақты мәні</span><span class="sxs-lookup"><span data-stu-id="27b88-110">Unbilled sales actual</span></span>

<span data-ttu-id="27b88-111">Шот ұсынылмаған сатылымның нақты мәндері шоттың орындалмаған әрекеттерін білдіреді, және олардың шот ұсыну күйін **Есеп-шот ұсынуға дайын** күйіне орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="27b88-111">Unbilled sales actuals represent the billing backlog, and their billing status must be set to **Ready to Invoice**.</span></span> <span data-ttu-id="27b88-112">Жоба есеп-шоты жасалған кезде, **Есеп-шот ұсынуға дайын** деп белгіленген шот ұсынылмаған сатылымның нақты мәндері есеп-шот жолы туралы мәліметтер ретінде көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="27b88-112">When a project invoice is created, unbilled sales actuals that are marked **Ready to Invoice** are copied over as invoice line details.</span></span>

<span data-ttu-id="27b88-113">Уақыт және материалдық шоттың орындалмаған әрекеттерін қарап шығу үшін, **Сатылым** \> **Шот ұсыну** \> **Уақыт және материалдық шоттың орындалмаған әрекеттері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="27b88-113">To review the billing backlog for time and materials, go to **Sales** \> **Billing** \> **Time and Material Billing Backlog**.</span></span> <span data-ttu-id="27b88-114">Есеп-шот ұсынуға дайын барлық шот ұсынылмаған сатылымның нақты мәндерін таңдап, **Есеп-шот ұсынуға дайын** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="27b88-114">Select all the unbilled sales actuals that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="27b88-115">Осы кезде осы мәндердің шот ұсыну күйі **Есеп-шот ұсынуға дайын** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="27b88-115">The billing status of these actuals is changed to **Ready to Invoice**.</span></span>

![Уақыт және материалдық шоттың орындалмаған әрекеттері](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a><span data-ttu-id="27b88-117">Өнім шотының орындалмаған әрекеттерін қарап шығу</span><span class="sxs-lookup"><span data-stu-id="27b88-117">Review the product billing backlog</span></span>

<span data-ttu-id="27b88-118">PSA бағдарламасында, жоба келісім-шартының өнімге негізделген келісім-шарт жолдары болған кезде, жоба келісім-шарты үшін есеп-шот жасалған уақытта осы жолдар есеп-шот ұсыну үшін қарастырылады.</span><span class="sxs-lookup"><span data-stu-id="27b88-118">In PSA, when a project contract has product-based contract lines, those lines are considered for invoicing whenever an invoice is created for the project contract.</span></span> <span data-ttu-id="27b88-119">**Есеп-шот ұсынуға дайын** деп белгіленген келісім-шарт жолдары бар кез келген өнім жоба есеп-шотына оның жолдары ретінде көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="27b88-119">Any product that has contract lines that are marked **Ready to Invoice** is copied over to the project invoice as project invoice lines.</span></span>

<span data-ttu-id="27b88-120">Өнімдер шотының орындалмаған әрекеттерін қарап шығу үшін, **Сатылым** \> **Шот ұсыну** \> **Өнім шотының орындалмаған әрекеттері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="27b88-120">To review the billing backlog for products, go to **Sales** \> **Billing** \> **Product Billing Backlog**.</span></span> <span data-ttu-id="27b88-121">Есеп-шот ұсынуға дайын барлық өнімге негізделген келісім-шарт жолдарын таңдап, **Есеп-шот ұсынуға дайын** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="27b88-121">Select all the product-based contract lines that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="27b88-122">Осы кезде осы жолдардың шот ұсыну күйі **Есеп-шот ұсынуға дайын** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="27b88-122">The billing status of these lines is changed to **Ready to Invoice**.</span></span>

![Өнім шотының орындалмаған әрекеттері](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a><span data-ttu-id="27b88-124">Бекітілген баға келісім-шарттарындағы шот ұсыну кезеңдерін қарап шығу</span><span class="sxs-lookup"><span data-stu-id="27b88-124">Review billing milestones on fixed-price contracts</span></span>

<span data-ttu-id="27b88-125">Бекітілген баға бойынша шот ұсыну әдісі бар әрбір жоба келісім-шартының жолы келісім-шарт кезеңдерін анықтауы керек.</span><span class="sxs-lookup"><span data-stu-id="27b88-125">Each project contract line that has a fixed-price billing method must define contract milestones.</span></span> <span data-ttu-id="27b88-126">Осы келісім-шарт кезеңдері **Есеп-шот ұсынуға дайын** деп белгіленсе ғана олар бойынша есеп-шот ұсынуға болады.</span><span class="sxs-lookup"><span data-stu-id="27b88-126">These contract milestones can be invoiced only if they are marked **Ready to Invoice**.</span></span> 

<span data-ttu-id="27b88-127">Шот ұсыну кезеңдерін қарап шығу үшін, **Сатылым** \> **Шот ұсыну** \> **Бекітілген баға кезеңдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="27b88-127">To review billing milestones, go to **Sales** \> **Billing** \> **Fixed Price Milestones**.</span></span> <span data-ttu-id="27b88-128">Есеп-шот ұсынуға дайын кезеңдерді таңдап, **Есеп-шот ұсынуға дайын** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="27b88-128">Select the milestones that are ready to be invoiced, and then select **Ready to invoice**.</span></span> <span data-ttu-id="27b88-129">Осы кезде осы кезеңдердің шот ұсыну күйі **Есеп-шот ұсынуға дайын** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="27b88-129">The billing status of these milestones is changed to **Ready to Invoice**.</span></span>

![Бекітілген баға кезеңдері](media/FPBacklog.png)
