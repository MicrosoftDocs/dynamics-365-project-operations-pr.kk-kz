---
title: Мақұлдау жинақтары
description: Бұл тақырыпта сол операциялардың мақұлдау жинағы, сұраулар және қосалқы жинақтар туралы ақпарат берілген.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116878"
---
# <a name="approval-sets"></a><span data-ttu-id="ea0ce-103">Мақұлдау жинақтары</span><span class="sxs-lookup"><span data-stu-id="ea0ce-103">Approval sets</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ea0ce-104">Мақұлдау топтардың мақұлдау сұрауларын операциялардың шағын қосалқы жинақтарына біріктіреді.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-104">Approval sets group approval requests together into smaller subsets of operations.</span></span> <span data-ttu-id="ea0ce-105">Бұл топтау мақұлдауды жоба бойынша өңдеуге мүмкіндік береді және әрекетті қайталап көруге және ретке келтіруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-105">This grouping allows approvals to be processed in order by Project and allows for retrying and sequencing.</span></span> <span data-ttu-id="ea0ce-106">Топтау үлкен көлемдегі мақұлдау үшін мақұлдауды өңдеудің сенімділігі мен бақылануын арттырады.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-106">Grouping improves the reliability and traceability of approval processing for large volumes of approvals.</span></span>

<span data-ttu-id="ea0ce-107">Мақұлдау жинақтары олардың қатысты жазбаларының жалпы өңдеу күйін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-107">Approval sets indicate the overall processing state of their related records.</span></span> <span data-ttu-id="ea0ce-108">Мақұлдау жазбасы мақұлдау жинағы арқылы өңделгенде, жазба **Жіберілді** күйінен **Мақұлданды** күйіне ауысады және мақұлдау жинағынан ажыратылады.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-108">When an approval record is processed using an approval set, the record moves from **Submitted** to **Approved**, and is unlinked from the approval set.</span></span> <span data-ttu-id="ea0ce-109">Егер жазба мақұлдауға жіберілген кезде сәтсіздік аяқталса, жазба **Жіберілді** күйінде қалады және мақұлдау жинағы сәтсіз аяқталды деп белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-109">If a record fails when it is submitted for approval, the record remains in a status of **Submitted** and the approval set is marked as failed.</span></span> <span data-ttu-id="ea0ce-110">Мақұлдау жинағы қате туралы хабарды тіркейді.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-110">The approval set logs the error message of the failure.</span></span>

## <a name="processing-approvals-and-approval-sets"></a><span data-ttu-id="ea0ce-111">Мақұлдаулар мен мақұлдау жинақтарын өңдеу</span><span class="sxs-lookup"><span data-stu-id="ea0ce-111">Processing approvals and approval sets</span></span>
<span data-ttu-id="ea0ce-112">Өңдеуге кезекте тұрған мақұлдаулар **Өңделетін мақұлдаулар** көрінісінде көрінеді.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-112">Approvals that are queued for processing are visible in the **Processing Approvals** view.</span></span> <span data-ttu-id="ea0ce-113">Жүйе барлық жазбаларды бірнеше рет үндестірілмеген түрде өңдеуге тырысады, бұған дейінгі әрекеттер сәтсіз аяқталған жағдайда мақұлдауды қайталауға тырысады.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-113">The system tries to process all the entries multiple times asynchronously, including retrying an approval if previous attempts failed.</span></span>

<span data-ttu-id="ea0ce-114">**Мақұлдау жинағының мерзімі** өрісі жинақты сәтсіз деп белгілегенге дейін қанша өңдеу әрекеті қалғанын жазады.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-114">The **Approval Set Lifetime** field records the number of attempts left to process the set before it's marked as failed.</span></span>

## <a name="failed-approvals-and-approval-sets"></a><span data-ttu-id="ea0ce-115">Сәтсіз аяқталған мақұлдаулар мен мақұлдау жинақтары</span><span class="sxs-lookup"><span data-stu-id="ea0ce-115">Failed approvals and approval sets</span></span>
<span data-ttu-id="ea0ce-116">**Сәтсіз аяқталған мақұлдаулар** көрінісі пайдаланушының араласуын қажет ететін барлық мақұлдау тізімдерін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-116">The **Failed Approvals** view lists all approvals that require user intervention.</span></span> <span data-ttu-id="ea0ce-117">Сәтсіздіктің себебін анықтау үшін байланысты мақұлдау жинағының журналдарын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-117">Open the associated approval set logs to identify the cause of the failure.</span></span>
<span data-ttu-id="ea0ce-118">**Әрекетті қайталау** түймешігі мақұлдау жинағына мерзім санағын қосады, мақұлдау жинағын қайта **Өңделуде** күйіне қайтарады және қалған жазбаларды өңдеуге тырысады.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-118">Selecting **Retry** adds to the approval set lifetime count, moves the approval set back to a status of **Processing**, and attempts to process the remaining records.</span></span>

## <a name="configure-approval-sets"></a><span data-ttu-id="ea0ce-119">Мақұлдау жинақтарын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="ea0ce-119">Configure approval sets</span></span>

###  <a name="enable-the-approval-sets-feature"></a><span data-ttu-id="ea0ce-120">Мақұлдау жинақтары функциясын қосу</span><span class="sxs-lookup"><span data-stu-id="ea0ce-120">Enable the Approval sets feature</span></span>
<span data-ttu-id="ea0ce-121">Мақұлдау жинақтары функциясын қоспас бұрын, қазір өңделіп жатқан мақұлдаулардың жоқтығын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-121">Before you enable the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="ea0ce-122">**Жоба параметрлері** бетіне өтіңіз және **Функция басқару элементі** > **Заманауи мақұлдауды қосу** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-122">Go to the **Project parameters** page and select **Feature Control** > **Enable Modern Approvals**.</span></span>

### <a name="turn-off-the-approval-sets-feature"></a><span data-ttu-id="ea0ce-123">Мақұлдау жинақтары функциясын өшіру</span><span class="sxs-lookup"><span data-stu-id="ea0ce-123">Turn off the Approval sets feature</span></span>
<span data-ttu-id="ea0ce-124">Мақұлдау жинақтары функциясын өшірмес бұрын, қазір өңделіп жатқан мақұлдаулардың жоқтығын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-124">Before you turn off the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="ea0ce-125">**Жоба параметрлері** бетіне өтіңіз және **Функция басқару элементі** > **Заманауи мақұлдауды өшіру** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-125">Go to the **Project Parameters** page and select **Feature Control** > **Disable Modern Approvals**.</span></span>

### <a name="configuring-the-asynchronous-threshold"></a><span data-ttu-id="ea0ce-126">Үндестірілмеген шекті конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="ea0ce-126">Configuring the asynchronous threshold</span></span> 
<span data-ttu-id="ea0ce-127">Мақұлдау жинақтары жасалған кезде, мақұлдау үшін жазбалардың таңдалған саны көрсетілген шектен асқан кезде өңдеу фондық режимге ауысады.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-127">When approval sets are created, processing moves to the background when the selected number of records for approval exceeds the indicated threshold.</span></span> <span data-ttu-id="ea0ce-128">Мақұлдауды өңдеу синхронды немесе асинхронды түрде іске қосылатын кезде конфигурациялау үшін **Асинхронды шек** өрісін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-128">Use the **Asynchronous Threshold** field to configure when approval processing should be run synchronously or asynchronously.</span></span>
<span data-ttu-id="ea0ce-129">Жарамды мәндер:</span><span class="sxs-lookup"><span data-stu-id="ea0ce-129">Valid values are:</span></span>

  - <span data-ttu-id="ea0ce-130">Нөл: барлық сұраулар асинхронды түрде өңделуі керек.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-130">Zero: All requests should be processed asynchronously.</span></span> 
  - <span data-ttu-id="ea0ce-131">Нөлден үлкен сандар: мақұлдаудың ұсынылған саны осы мәннен асқан кезде ғана мақұлдау асинхронды түрде өңделеді.</span><span class="sxs-lookup"><span data-stu-id="ea0ce-131">Numbers greater than zero: Approvals are processed asynchronously only when the submitted number of approvals exceeds this value.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
