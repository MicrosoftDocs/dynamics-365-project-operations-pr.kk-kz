---
title: Шығысты басқару үшін жұмыс ағындарын орнату
description: Сіз іссапар мен шығыстар туралы құжаттарды қарау және растау үшін жұмыс ағыны процесін орнатуға болады.
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
ms.openlocfilehash: 36ab1edc4769013684fa9248e6c5eac025637bbd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271630"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="a4d33-103">Шығысты басқару үшін жұмыс ағындарын орнату</span><span class="sxs-lookup"><span data-stu-id="a4d33-103">Set up Expense management workflows</span></span>

<span data-ttu-id="a4d33-104">Сіз іссапар мен шығыстар туралы құжаттарды қарау және растау үшін пайдаланылатын жұмыс ағыны процесін орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="a4d33-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="a4d33-105">Жұмыс процестерін анықтауға болатын құжаттарға шығыстар туралы есептер, іссапар туралы сұраныстар және ақшалай аванстық өтінімдер кіреді.</span><span class="sxs-lookup"><span data-stu-id="a4d33-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="a4d33-106">Жұмыс ағыны бизнес процесті білдіреді.</span><span class="sxs-lookup"><span data-stu-id="a4d33-106">A workflow represents a business process.</span></span> <span data-ttu-id="a4d33-107">Ол құжаттың жүйемен қалай өтетінін анықтайды және тапсырманы кім орындауы немесе құжатты мақұлдауы керек екенін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="a4d33-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="a4d33-108">Ұйымыңызда жұмыс ағыны жүйесін пайдаланудың бірнеше артықшылықтары бар:</span><span class="sxs-lookup"><span data-stu-id="a4d33-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="a4d33-109">**Тұрақты процестер** — сіз сатып алу сұраныстары мен шығыс туралы есептер сияқты нақты құжаттардың растау процесін анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="a4d33-110">Жұмыс ағыны жүйесін пайдалану құжаттардың сәйкес және тиімді түрде өңделуін және мақұлдануын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="a4d33-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="a4d33-111">Өңдеуді көру мүмкіндігі — сіз нақты жұмыс ағыны данасының күйін, тарихын және өнімділік көрсеткіштерін бақылай аласыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="a4d33-112">Бұл тиімділікті арттыру үшін жұмыс ағынына өзгертулер енгізу керектігін анықтауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="a4d33-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="a4d33-113">Орталықтандырылған жұмыс тізімі — пайдаланушылар жұмыс ағынының тапсырмаларын және оларға бекітілген растауды көру үшін орталықтандырылған жұмыс тізімін көре алады.</span><span class="sxs-lookup"><span data-stu-id="a4d33-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="a4d33-114">**Жасауға болатын жұмыс ағындарының түрлері**</span><span class="sxs-lookup"><span data-stu-id="a4d33-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="a4d33-115">Келесі кесте **Шығыс** бағанында жасауға болатын жұмыс ағынының түрлерін тізімдейді.</span><span class="sxs-lookup"><span data-stu-id="a4d33-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="a4d33-116"><strong>Түрі</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="a4d33-117"><strong>Бұл типті</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="a4d33-118"><strong>Шығыс есеп</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="a4d33-119">Шығыс туралы есеп үшін растау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="a4d33-120"><strong>шығыс туралы есепті автоматты түрде жариялау үшін пайдаланыңыз</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="a4d33-121">Шығыс туралы есеп үшін автоматты түрде жариялау ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="a4d33-122"><strong>Жығыс бабының элементі</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="a4d33-123">Шығыс туралы есептеріндегі шығыс бабының элементтері үшін растау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="a4d33-124"><strong>Шығыс бабының элементін автоматты түрде жариялау</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="a4d33-125">Шығыс туралы есептеріндегі шығыс бабының элементтері үшін автоматты түрде жариялау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="a4d33-126"><strong>Іссапарға өтінім</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="a4d33-127">Іссапарларға сұраныстар үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="a4d33-128"><strong>Ақшалай алдын ала өтінім</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="a4d33-129">Ақшалай алдын ала өтінім үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="a4d33-130"><strong>ҚҚС салығын қалпына келтіру</strong></span><span class="sxs-lookup"><span data-stu-id="a4d33-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="a4d33-131">Қосылған құн салығын (VAT) қалпына келтіру үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="a4d33-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |



[!INCLUDE[footer-include](../includes/footer-banner.md)]