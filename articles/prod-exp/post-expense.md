---
title: Шығыс туралы есепті орналастыру
description: Бұл тақырып шығыстар туралы есепті бас кітапқа енгізу жолын түсіндіреді.
author: saraschi2
manager: AnnBe
ms.date: 02/26/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 2d008ef8dd55550431fbb9e329cd7d9428a08831
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079806"
---
# <a name="post-an-expense-report"></a><span data-ttu-id="58585-103">Шығыс туралы есепті орналастыру</span><span class="sxs-lookup"><span data-stu-id="58585-103">Post an expense report</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="58585-104">Шығыс туралы есеп мақұлданғаннан кейін және негізгі журналға жіберілгеннен кейін, оны бас кітапқа енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="58585-104">After an expense report has been approved and transferred to the general journal, it can be posted to the general ledger.</span></span> <span data-ttu-id="58585-105">Шығыс туралы есепті жариялаған кезде, қосылған құн салығын (ҚҚС) алуға жарамды шығыстар анықталады.</span><span class="sxs-lookup"><span data-stu-id="58585-105">When you post an expense report, expenses that are eligible for recovery of value-added tax (VAT) are identified.</span></span> <span data-ttu-id="58585-106">ҚҚС бойынша төлемдерді тексеру және қалпына келтіру міндеті шығыс туралы есепті тексеруге жауапты қызметкерге жүктелген.</span><span class="sxs-lookup"><span data-stu-id="58585-106">The task of verifying and recovering VAT payments is assigned to the employee who is responsible for verifying the expense report.</span></span>

<span data-ttu-id="58585-107">Егер шығыс туралы есептегі шығыстар қызметкерді жалдайтын компаниядан басқа компанияға есептелсе, онда осы шығыстар тиесілі компанияны да және шығыстар алынатын компанияны да тексеру қажет.</span><span class="sxs-lookup"><span data-stu-id="58585-107">If expenses on an expense report are charged to a company other than the company that employs the employee, you must verify the company that those expenses are owed to and the company that the expenses are owed from.</span></span> <span data-ttu-id="58585-108">Мысалы, шығыс туралы есеп берген қызметкер DAT компаниясында жұмыс істейді, бірақ шығыстарды DIR компаниясына аударды.</span><span class="sxs-lookup"><span data-stu-id="58585-108">For example, the employee who submitted an expense report works for the DAT company but charged an expense to the DIR company.</span></span> <span data-ttu-id="58585-109">Бұл жағдайда DAT - бұл шығыстар тиесілі компания, ал DIR - бұл шығыстар алынатын компания.</span><span class="sxs-lookup"><span data-stu-id="58585-109">In this case, DAT is the company that the expense is owed to, and DIR is the company that the expense is owed from.</span></span> <span data-ttu-id="58585-110">Осы журнал жолдарын тексергеннен кейін, шығыс жолдарын жалпы тіркелімге жариялауға болады.</span><span class="sxs-lookup"><span data-stu-id="58585-110">After you verify these journal lines, you can post the expense lines to the general ledger.</span></span>

<span data-ttu-id="58585-111">Шығыс туралы есепті жариялау үшін **Бекітілген шығыс туралы есептер** бетінде шығыс туралы есепті таңдап, Әрекеттер тақтасында **Жариялау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="58585-111">To post an expense report, on the **Approved expense reports** page, select the expense report, and then, on the Action Pane, select **Post**.</span></span>

<span data-ttu-id="58585-112">Сонымен қатар тізімдегі барлық шығыс туралы есептерді бір уақытта жариялауға болады.</span><span class="sxs-lookup"><span data-stu-id="58585-112">You can also post all the expense reports in the list at the same time.</span></span> <span data-ttu-id="58585-113">Барлық шығыс туралы есептерді таңдап, содан кейін **Жариялау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="58585-113">Select all the expense reports, and then select **Post**.</span></span>