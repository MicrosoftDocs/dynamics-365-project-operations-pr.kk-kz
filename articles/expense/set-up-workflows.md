---
title: Шығысты басқару үшін жұмыс ағындарын орнату
description: Сіз іссапар мен шығыстар туралы құжаттарды қарау және растау үшін пайдаланылатын жұмыс ағыны процесін орнатуға болады.
author: suvaidya
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: aab6e18d1ddcffa57cf7cd4cb09eec5a4b89c0fd
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001028"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="56e8a-103">Шығысты басқару үшін жұмыс ағындарын орнату</span><span class="sxs-lookup"><span data-stu-id="56e8a-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="56e8a-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="56e8a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="56e8a-105">Сіз іссапар мен шығыстар туралы құжаттарды қарау және растау үшін жұмыс ағыны процесін орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="56e8a-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="56e8a-106">Сіз шығыс туралы есептер, іссапарлар туралы сұранымдар және ақшалай адын-ала өтінімдер бойынша жұмыс ағындарын анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="56e8a-107">Жұмыс ағыны бизнес процесті білдіреді және құжаттың жүйе арқылы қалай өтетіндігін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="56e8a-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="56e8a-108">Сондай-ақ жұмыс ағынында тапсырманы кім орындауы немесе құжатты мақұлдауы керек екендігі көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="56e8a-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="56e8a-109">Ұйымыңызда жұмыс ағыны жүйесін пайдаланудың бірнеше артықшылықтары бар:</span><span class="sxs-lookup"><span data-stu-id="56e8a-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="56e8a-110">**Тұрақты процестер**: сіз сатып алу сұраныстары мен шығыс туралы есептер сияқты нақты құжаттардың растау процесін анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="56e8a-111">Жұмыс ағыны жүйесін пайдалану құжаттардың дәйекті және тиімді түрде өңделуін және расталуын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="56e8a-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="56e8a-112">**Өңдеуді көру мүмкіндігі**: сіз нақты жұмыс ағыны данасының күйін, тарихын және өнімділік көрсеткіштерін бақылай аласыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="56e8a-113">Бұл тиімділікті арттыру үшін жұмыс ағынына өзгертулер енгізу керектігін анықтауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="56e8a-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="56e8a-114">**Орталықтандырылған жұмыс тізімі**: пайдаланушылар жұмыс ағынының тапсырмаларын және оларға бекітілген растауды көру үшін орталықтандырылған жұмыс тізімін көре алады.</span><span class="sxs-lookup"><span data-stu-id="56e8a-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="56e8a-115">Жұмыс ағынының түрлері</span><span class="sxs-lookup"><span data-stu-id="56e8a-115">Workflow types</span></span>

<span data-ttu-id="56e8a-116">Келесі кесте **Шығысты басқару** бағдарламасындағы жұмыс ағынының түрлерін тізімдейді.</span><span class="sxs-lookup"><span data-stu-id="56e8a-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="56e8a-117"><strong>Түрі</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="56e8a-118"><strong>Бұл типті</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="56e8a-119"><strong>шығыс туралы есепті автоматты түрде растау үшін пайдаланыңыз</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="56e8a-120">Шығыс туралы есеп үшін растау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="56e8a-121"><strong>шығыс туралы есепті автоматты түрде жариялау үшін пайдаланыңыз</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="56e8a-122">Шығыс туралы есеп үшін автоматты түрде жариялау ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="56e8a-123"><strong>Жығыс бабының элементі</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="56e8a-124">Шығыс туралы есептеріндегі шығыс бабының элементтері үшін растау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="56e8a-125"><strong>Шығыс бабының элементін автоматты түрде жариялау</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="56e8a-126">Шығыс туралы есептеріндегі шығыс бабының элементтері үшін автоматты түрде жариялау жұмыс ағындарын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="56e8a-127"><strong>Іссапарға өтінім</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="56e8a-128">Іссапарларға сұраныстар үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="56e8a-129"><strong>Ақшалай алдын ала өтінім</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="56e8a-130">Ақшалай алдын ала өтінім үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="56e8a-131"><strong>ҚҚС салығын қалпына келтіру</strong></span><span class="sxs-lookup"><span data-stu-id="56e8a-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="56e8a-132">Қосылған құн салығын (VAT) қалпына келтіру үшін расталған жұмыс ағынын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="56e8a-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |


[!INCLUDE[footer-include](../includes/footer-banner.md)]