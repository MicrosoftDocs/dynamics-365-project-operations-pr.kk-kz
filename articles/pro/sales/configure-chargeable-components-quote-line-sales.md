---
title: Баға ұсынысы жолының ақылы компоненттерін конфигурациялау
description: Бұл тақырып жобаға негізделген баға ұсыну жолындағы ақылы және ақысыз компоненттерді орнату туралы ақпарат береді.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a9e1851bd8c5a4070df2774c945d1f3eabaaa8a
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858300"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="57ca7-103">Баға ұсыну жолының ақылы құрамдастарын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="57ca7-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="57ca7-104">_**Қолданылу аясы:** жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі, ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="57ca7-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="57ca7-105">Жобаға негізделген баға ұсыну жолында *қосылған* компоненттер мен *ақылы* компоненттер ұғымы болады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="57ca7-106">Қосылатын компоненттер мыналарға жатады:</span><span class="sxs-lookup"><span data-stu-id="57ca7-106">Included components are subject to:</span></span>

  - <span data-ttu-id="57ca7-107">Төлем әдісі және тұтынушылардың бөлінуі</span><span class="sxs-lookup"><span data-stu-id="57ca7-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="57ca7-108">Асырмау шектері</span><span class="sxs-lookup"><span data-stu-id="57ca7-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="57ca7-109">Жобаға негізделген баға ұсыну жолында анықталатын есеп-шот ұсыну жиілігінің параметрлері</span><span class="sxs-lookup"><span data-stu-id="57ca7-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="57ca7-110">Қосылған компоненттердің ішкі жиыны **Төлем түрі** өрісі арқылы ақылы ретінде белгіленуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="57ca7-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="57ca7-111">**Төлем түрі** өрісі - баға ұсыну жолының контекстінде келесі мәндерге мүмкіндік беретін параметрлер жиынтығы:</span><span class="sxs-lookup"><span data-stu-id="57ca7-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="57ca7-112">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-112">Chargeable</span></span>
  - <span data-ttu-id="57ca7-113">Ақысыз</span><span class="sxs-lookup"><span data-stu-id="57ca7-113">Non-chargeable</span></span>

<span data-ttu-id="57ca7-114">Ақылы компоненттерді тапсырмалар, рөлдер және транзакциялар санаттары бойынша анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="57ca7-115">Төлем қабілеттілігі баға ұсыну жолына арналған тапсырмалар бойынша анықталады және сол жолға енгізілген барлық транзакциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="57ca7-116">Егер **Тапсырмаларды қосу** өрісі **Барлық жоба** параметріне орнатылса немесе бос қалдырылса, **Ақылы тапсырмалар** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="57ca7-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="57ca7-117">Төлем қабілеттілігі баға ұсыну жолындағы рөлдер бойынша анықталған және тек **Мерзімдік** операциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="57ca7-118">Егер жобаның баға ұсыну жолындағы **Мерзімін қосу** өрісі **Жоқ** опциясына орнатылса, **Ақылы рөлдер** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="57ca7-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="57ca7-119">Төлем қабілеттілігі баға ұсыну жолындағы операциялық санаттар бойынша анықталады және тек **Шығыс** операциялар класына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="57ca7-120">Егер жобаның баға ұсыну жолындағы **Шығыстарды қосу** өрісі **Жоқ** опциясына орнатылса, **Ақылы санаттар** қойыншасы қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="57ca7-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="57ca7-121">Жоба тапсырмасын ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="57ca7-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="57ca7-122">Жоба тапсырмасы жобаға негізделген белгілі бір баға ұсыну жолының контекстінде ақылы немесе ақысыз болуы мүмкін, бұл келесі параметрлерді жасауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="57ca7-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="57ca7-123">Егер жобаға негізделген баға ұсыну жолында **Уақыт** және **Т1** тапсырмасы қамтылса, тапсырма баға ұсыну жолына ақылы ретінде байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="57ca7-124">Егер **Шығыстарды** қамтитын екінші баға ұсыну жолы болса, сіз баға ұсыну жолындағы **T1** тапсырмасын ақысыз деп байланыстыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="57ca7-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="57ca7-125">Нәтижесінде тапсырмаға жазылған барлық уақыт ақылы және тапсырмаға жазылған барлық шығындар ақысыз болады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="57ca7-126">Тапсырманың төлем түрін **Баға ұсыну жолының тапсырмалары** қосалқы торындағы **Шот түрі** өрісін жаңарту арқылы жоба негізіндегі бағаны ұсыну жолындағы **Ақылы тапсырмалар** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="57ca7-127">Не болмаса, жоба тапсырмасы үшін шот түрін тапсырмаға байланысты баға ұсыну жолдарын көрсететін жобаның тапсырма шотын орнату қосалқы торында **Шот түрі** өрісінде жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="57ca7-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="57ca7-128">Рөлді ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="57ca7-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="57ca7-129">Рөл белгілі бір жобаға негізделген баға ұсыну жолының контекстінде ақылы немесе ақысыз болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="57ca7-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="57ca7-130">Рөлдің шот түрін **Ақылы рөлдер** қосалқы торындағы **Шот түрі** өрісін жаңарту арқылы бағаны ұсыну жолындағы **Ақылы рөлдер** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="57ca7-131">Операция санатын ақылы немесе ақысыз ретінде жаңарту</span><span class="sxs-lookup"><span data-stu-id="57ca7-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="57ca7-132">Операция санаты белгілі бір баға ұсыну жолы бойынша ақылы немесе ақысыз болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="57ca7-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="57ca7-133">Транзакцияның шот түрін **Ақылы санаттар** қосалқы торындағы **Шот түрі** өрісін жаңарту арқылы бағаны ұсыну жолындағы **Ақылы санаттар** қойыншасында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="57ca7-134">Төлем қабілеттілігін шешу</span><span class="sxs-lookup"><span data-stu-id="57ca7-134">Resolve chargeability</span></span>
<span data-ttu-id="57ca7-135">Уақыт бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="57ca7-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="57ca7-136">**Уақыт** баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="57ca7-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="57ca7-137">**Рөлі** баға ұсыну жолында ақылы болып конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="57ca7-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="57ca7-138">**Қамтылған тапсырмалар** баға ұсыну жолында **Таңдалған тапсырмалар** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="57ca7-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="57ca7-139">Егер осы үш нәрсе дұрыс болса, **Тапсырма** да ақылы болып конфигурацияланады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="57ca7-140">Шығын бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="57ca7-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="57ca7-141">**Шығын** баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="57ca7-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="57ca7-142">**Транзакция санаты** баға ұсыну жолында ақылы болып конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="57ca7-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="57ca7-143">**Қамтылған тапсырмалар** баға ұсыну жолында **Таңдалған тапсырмалар** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="57ca7-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="57ca7-144">Егер осы үш нәрсе дұрыс болса, **Тапсырма** да ақылы болып конфигурацияланады.</span><span class="sxs-lookup"><span data-stu-id="57ca7-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="57ca7-145">Материал бойынша жасалған болжам немесе нақты көрсеткіш тек келесі жағдайда ғана ақылы болып саналады:</span><span class="sxs-lookup"><span data-stu-id="57ca7-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="57ca7-146">**Материалдар** баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="57ca7-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="57ca7-147">**Қамтылған тапсырмалар** баға ұсыну жолында **Таңдалған тапсырмалар** мәніне орнатылған.</span><span class="sxs-lookup"><span data-stu-id="57ca7-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="57ca7-148">Егер осы екі нәрсе дұрыс болса, **Тапсырма** да ақылы болып конфигурациялануы тиіс.</span><span class="sxs-lookup"><span data-stu-id="57ca7-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="57ca7-149">
                    <strong>Уақытпен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="57ca7-150">
                    <strong>Шығыспен қоса</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="57ca7-151">
                    <strong>Материалдарды қамтиды</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="57ca7-152">
                    <strong>Қосылған тапсырмалар</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-153">
                    <strong>Рөл</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="57ca7-154">
                    <strong>Санат</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-155">
                    <strong>Тапсырма</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="57ca7-156">
                    <strong>Төлем қабілеттілігінің әсері</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-157">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-158">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-159">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-160">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="57ca7-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-161">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-162">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-163">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-164">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-165">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-166">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-167">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-168">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-169">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-170">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="57ca7-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-171">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-172">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-173">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-174">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-175">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-176">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-177">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-178">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-179">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-180">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="57ca7-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-181">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-182">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-183">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-184">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-185">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-186">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-187">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-188">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-189">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-190">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="57ca7-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-191">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-192">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-193">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-194">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-195">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-196">Материал нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-197">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-198">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-199">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-200">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="57ca7-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-201">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-202">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-203">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-204">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-205">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-206">Материал нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-207">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-208">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-209">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-210">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="57ca7-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-211">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="57ca7-212">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-213">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-214">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-215">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-216">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="57ca7-217">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-218">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-219">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-220">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="57ca7-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-221">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="57ca7-222">
                    <strong>Ақылы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-223">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-224">Уақыт нақты мәніндегі шот ұсыну: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-225">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-226">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="57ca7-227">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-228">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-229">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-230">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="57ca7-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-231">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="57ca7-232">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-233">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-234">Уақыт нақты мәніндегі шот ұсыну: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-235">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-236">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-237">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="57ca7-238">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-239">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-240">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="57ca7-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-241">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-242">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-243">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-244">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-245">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-246">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-247">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="57ca7-248">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="57ca7-249">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-250">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="57ca7-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-251">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-252">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-253">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-254">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-255">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-256">Материал нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-257">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-258">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="57ca7-259">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-260">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="57ca7-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-261">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-262">Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-263">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-264">Уақыт нақты мәніндегі шот ұсыну: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-265">Шығыс нақты мәніндегі шот ұсыну түрі: Ақылы</span><span class="sxs-lookup"><span data-stu-id="57ca7-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="57ca7-266">Материал нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="57ca7-267">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="57ca7-268">Иә</span><span class="sxs-lookup"><span data-stu-id="57ca7-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="57ca7-269">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="57ca7-270">Барлық жоба</span><span class="sxs-lookup"><span data-stu-id="57ca7-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="57ca7-271">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="57ca7-272">
                    <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="57ca7-273">Орнату мүмкін емес</span><span class="sxs-lookup"><span data-stu-id="57ca7-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="57ca7-274">Уақыт нақты мәніндегі шот ұсыну: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-275">Шығын нақты мәніндегі шот ұсыну түрі: <strong>Ақысыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="57ca7-276">Материал нақты мәніндегі шот ұсыну түрі: <strong>Қолжетімді емес</strong>
                </span><span class="sxs-lookup"><span data-stu-id="57ca7-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
