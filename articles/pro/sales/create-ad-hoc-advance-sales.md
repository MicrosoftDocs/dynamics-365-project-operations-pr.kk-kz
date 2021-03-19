---
title: Келісім-шартта арнайы аванс жасау
description: Бұл тақырыпта қажетінше келісім-шартта авансты жасау туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2f0a6391a3bf6dd39d21504a6f286e4ff1954183
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273604"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract"></a><span data-ttu-id="92619-103">Келісім-шартта арнайы аванс жасау</span><span class="sxs-lookup"><span data-stu-id="92619-103">Creating an ad hoc advance on a contract</span></span>

<span data-ttu-id="92619-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="92619-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="92619-105">Microsoft Dynamics 365 Project Operations алдын ала төлемдер мен аванстарды қамтитын есеп-шотты ұсыну сценарийлерін қолдайды.</span><span class="sxs-lookup"><span data-stu-id="92619-105">Microsoft Dynamics 365 Project Operations supports invoicing scenarios that involve pre-payments and advances.</span></span> <span data-ttu-id="92619-106">**Project Operations** бағдарламасында **Аванстар** келісім-шарттарын пайдалану процесі **Қаламақы** келісім-шарттарына ұқсас.</span><span class="sxs-lookup"><span data-stu-id="92619-106">The process for using **Advances** in **Project Operations** is similar to **Retainer** contracts.</span></span> 

<span data-ttu-id="92619-107">Тұтынушыға авансына есеп-шотты ұсыну үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="92619-107">Complete the following steps to invoice the customer for an advance.</span></span>

1. <span data-ttu-id="92619-108">**Жобалық келісім-шарт** бетіне өтіп, содан кейін **Аванстар және қаламақылар** қойындысын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="92619-108">Go to the **Project Contract** page, and then select the **Advances and Retainers** tab.</span></span>
2. <span data-ttu-id="92619-109">Бұрын жазылған барлық аванстар мен алдын ала төлемдер тізілген қосымша тордан **+ Жаңа жобаның келісім-шарт қаламақысы** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="92619-109">In the subgrid that lists all the previously recorded advances and prepayments, select **+ New Project contract retainer**.</span></span> 

    <span data-ttu-id="92619-110">Алдын ала төлемді немесе авансты жазу үшін **Жылдам жасау** пішіні ашылады.</span><span class="sxs-lookup"><span data-stu-id="92619-110">The **Quick Create** form opens for recording a prepayment or advance.</span></span>
    
3. <span data-ttu-id="92619-111">Төмендегі кестеде аванс жазуға арналған өрістер мен жаңаларын жасаған кезде ескеретін жайттар келтірілген:</span><span class="sxs-lookup"><span data-stu-id="92619-111">The table below lists the fields for recording an advance and the considerations to keep in mind as you create new ones:</span></span>

    | <span data-ttu-id="92619-112">Өріс</span><span class="sxs-lookup"><span data-stu-id="92619-112">Field</span></span> | <span data-ttu-id="92619-113">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="92619-113">Description</span></span> | <span data-ttu-id="92619-114">Төменгі әсер</span><span class="sxs-lookup"><span data-stu-id="92619-114">Downstream impact</span></span> |
    | --- | --- | --- |
    | <span data-ttu-id="92619-115">**Жоба келісім-шарты тұтынушысы**</span><span class="sxs-lookup"><span data-stu-id="92619-115">**Project Contract Customer**</span></span> | <span data-ttu-id="92619-116">Бұл өріс келісім-шарт бойынша қай тұтынушыға осы аванс үшін есеп-шот ұсынылатынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="92619-116">This field indicates which customer on the contract will be invoiced for this advance.</span></span> | <span data-ttu-id="92619-117">Келісім-шарт бойынша бірнеше тұтынушылар болса және олардың әрқайсысына белгілі бір қаламақы немесе аванс сомасына есеп-шот ұсынғыңыз келсе, әр тұтынушы үшін авансты жеке жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="92619-117">If you have multiple customers on the contract and want to invoice each of them for a specific retainer or advance amount, create an advance for each customer individually.</span></span> |
    | <span data-ttu-id="92619-118">**Сипаттамасы**</span><span class="sxs-lookup"><span data-stu-id="92619-118">**Description**</span></span> | <span data-ttu-id="92619-119">Осы авансты анықтауға көмектесетін аванс мақсатының немесе уақытының сипаттамасы.</span><span class="sxs-lookup"><span data-stu-id="92619-119">The description of the purpose or timing of the advance to help identify this advance.</span></span> | <span data-ttu-id="92619-120">Бұл сипаттама осы аванс үшін есеп-шот жолында көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="92619-120">This description is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="92619-121">**Мөлшер**</span><span class="sxs-lookup"><span data-stu-id="92619-121">**Amount**</span></span> | <span data-ttu-id="92619-122">Алдын ала төлемнің немесе аванстың сомасы.</span><span class="sxs-lookup"><span data-stu-id="92619-122">The amount for the pre-payment or advance.</span></span> | <span data-ttu-id="92619-123">Бұл сома осы аванс үшін есеп-шот жолында көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="92619-123">This amount is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="92619-124">**Есеп-шот күні**</span><span class="sxs-lookup"><span data-stu-id="92619-124">**Invoice Date**</span></span> | <span data-ttu-id="92619-125">Тұтынушыға осы аванстың есеп-шоты ұсынылған күн.</span><span class="sxs-lookup"><span data-stu-id="92619-125">The date on which this advance is invoiced to the customer.</span></span> | <span data-ttu-id="92619-126">Осы аванс үшін есеп-шот жолын жасау үшін автоматтандырылған есеп-шотты жасау процесінің күні.</span><span class="sxs-lookup"><span data-stu-id="92619-126">This is the date for the automated invoice creation process to create an invoice line for this advance.</span></span> |
    | <span data-ttu-id="92619-127">**Есеп-шот күйі**</span><span class="sxs-lookup"><span data-stu-id="92619-127">**Invoice Status**</span></span> | <span data-ttu-id="92619-128">Бұл осы тұтынушы үшін жоба есеп-шотына осы аванстың қосылатынын немесе қосылмайтындығын көрсететін параметрі.</span><span class="sxs-lookup"><span data-stu-id="92619-128">This is an option setting that indicates whether this advance is added to a draft invoice for this customer.</span></span> <span data-ttu-id="92619-129">Ықтимал мәндер:</span><span class="sxs-lookup"><span data-stu-id="92619-129">The possible values are:</span></span></br><span data-ttu-id="92619-130">- **Есеп-шот ұсынуға дайын емес**</span><span class="sxs-lookup"><span data-stu-id="92619-130">- **Not ready to invoice**</span></span></br><span data-ttu-id="92619-131">- **Есеп-шот ұсынуға дайын**</span><span class="sxs-lookup"><span data-stu-id="92619-131">- **Ready to invoice**</span></span> | <span data-ttu-id="92619-132">Аванс немесе алдын ала төлем **Есеп-шот ұсынуға дайын** ретінде белгіленген кезде, ол жоба есеп-шотына жол уақыты ретінде қосылады.</span><span class="sxs-lookup"><span data-stu-id="92619-132">When an advance or pre-payment is marked as **Ready to invoice**, it is added as a line time on a draft invoice.</span></span> <span data-ttu-id="92619-133">Келесі есеп-шот ұсыну кезеңіндегі жоба шығындарымен салыстыру үшін тек толық есеп-шоты ұсынылған авансты пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="92619-133">Only a fully invoiced advance can be used to reconcile against project costs for the next invoice period.</span></span> |

4. <span data-ttu-id="92619-134">Авансты немесе алдын ала төлемді жазу үшін жылдам құру диалогында **Сақтау және жабу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="92619-134">Select **Save and close** on the quick create dialog to record the advance or the pre-payment.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]