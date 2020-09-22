---
title: Жоба кезеңдері
description: Бұл тақырыпта жоба кезеңдері туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 983c25a0-ed21-4151-a109-b385a88285fa
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 70aa057e127df7ba925e84f5d056a06a4cc8833e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753040"
---
# <a name="project-stages"></a><span data-ttu-id="7b5b7-103">Жоба кезеңдері</span><span class="sxs-lookup"><span data-stu-id="7b5b7-103">Project stages</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="7b5b7-104">Жоба кезеңдері жобаның күйін ілгерілеген сайын көрсету үшін жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-104">Project stages are updated to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="7b5b7-105">Әдепкі бизнес процесінің ағыны жобаның кейбір кезеңдерін автоматты түрде жаңартады, ал басқалары жоба менеджерімен қолмен жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-105">The default business process flow automatically updates some stages of the project while others are manually updated by the project manager.</span></span> 

<span data-ttu-id="7b5b7-106">Келесі кезеңдер әдепкі бизнес процесінің ағынында анықталады:</span><span class="sxs-lookup"><span data-stu-id="7b5b7-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="7b5b7-107">Жаңа</span><span class="sxs-lookup"><span data-stu-id="7b5b7-107">New</span></span>
- <span data-ttu-id="7b5b7-108">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="7b5b7-108">Quote</span></span>
- <span data-ttu-id="7b5b7-109">Жоспар</span><span class="sxs-lookup"><span data-stu-id="7b5b7-109">Plan</span></span>
- <span data-ttu-id="7b5b7-110">Жеткізу</span><span class="sxs-lookup"><span data-stu-id="7b5b7-110">Deliver</span></span>
- <span data-ttu-id="7b5b7-111">Орындалды</span><span class="sxs-lookup"><span data-stu-id="7b5b7-111">Complete</span></span>
- <span data-ttu-id="7b5b7-112">Жабу</span><span class="sxs-lookup"><span data-stu-id="7b5b7-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="7b5b7-113">Жаңа</span><span class="sxs-lookup"><span data-stu-id="7b5b7-113">New</span></span>

<span data-ttu-id="7b5b7-114">Жоба жасаған кезде, жоба кезеңі **Жаңа** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="7b5b7-115">Егер жоба үлгіден жасалған болса, онда кесте, болжам және топ деректері болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="7b5b7-116">Әйтпесе, бұл тек жобаның құрылымы болып, ал қалған компоненттерді енгізу керек болады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="7b5b7-117">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="7b5b7-117">Quote</span></span>

<span data-ttu-id="7b5b7-118">Жобаны баға ұсынысымен байланыстырғанда немесе баға ұсынысынан жасағанда жоба кезеңі **Баға ұсыну** күйіне орнатылады және болжалды басталу және аяқталу күні жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="7b5b7-119">Жоба **Баға ұсыну** кезеңінде болғанда, **Жоба нысаны** бетіндегі **Сатылым** қойыншасында баға ұсыну мәліметтері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="7b5b7-120">Жоспар</span><span class="sxs-lookup"><span data-stu-id="7b5b7-120">Plan</span></span>

<span data-ttu-id="7b5b7-121">Жобамен байланысты баға ұсынысын жеңіп алған кезде және тапсырма **Келісім-шарт** кезеңіне өткенде, жоба кезеңі **Жоспар** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="7b5b7-122">Жоба **Жоспар** кезеңінде болғанда, **Жоба нысаны** бетінде келісім-шарт мәліметтері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="7b5b7-123">Жеткізу</span><span class="sxs-lookup"><span data-stu-id="7b5b7-123">Deliver</span></span>

<span data-ttu-id="7b5b7-124">Жоба жоспары аяқталғанда және жобаны бастауға дайын болсаңыз, жоба менеджері жобаның басталғанын көрсету үшін жоба кезеңін **Жеткізу** күйіне өзгертуі керек.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="7b5b7-125">Орындалды</span><span class="sxs-lookup"><span data-stu-id="7b5b7-125">Complete</span></span> 

<span data-ttu-id="7b5b7-126">Жоба бойынша жұмыс аяқталған кезде, жоба менеджері кезеңді **Орындалды** күйіне жаңарта алады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="7b5b7-127">Жоба кезеңін **Орындалды** күйіне жаңарту арқылы, жоба менеджері жұмыстың 100 пайыз аяқталғанын, бірақ жобаның кез келген күтілетін уақыт пен шығыс жазбаларын жазуға болатындай ашық тұрғанын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="7b5b7-128">Жабу</span><span class="sxs-lookup"><span data-stu-id="7b5b7-128">Close</span></span>

<span data-ttu-id="7b5b7-129">Жоба бойынша барлық транзакциялар жазылған кезде, жоба менеджері кезеңді **Жабық** күйіне жаңарта алады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="7b5b7-130">Бұл кезде ешқандай транзакцияларды жазу мүмкін емес және жоба тек оқуға арналған күйге орнатылады.</span><span class="sxs-lookup"><span data-stu-id="7b5b7-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>
