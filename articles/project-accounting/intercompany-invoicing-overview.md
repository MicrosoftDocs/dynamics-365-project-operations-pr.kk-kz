---
title: Компанияаралық есеп-шот ұсынуға шолу
description: Бұл тақырыпта жобалар үшін компанияаралық есеп-шот туралы ақпарат пен мысалдар келтірілген.
author: sigitac
ms.date: 11/19/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: c1dcf642f79ce64cb83285ac6dc6d7eaf815145c
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369383"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="c3a22-103">Компанияаралық есеп-шот ұсынуға шолу</span><span class="sxs-lookup"><span data-stu-id="c3a22-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="c3a22-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="c3a22-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c3a22-105">Ұйымыңызда жобалар бойынша бір-біріне өнімдер мен қызметтерді тасымалдайтын бірнеше бөлімдер, еншілес бөлімшелер және басқа заңды тұлғалар болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="c3a22-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="c3a22-106">Қызмет немесе өнімді ұсынатын заңды тұлға *несие беруші заңды тұлға* деп аталады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="c3a22-107">Қызмет немесе өнімді алатын заңды тұлға *несие алушы заңды тұлға* деп аталады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="c3a22-108">Келесі кескінде екі заңды тұлға, Contoso Robotics USA (қарыз алушы заңды тұлға) және Contoso Robotics UK (несие беретін заңды тұлға) Adventure Works тұтынушысына жобаны ұсыну үшін ресурстарды бөлісетін әдеттегі сценарий көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="c3a22-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="c3a22-109">Осы сценарий үшін Contoso Robotics USA компаниясымен Adventure Works тұтынушысы үшін жұмысты орындау келісімшарты жасалды.</span><span class="sxs-lookup"><span data-stu-id="c3a22-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![Компанияаралық шот жіберу](./media/IntercompanyScenario.png) 

<span data-ttu-id="c3a22-111">Dynamics 365 Project Operations бағдарламасы компанияаралық транзакцияларды өңдеу үшін келесі ағынды пайдаланады:</span><span class="sxs-lookup"><span data-stu-id="c3a22-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="c3a22-112">Несие беруші заңды тұлға жазбасындағы ресурстар қарыз алушы заңды тұлғаның жобалары бойынша тапсырыс уақыты мен шығыстар арқылы компанияаралық уақытты немесе шығыс транзакцияларын есепке алады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="c3a22-113">Уақыт пен шығыс құндары несие беруші компанияда несие алушы компанияның бірлігінің құн бағатізбесін пайдалану арқылы жазылады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="c3a22-114">Компанияаралық шот ұсынылмаған сатылым транзакциялар несие беруші компанияда несие алушы компанияның бірлігінің құн бағатізбесін пайдалану арқылы жазылады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="c3a22-115">Шот ұсынылмаған табыс несие алушы компанияда жобаның келісім-шарт сатылым бағатізбесін пайдалана отырып жазылады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="c3a22-116">Тұтынушыға шот ұсынылмаған табыс жазылған кезде шот ұсынылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="c3a22-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="c3a22-117">Тұтынушы компанияаралық есеп-шотты өңдеу аяқталғанша күтудің қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="c3a22-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="c3a22-118">Компанияаралық тұтынушы есеп-шоттары кезеңдік негізде несие теруші компанияда жасалады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="c3a22-119">Есеп-шоттар қолмен немесе кезеңдік автоматтандырылған процесті пайдалану арқылы жасалады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="c3a22-120">Әрбір несие алушы заңды тұлға үшін бір есеп-шот немесе жеке есеп-шот жоба бойынша жасалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="c3a22-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="c3a22-121">Компанияаралық тұтынушының есеп-шоты несие беретін заңды тұлғада жарияланған кезде, тиісті жеткізушінің күтілетін есеп-шоты несие алушы заңды тұлғада жасалады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="c3a22-122">Жеткізушінің күтілетін есеп-шотындағы құндар есеп-шот жарияланған кезде жоба қосалқы кітабына жазылады.</span><span class="sxs-lookup"><span data-stu-id="c3a22-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="c3a22-123">Төмендегі диаграмма бухгалтерлік оқиғаларға және бас кітапқа күтілетін орналастыруларға қатысты болғандықтан, компанияаралық есеп-шоттарды көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="c3a22-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![Компанияаралық ағын](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="c3a22-125">Қосымша ресурстар</span><span class="sxs-lookup"><span data-stu-id="c3a22-125">Additional resources</span></span>

- [<span data-ttu-id="c3a22-126">Компанияаралық шот ұсынуды конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="c3a22-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="c3a22-127">Компанияаралық транзакцияларды жазу</span><span class="sxs-lookup"><span data-stu-id="c3a22-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="c3a22-128">Тұтынушылар мен жеткізушілердің компанияаралық есеп-шоттарын жасау</span><span class="sxs-lookup"><span data-stu-id="c3a22-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]