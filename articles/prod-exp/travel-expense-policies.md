---
title: Шығын ережелерін орнату
description: Сіз Microsoft Dynamics 365 Finance бағдарламасында шығын есептері мен іссапар өтінімдерін енгізу және жіберу кезінде сіздің жұмысшыларыңыз ұстанатын шығын ережелерін орната аласыз.
author: suvaidya
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9c014b0593a87ce50f09175b77d9cf498a65391e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271270"
---
# <a name="set-up-expense-policies"></a><span data-ttu-id="3513f-103">Шығын ережелерін орнату</span><span class="sxs-lookup"><span data-stu-id="3513f-103">Set up expense policies</span></span>

<span data-ttu-id="3513f-104">Шығыстар туралы есептер мен саяхат талаптарын енгізу және ұсыну кезінде сіздің жұмысшыларыңыз ұстанатын саясатты анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="3513f-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="3513f-105">Шығыс саясаттарын іске асыру шығыстарды тиімді басқаруға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="3513f-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="3513f-106">Мысалы, Нью-Йорк қаласындағы қонақүй шығыстары үшін саясатты орнатуға болады, ол жерде бір түн бойынша шығыс 250 АҚШ долларынан аспау қажет.</span><span class="sxs-lookup"><span data-stu-id="3513f-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="3513f-107">Егер жұмысшы шығын есебін немесе іссапарға өтінімді жіберсе, іссапар құны осы сомадан асса, жүйе</span><span class="sxs-lookup"><span data-stu-id="3513f-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="3513f-108">жұмысшыға шығыс бойынша саясат сомасы асып кеткені туралы хабарлайды.</span><span class="sxs-lookup"><span data-stu-id="3513f-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="3513f-109">Сіз саясатты анықтаған кезде жұмысшы алатын</span><span class="sxs-lookup"><span data-stu-id="3513f-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="3513f-110">хабарды конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="3513f-110">define the policy.</span></span>      
        
<span data-ttu-id="3513f-111">Саясаттардың үш түрін анықтай аласыз:</span><span class="sxs-lookup"><span data-stu-id="3513f-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="3513f-112">Ескерту – жұмысшыға шығын туралы есепті немесе іссапар өтінімін беруді ұсынады, бірақ шығын барлық мақұлдаушылар үшін және</span><span class="sxs-lookup"><span data-stu-id="3513f-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="3513f-113">кейінірек есеп беру үшін белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="3513f-113">for later reporting.</span></span>        

- <span data-ttu-id="3513f-114">Қате – шығын туралы есепті немесе іссапар өтінімін ұсынар алдында жұмысшыдан іссапарға сай келу үшін шығынды қайта қарауды талап етеді.</span><span class="sxs-lookup"><span data-stu-id="3513f-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="3513f-115">Негіздеме – жұмысшыдан немесе менеджерден шығындар туралы есеп немесе іссапар өтінімі берілгенге дейін іссапар сомасынан асып кетуіне негіздеме енгізуді талап етеді.</span><span class="sxs-lookup"><span data-stu-id="3513f-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="3513f-116">Саясат бойынша кеңестер</span><span class="sxs-lookup"><span data-stu-id="3513f-116">Policy tips</span></span>
<span data-ttu-id="3513f-117">Шығынды басқару үшін жаңа ережелерді жасау кезінде сізге көмектесетін бірнеше ұсыныстар бар.</span><span class="sxs-lookup"><span data-stu-id="3513f-117">Here are a few suggestions that can assist you when creating new policies for expense management.</span></span> 
* <span data-ttu-id="3513f-118">Ережелер күндерге тікелей тәуелді және егер ереже шығын шыққан күннен кейінгі күні жасалса, күшіне енбейді.</span><span class="sxs-lookup"><span data-stu-id="3513f-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="3513f-119">Мысалы, егер сіз тамақтанудың максималды шығынын $50 етіп, жаңа ереже жасасаңыз, онда кеше жасалған барлық шығындардың осы ережеге сәйкес екендігі тексерілмейді.</span><span class="sxs-lookup"><span data-stu-id="3513f-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="3513f-120">Элементтеуге болмайтын шығыс санаты үшін саясат жасаған кезде, шығыс бабының түрі үшін шарт қосуды қарастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="3513f-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="3513f-121">Түбіртекті талап ету сияқты кейбір ережелердің егжей-тегжейлі жолдар үшін мағынасы болмауы мүмкін және тек тақырып жолына немесе егжей-тегжейлі емес жолға қолданылуы керек.</span><span class="sxs-lookup"><span data-stu-id="3513f-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 
* <span data-ttu-id="3513f-122">Шығыстарды басқару саясаты әдепкі бойынша бастапқы нысанмен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="3513f-122">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="3513f-123">Компанияаралық сценарийлер үшін сіз оның орнына мақсатты нысанға (қарыз алушы) қатысты бағаланатын саясатты орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="3513f-123">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="3513f-124">Мақсатты нысанға қатысты ережелерді іске қосу үшін **Мүмкіндікті басқару** жұмыс кеңістігіндегі "Шығын ережесін қарыз алушы заңды тұлғамен салыстырып бағалау" мүмкіндігін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="3513f-124">To run the policies against the destination entity, turn on the "Evaluate Expense policy against borrowing legal entity" feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="3513f-125">Саясаттарды бағалаған кезде</span><span class="sxs-lookup"><span data-stu-id="3513f-125">When to evaluate policies</span></span>

<span data-ttu-id="3513f-126">Шығынды басқару параметрлерінде жол сақталған кезде шығынды басқару ережелерін немесе шығын туралы есеп жіберілген кезде бағалау мүмкіндігі бар.</span><span class="sxs-lookup"><span data-stu-id="3513f-126">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="3513f-127">Жолдың қашан сақталатынын бағалауды таңдайтын болсаңыз, бұл пайдаланушылар өздерінің шығындары туралы есепті бірден толтыру үшін не істеу керек екенін ерте білуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="3513f-127">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="3513f-128">Әйтпесе, сіз ережені бағалауды кейінге қалдыра аласыз және жұмыс ағынына жіберілген кезде, соңында тексеру аяқталса, уақытты үнемдей аласыз.</span><span class="sxs-lookup"><span data-stu-id="3513f-128">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]