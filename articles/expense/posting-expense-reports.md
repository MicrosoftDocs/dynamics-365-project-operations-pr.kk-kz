---
title: Шығыс туралы есептерді өткізу
description: Бұл тақырыпта шығыс туралы есептерді жариялау әдісі түсіндірілген.
author: suvaidya
manager: AnnBe
ms.date: 09/09/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: ec897373cd74f7d7f63cd9ca4c46f4245336eb7f
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907415"
---
# <a name="post-expense-reports"></a><span data-ttu-id="3fe94-103">Шығыс туралы есептерді өткізу</span><span class="sxs-lookup"><span data-stu-id="3fe94-103">Post expense reports</span></span>

<span data-ttu-id="3fe94-104">Шығыс туралы есеп мақұлданғаннан кейін және негізгі журналға жіберілгеннен кейін, оны жариялауға болады.</span><span class="sxs-lookup"><span data-stu-id="3fe94-104">After an expense report has been approved and transferred to the general journal, it can be posted.</span></span> <span data-ttu-id="3fe94-105">Шығыс туралы есепті жариялаған кезде, қосылған құн салығын (ҚҚС) алуға жарамды шығыстар анықталады.</span><span class="sxs-lookup"><span data-stu-id="3fe94-105">When you post an expense report, expenses that are eligible for recovery of value-added tax (VAT) are identified.</span></span> <span data-ttu-id="3fe94-106">ҚҚС бойынша төлемдерді тексеру және қалпына келтіру міндеті шығыс туралы есепті тексеруге жауапты қызметкерге жүктелген.</span><span class="sxs-lookup"><span data-stu-id="3fe94-106">The task of verifying and recovering VAT payments is assigned to the employee who is responsible for verifying the expense report.</span></span>

<span data-ttu-id="3fe94-107">Егер шығыс туралы есептегі шығыстар қызметкерді жалдайтын компаниядан басқа компанияға есептелсе, онда осы шығыстар тиесілі компанияны да және шығыстар алынатын компанияны да тексеру қажет.</span><span class="sxs-lookup"><span data-stu-id="3fe94-107">If expenses on an expense report are charged to a company other than the company that employs the employee, you must verify both the company that those expenses are owed to and the company that they are owed from.</span></span> <span data-ttu-id="3fe94-108">Мысалы, шығыс туралы есеп берген қызметкер DAT компаниясында жұмыс істейді, бірақ шығыстарды DIR компаниясына аударды.</span><span class="sxs-lookup"><span data-stu-id="3fe94-108">For example, the employee who submitted an expense report works for the DAT company but charged an expense to the DIR company.</span></span> <span data-ttu-id="3fe94-109">Бұл жағдайда DAT - бұл шығыстар тиесілі компания, ал DIR - бұл шығыстар алынатын компания.</span><span class="sxs-lookup"><span data-stu-id="3fe94-109">In this case, DAT is the company that the expense is owed to, and DIR is the company that the expense is owed from.</span></span> <span data-ttu-id="3fe94-110">Осы журнал жолдарын тексергеннен кейін, шығыс жолдарын жалпы тіркелімге жариялауға болады.</span><span class="sxs-lookup"><span data-stu-id="3fe94-110">After you verify these journal lines, you can post the expense lines to the general ledger.</span></span>

<span data-ttu-id="3fe94-111">Шығыс туралы есепті жариялау үшін **Бекітілген шығыс туралы есептер** бетінде шығыс туралы есепті таңдап, Әрекеттер тақтасында **Жариялау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3fe94-111">To post an expense report, on the **Approved expense reports** page, select the expense report, and then, on the Action Pane, select **Post**.</span></span>

<span data-ttu-id="3fe94-112">Сонымен қатар тізімдегі барлық шығыс туралы есептерді бір уақытта жариялауға болады.</span><span class="sxs-lookup"><span data-stu-id="3fe94-112">You can also post all the expense reports in the list at the same time.</span></span> <span data-ttu-id="3fe94-113">Барлық шығыс туралы есептерді таңдап, содан кейін **Жариялау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3fe94-113">Select all the expense reports, and then select **Post**.</span></span>