---
title: Есеп-шоттардың автоматты жасалуын конфигурациялау
description: Бұл мақалада есеп-шоттарды автоматты құру үшін жүйені конфигурациялау әдісі туралы ақпарат берілген.
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
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898133"
---
# <a name="configure-automated-invoice-creation"></a><span data-ttu-id="239e8-103">Есеп-шоттардың автоматты жасалуын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="239e8-103">Configure automated invoice creation</span></span>

<span data-ttu-id="239e8-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="239e8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="239e8-105">Есеп-шоттың автоматты іске қосылуын конфигурациялау үшін Project Оperations бағдарламасындағы келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="239e8-105">Complete the following steps to configure an automated invoice run in Project operations.</span></span>

1. <span data-ttu-id="239e8-106">**Параметрлер** \> **Жиынтық тапсырмалар** тармағы бойынша өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="239e8-106">Go to **Settings** \> **Batch jobs**.</span></span>
2. <span data-ttu-id="239e8-107">Жиынтық тапсырманы жасап, оны **Project Оperations есеп-шоттарын жасау** деп атаңыз.</span><span class="sxs-lookup"><span data-stu-id="239e8-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="239e8-108">Жиынтық тапсырма атында "Есеп-шоттар жасау" термині кірістірілуі керек.</span><span class="sxs-lookup"><span data-stu-id="239e8-108">The name of the batch job must include the term "create invoices."</span></span>
3. <span data-ttu-id="239e8-109">**Тапсырма түрі** өрісінде **Жоқ** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="239e8-109">In the **Job type** field, select **None**.</span></span> <span data-ttu-id="239e8-110">Әдепкі бойынша, **Күнделікті жиілік** және **Белсенді** параметрлері **Иә** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="239e8-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="239e8-111">**Жұмыс ағынын іске қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="239e8-111">Select **Run Workflow**.</span></span> <span data-ttu-id="239e8-112">**Жазбаны іздеу** диалогтық терезесінде үш жұмыс ағынын көресіз:</span><span class="sxs-lookup"><span data-stu-id="239e8-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="239e8-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="239e8-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="239e8-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="239e8-114">ProcessRunner</span></span>
    - <span data-ttu-id="239e8-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="239e8-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="239e8-116">**ProcessRunCaller** параметрін, содан кейін **Қосу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="239e8-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="239e8-117">Келесі диалогтық терезеде **OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="239e8-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="239e8-118">**Процесс** жұмыс ағынынан кейін **Ұйқы** жұмыс ағыны болады.</span><span class="sxs-lookup"><span data-stu-id="239e8-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

    <span data-ttu-id="239e8-119">Сондай-ақ **ProcessRunner** параметрін 5-қадамда таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="239e8-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="239e8-120">Содан кейін **OK** пәрменін таңдаған кезде, **Процесс** жұмыс ағынынан кейіннен **Ұйқы** жұмыс ағынына өтеді.</span><span class="sxs-lookup"><span data-stu-id="239e8-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="239e8-121">Есеп-шоттар **ProcessRunCaller** және **ProcessRunner** жұмыс ағындарында жасалады.</span><span class="sxs-lookup"><span data-stu-id="239e8-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="239e8-122">**ProcessRunCaller** жұмыс ағыны **ProcessRunner** жұмыс ағынын шақырады.</span><span class="sxs-lookup"><span data-stu-id="239e8-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="239e8-123">**ProcessRunner** — бұл есеп-шоттар жасалатын жұмыс ағыны.</span><span class="sxs-lookup"><span data-stu-id="239e8-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="239e8-124">Ол есеп-шоттар жасалуы керек барлық келісім-шарт жолдарынан өтіп сол жолдар үшін есеп-шоттар жасайды.</span><span class="sxs-lookup"><span data-stu-id="239e8-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="239e8-125">Есеп-шоттар жасалуы керек келісім-шарт жолдарын анықтау үшін, тапсырма келісім-шарт жолдары бойынша есеп-шоттың орындалу мерзімдерін қарастырады.</span><span class="sxs-lookup"><span data-stu-id="239e8-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="239e8-126">Егер бір келісім-шартқа жататын келісім-шарт жолдарында есеп-шоттың орындалу мерзімі бірдей болса, транзакциялар екі есеп-шот жолы бар бір есеп-шотқа біріктіріледі.</span><span class="sxs-lookup"><span data-stu-id="239e8-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="239e8-127">Егер есеп-шот жасау бойынша транзакциялар болмаса, тапсырма есеп-шотты жасау қадамын өткізіп жібереді.</span><span class="sxs-lookup"><span data-stu-id="239e8-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="239e8-128">**ProcessRunner** іске қосылғаннан кейін, ол **ProcessRunCaller** жұмыс ағынын шақырып, аяқталу уақытын қамтамасыз етіп, жабылады.</span><span class="sxs-lookup"><span data-stu-id="239e8-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="239e8-129">Содан кейін **ProcessRunCaller** жұмыс ағыны көрсетілген аяқталу уақытынан бастап 24 сағат бойын жұмыс істейтін таймерді іске қосады.</span><span class="sxs-lookup"><span data-stu-id="239e8-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="239e8-130">Таймердің соңында **ProcessRunCaller** жұмыс ағыны жабылады.</span><span class="sxs-lookup"><span data-stu-id="239e8-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="239e8-131">Есеп-шоттар жасауға арналған жиынтықты өңдеу тапсырмасы қайталанатын тапсырма болып табылады.</span><span class="sxs-lookup"><span data-stu-id="239e8-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="239e8-132">Егер бұл жиынтықты өңдеу бірнеше рет орындалса, онда бірнеше тапсырма жасалып, қателіктер туындайды.</span><span class="sxs-lookup"><span data-stu-id="239e8-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="239e8-133">Сондықтан, жиынтықты өңдеуді тек бір рет орындауыңыз керек және ол тоқтағаннан кейін ғана қайта орындауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="239e8-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="239e8-134">Жиынтық шот жіберу есеп-шот кестелері арқылы конфигурацияланатын жобаның келісімшарт жолдары үшін ғана іске қосылады.</span><span class="sxs-lookup"><span data-stu-id="239e8-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="239e8-135">Белгіленген бағамен шот ұсыну әдісі бар келісім-шарт жолында кезеңдер теңшелген болуы керек.</span><span class="sxs-lookup"><span data-stu-id="239e8-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="239e8-136">Уақыт пен материалдық шот ұсыну әдісі бар жобаның келісім-шарт жолы күнтізбелік есеп-шот кестесін қажет етеді.</span><span class="sxs-lookup"><span data-stu-id="239e8-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="239e8-137">Бұл жобаға негізделген келісім-шарт жолына да қатысты.</span><span class="sxs-lookup"><span data-stu-id="239e8-137">The same applies to a project-based contract line.</span></span>     
