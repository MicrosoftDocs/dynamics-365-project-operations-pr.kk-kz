---
title: Компанияаралық есеп-шот ұсынуға шолу
description: Бұл тақырыпта жобалар үшін компанияаралық есеп-шот туралы ақпарат пен мысалдар келтірілген.
author: sigitac
manager: tfehr
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 3ad75089de1a2f99646f7aba213e199a2bec347d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287335"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="da6d3-103">Компанияаралық есеп-шот ұсынуға шолу</span><span class="sxs-lookup"><span data-stu-id="da6d3-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="da6d3-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="da6d3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="da6d3-105">Ұйымыңызда жобалар бойынша бір-біріне өнімдер мен қызметтерді тасымалдайтын бірнеше бөлімдер, еншілес бөлімшелер және басқа заңды тұлғалар болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da6d3-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="da6d3-106">Қызмет немесе өнімді ұсынатын заңды тұлға *несие беруші заңды тұлға* деп аталады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="da6d3-107">Қызмет немесе өнімді алатын заңды тұлға *несие алушы заңды тұлға* деп аталады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="da6d3-108">Келесі суретте екі заңды тұлға, яғни Contoso Robotics USA (қарыз алушы заңды тұлға) және Contoso Robotics UK (несие беруші заңды тұлға) Adventure works тұтынушысына жобаны ұсынуға арналған ресурстарды бөлісетін әдеттегі сценарий көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="da6d3-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="da6d3-109">Осы сценарий үшін Contoso Robotics USA компаниясы Adventure Works дерекқорына жұмысты жеткізуге келісім-шарт жасады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![Компанияаралық шот жіберу](./media/IntercompanyScenario.png) 

<span data-ttu-id="da6d3-111">Dynamics 365 Project Operations бағдарламасы компанияаралық транзакцияларды өңдеу үшін келесі ағынды пайдаланады:</span><span class="sxs-lookup"><span data-stu-id="da6d3-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="da6d3-112">Несие беруші заңды тұлға жазбасындағы ресурстар қарыз алушы заңды тұлғаның жобалары бойынша тапсырыс уақыты мен шығыстар арқылы компанияаралық уақытты немесе шығыс транзакцияларын есепке алады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="da6d3-113">Уақыт пен шығыс құндары несие беруші компанияда несие алушы компанияның бірлігінің құн бағатізбесін пайдалану арқылы жазылады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="da6d3-114">Компанияаралық шот ұсынылмаған сатылым транзакциялар несие беруші компанияда несие алушы компанияның бірлігінің құн бағатізбесін пайдалану арқылы жазылады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="da6d3-115">Шот ұсынылмаған табыс несие алушы компанияда жобаның келісім-шарт сатылым бағатізбесін пайдалана отырып жазылады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="da6d3-116">Тұтынушыға шот ұсынылмаған табыс жазылған кезде шот ұсынылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da6d3-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="da6d3-117">Тұтынушы компанияаралық есеп-шотты өңдеу аяқталғанша күтудің қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="da6d3-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="da6d3-118">Компанияаралық тұтынушы есеп-шоттары кезеңдік негізде несие теруші компанияда жасалады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="da6d3-119">Есеп-шоттар қолмен немесе кезеңдік автоматтандырылған процесті пайдалану арқылы жасалады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="da6d3-120">Әрбір несие алушы заңды тұлға үшін бір есеп-шот немесе жеке есеп-шот жоба бойынша жасалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="da6d3-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="da6d3-121">Компанияаралық тұтынушының есеп-шоты несие беретін заңды тұлғада жарияланған кезде, тиісті жеткізушінің күтілетін есеп-шоты несие алушы заңды тұлғада жасалады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="da6d3-122">Жеткізушінің күтілетін есеп-шотындағы құндар есеп-шот жарияланған кезде жоба қосалқы кітабына жазылады.</span><span class="sxs-lookup"><span data-stu-id="da6d3-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="da6d3-123">Төмендегі диаграмма бухгалтерлік оқиғаларға және бас кітапқа күтілетін орналастыруларға қатысты болғандықтан, компанияаралық есеп-шоттарды көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="da6d3-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![Компанияаралық ағын](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="da6d3-125">Қосымша ресурстар</span><span class="sxs-lookup"><span data-stu-id="da6d3-125">Additional resources</span></span>

- [<span data-ttu-id="da6d3-126">Компанияаралық шот ұсынуды конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="da6d3-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="da6d3-127">Компанияаралық транзакцияларды жазу</span><span class="sxs-lookup"><span data-stu-id="da6d3-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="da6d3-128">Тұтынушылар мен жеткізушілердің компанияаралық есеп-шоттарын жасау</span><span class="sxs-lookup"><span data-stu-id="da6d3-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]