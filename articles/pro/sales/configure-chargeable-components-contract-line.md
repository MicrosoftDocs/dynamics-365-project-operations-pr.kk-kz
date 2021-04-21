---
title: Жобаға негізделген келісім-шарт жолының ақылы құрамдастарын конфигурациялау
description: Бұл тақырып Project Operations жүйесінде ақылы компоненттерді келісім-шарт жолдарына қосу жолдары туралы ақпарат береді.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ddada2cb412ba7370fb0a750325a84772937d8d0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858480"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="1bfe0-103">Жобаға негізделген келісім-шарт жолының ақылы құрамдастарын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="1bfe0-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="1bfe0-104">_**Қолданылу аясы:** жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі, ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="1bfe0-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="1bfe0-105">Жобаға негізделген келісім-шарт жолында *қосылған* компоненттер мен *ақылы* компоненттер болады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="1bfe0-106">Қосылған компоненттер төмендегілерге жататын компоненттер болып табылады:</span><span class="sxs-lookup"><span data-stu-id="1bfe0-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="1bfe0-107">Төлем әдісі және тұтынушылардың бөлінуі</span><span class="sxs-lookup"><span data-stu-id="1bfe0-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="1bfe0-108">Асырмау шектері</span><span class="sxs-lookup"><span data-stu-id="1bfe0-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="1bfe0-109">Жобаға негізделген келісім-шарт жолында анықталатын есеп-шот ұсыну жиілігінің параметрлері</span><span class="sxs-lookup"><span data-stu-id="1bfe0-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="1bfe0-110">Қосылған компоненттердің ішкі жиыны **Төлем түрі** өрісі арқылы ақылы ретінде белгіленуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="1bfe0-111">**Төлем түрі** өрісі - келісім-шарт жолының контекстінде келесі мәндерге мүмкіндік беретін параметрлер жиынтығы:</span><span class="sxs-lookup"><span data-stu-id="1bfe0-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="1bfe0-112">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-112">Chargeable</span></span>
  - <span data-ttu-id="1bfe0-113">Ақысыз</span><span class="sxs-lookup"><span data-stu-id="1bfe0-113">Non-chargeable</span></span>

<span data-ttu-id="1bfe0-114">Ақылы компоненттерді тапсырмалар, рөлдер және транзакциялар санаттары бойынша анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="1bfe0-115">Төлем қабілеттілігі жобаның келісім-шарттық жолына арналған тапсырмалар бойынша анықталады және жолға енгізілген барлық транзакциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="1bfe0-116">Егер келісім-шарт жолындағы **Тапсырмаларды қосу** өрісі бос болса немесе **Барлық жоба** параметріне орнатылса, **Ақылы тапсырмалар** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="1bfe0-117">Жобаның келісім-шарт жолындағы рөлдер бойынша анықталған төлем қабілеттілігі тек **Мерзімдік** операциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="1bfe0-118">Егер келісім-шарт жолындағы **Мерзімін қосу** өрісі **Жоқ** опциясына орнатылса, **Ақылы тапсырмалар** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="1bfe0-119">Жобаның келісім-шарт жолындағы операциялық санаттар бойынша анықталған төлем қабілеттілігі тек **Шығыс** операциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="1bfe0-120">Егер келісім-шарт жолындағы **Шығыстарды қосу** өрісі **Жоқ** опциясына орнатылса, **Ақылы санаттар** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1bfe0-121">Жоба тапсырмасын ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="1bfe0-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="1bfe0-122">Жобаның тапсырмасы белгілі бір келісім-шарт бойынша ақылы немесе ақысыз болуы мүмкін, бұл келесі параметрлерді жасауға мүмкіндік береді:</span><span class="sxs-lookup"><span data-stu-id="1bfe0-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="1bfe0-123">Егер жобаға негізделген келісім-шарт жолы **Мерзім** және белгілі бір тапсырманы қамтитын болса, **T1** параметрі онымен ақылы ретінде байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="1bfe0-124">Егер **Шығысты** қамтитын екінші келісім-шарт жолы болса, сіз келісім-шарттағы T1 тапсырмасын ақысыз деп байланыстыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="1bfe0-125">Нәтижесінде тапсырмаға жазылған барлық уақыт ақылы және барлық шығындар ақысыз болады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="1bfe0-126">Тапсырманың шот түрін келісім-шарт жолындағы тапсырмалар қосымша торындағы **Шот түрі** өрісін жаңарту арқылы келісім-шарт жолындағы **Ақылы тапсырмалар** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="1bfe0-127">Не болмаса, тапсырмаға байланысты келісім-шарт жолдарын көрсететін жобаның тапсырма шотын орнату қосымша торында **Шот түрі** өрісін жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1bfe0-128">Рөлді ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="1bfe0-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="1bfe0-129">Рөл белгілі бір келісім-шарт жолы бойынша ақылы немесе ақысыз болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="1bfe0-130">Рөлдің төлем түрін келісім-шарт жолының **Ақылы рөлдер** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="1bfe0-131">Бұл әрекетті орындау үшін **Ақылы рөлдер** қосалқы торындағы **Шот түрі** өрісін жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1bfe0-132">Операция санатын ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="1bfe0-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="1bfe0-133">Операция санаты белгілі бір келісім-шарт жолы бойынша ақылы немесе ақысыз болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="1bfe0-134">Операция санатының төлем түрін жобаға негізделген келісім-шарт жолының **Ақылы санаттар** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="1bfe0-135">Бұл әрекетті орындау үшін **Ақылы санаттар** қосалқы торындағы **Шот түрі** өрісін жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="1bfe0-136">Төлем қабілеттілігін шешу</span><span class="sxs-lookup"><span data-stu-id="1bfe0-136">Resolve chargeability</span></span>

<span data-ttu-id="1bfe0-137">Уақыт бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="1bfe0-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="1bfe0-138">**Уақыт** келісім-шарт жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="1bfe0-139">**Рөлі** келісім-шарт жолында ақылы болып конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="1bfe0-140">**Қамтылған тапсырмалар** келісім-шарт жолында **Таңдалған тапсырмалар** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="1bfe0-141">Егер осы үш нәрсе дұрыс болса, тапсырма ақылы болып конфигурацияланады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="1bfe0-142">Шығын бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="1bfe0-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="1bfe0-143">**Шығын** келісім-шарт жолына енгізілген</span><span class="sxs-lookup"><span data-stu-id="1bfe0-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="1bfe0-144">**Транзакция санаты** келісім-шарт жолында ақылы болып конфигурацияланған</span><span class="sxs-lookup"><span data-stu-id="1bfe0-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="1bfe0-145">**Қамтылған тапсырмалар** келісім-шарт жолында **Таңдалған тапсырма** мәніне орнатылған</span><span class="sxs-lookup"><span data-stu-id="1bfe0-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="1bfe0-146">Егер осы үш нәрсе дұрыс болса, **Тапсырма** ақылы болып конфигурацияланады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="1bfe0-147">Материал бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="1bfe0-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="1bfe0-148">**Материалдар** келісім-шарт жолына енгізілген</span><span class="sxs-lookup"><span data-stu-id="1bfe0-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="1bfe0-149">**Қамтылған тапсырмалар** келісім-шарт жолында **Таңдалған тапсырмалар** мәніне орнатылған</span><span class="sxs-lookup"><span data-stu-id="1bfe0-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="1bfe0-150">Егер осы екі нәрсе дұрыс болса, **Тапсырма** ақылы болып конфигурацияланады.</span><span class="sxs-lookup"><span data-stu-id="1bfe0-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bfe0-151">
                    <strong>Уақытпен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1bfe0-152">
                    <strong>Шығыспен қоса</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1bfe0-153">
                    <strong>Материалдарды қамтиды</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="1bfe0-154">
                    <strong>Қосылған тапсырмалар</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-155">
                    <strong>Рөл</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bfe0-156">
                    <strong>Санат</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-157">
                    <strong>Тапсырма</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="1bfe0-158">
                    <strong>Төлем қабілеттілігінің әсері</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-159">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-160">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-161">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-162">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="1bfe0-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-163">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-164">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-165">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-166">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-167">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-168">Материал нақты мәніндегі шот ұсыну түрі: <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-169">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-170">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-171">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-172">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="1bfe0-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-173">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-174">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-175">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-176">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-177">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-178">Материал нақты мәніндегі шот ұсыну түрі: <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-179">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-180">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-181">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-182">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="1bfe0-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-183">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-184">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-185">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-186">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-187">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bfe0-188">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-189">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-190">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-191">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-192">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="1bfe0-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-193">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-194">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-195">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-196">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-197">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-198">Материал нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-199">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-200">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-201">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-202">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="1bfe0-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-203">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-204">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-205">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-206">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-207">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-208">Материал нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-209">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-210">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-211">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-212">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="1bfe0-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-213">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bfe0-214">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-215">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-216">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-217">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-218">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bfe0-219">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-220">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-221">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-222">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="1bfe0-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-223">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bfe0-224">
                    <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-225">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-226">Уақыт нақты мәніндегі шот ұсыну: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-227">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bfe0-228">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bfe0-229">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-230">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-231">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-232">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="1bfe0-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-233">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bfe0-234">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-235">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-236">Уақыт нақты мәніндегі шот ұсыну: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-237">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-238">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-239">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1bfe0-240">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-241">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-242">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="1bfe0-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-243">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-244">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-245">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-246">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bfe0-247">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-248">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-249">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1bfe0-250">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bfe0-251">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-252">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="1bfe0-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-253">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-254">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-255">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-256">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-257">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-258">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-259">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-260">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1bfe0-261">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-262">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="1bfe0-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-263">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-264">Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-265">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-266">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bfe0-267">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="1bfe0-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bfe0-268">Материал нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bfe0-269">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bfe0-270">Иә</span><span class="sxs-lookup"><span data-stu-id="1bfe0-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1bfe0-271">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bfe0-272">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="1bfe0-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bfe0-273">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bfe0-274">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bfe0-275">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="1bfe0-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bfe0-276">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-277">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bfe0-278">Материал нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bfe0-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
