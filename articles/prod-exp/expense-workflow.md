---
title: Шығысты басқару жұмыс ағыны
description: Бұл тақырыпта Microsoft Dynamics 365 Finance жүйесінде жұмыс ағыны жүйесін пайдалану жолы, шығыстарды басқаруда шығыс туралы есептерді қарау процесін құру жолы түсіндіріледі.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5207be92cb58d8ab2658096b3e0f3fc81d73d91e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079815"
---
# <a name="expense-management-workflow"></a><span data-ttu-id="512d7-103">Шығысты басқару жұмыс ағыны</span><span class="sxs-lookup"><span data-stu-id="512d7-103">Expense management workflow</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="512d7-104">Шығыстарды басқаруда шығыс туралы есептерді қарау процесін құру үшін жұмыс ағыны жүйесін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="512d7-104">You can use the workflow system to set up a review process for expense reports in Expense management.</span></span> <span data-ttu-id="512d7-105">Шығыс туралы есептерді кім мақұлдайтынын анықтау үшін келесі критерийлерді пайдаланатын жұмыс ағынын орнатуға болады:</span><span class="sxs-lookup"><span data-stu-id="512d7-105">You can set up a workflow that uses the following criteria to determine who approves expense reports:</span></span>

- <span data-ttu-id="512d7-106">Қызметкер иерархия және алдын-ала анықталған мақұлдау шектері туралы есеп береді</span><span class="sxs-lookup"><span data-stu-id="512d7-106">The employee reporting hierarchy and predefined approval limits</span></span>
- <span data-ttu-id="512d7-107">Аралық мақұлдаушылар мен соңғы мақұлдаушыларды қолдайтын көп деңгейлі мақұлдау</span><span class="sxs-lookup"><span data-stu-id="512d7-107">Multi-level approval that supports interim approvers and a final approver</span></span>
- <span data-ttu-id="512d7-108">Қаржылық өлшемдер және жобаның жауапкершілігі</span><span class="sxs-lookup"><span data-stu-id="512d7-108">Financial dimensions and project responsibility</span></span>
- <span data-ttu-id="512d7-109">Белгілі бір пайдаланушыларға немесе пайдаланушы топтарға тағайындау</span><span class="sxs-lookup"><span data-stu-id="512d7-109">Assignment to specific users or user groups</span></span>

<span data-ttu-id="512d7-110">Жұмыс ағыны мақұлдауларын шығыс туралы есептер, іссапар өтінімдері, ақшалай аванстар және қосылған құн салығын (ҚҚС) қалпына келтіру үшін жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="512d7-110">Workflow approvals can be created for expense reports, travel requisitions, cash advances, and value-added tax (VAT) recovery.</span></span>

<span data-ttu-id="512d7-111">**Мысал**</span><span class="sxs-lookup"><span data-stu-id="512d7-111">**Example**</span></span>

<span data-ttu-id="512d7-112">Келесі процесс шығыс туралы есеп үшін шығыстарды басқару бойынша жұмыс ағынының мысалы болып табылады.</span><span class="sxs-lookup"><span data-stu-id="512d7-112">The following process is an example of the expense management workflow for an expense report.</span></span>

1. <span data-ttu-id="512d7-113">Қызметкер шығыс туралы есеп жасайды және сақтайды.</span><span class="sxs-lookup"><span data-stu-id="512d7-113">An employee creates and saves an expense report.</span></span>
2. <span data-ttu-id="512d7-114">Қызметкер шығыс туралы есепті мақұлдау үшін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="512d7-114">The employee submits the expense report for approval.</span></span> <span data-ttu-id="512d7-115">Бекітуші жұмыс ағыны орнатылған кезде анықталған ережелер негізінде анықталады.</span><span class="sxs-lookup"><span data-stu-id="512d7-115">The approver is identified based on the rules that were defined when the workflow was set up.</span></span>
3. <span data-ttu-id="512d7-116">Бекітуші шығыс туралы есепті мақұлдауға дайын екендігі туралы хабарлама алады.</span><span class="sxs-lookup"><span data-stu-id="512d7-116">The approver receives a notification that an expense report is ready for approval.</span></span> <span data-ttu-id="512d7-117">Бекітуші шығыс туралы есепті қарастырады және келесі шарттардың орындалғанын тексереді:</span><span class="sxs-lookup"><span data-stu-id="512d7-117">The approver reviews the expense report and verifies that the following conditions are met:</span></span>

    - <span data-ttu-id="512d7-118">Шығыстар ешқандай шығыстар саясатын бұзбайды.</span><span class="sxs-lookup"><span data-stu-id="512d7-118">The expenses don't violate any expense policies.</span></span> <span data-ttu-id="512d7-119">Егер шығыстар саясатты бұзса, бекітуші шығыс туралы есепте бизнестің жарамды негіздемесі бар екенін тексереді.</span><span class="sxs-lookup"><span data-stu-id="512d7-119">If an expense violates a policy, the approver verifies that the expense report includes a valid business justification.</span></span>
    - <span data-ttu-id="512d7-120">Электрондық түбіртектер шығыс туралы есепке бекітіледі.</span><span class="sxs-lookup"><span data-stu-id="512d7-120">Electronic receipts are attached to the expense report.</span></span>

4. <span data-ttu-id="512d7-121">Бекітуші шығыс туралы есепті мақұлдайды.</span><span class="sxs-lookup"><span data-stu-id="512d7-121">The approver approves the expense report.</span></span>
5. <span data-ttu-id="512d7-122">Шығыс туралы есеп жариялау үшін несие берушілер үйлестірушісіне беріледі.</span><span class="sxs-lookup"><span data-stu-id="512d7-122">The expense report is assigned to the Accounts payable coordinator for posting.</span></span>
6. <span data-ttu-id="512d7-123">Автоматты түрде жариялаудың конфигурацияланғанына байланысты келесі қадамдардың бірі орын алады:</span><span class="sxs-lookup"><span data-stu-id="512d7-123">One of the following steps occurs, depending on whether automatic posting is configured:</span></span>

    - <span data-ttu-id="512d7-124">Егер автоматты жариялау конфигурацияланған болса, шығыс туралы есеп төлем үшін өңделеді, ал шығыс туралы есеп күйі жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="512d7-124">If automatic posting is configured, the expense report is processed for payment, and the status of the expense report is updated.</span></span>
    - <span data-ttu-id="512d7-125">Егер автоматты түрде жариялау конфигурацияланбаса, несие берушілер үйлестірушісі барлық түбіртектердің тапсырылғанын және түбіртектер шығыс туралы есептегі шығыстармен сәйкестендірілгенін тексереді.</span><span class="sxs-lookup"><span data-stu-id="512d7-125">If automatic posting isn't configured, the Accounts payable coordinator verifies that all original receipts have been submitted, and that the receipts are aligned with the expenses on the expense report.</span></span> <span data-ttu-id="512d7-126">Шығыс туралы есепке енгізілген барлық салық кодтары да дұрыс деп тексерілуі керек.</span><span class="sxs-lookup"><span data-stu-id="512d7-126">All tax codes that are entered on the expense report must also be verified as correct.</span></span>

<span data-ttu-id="512d7-127">Осы талаптар тексерілгеннен кейін шығыс туралы есеп орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="512d7-127">After these requirements are verified, the expense report is posted.</span></span>

<span data-ttu-id="512d7-128">Шығыс туралы есеп жарияланғаннан кейін, шығыс туралы есепке ақы төленеді, ал қызметкерге шығындар қайтарылады.</span><span class="sxs-lookup"><span data-stu-id="512d7-128">After the expense report is posted, payment is authorized for the expense report, and the employee is reimbursed.</span></span>
