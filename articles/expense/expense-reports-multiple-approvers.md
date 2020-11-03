---
title: Шығыс туралы есептер және бірнеше растаушылар
description: Бұл тақырып бірден көп адамның растауын қажет ететін шығыс туралы есептер жайлы ақпаратпен қамтамасыз етеді.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 548673541cee5ce598721f94415c0444995c8325
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079663"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="5f0b8-103">Шығыс туралы есептер және бірнеше растаушылар</span><span class="sxs-lookup"><span data-stu-id="5f0b8-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="5f0b8-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="5f0b8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5f0b8-105">Ұйымыңыздың шығысты растау саясатына байланысты жіберілген шығыс туралы есеп үшін растау бірден көп адамнан алынуы керек болуы мүмкін.  </span><span class="sxs-lookup"><span data-stu-id="5f0b8-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="5f0b8-106">Шығыс туралы есепті растау үшін жұмыс ағыны процесін орнатқан кезде сіз бір немесе бірнеше шығыс туралы есепті растаушыларға тапсырмалары мен қадамдары бар жұмыс ағыны элементтерін қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="5f0b8-107">Мысалы, барлық шығыс туралы есептерді екі басқа адамның растауы қажет болуы мүмкін, есепті тапсырған жұмысшының менеджері және кредиторлық берешек бөлімінің координаторы.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="5f0b8-108">Бірнеше шығыс туралы есепті растаушылар керек деп шешсеңіз, жұмыс ағыны элементтерін келесідегі кез келген жолмен қосуыңызға болады: </span><span class="sxs-lookup"><span data-stu-id="5f0b8-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="5f0b8-109">Бір қадамы бар бір растау элементін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-109">Add one approval element that has one step.</span></span> <span data-ttu-id="5f0b8-110">Мысалы, қадам шығыс туралы есепті пайдаланушы топқа тағайындауын және пайдаланушы топ мүшелерінің 50 пайызының растауын талап етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="5f0b8-111">Бірнеше қадамы бар бір растау элементін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="5f0b8-112">Мысалы, растау элементі келесі қадамдарды қамтуы мүмкін:</span><span class="sxs-lookup"><span data-stu-id="5f0b8-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="5f0b8-113">Шығыс туралы есепті жіберген жұмысшының менеджері оны растайды.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="5f0b8-114">Кредиторлық берешек бөлімінің жұмысшысы түсімдерді және шығыс туралы есеп элементтерін тексереді.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="5f0b8-115">Бюджет өкімшісі шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="5f0b8-116">Әрқайсысында бір қадамы бар бірнеше растау элементтерін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="5f0b8-117">Мысалы, жеке растау элементін келесі қадамдардың әрқайсысы үшін қоса аласыз:</span><span class="sxs-lookup"><span data-stu-id="5f0b8-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="5f0b8-118">Жұмысшының менеджері шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="5f0b8-119">Бюджет өкімшісі шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="5f0b8-119">The budget owner approves the expense report.</span></span>
