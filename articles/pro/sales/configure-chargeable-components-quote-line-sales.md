---
title: Баға ұсынысы жолының ақылы компоненттерін конфигурациялау
description: Бұл тақырып жобаға негізделген баға ұсыну жолындағы ақылы және ақысыз компоненттерді орнату туралы ақпарат береді.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c933a3800aae72624dbcbe3f06df20e5981d74d4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003773"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="91a84-103">Баға ұсыну жолының ақылы құрамдастарын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="91a84-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="91a84-104">_**Қолданылу аясы:** жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі, ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="91a84-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="91a84-105">Жобаға негізделген баға ұсыну жолында *қосылған* компоненттер мен *ақылы* компоненттер ұғымы болады.</span><span class="sxs-lookup"><span data-stu-id="91a84-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="91a84-106">Қосылатын компоненттер мыналарға жатады:</span><span class="sxs-lookup"><span data-stu-id="91a84-106">Included components are subject to:</span></span>

  - <span data-ttu-id="91a84-107">Төлем әдісі және тұтынушылардың бөлінуі</span><span class="sxs-lookup"><span data-stu-id="91a84-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="91a84-108">Асырмау шектері</span><span class="sxs-lookup"><span data-stu-id="91a84-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="91a84-109">Жобаға негізделген баға ұсыну жолында анықталатын есеп-шот ұсыну жиілігінің параметрлері</span><span class="sxs-lookup"><span data-stu-id="91a84-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="91a84-110">Қосылған компоненттердің ішкі жиыны **Төлем түрі** өрісі арқылы ақылы ретінде белгіленуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="91a84-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="91a84-111">**Төлем түрі** өрісі - баға ұсыну жолының контекстінде келесі мәндерге мүмкіндік беретін параметрлер жиынтығы:</span><span class="sxs-lookup"><span data-stu-id="91a84-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="91a84-112">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-112">Chargeable</span></span>
  - <span data-ttu-id="91a84-113">Ақысыз</span><span class="sxs-lookup"><span data-stu-id="91a84-113">Non-chargeable</span></span>

<span data-ttu-id="91a84-114">Ақылы компоненттерді тапсырмалар, рөлдер және транзакциялар санаттары бойынша анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="91a84-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="91a84-115">Төлем қабілеттілігі баға ұсыну жолына арналған тапсырмалар бойынша анықталады және сол жолға енгізілген барлық транзакциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="91a84-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="91a84-116">Егер **Тапсырмаларды қосу** өрісі **Барлық жоба** параметріне орнатылса немесе бос қалдырылса, **Ақылы тапсырмалар** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="91a84-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="91a84-117">Төлем қабілеттілігі баға ұсыну жолындағы рөлдер бойынша анықталған және тек **Мерзімдік** операциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="91a84-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="91a84-118">Егер жобаның баға ұсыну жолындағы **Мерзімін қосу** өрісі **Жоқ** опциясына орнатылса, **Ақылы рөлдер** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="91a84-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="91a84-119">Төлем қабілеттілігі баға ұсыну жолындағы операциялық санаттар бойынша анықталады және тек **Шығыс** операциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="91a84-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="91a84-120">Егер жобаның баға ұсыну жолындағы **Шығыстарды қосу** өрісі **Жоқ** опциясына орнатылса, **Ақылы санаттар** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="91a84-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="91a84-121">Жоба тапсырмасын ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="91a84-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="91a84-122">Жоба тапсырмасы жобаға негізделген белгілі бір баға ұсыну жолының контекстінде ақылы немесе ақысыз болуы мүмкін, бұл келесі параметрлерді жасауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="91a84-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="91a84-123">Егер жобаға негізделген баға ұсыну жолында **Уақыт** және **Т1** тапсырмасы қамтылса, тапсырма баға ұсыну жолына ақылы ретінде байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="91a84-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="91a84-124">Егер **Шығыстарды** қамтитын екінші баға ұсыну жолы болса, сіз баға ұсыну жолындағы **T1** тапсырмасын ақысыз деп байланыстыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="91a84-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="91a84-125">Нәтижесінде тапсырмаға жазылған барлық уақыт ақылы және тапсырмаға жазылған барлық шығындар ақысыз болады.</span><span class="sxs-lookup"><span data-stu-id="91a84-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="91a84-126">Тапсырманың төлем түрін **Баға ұсыну жолының тапсырмалары** қосалқы торындағы **Шот түрі** өрісін жаңарту арқылы жоба негізіндегі бағаны ұсыну жолындағы **Ақылы тапсырмалар** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="91a84-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="91a84-127">Не болмаса, жоба тапсырмасы үшін шот түрін тапсырмаға байланысты баға ұсыну жолдарын көрсететін жобаның тапсырма шотын орнату қосалқы торында **Шот түрі** өрісінде жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="91a84-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="91a84-128">Рөлді ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="91a84-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="91a84-129">Рөл белгілі бір жобаға негізделген баға ұсыну жолының контекстінде ақылы немесе ақысыз болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="91a84-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="91a84-130">Рөлдің шот түрін **Ақылы рөлдер** қосалқы торындағы **Шот түрі** өрісін жаңарту арқылы бағаны ұсыну жолындағы **Ақылы рөлдер** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="91a84-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="91a84-131">Операция санатын ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="91a84-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="91a84-132">Операция санаты белгілі бір баға ұсыну жолы бойынша ақылы немесе ақысыз болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="91a84-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="91a84-133">Транзакцияның шот түрін **Ақылы санаттар** қосалқы торындағы **Шот түрі** өрісін жаңарту арқылы бағаны ұсыну жолындағы **Ақылы санаттар** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="91a84-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="91a84-134">Төлем қабілеттілігін шешу</span><span class="sxs-lookup"><span data-stu-id="91a84-134">Resolve chargeability</span></span>
<span data-ttu-id="91a84-135">Уақыт бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="91a84-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="91a84-136">**Уақыт** баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="91a84-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="91a84-137">**Рөлі** баға ұсыну жолында ақылы болып конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="91a84-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="91a84-138">**Қамтылған тапсырмалар** баға ұсыну жолында **Таңдалған тапсырмалар** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="91a84-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="91a84-139">Егер осы үш нәрсе дұрыс болса, **Тапсырма** да ақылы болып конфигурацияланады.</span><span class="sxs-lookup"><span data-stu-id="91a84-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="91a84-140">Шығын бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="91a84-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="91a84-141">**Шығын** баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="91a84-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="91a84-142">**Транзакция санаты** баға ұсыну жолында ақылы болып конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="91a84-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="91a84-143">**Қамтылған тапсырмалар** баға ұсыну жолында **Таңдалған тапсырмалар** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="91a84-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="91a84-144">Егер осы үш нәрсе дұрыс болса, **Тапсырма** да ақылы болып конфигурацияланады.</span><span class="sxs-lookup"><span data-stu-id="91a84-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="91a84-145">Материал бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="91a84-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="91a84-146">**Материалдар** баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="91a84-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="91a84-147">**Қамтылған тапсырмалар** баға ұсыну жолында **Таңдалған тапсырмалар** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="91a84-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="91a84-148">Егер осы екі нәрсе дұрыс болса, **Тапсырма** да ақылы болып конфигурациялануы тиіс.</span><span class="sxs-lookup"><span data-stu-id="91a84-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="91a84-149">
                    <strong>Уақытпен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="91a84-150">
                    <strong>Шығыспен қоса</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="91a84-151">
                    <strong>Материалдарды қамтиды</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="91a84-152">
                    <strong>Қосылған тапсырмалар</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-153">
                    <strong>Рөл</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="91a84-154">
                    <strong>Санат</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-155">
                    <strong>Тапсырма</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="91a84-156">
                    <strong>Төлем қабілеттілігінің әсері</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-157">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-158">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-159">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-160">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="91a84-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-161">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-162">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-163">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-164">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-165">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-166">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-167">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-168">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-169">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-170">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="91a84-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-171">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-172">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-173">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-174">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-175">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-176">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-177">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-178">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-179">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-180">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="91a84-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-181">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-182">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-183">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-184">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-185">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-186">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-187">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-188">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-189">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-190">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="91a84-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-191">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-192">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-193">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-194">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-195">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-196">Материал нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-197">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-198">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-199">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-200">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="91a84-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-201">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-202">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-203">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-204">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-205">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-206">Материал нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-207">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-208">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-209">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-210">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="91a84-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-211">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="91a84-212">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-213">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-214">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-215">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-216">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="91a84-217">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-218">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-219">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-220">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="91a84-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-221">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="91a84-222">
                    <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-223">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-224">Уақыт нақты мәніндегі шот ұсыну: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-225">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-226">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="91a84-227">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-228">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-229">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-230">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="91a84-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-231">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="91a84-232">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-233">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-234">Уақыт нақты мәніндегі шот ұсыну: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-235">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-236">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-237">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="91a84-238">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-239">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-240">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="91a84-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-241">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-242">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-243">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-244">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-245">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-246">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-247">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="91a84-248">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="91a84-249">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-250">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="91a84-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-251">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-252">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-253">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-254">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-255">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-256">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-257">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-258">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="91a84-259">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-260">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="91a84-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-261">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-262">Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-263">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-264">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-265">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="91a84-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="91a84-266">Материал нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="91a84-267">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="91a84-268">Иә</span><span class="sxs-lookup"><span data-stu-id="91a84-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="91a84-269">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="91a84-270">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="91a84-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="91a84-271">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="91a84-272">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="91a84-273">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="91a84-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="91a84-274">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-275">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="91a84-276">Материал нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="91a84-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
