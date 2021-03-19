---
title: Жоба болжамын жою
description: Бұл тақырыпта жоба болжамы аяқталғаннан кейін оны жою туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 000eabdac41f30a6e7dd37e34b8fd91d7c51f6c4
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270685"
---
# <a name="eliminate-a-project-estimate"></a><span data-ttu-id="699bc-103">Жоба болжамын жою</span><span class="sxs-lookup"><span data-stu-id="699bc-103">Eliminate a project estimate</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="699bc-104">Жоба болжамдары жоба үшін болжанған және жоспарланған жұмыстың қаржылық көрінісін береді.</span><span class="sxs-lookup"><span data-stu-id="699bc-104">Project estimates provide the financial view for work that is estimated and scheduled for a project.</span></span> <span data-ttu-id="699bc-105">Жоба болжамдарымен жұмыс істеу үшін жобаны болжамды жобаға бекіту керек.</span><span class="sxs-lookup"><span data-stu-id="699bc-105">To work with estimates for a project, you must attach the project to an estimate project.</span></span> <span data-ttu-id="699bc-106">Болжамды жоба әрдайым бұрыннан бар жобаға негізделеді, бірақ бірнеше жоба бір болжамды жобаға сілтеме жасай алады.</span><span class="sxs-lookup"><span data-stu-id="699bc-106">An estimate project is always based on an existing project, however multiple projects can refer to a single estimate project.</span></span> <span data-ttu-id="699bc-107">Болжамды жобаларға тек бағасы белгіленген және инвестициялық жобалар ғана қосылуы мүмкін, және ол жобалар болжамды жобамен бір жоба тобына кіруі керек.</span><span class="sxs-lookup"><span data-stu-id="699bc-107">Only fixed-price and investment projects can be attached to estimate projects, and those projects must belong to the same project group as the estimate project.</span></span>

<span data-ttu-id="699bc-108">Болжамды жобаны жою үшін ол аяқталуы керек.</span><span class="sxs-lookup"><span data-stu-id="699bc-108">To eliminate an estimate project, it must be complete.</span></span> <span data-ttu-id="699bc-109">Келесі қадамдар болжамды қалай жоюға болатынын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="699bc-109">The following steps explain how to eliminate an estimate.</span></span>

1. <span data-ttu-id="699bc-110">**Жобаларды басқару және есепке алу** > **Барлық жобалар** тармағына өтіп, жобаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-110">Go to **Project management and accounting** > **All Projects** and open the project.</span></span> 
2. <span data-ttu-id="699bc-111">**Басқару** қойыншасында **Болжамдар** және **Болжам** бетінде **Жою** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-111">On the **Manage** tab, select **Estimates**, and on the **Estimate** page select **Eliminate**.</span></span>
3. <span data-ttu-id="699bc-112">**Жалпы** қойыншасындағы **Болжамды жою** бетінде келесі опцияларды орнатыңыз:</span><span class="sxs-lookup"><span data-stu-id="699bc-112">On the **Eliminate estimate** page on the **General** tab, set the following options:</span></span>

   - <span data-ttu-id="699bc-113">**Кезең коды**: тиісті болжамды жобаларды таңдау үшін кезең кодын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-113">**Period code**: Select the period code to choose the appropriate estimate projects.</span></span> 
   - <span data-ttu-id="699bc-114">**Болжамды күн**: жою үшін тиісті болжамды күнді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-114">**Estimate date**: Select the appropriate estimate date for elimination.</span></span>
   - <span data-ttu-id="699bc-115">**WIP ескертулерімен жою**: орындалудағы жұмыспен (WIP) байланысты болжам жойылатын кезде хабарландыру беру үшін осы опцияны қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-115">**Eliminate with WIP warnings**: Enable this option to provide notification when an estimate that is associated with a work in progress (WIP) will be eliminated.</span></span> <span data-ttu-id="699bc-116">Бұл опция қосылмаған кезде, қандай да бір болжанбаған транзакциялар болса, жоюды жалғастыру мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="699bc-116">When this option is not enabled, elimination can’t continue if any non-estimated transactions exist.</span></span> 
   > [!NOTE]
   > <span data-ttu-id="699bc-117">Бұл опция болжам жобасына жою қолданылған кезде ғана қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="699bc-117">This option is available only when elimination is applied to an estimate project.</span></span> <span data-ttu-id="699bc-118">Егер сіз мерзімді хабарландыруларды қолдансаңыз, ол қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="699bc-118">It is not available if you are using periodic postings.</span></span> <span data-ttu-id="699bc-119">Бұл параметр **Болжанбаған транзакциялар шыққан кезде жоюға мүмкіндік беру** өріс тобындағы **Жоба параметрлері** бетінде **Болжам** қойыншасындағы параметрлермен жұмыс істейді.</span><span class="sxs-lookup"><span data-stu-id="699bc-119">This setting works with the settings on the **Estimate** tab on the **Project parameters** page, in the **Allow elimination when non-estimated transactions exist** field group.</span></span>
   - <span data-ttu-id="699bc-120">**Кезеңді аяқталған деп белгілеу**: жоюды іске қосқаннан кейін, болжамды жоба кезеңін **Аяқталды** күйіне орнату үшін осы опцияны қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-120">**Set stage to Finished**: Enable this option to set the estimate project’s stage to **Finished** after you run the elimination.</span></span>
   - <span data-ttu-id="699bc-121">**Болжам тізімін басып шығару**: болжам тізімі басылып шығарылған кезде енгізілетін ақпаратты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-121">**Print estimate list**: Select the information to be included when the estimate list is printed.</span></span>
   - <span data-ttu-id="699bc-122">**Инфологты көрсету**: инфологты көрсету үшін осы параметрді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-122">**Show Infolog**: Enable this option to display the Infolog.</span></span>
   - <span data-ttu-id="699bc-123">**Жарияланған күні**: болжамның жарияланған күнін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-123">**Posting date**: Choose the ledger posting date of the estimate.</span></span>

4.  <span data-ttu-id="699bc-124">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-124">Select **OK**.</span></span>
5. <span data-ttu-id="699bc-125">Жою процесі аяқталғаннан кейін, жойылған болжамды жоба теріс мәнмен көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="699bc-125">After the elimination process is complete, the eliminated estimate project is displayed with a negative value.</span></span> 

<span data-ttu-id="699bc-126">Егер сіз болжамды жойғыңыз келмеген болса, сіз жойылған болжамды таңдап, **Кері жою** пәрменін таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="699bc-126">If you did not intend to eliminate an estimate, you can select the eliminated estimate and select **Reverse elimination**.</span></span>   


[!INCLUDE[footer-include](../includes/footer-banner.md)]