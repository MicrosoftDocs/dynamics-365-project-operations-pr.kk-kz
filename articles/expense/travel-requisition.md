---
title: Іссапарға өтінімдер
description: Бұл тақырыпта іссапарға өтінімдер туралы ақпарат берілген.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 0261405abb9305d7f6abcde9cb90d9b184868580
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906232"
---
# <a name="travel-requisitions"></a><span data-ttu-id="a71f3-103">Іссапарға өтінімдер</span><span class="sxs-lookup"><span data-stu-id="a71f3-103">Travel requisitions</span></span>

<span data-ttu-id="a71f3-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="a71f3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a71f3-105">Іссапарға өтінімде іссапарға жұмсалатын шығындар көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="a71f3-105">A travel requisition lists the expenses that will be incurred for the purpose of travel.</span></span> <span data-ttu-id="a71f3-106">Іссапарға өтінім сараптауға жіберілген және оны шығыстарға рұқсат беру үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-106">A travel requisition is submitted for review and can be used to authorize expenses.</span></span>

<span data-ttu-id="a71f3-107">Ұйымға ұсынылатын кез келген шығыстарды жұмсамас бұрын, сізден іссапарға өтінімді жіберу талап етілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="a71f3-107">You may be required to submit a travel requisition before you incur any expense that is charged to the organization.</span></span> <span data-ttu-id="a71f3-108">Бұл талап корпоративтік несие картасына шығыстар алғаныңызға, ақшалай аванстан алған ақшаңызды жұмсағаныңызға немесе ұйымның өтейтін қолма-қол шығыстарына қарамастан қолданылады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-108">This requirement applies, regardless of whether you charge expenses to a corporate credit card, spend cash that you received from a cash advance, or incur out-of-pocket expenses that will be reimbursed by the organization.</span></span>

<span data-ttu-id="a71f3-109">Ұйым шығындарын басқаруға көмектесу үшін іссапарға өтінімдер мен саясаттарды пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-109">Travel requisitions and policies can be used to help manage organization expenditures.</span></span> <span data-ttu-id="a71f3-110">Мысалы, ұйымыңыз іссапарды қажет ететін бекітілген баға жобасымен жұмыс істеп жатқан болса, жоба тобы мүшелерінің іссапар шығыстары жоба бюджетіне сәйкес келуі керек.</span><span class="sxs-lookup"><span data-stu-id="a71f3-110">For example, if your organization is working on a fixed-price project that requires travel, the travel expenses of the project's team members must fit within the project budget.</span></span> <span data-ttu-id="a71f3-111">Іссапар шығыстарын жұмсағанға дейін растауды талап ету арқылы ұйым жобаның бюджетке сәйкес келуіне көз жеткізе алады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-111">By requiring that travel expenses be approved before they are incurred, the organization can help make sure that the project remains within budget.</span></span>

## <a name="configuration"></a><span data-ttu-id="a71f3-112">Теңшелім</span><span class="sxs-lookup"><span data-stu-id="a71f3-112">Configuration</span></span> 

<span data-ttu-id="a71f3-113">Іссапарға өтінімдерді Шығысты басқару параметрлерінде «Сапарды алдын ала авторизациялау міндетті болып табылады» параметрін қосу арқылы «міндетті» ретінде конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-113">Travel Requisitions can be configured as "mandatory" by enabling the "Pre-authorization of travel is mandatory" parameter in Expense Management Parameters.</span></span> 

## <a name="create-and-submit-a-travel-requisition"></a><span data-ttu-id="a71f3-114">Іссапарға өтінімді жасап, жіберу</span><span class="sxs-lookup"><span data-stu-id="a71f3-114">Create and submit a travel requisition</span></span>

1. <span data-ttu-id="a71f3-115">**Менің шығыстарым: іссапарға өтінім** тармағына өтіп, **Жаңа іссапарға өтінім** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-115">Go to **My expenses: Travel Requisition**, and select **New travel Requisition**.</span></span>
2. <span data-ttu-id="a71f3-116">Іссапардың мақсаты мен межелі орнын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-116">Enter a purpose and destination for the requisition.</span></span>
3. <span data-ttu-id="a71f3-117">**Іссапар сипаттамасы** өрісіне кез келген қосымша ақпаратты енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-117">In the  **Travel description** field, enter any additional information.</span></span> 
4. <span data-ttu-id="a71f3-118">Ұшу, тамақтану немесе автокөлік жалдау сияқты күтілетін шығыстардың әрқайсысы үшін шығыстар жолы элементін жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-118">For each of the expected expenses, such as Flight, meals, or car rental, create an expense line item.</span></span> <span data-ttu-id="a71f3-119">Болжалды күнді, болжалды соманы және әр шығыстың валютасын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-119">Include the estimated date, estimated amount, and the currency for each expense.</span></span> 
5. <span data-ttu-id="a71f3-120">Күтілетін шығыстарды қосуды аяқтағаннан кейін **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-120">When you have finished adding the expected expenses, select **Save**.</span></span>
6. <span data-ttu-id="a71f3-121">Іссапарға өтінімді жіберуге дайын болған кезде, **Жұмыс ағыны** > **Жіберу** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-121">When you are ready to submit the travel requisition, select **Workflow** > **Submit**.</span></span>

<span data-ttu-id="a71f3-122">Расталған іссапарға өтінімдерді **Менің шығыстарым: іссапарға өтінім** тармағында көруге болады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-122">You can view your approved travel requisitions under **My Expenses: Travel Requisition**.</span></span> 

## <a name="view-available-travel-requisitions"></a><span data-ttu-id="a71f3-123">Қолжетімді іссапарға өтінімдерді қарау</span><span class="sxs-lookup"><span data-stu-id="a71f3-123">View available travel requisitions</span></span>

<span data-ttu-id="a71f3-124">Іссапарға өтінімдердің барлығын **Менің шығыстарым: іссапарға өтінімдер** тармағында көруге болады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-124">You can view all of your travel requisitions under **My Expenses: Travel Requisitions**.</span></span>

## <a name="approve-travel-requisitions"></a><span data-ttu-id="a71f3-125">Іссапарға өтінімдерді растау</span><span class="sxs-lookup"><span data-stu-id="a71f3-125">Approve travel requisitions</span></span>

<span data-ttu-id="a71f3-126">Растау қажет іссапарға өтінімді таңдаңыз, содан кейін **Жұмыс ағыны** > **Растау** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-126">Select the travel requisition that you want to approve, and then select **Workflow** > **Approve**.</span></span>  

## <a name="submit-an-expense-report-using-your-approved-travel-requisition"></a><span data-ttu-id="a71f3-127">Расталған іссапарға өтінім көмегімен шығыс туралы есепті жіберу</span><span class="sxs-lookup"><span data-stu-id="a71f3-127">Submit an expense report using your approved travel requisition</span></span>

1. <span data-ttu-id="a71f3-128">Жаңа шығыс туралы есепті жасап, шығыс туралы есептер тақырыбында және расталған іссапарға өтінім тізімінен **Іссапар үшін салыстыру өтінімі** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-128">Create a new expense report and in the expense report header, and from the list of approved travel requisitions, select **Map to Travel requisition**.</span></span>
2. <span data-ttu-id="a71f3-129">**Іссапарға өтінім сомасы** өрісі шығыс туралы есеп тақырыбында автоматты түрде жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-129">The **Travel requisition amount** field is automatically updated in the expense report header.</span></span>
3. <span data-ttu-id="a71f3-130">Сапарға жұмсалған әр шығысты қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="a71f3-130">Add each expense incurred for the trip.</span></span> <span data-ttu-id="a71f3-131">**Алдын ала рұқсат етілген** өрісі қосылса, нақты шығыс санаты үшін сәйкестендірілген сома және рұқсат етілген сома жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="a71f3-131">If the **Pre-authorized** field is enabled, the reconciled amount and authorized amount for the specific expense category will be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="a71f3-132">Шығыс туралы есепті расталған іссапарға өтініммен салыстырған кезде, транзакция сомасы рұқсат етілген сомадан артық болмауы керек.</span><span class="sxs-lookup"><span data-stu-id="a71f3-132">When you map an expense report to an approved travel requisition, the transaction amount can't be greater than the authorized amount.</span></span> 
