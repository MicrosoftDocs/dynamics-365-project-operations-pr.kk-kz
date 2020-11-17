---
title: Қаржылық өлшемнің әдепкі мәндері
description: Бұл бөлімде қаржылық өлшемнің әдепкі мәндері үшін әдепкі параметрлерді орнату туралы ақпарат берілген.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: aa6771ba5346fd4133b82c3e670badfa7655299f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131890"
---
# <a name="financial-dimension-defaults"></a><span data-ttu-id="099b1-103">Қаржылық өлшемнің әдепкі мәндері</span><span class="sxs-lookup"><span data-stu-id="099b1-103">Financial dimension defaults</span></span>

<span data-ttu-id="099b1-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="099b1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="099b1-105">Dynamics 365 Project Operations жүйесі жобалық қосалқы кітап пен жалпы қосалқы кітап транзакциялары туралы қосымша түсініктер беру үшін Dynamics 365 Finance жүйесіндегі [Қаржылық өлшемдер](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) құрылымын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="099b1-105">Dynamics 365 Project Operations uses the [Financial dimensions](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="099b1-106">Әдепкі қаржылық өлшемдер тапсырыс беруші, жобаны қаржыландыру көзі, аралық кезең, жобаның келісім-шарт жолы немесе жоба бойынша белгіленуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="099b1-106">Default financial dimensions can be set on a customer, project funding source, milestone, project contract line, or project.</span></span>

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="099b1-107">Тұтынушының әдепкі қаржылық өлшемдерін анықтау</span><span class="sxs-lookup"><span data-stu-id="099b1-107">Define default financial dimensions for a customer</span></span>

<span data-ttu-id="099b1-108">Тұтынушы өлшемінің әдепкі параметрлері Finance бағдарламасында көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="099b1-108">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="099b1-109">Өлшемнің әдепкі мәндерін орнату үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-109">Complete the following steps to set dimension defaults.</span></span>

1. <span data-ttu-id="099b1-110">**Дебиторлық қарыз** > **Тұтынушылар** > **Барлық тұтынушылар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="099b1-110">Go to **Accounts receivable** > **Customers** > **All customers**.</span></span>
2. <span data-ttu-id="099b1-111">**Тұтынушылар** бетінде, **Қаржылық өлшемдер** қойыншасында нақты тұтынушыға арналған қаржылық өлшем мәндерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-111">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="099b1-112">Жоба келісім-шарттарының әдепкі қаржылық өлшемдерін анықтау</span><span class="sxs-lookup"><span data-stu-id="099b1-112">Define default financial dimensions for project contracts</span></span>

<span data-ttu-id="099b1-113">Жобалық келісім-шарттар Common Data Service (CDS) жүйесінде жасалып, сақталады.</span><span class="sxs-lookup"><span data-stu-id="099b1-113">Project contracts are created and maintained in Common Data Service (CDS).</span></span> <span data-ttu-id="099b1-114">Жобалық келісім-шарттардың есеп төлсипаттары Finance бағдарламасындағы **Жобаларды басқару және есеп** модулінде орнатылады.</span><span class="sxs-lookup"><span data-stu-id="099b1-114">Accounting attributes for project contracts are set in the **Project management and accounting** module in Finance.</span></span>

### <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="099b1-115">Жобаны қаржыландыру көзі үшін қаржылық өлшемдерді орнату</span><span class="sxs-lookup"><span data-stu-id="099b1-115">Set financial dimensions for a project funding source</span></span>

1. <span data-ttu-id="099b1-116">**Жобаларды басқару және есепке алу** > **Жобалар** > **Жоба келісім-шарттары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="099b1-116">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="099b1-117">Жаңартқыңыз келетін жазбаны таңдап, **Жобалық келісім-шарт** қойыншасында **Әдепкі есепті көрсету** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-117">Select the record you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="099b1-118">**Байланысты ақпарат** терезесін ашып, **Қаржыландыру көздері** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-118">Expand **Related information** and select the **Funding sources** tab.</span></span>
4. <span data-ttu-id="099b1-119">Қаржылық өлшемнің әдепкі мәндерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-119">Set the financial dimension defaults.</span></span> <span data-ttu-id="099b1-120">Қаржылық өлшемдер әдепкі бойынша тұтынушы тіркелгісіне қатысты болатынын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="099b1-120">Notice that the financial dimensions default from the customer account.</span></span>

### <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="099b1-121">Жобалық келісім-шарт жолы үшін қаржылық өлшемдерді орнату</span><span class="sxs-lookup"><span data-stu-id="099b1-121">Set financial dimensions for a project contract line</span></span>

1. <span data-ttu-id="099b1-122">**Жобаларды басқару және есепке алу** > **Жобалар** > **Жоба келісім-шарттары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="099b1-122">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="099b1-123">Жаңартқыңыз келетін жазбаны таңдап, **Жобалық келісім-шарт** қойыншасында **Әдепкі есепті көрсету** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-123">Select the record you want to update and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="099b1-124">**Байланысты ақпарат** терезесін ашып, **Келісім-шарт жолдары** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-124">Expand **Related information** and select the **Contract lines** tab.</span></span>
4. <span data-ttu-id="099b1-125">Қаржылық өлшемнің әдепкі мәндерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-125">Set the financial dimension defaults.</span></span> <span data-ttu-id="099b1-126">Қаржылық өлшемнің әдепкі мәндері қолданылады және оларды тек белгіленген баға (аралық кезең) келісім-шарт жолдарымен пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="099b1-126">The financial dimension defaults are applicable and can be used only with Fixed price (milestone) contract lines.</span></span>

<span data-ttu-id="099b1-127">Бұл әдепкі мәндер байланысты жобаның шоттағы операциялар мен шот-фактуралар желілерінде пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="099b1-127">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="099b1-128">Жобалардың әдепкі қаржылық өлшемдерін анықтау</span><span class="sxs-lookup"><span data-stu-id="099b1-128">Define default financial dimensions for projects</span></span>

<span data-ttu-id="099b1-129">Жобалар CDS жүйесінде жасалып, сақталады.</span><span class="sxs-lookup"><span data-stu-id="099b1-129">Projects are created and maintained in CDS.</span></span> <span data-ttu-id="099b1-130">Жобалардың есеп төлсипаттары Finance бағдарламасындағы **Жобаларды басқару және есеп** модулінде орнатылады.</span><span class="sxs-lookup"><span data-stu-id="099b1-130">Accounting attributes for projects are set in the **Project management and accounting** module in Finance.</span></span>

1. <span data-ttu-id="099b1-131">**Жобаларды басқару және есепке алу** > **Жобалар** > **Барлық жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="099b1-131">Go to **Project management and accounting** > **Projects** > **All projects**.</span></span>
2. <span data-ttu-id="099b1-132">Жаңартқыңыз келетін жазбаны таңдап, **Жоба** қойыншасында **Әдепкі есепті көрсету** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-132">Select the record that you want to update and on the **Project** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="099b1-133">**Байланысты ақпарат** терезесін ашып, **Орнату** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-133">Expand **Related information** and select the **Setup** tab.</span></span>
4. <span data-ttu-id="099b1-134">Қаржылық өлшемнің әдепкі мәндерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="099b1-134">Set the financial dimension defaults.</span></span> <span data-ttu-id="099b1-135">Қаржылық өлшемдер әдепкі бойынша тұтынушы тіркелгісіне қатысты болатынын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="099b1-135">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="099b1-136">Егер жоба бірнеше келісім-шарттық тұтынушылары бар келісім-шарт жолымен байланысты болса, әдепкі қаржылық өлшемдер үшін негізгі тұтынушы пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="099b1-136">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="099b1-137">Жобаның әдепкі қаржылық өлшемдері **Project Operations біріктіру журналындағы** және байланысты жобалық есеп-шот жолдарындағы уақыт, шығыс және ақы транзакцияларына арналған журнал жолының әдепкі мәндерін орнату үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="099b1-137">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration Journal** and on related project invoice lines.</span></span>
