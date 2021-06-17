---
title: Шығыс туралы есептер және бірнеше растаушылар
description: Бұл тақырып бірден көп адамның растауын қажет ететін шығыс туралы есептер жайлы ақпаратпен қамтамасыз етеді.
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
ms.openlocfilehash: 2502b2975ad3aebad720970e693ea68eac0a302c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002063"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="f2152-103">Шығыс туралы есептер және бірнеше растаушылар</span><span class="sxs-lookup"><span data-stu-id="f2152-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="f2152-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="f2152-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f2152-105">Ұйымыңыздың шығысты растау саясатына байланысты жіберілген шығыс туралы есеп үшін растау бірден көп адамнан алынуы керек болуы мүмкін.  </span><span class="sxs-lookup"><span data-stu-id="f2152-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="f2152-106">Шығыс туралы есепті растау үшін жұмыс ағыны процесін орнатқан кезде сіз бір немесе бірнеше шығыс туралы есепті растаушыларға тапсырмалары мен қадамдары бар жұмыс ағыны элементтерін қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="f2152-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="f2152-107">Мысалы, барлық шығыс туралы есептерді екі басқа адамның растауы қажет болуы мүмкін, есепті тапсырған жұмысшының менеджері және кредиторлық берешек бөлімінің координаторы.</span><span class="sxs-lookup"><span data-stu-id="f2152-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="f2152-108">Бірнеше шығыс туралы есепті растаушылар керек деп шешсеңіз, жұмыс ағыны элементтерін келесідегі кез келген жолмен қосуыңызға болады: </span><span class="sxs-lookup"><span data-stu-id="f2152-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="f2152-109">Бір қадамы бар бір растау элементін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f2152-109">Add one approval element that has one step.</span></span> <span data-ttu-id="f2152-110">Мысалы, қадам шығыс туралы есепті пайдаланушы топқа тағайындауын және пайдаланушы топ мүшелерінің 50 пайызының растауын талап етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f2152-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="f2152-111">Бірнеше қадамы бар бір растау элементін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f2152-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="f2152-112">Мысалы, растау элементі келесі қадамдарды қамтуы мүмкін:</span><span class="sxs-lookup"><span data-stu-id="f2152-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="f2152-113">Шығыс туралы есепті жіберген жұмысшының менеджері оны растайды.</span><span class="sxs-lookup"><span data-stu-id="f2152-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="f2152-114">Кредиторлық берешек бөлімінің жұмысшысы түсімдерді және шығыс туралы есеп элементтерін тексереді.</span><span class="sxs-lookup"><span data-stu-id="f2152-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="f2152-115">Бюджет өкімшісі шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="f2152-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="f2152-116">Әрқайсысында бір қадамы бар бірнеше растау элементтерін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f2152-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="f2152-117">Мысалы, жеке растау элементін келесі қадамдардың әрқайсысы үшін қоса аласыз:</span><span class="sxs-lookup"><span data-stu-id="f2152-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="f2152-118">Жұмысшының менеджері шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="f2152-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="f2152-119">Бюджет өкімшісі шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="f2152-119">The budget owner approves the expense report.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]