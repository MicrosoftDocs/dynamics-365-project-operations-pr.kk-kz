---
title: Түзетілген есеп-шоттар
description: Түзетілген есеп-шоттар туралы ақпаратты ұсынады.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e14da1c07d5b697de6caf1b9041c30581ecff102
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898088"
---
# <a name="corrected-invoices"></a><span data-ttu-id="f37c2-103">Түзетілген есеп-шоттар</span><span class="sxs-lookup"><span data-stu-id="f37c2-103">Corrected invoices</span></span>

<span data-ttu-id="f37c2-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="f37c2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f37c2-105">Расталған есеп-шоттарды өңдеуге болады.</span><span class="sxs-lookup"><span data-stu-id="f37c2-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="f37c2-106">Расталған есеп-шотты өңдеген кезде түзетілген есеп-шоттың нобайы жасалады.</span><span class="sxs-lookup"><span data-stu-id="f37c2-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="f37c2-107">Сіз барлық транзакциялар мен мөлшерлерді бастапқы есеп-шоттан алып тастағыңыз келеді деген болжам болғандықтан, түзетілген есеп-шот бастапқы есеп-шоттағы барлық транзакцияларды қамтиды және ондағы барлық мөлшерлер нөлге (0) тең.</span><span class="sxs-lookup"><span data-stu-id="f37c2-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="f37c2-108">Транзакциялар түзетуді қажет етпеген кезде, оларды нобай түзетпе есеп-шоттан жоюға болады.</span><span class="sxs-lookup"><span data-stu-id="f37c2-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="f37c2-109">Жартылай мөлшерді түзету немесе қайтару үшін, жол мәліметіндегі Мөлшер өрісін өңдеуге болады.</span><span class="sxs-lookup"><span data-stu-id="f37c2-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="f37c2-110">Егер есеп-шот жолы туралы мәліметті ашсаңыз, есеп-шоттың бастапқы мөлшерін көре аласыз.</span><span class="sxs-lookup"><span data-stu-id="f37c2-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="f37c2-111">Содан кейін сіз ағымдағы есеп-шот мөлшерін бастапқы есеп-шоттың мөлшерінен аз немесе көп болатындай етіп өңдей аласыз.</span><span class="sxs-lookup"><span data-stu-id="f37c2-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="f37c2-112">Түзетілген есеп-шотты растаған кезде, бастапқы шот ұсынылмаған сатылымның нақты мәні кері бағытталады және жаңа шот ұсынылған сатылымның нақты мәні жасалады.</span><span class="sxs-lookup"><span data-stu-id="f37c2-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="f37c2-113">Егер мөлшері азайтылған болса, туындаған айырмашылықтан жаңа шот ұсынылмаған сатылымның нақты мәні де жасалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f37c2-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="f37c2-114">Мысалы, шот-фактураның алғашқы сатылымы сегіз сағатқа созылған болса, ал түзетілген есеп-шоттың жолының мәліметі алты сағатқа азайтылған болса, шот-фактура сатылымының бастапқы сызығы түзетіліп, екі жаңа есептеу әдісі жасалады:</span><span class="sxs-lookup"><span data-stu-id="f37c2-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="f37c2-115">Алты сағатқа арналған шот ұсынылған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="f37c2-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="f37c2-116">Қалған екі сағатқа арналған шот ұсынылмаған сатылымның нақты мәні.</span><span class="sxs-lookup"><span data-stu-id="f37c2-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="f37c2-117">Бұл транзакцияға кейінірек есеп-шот ұсынылуы мүмкін немесе тұтынушымен жасалған келіссөздерге байланысты ақылы емес болып белгіленуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f37c2-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
