---
title: Жоба кезеңдері
description: Осы тақырыпта Microsoft Dynamics Project Operations бағдарламасында қолжетімді жоба кезеңдері туралы ақпарат ұсынылған.
author: ruhercul
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 079c3d2d16cf802d2b9ecc779577e6e390d92ddc
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996933"
---
# <a name="project-stages"></a><span data-ttu-id="d0ae6-103">Жоба кезеңдері</span><span class="sxs-lookup"><span data-stu-id="d0ae6-103">Project stages</span></span>

<span data-ttu-id="d0ae6-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="d0ae6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d0ae6-105">Жоба кезеңдері жобаның күйін ілгерілеген сайын көрсетуге жобаланған.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="d0ae6-106">Теңшелімдерді бизнес процестерінің ағынымен, Power Automate немесе қосылатын модуль кеңейтімдерімен автоматты түрде жаңарту үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="d0ae6-107">Келесі кезеңдер әдепкі бизнес процесінің ағынында анықталған:</span><span class="sxs-lookup"><span data-stu-id="d0ae6-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="d0ae6-108">Жаңа</span><span class="sxs-lookup"><span data-stu-id="d0ae6-108">New</span></span>
- <span data-ttu-id="d0ae6-109">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="d0ae6-109">Quote</span></span>
- <span data-ttu-id="d0ae6-110">Жоспар</span><span class="sxs-lookup"><span data-stu-id="d0ae6-110">Plan</span></span>
- <span data-ttu-id="d0ae6-111">Жеткізу</span><span class="sxs-lookup"><span data-stu-id="d0ae6-111">Deliver</span></span>
- <span data-ttu-id="d0ae6-112">Аяқталған</span><span class="sxs-lookup"><span data-stu-id="d0ae6-112">Complete</span></span>
- <span data-ttu-id="d0ae6-113">Жабу</span><span class="sxs-lookup"><span data-stu-id="d0ae6-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="d0ae6-114">Жаңа</span><span class="sxs-lookup"><span data-stu-id="d0ae6-114">New</span></span>

<span data-ttu-id="d0ae6-115">Жоба жасаған кезде, жоба кезеңі **Жаңа** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="d0ae6-116">Егер жоба үлгіден жасалған болса, онда кесте, болжам және топ деректері болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="d0ae6-117">Әйтпесе, ол жобаның құрылымы және қалған құрамдастар енгізілуі керек.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="d0ae6-118">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="d0ae6-118">Quote</span></span>

<span data-ttu-id="d0ae6-119">Жобаны баға ұсынысымен байланыстырғанда немесе баға ұсынысынан жасағанда жоба кезеңі **Баға ұсыну** күйіне орнатылады және болжалды басталу және аяқталу күні жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="d0ae6-120">Жоба **Баға ұсыну** кезеңінде болғанда, **Жоба нысаны** бетіндегі **Сатылым** қойыншасында баға ұсыну мәліметтері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="d0ae6-121">Жоспар</span><span class="sxs-lookup"><span data-stu-id="d0ae6-121">Plan</span></span>

<span data-ttu-id="d0ae6-122">Жобамен байланысты баға ұсынысын жеңіп алған кезде және тапсырма **Келісім-шарт** кезеңіне өткенде, жоба кезеңі **Жоспар** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="d0ae6-123">Жоба **Жоспар** кезеңінде болғанда, **Жоба нысаны** бетінде келісім-шарт мәліметтері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="d0ae6-124">Жеткізу</span><span class="sxs-lookup"><span data-stu-id="d0ae6-124">Deliver</span></span>

<span data-ttu-id="d0ae6-125">Жоба жоспары аяқталғанда және жобаны бастауға дайын болсаңыз, жоба менеджері жобаның басталғанын көрсету үшін жоба кезеңін **Жеткізу** күйіне өзгертуі керек.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="d0ae6-126">Орындалды</span><span class="sxs-lookup"><span data-stu-id="d0ae6-126">Complete</span></span> 

<span data-ttu-id="d0ae6-127">Жоба бойынша жұмыс аяқталған кезде, жоба менеджері кезеңді **Орындалды** күйіне жаңарта алады.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="d0ae6-128">Жоба кезеңін **Орындалды** күйіне жаңарту арқылы, жоба менеджері жұмыстың 100 пайыз аяқталғанын, бірақ жобаның кез келген күтілетін уақыт пен шығыс жазбаларын жазуға болатындай ашық тұрғанын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-128">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="d0ae6-129">Жабу</span><span class="sxs-lookup"><span data-stu-id="d0ae6-129">Close</span></span>

<span data-ttu-id="d0ae6-130">Жоба бойынша барлық транзакциялар жазылған кезде, жоба менеджері кезеңді **Жабық** күйіне жаңарта алады.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="d0ae6-131">Бұл кезде ешқандай транзакцияларды жазу мүмкін емес және жоба тек оқуға арналған күйге орнатылады.</span><span class="sxs-lookup"><span data-stu-id="d0ae6-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]