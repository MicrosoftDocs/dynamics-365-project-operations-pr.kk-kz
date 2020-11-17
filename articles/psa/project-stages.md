---
title: Жоба кезеңінің түрлері
description: Бұл тақырыпта жоба кезеңдері туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 06/19/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: aa423979a794b07a8bd27440f47a29480b74b518
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123069"
---
# <a name="project-stage-types"></a><span data-ttu-id="5f230-103">Жоба кезеңінің түрлері</span><span class="sxs-lookup"><span data-stu-id="5f230-103">Project stage types</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="5f230-104">Жоба кезеңдері жобаның күйін ілгерілеген сайын көрсетуге жобаланған.</span><span class="sxs-lookup"><span data-stu-id="5f230-104">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="5f230-105">Теңшелімдерді бизнес процестерінің ағынымен, Power Automate немесе қосылатын модуль кеңейтімдерімен автоматты түрде жаңарту үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="5f230-105">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="5f230-106">Келесі кезеңдер әдепкі бизнес процесінің ағынында анықталады:</span><span class="sxs-lookup"><span data-stu-id="5f230-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="5f230-107">Жаңа</span><span class="sxs-lookup"><span data-stu-id="5f230-107">New</span></span>
- <span data-ttu-id="5f230-108">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="5f230-108">Quote</span></span>
- <span data-ttu-id="5f230-109">Жоспар</span><span class="sxs-lookup"><span data-stu-id="5f230-109">Plan</span></span>
- <span data-ttu-id="5f230-110">Жеткізу</span><span class="sxs-lookup"><span data-stu-id="5f230-110">Deliver</span></span>
- <span data-ttu-id="5f230-111">Орындалды</span><span class="sxs-lookup"><span data-stu-id="5f230-111">Complete</span></span>
- <span data-ttu-id="5f230-112">Жабу</span><span class="sxs-lookup"><span data-stu-id="5f230-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="5f230-113">Жаңа</span><span class="sxs-lookup"><span data-stu-id="5f230-113">New</span></span>

<span data-ttu-id="5f230-114">Жоба жасаған кезде, жоба кезеңі **Жаңа** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="5f230-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="5f230-115">Егер жоба үлгіден жасалған болса, онда кесте, болжам және топ деректері болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="5f230-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="5f230-116">Әйтпесе, бұл тек жобаның құрылымы болып, ал қалған компоненттерді енгізу керек болады.</span><span class="sxs-lookup"><span data-stu-id="5f230-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="5f230-117">Баға ұсыну</span><span class="sxs-lookup"><span data-stu-id="5f230-117">Quote</span></span>

<span data-ttu-id="5f230-118">Жобаны баға ұсынысымен байланыстырғанда немесе баға ұсынысынан жасағанда жоба кезеңі **Баға ұсыну** күйіне орнатылады және болжалды басталу және аяқталу күні жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="5f230-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="5f230-119">Жоба **Баға ұсыну** кезеңінде болғанда, **Жоба нысаны** бетіндегі **Сатылым** қойыншасында баға ұсыну мәліметтері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="5f230-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="5f230-120">Жоспар</span><span class="sxs-lookup"><span data-stu-id="5f230-120">Plan</span></span>

<span data-ttu-id="5f230-121">Жобамен байланысты баға ұсынысын жеңіп алған кезде және тапсырма **Келісім-шарт** кезеңіне өткенде, жоба кезеңі **Жоспар** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="5f230-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="5f230-122">Жоба **Жоспар** кезеңінде болғанда, **Жоба нысаны** бетінде келісім-шарт мәліметтері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="5f230-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="5f230-123">Жеткізу</span><span class="sxs-lookup"><span data-stu-id="5f230-123">Deliver</span></span>

<span data-ttu-id="5f230-124">Жоба жоспары аяқталғанда және жобаны бастауға дайын болсаңыз, жоба менеджері жобаның басталғанын көрсету үшін жоба кезеңін **Жеткізу** күйіне өзгертуі керек.</span><span class="sxs-lookup"><span data-stu-id="5f230-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="5f230-125">Орындалды</span><span class="sxs-lookup"><span data-stu-id="5f230-125">Complete</span></span> 

<span data-ttu-id="5f230-126">Жоба бойынша жұмыс аяқталған кезде, жоба менеджері кезеңді **Орындалды** күйіне жаңарта алады.</span><span class="sxs-lookup"><span data-stu-id="5f230-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="5f230-127">Жоба кезеңін **Орындалды** күйіне жаңарту арқылы, жоба менеджері жұмыстың 100 пайыз аяқталғанын, бірақ жобаның кез келген күтілетін уақыт пен шығыс жазбаларын жазуға болатындай ашық тұрғанын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="5f230-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="5f230-128">Жабу</span><span class="sxs-lookup"><span data-stu-id="5f230-128">Close</span></span>

<span data-ttu-id="5f230-129">Жоба бойынша барлық транзакциялар жазылған кезде, жоба менеджері кезеңді **Жабық** күйіне жаңарта алады.</span><span class="sxs-lookup"><span data-stu-id="5f230-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="5f230-130">Бұл кезде ешқандай транзакцияларды жазу мүмкін емес және жоба тек оқуға арналған күйге орнатылады.</span><span class="sxs-lookup"><span data-stu-id="5f230-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>
