---
title: Шығыс туралы есептегі бірнеше бекітуші
description: Бұл тақырыпта бірнеше адамның мақұлдауын қажет ететін шығыс туралы есептер туралы ақпарат беріледі.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: ce24b156a268f9f5aada35f9314d2d9c6607200b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079816"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="8cd07-103">Шығыс туралы есептегі бірнеше бекітуші</span><span class="sxs-lookup"><span data-stu-id="8cd07-103">Multiple approvers on an expense report</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="8cd07-104">Ұйымыңыздың шығыстарды мақұлдау саясатына байланысты, бірнеше адам қызметкер ұсынған шығыс туралы есепті мақұлдауы керек.</span><span class="sxs-lookup"><span data-stu-id="8cd07-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="8cd07-105">Шығыс туралы есепті растау үшін жұмыс ағыны процесін орнатқан кезде сіз бір немесе бірнеше шығыс туралы есепті растаушыларға тапсырмалары мен қадамдары бар жұмыс ағыны элементтерін қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="8cd07-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="8cd07-106">Мысалы, барлық шығыс туралы есептерді алдымен есепті берген қызметкердің менеджері, содан кейін несие берушілер үйлестірушісі мақұлдауын талап ете аласыз.</span><span class="sxs-lookup"><span data-stu-id="8cd07-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="8cd07-107">Бірнеше шығыс туралы есепті растаушылар керек деп шешсеңіз, жұмыс ағыны элементтерін келесідегі кез келген жолмен қосуыңызға болады: </span><span class="sxs-lookup"><span data-stu-id="8cd07-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="8cd07-108">Бір қадамы бар бір растау элементін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="8cd07-108">Add one approval element that has one step.</span></span> <span data-ttu-id="8cd07-109">Мысалы, қадам шығыс туралы есепті пайдаланушы топқа тағайындауын және пайдаланушы топ мүшелерінің 50 пайызының растауын талап етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8cd07-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="8cd07-110">Бірнеше қадамы бар бір растау элементін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="8cd07-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="8cd07-111">Мысалы, растау элементі келесі қадамдарды қамтуы мүмкін:</span><span class="sxs-lookup"><span data-stu-id="8cd07-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="8cd07-112">Шығыс туралы есепті жіберген жұмысшының менеджері оны растайды.</span><span class="sxs-lookup"><span data-stu-id="8cd07-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="8cd07-113">Кредиторлық берешек бөлімінің жұмысшысы түсімдерді және шығыс туралы есеп элементтерін тексереді.</span><span class="sxs-lookup"><span data-stu-id="8cd07-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="8cd07-114">Бюджет өкімшісі шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="8cd07-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="8cd07-115">Әрқайсысында бір қадамы бар бірнеше растау элементтерін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="8cd07-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="8cd07-116">Мысалы, жеке растау элементін келесі қадамдардың әрқайсысы үшін қоса аласыз:</span><span class="sxs-lookup"><span data-stu-id="8cd07-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="8cd07-117">Жұмысшының менеджері шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="8cd07-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="8cd07-118">Бюджет өкімшісі шығыс туралы есепті растайды.</span><span class="sxs-lookup"><span data-stu-id="8cd07-118">The budget owner approves the expense report.</span></span>
