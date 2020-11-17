---
title: Шығысты басқару үшін жұмыс ағындарын орнату
description: Сіз іссапар мен шығыстар туралы құжаттарды қарау және растау үшін пайдаланылатын жұмыс ағыны процесін орнатуға болады.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: af6463b07e282ae1ff6aa7dc1a540ff7c8cc318a
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127705"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="dfee7-103">Шығысты басқару үшін жұмыс ағындарын орнату</span><span class="sxs-lookup"><span data-stu-id="dfee7-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="dfee7-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="dfee7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="dfee7-105">Сіз іссапар мен шығыстар туралы құжаттарды қарау және растау үшін жұмыс ағыны процесін орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="dfee7-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="dfee7-106">Сіз шығыс туралы есептер, іссапарлар туралы сұранымдар және ақшалай адын-ала өтінімдер бойынша жұмыс ағындарын анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="dfee7-107">Жұмыс ағыны бизнес процесті білдіреді және құжаттың жүйе арқылы қалай өтетіндігін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="dfee7-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="dfee7-108">Сондай-ақ жұмыс ағынында тапсырманы кім орындауы немесе құжатты мақұлдауы керек екендігі көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="dfee7-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="dfee7-109">Ұйымыңызда жұмыс ағыны жүйесін пайдаланудың бірнеше артықшылықтары бар:</span><span class="sxs-lookup"><span data-stu-id="dfee7-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="dfee7-110">**Тұрақты процестер**: сіз сатып алу сұраныстары мен шығыс туралы есептер сияқты нақты құжаттардың растау процесін анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="dfee7-111">Жұмыс ағыны жүйесін пайдалану құжаттардың дәйекті және тиімді түрде өңделуін және расталуын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="dfee7-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="dfee7-112">**Өңдеуді көру мүмкіндігі**: сіз нақты жұмыс ағыны данасының күйін, тарихын және өнімділік көрсеткіштерін бақылай аласыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="dfee7-113">Бұл тиімділікті арттыру үшін жұмыс ағынына өзгертулер енгізу керектігін анықтауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="dfee7-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="dfee7-114">**Орталықтандырылған жұмыс тізімі**: пайдаланушылар жұмыс ағынының тапсырмаларын және оларға бекітілген растауды көру үшін орталықтандырылған жұмыс тізімін көре алады.</span><span class="sxs-lookup"><span data-stu-id="dfee7-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="dfee7-115">Жұмыс ағынының түрлері</span><span class="sxs-lookup"><span data-stu-id="dfee7-115">Workflow types</span></span>

<span data-ttu-id="dfee7-116">Келесі кесте **Шығысты басқару** бағдарламасындағы жұмыс ағынының түрлерін тізімдейді.</span><span class="sxs-lookup"><span data-stu-id="dfee7-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="dfee7-117"><strong>Түрі</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="dfee7-118"><strong>Бұл типті</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="dfee7-119"><strong>шығыс туралы есепті автоматты түрде растау үшін пайдаланыңыз</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="dfee7-120">Шығыс туралы есеп үшін растау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="dfee7-121"><strong>шығыс туралы есепті автоматты түрде жариялау үшін пайдаланыңыз</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="dfee7-122">Шығыс туралы есеп үшін автоматты түрде жариялау ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="dfee7-123"><strong>Жығыс бабының элементі</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="dfee7-124">Шығыс туралы есептеріндегі шығыс бабының элементтері үшін растау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="dfee7-125"><strong>Шығыс бабының элементін автоматты түрде жариялау</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="dfee7-126">Шығыс туралы есептеріндегі шығыс бабының элементтері үшін автоматты түрде жариялау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="dfee7-127"><strong>Іссапарға өтінім</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="dfee7-128">Іссапарларға сұраныстар үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="dfee7-129"><strong>Ақшалай алдын ала өтінім</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="dfee7-130">Ақшалай алдын ала өтінім үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="dfee7-131"><strong>ҚҚС салығын қалпына келтіру</strong></span><span class="sxs-lookup"><span data-stu-id="dfee7-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="dfee7-132">Қосылған құн салығын (VAT) қалпына келтіру үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="dfee7-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |
