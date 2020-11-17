---
title: Шығыс саясаттарын анықтау
description: Шығыстар туралы есептер мен саяхат талаптарын енгізу және ұсыну кезінде сіздің жұмысшыларыңыз ұстанатын шығындар саясатын анықтай аласыз.
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
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: c55cec132649daf9ee08ea4d8db3668860247934
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128425"
---
# <a name="define-expense-policies"></a><span data-ttu-id="5582b-103">Шығыс саясаттарын анықтау</span><span class="sxs-lookup"><span data-stu-id="5582b-103">Define expense policies</span></span>

<span data-ttu-id="5582b-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="5582b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5582b-105">Шығыстар туралы есептер мен саяхат талаптарын енгізу және ұсыну кезінде сіздің жұмысшыларыңыз ұстанатын саясатты анықтай аласыз.</span><span class="sxs-lookup"><span data-stu-id="5582b-105">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="5582b-106">Шығыс саясаттарын іске асыру шығыстарды тиімді басқаруға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="5582b-106">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="5582b-107">Мысалы, Нью-Йорк қаласындағы қонақүй шығыстары үшін саясатты орнатуға болады, ол жерде бір түн бойынша шығыс 250 АҚШ долларынан аспау қажет.</span><span class="sxs-lookup"><span data-stu-id="5582b-107">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="5582b-108">Егер жұмысшы бөлме бойынша мөлшерлеме осы сомадан асатын шығыс есебін немесе саяхат өтінімін жіберетін болса, жүйе</span><span class="sxs-lookup"><span data-stu-id="5582b-108">If a worker submits an expense report or travel requisition where the room rate exceeds this amount, the system will notify the</span></span>         
<span data-ttu-id="5582b-109">жұмысшыға шығыс бойынша саясат сомасы асып кеткені туралы хабарлайды.</span><span class="sxs-lookup"><span data-stu-id="5582b-109">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="5582b-110">Сіз саясатты анықтаған кезде жұмысшы алатын</span><span class="sxs-lookup"><span data-stu-id="5582b-110">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="5582b-111">хабарды конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="5582b-111">define the policy.</span></span>      
        
<span data-ttu-id="5582b-112">Саясаттардың үш түрін анықтай аласыз:</span><span class="sxs-lookup"><span data-stu-id="5582b-112">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="5582b-113">**Ескерту**: Жұмысшыға шығыстар туралы есепті немесе саяхат өтінімін беруді ұсынады, бірақ шығын барлық мақұлдаушылар үшін және</span><span class="sxs-lookup"><span data-stu-id="5582b-113">**Warning**: Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>         
  <span data-ttu-id="5582b-114">кейінірек есеп беру үшін белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="5582b-114">for later reporting.</span></span>        

- <span data-ttu-id="5582b-115">**Қате**: Шығындар туралы есепті немесе саяхат өтінімін ұсынар алдында жұмысшыдан саясатты сақтау үшін шығындарды қайта қарауды талап етеді.</span><span class="sxs-lookup"><span data-stu-id="5582b-115">**Error**: Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>        
 
 - <span data-ttu-id="5582b-116">**Негіздеме**: Жұмысшыдан немесе менеджерден шығындар туралы есеп немесе саяхат өтінімі берілгенге дейін саясат сомасынан асып кетуінен негіздеме енгізуді талап етеді.</span><span class="sxs-lookup"><span data-stu-id="5582b-116">**Justification**: Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="5582b-117">Саясат бойынша кеңестер</span><span class="sxs-lookup"><span data-stu-id="5582b-117">Policy tips</span></span>
<span data-ttu-id="5582b-118">Шығысты басқару үшін жаңа саясаттарын жасау кезінде сізге көмектесетін бірнеше ұсыныстар бар:</span><span class="sxs-lookup"><span data-stu-id="5582b-118">Here are a few suggestions that can assist you when creating new policies for expense management:</span></span> 

- <span data-ttu-id="5582b-119">Саясат күшіне енеді, демек, саясат шығындар пайда болған күннен кейінгі күнмен жасалған жағдайда күшіне енбейді.</span><span class="sxs-lookup"><span data-stu-id="5582b-119">Policies are date effective which means a policy won't take effect if it's created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="5582b-120">Мысалы, сіз бүгін 50 доллардан тұратын максималды тамақтану шығыстарын орындау үшін жаңа саясат жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="5582b-120">For example, you create a new policy today to enforce a maximum meal expense of $50.</span></span> <span data-ttu-id="5582b-121">Кешегі күнге енгізілген барлық шығыстар осы саясатқа сәйкес тексерілмейді.</span><span class="sxs-lookup"><span data-stu-id="5582b-121">Any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
- <span data-ttu-id="5582b-122">Элементтеуге болмайтын шығыс санаты үшін саясат жасаған кезде, шығыс бабының түрі үшін шарт қосуды қарастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="5582b-122">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="5582b-123">Түбіртекті талап ету сияқты кейбір ережелер элементтелген жолдар үшін мағынасы болмауы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="5582b-123">Some policies, such as requiring a receipt, may not make sense for itemized lines.</span></span> <span data-ttu-id="5582b-124">Мұндай жағдайда саясат тек тақырып жолына немесе элементтелмеген жолға қолданылады.</span><span class="sxs-lookup"><span data-stu-id="5582b-124">In this situation, the policy only is applied to the header line or a non-itemized line.</span></span> 
- <span data-ttu-id="5582b-125">Шығыстарды басқару саясаты әдепкі бойынша бастапқы нысанмен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="5582b-125">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="5582b-126">Компанияаралық сценарийлер үшін сіз оның орнына мақсатты нысанға (қарыз алушы) қатысты бағаланатын саясатты орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="5582b-126">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="5582b-127">Мақсатты нысанға қатысты саясаттарды іске қосу үшін **Мүмкіндікті басқару** жұмыс кеңістігіндегі **Шығыс саясатын қарыз алушы заңды тұлғамен салыстырып бағалау** мүмкіндігін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="5582b-127">To run the policies against the destination entity, turn on the **Evaluate Expense policy against borrowing legal entity** feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="5582b-128">Саясаттарды бағалаған кезде</span><span class="sxs-lookup"><span data-stu-id="5582b-128">When to evaluate policies</span></span>

<span data-ttu-id="5582b-129">Шығысты басқару параметрлерінде шығысты басқару саясаттарын бағалау үшін жол сақталған кезде немесе шығыс туралы есеп жіберілген кезде таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="5582b-129">In expense management parameters, you can select to evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="5582b-130">Жол сақталған кезде бағалауды таңдасаңыз, пайдаланушылар өздерінің шығыстары туралы есепті бірден толтыру үшін не істеу керектігін ертерек біледі.</span><span class="sxs-lookup"><span data-stu-id="5582b-130">If you choose to evaluate when a line is saved, users will have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="5582b-131">Әйтпесе, сіз саясатты бағалауды кейінге қалдыра аласыз және жұмыс ағынына жіберу кезінде, соңында тексеру арқылы уақытты үнемдей аласыз.</span><span class="sxs-lookup"><span data-stu-id="5582b-131">Otherwise, you can delay policy evaluation and save time by validating at the end, during the submission to workflow.</span></span>
