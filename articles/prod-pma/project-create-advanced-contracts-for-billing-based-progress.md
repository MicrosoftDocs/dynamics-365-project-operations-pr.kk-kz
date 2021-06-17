---
title: Орындалу барысы бойынша шот ұсынуға арналған кеңейтілген келісім-шарттарды жасау
description: Бұл тақырыпта аяқталған жұмысқа негізделген есеп-шоттарды тұтынушыларға ұсына алу үшін жоба келісім-шарттарын жасау жолдары түсіндірілген.
author: RadhikaRS
ms.date: 03/26/2020
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 3b445488100e0a8335a05505405953b173ff836c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999678"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a><span data-ttu-id="09935-103">Орындалу барысы бойынша шот ұсынуға арналған кеңейтілген келісім-шарттарды жасау</span><span class="sxs-lookup"><span data-stu-id="09935-103">Create advanced contracts for billing based on progress</span></span>
[!include [banner](../includes/banner.md)]

<span data-ttu-id="09935-104">Бұл тақырыпта аяқталған жұмысқа негізделген есеп-шоттарды тұтынушыларға ұсына алу үшін жоба келісім-шарттарын жасау жолдары түсіндірілген.</span><span class="sxs-lookup"><span data-stu-id="09935-104">This topic explains how to create project contracts so that you can create invoices for customers, based on a percentage of completed work.</span></span> <span data-ttu-id="09935-105">Есеп-шот сомалары автоматты түрде жоба үшін орнатылған жұмыстың бюджет санаттары үшін есептеледі.</span><span class="sxs-lookup"><span data-stu-id="09935-105">Invoice amounts are automatically calculated for the budget categories of work that you set up for a project.</span></span> <span data-ttu-id="09935-106">Есеп-шот уақыты тұтынушымен жоба келісім-шартын жасаған кезде орнатылады.</span><span class="sxs-lookup"><span data-stu-id="09935-106">The invoice timing is set when you negotiate the project contract with the customer.</span></span>

<span data-ttu-id="09935-107">Осы тақырыптағы процедураларды, келісім-шарт, байланысты жоба және жоба үшін орнатылған жұмыстың бюджет санаттары үшін есеп-шот сомаларын есептейтін шот ұсыну ережелерін құру үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-107">Use the procedures in this topic to set up a contract, an associated project, and the billing rules that calculate invoice amounts for the budget categories of work that you set up for the project.</span></span>

<span data-ttu-id="09935-108">Келісім-шарт пен жобаны жасағаннан кейін, сіз жоба мәліметтерін орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="09935-108">After you've created the contract and the project, you can set up the details of the project.</span></span> <span data-ttu-id="09935-109">Мысалы, әрекеттерді анықтай аласыз және жобаға қызметкерлер тағайындай аласыз.</span><span class="sxs-lookup"><span data-stu-id="09935-109">For example, you can define activities and assign workers to the project.</span></span>

## <a name="example"></a><span data-ttu-id="09935-110">Мысал</span><span class="sxs-lookup"><span data-stu-id="09935-110">Example</span></span>

<span data-ttu-id="09935-111">Сіздің ұйымыңыз бағдарламалық жасақтама дайындайтын фирма.</span><span class="sxs-lookup"><span data-stu-id="09935-111">Your organization is a software development firm.</span></span> <span data-ttu-id="09935-112">Сіз жалпы төлемге 20 000 АҚШ долларын құрайтын тұтынушы үшін жалақы есебінің бумасын жасауға келісесіз.</span><span class="sxs-lookup"><span data-stu-id="09935-112">You agree to develop a payroll accounting package for a customer for a total fee of 20,000 US dollars (USD).</span></span> <span data-ttu-id="09935-113">Ұйымыңыз жобаның нақты пайыздық мөлшерлемесін аяқтаған кезде тұтынушыға есеп-шот жасауға келіседі.</span><span class="sxs-lookup"><span data-stu-id="09935-113">Your organization agrees to invoice the customer as you complete specific percentages of the project.</span></span> <span data-ttu-id="09935-114">Шот ұсыну процесінде қолдана алатындай, жұмыс үшін келесі жоба санаттарын орнатыңыз:</span><span class="sxs-lookup"><span data-stu-id="09935-114">You set up the following project categories for the work, so that you can use them in the billing process:</span></span>

- <span data-ttu-id="09935-115">Кеңес беру</span><span class="sxs-lookup"><span data-stu-id="09935-115">Consulting</span></span>
- <span data-ttu-id="09935-116">Құрастырушы</span><span class="sxs-lookup"><span data-stu-id="09935-116">Design</span></span>
- <span data-ttu-id="09935-117">Орнату</span><span class="sxs-lookup"><span data-stu-id="09935-117">Installation</span></span>

<span data-ttu-id="09935-118">Сонымен қатар, әр санаттағы аяқталған жоба жұмысының пайызына есеп-шот сомаларын автоматты түрде есептейтін төлем ережелерін орнаттыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-118">You also set up billing rules that automatically calculate the invoice amounts for the percentage of project work that is completed in each category.</span></span>

<span data-ttu-id="09935-119">Бюджет менеджері жоба санаттары үшін бюджет жасайды.</span><span class="sxs-lookup"><span data-stu-id="09935-119">The budget manager creates a budget for the project categories.</span></span> <span data-ttu-id="09935-120">Аяқталған жұмыстың көлемі автоматты түрде бюджеттің жоспарланған көлемімен салыстырғанда нақты жұмыстың пайызы ретінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="09935-120">The amount of completed work is automatically calculated as a percentage of actual work in comparison to the budgeted amounts.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09935-121">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="09935-121">Prerequisites</span></span>

<span data-ttu-id="09935-122">Шот ұсыну ережелерін пайдаланатын жоба жасамас бұрын, шот ұсыну ережелеріне арналған сандар тізбегін және ұсынылатын шоттар орналастыру үшін пайдаланылатын төлемдер журналын орнату керек.</span><span class="sxs-lookup"><span data-stu-id="09935-122">Before you create a project that uses billing rules, you must set up the number sequences for billing rules and a fee journal that is used to post progress billings.</span></span>

1. <span data-ttu-id="09935-123">**Жобаны басқару және есепке алу** \> **Орнату** \> **Жобаны басқару және есепке алу параметрлері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-123">Go to **Project management and accounting** \> **Setup** \> **Project management and accounting parameters**.</span></span>
2. <span data-ttu-id="09935-124">**Жобаны басқару және есепке алу параметрлері** бетіндегі **Сандар тізбегі** қойыншасында шот ұсыну ережелері жасалған кезде пайдалану керек сандар тізбегін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-124">On the **Project management and accounting parameters** page, on the **Number sequences** tab, set up the number sequence that you want to use when billing rules are created.</span></span>
3. <span data-ttu-id="09935-125">**Жобаны басқару және есепке алу** \> **Журналдар** \> **Төлемдер** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-125">Go to **Project management and accounting** \> **Journals** \> **Fee**.</span></span>
4. <span data-ttu-id="09935-126">**Төлемдер журналы** бетінен **Жаңа** параметрін таңдап, журнал атауын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-126">On the **Fee journal** page, select **New**, and enter the journal name.</span></span>

## <a name="create-a-contract-for-progress-billings"></a><span data-ttu-id="09935-127">Ұсынылатын шоттар үшін келісім-шарт жасау</span><span class="sxs-lookup"><span data-stu-id="09935-127">Create a contract for progress billings</span></span>

<span data-ttu-id="09935-128">Бұл процедураны бекітілген баға жобасына арналған жоба келісім-шартын жасау үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-128">Use this procedure to create a project contract for a fixed-price project.</span></span> <span data-ttu-id="09935-129">Жобадағы аяқталған жұмыс көрсетілген пайызға жеткен кезде сіз жоба есеп-шотын жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="09935-129">You create a project invoice when the work that is completed on the project reaches a specified percentage.</span></span>

1. <span data-ttu-id="09935-130">**Жобаларды басқару және есепке алу** \> **Жобалар** \> **Жоба келісім-шарттары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-130">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="09935-131">**Жоба келісім-шарттары** бетінде **Жаңа** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-131">On the **Project contracts** page, select **New**.</span></span>
3. <span data-ttu-id="09935-132">**Жаңа жоба келісім-шарты** диалогтік терезесінде келесі өрістерді орнатыңыз:</span><span class="sxs-lookup"><span data-stu-id="09935-132">In the **New project contract** dialog box, set the following fields:</span></span>

    - <span data-ttu-id="09935-133">**Атауы**</span><span class="sxs-lookup"><span data-stu-id="09935-133">**Name**</span></span>
    - <span data-ttu-id="09935-134">**Қаржыландыру түрі**</span><span class="sxs-lookup"><span data-stu-id="09935-134">**Funding type**</span></span>
    - <span data-ttu-id="09935-135">**Қаржыландыру көзі**</span><span class="sxs-lookup"><span data-stu-id="09935-135">**Funding source**</span></span>
    - <span data-ttu-id="09935-136">**Сатылым валютасы** - әдепкі бойынша, бұл валюта жоба келісім-шартына байланысты тұтынушы есеп-шоттарында пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="09935-136">**Sales currency** – By default, this currency is used for customer invoices that are associated with the project contract.</span></span> <span data-ttu-id="09935-137">Алайда, сіз сатылым валютасын белгілі бір тұтынушы есеп-шотында өзгерте аласыз.</span><span class="sxs-lookup"><span data-stu-id="09935-137">However, you can change the sales currency on a specific customer invoice.</span></span>

4. <span data-ttu-id="09935-138">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-138">Select **OK**.</span></span> <span data-ttu-id="09935-139">Ақпарат **Жоба келісім-шарттары** бетінің жоғарғы деректемесіне көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="09935-139">The information is copied to the header of the **Project contracts** page.</span></span>
5. <span data-ttu-id="09935-140">**Жоба келісім-шарттары** бетінде жобаға қажетті қалған ақпаратты толтырыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-140">On the **Project contracts** page, fill in the rest of the required information for the project.</span></span>

## <a name="create-a-project-for-progress-billings"></a><span data-ttu-id="09935-141">Ұсынылатын шоттар үшін жоба жасау</span><span class="sxs-lookup"><span data-stu-id="09935-141">Create a project for progress billings</span></span>

<span data-ttu-id="09935-142">Жобаны және жоба келісім-шартына байланысты кез келген ішкі жобаларды құру үшін осы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-142">Follow these steps to create a project and any subprojects that are associated with a project contract.</span></span>

1. <span data-ttu-id="09935-143">**Жобаларды басқару және есепке алу** \> **Жобалар** \> **Барлық жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-143">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="09935-144">**Барлық жобалар** бетінде **Жаңа** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-144">On the **All projects** page, select **New**.</span></span>
3. <span data-ttu-id="09935-145">**Жаңа жоба** диалогтік терезесінде, **Жоба түрі** өрісінен **Уақыт және материал** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-145">In the **New project** dialog box, in the **Project type** field, select **Time and material**.</span></span>
4. <span data-ttu-id="09935-146">Жоба тобын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-146">Select a project group.</span></span> <span data-ttu-id="09935-147">Жоба тобы топқа тағайындалған жобалар үшін орналастыру ақпаратын анықтайды.</span><span class="sxs-lookup"><span data-stu-id="09935-147">A project group defines the posting information for the projects that are assigned to the group.</span></span>
5. <span data-ttu-id="09935-148">**Жоба жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-148">Select **Create project**.</span></span>
6. <span data-ttu-id="09935-149">Жоба жасалғаннан кейін, жоба кезеңін **Орындалуда** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-149">After the project is created, set the project stage to **In process**.</span></span>

## <a name="create-a-budget-for-a-project"></a><span data-ttu-id="09935-150">Жоба үшін бюджет құру</span><span class="sxs-lookup"><span data-stu-id="09935-150">Create a budget for a project</span></span>

<span data-ttu-id="09935-151">Бюджет санаттары әр санат үшін аяқталған жұмыс пайызына есеп-шот сомаларын автоматты түрде есептеу үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="09935-151">Budget categories are used to automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="09935-152">Болжамды құнға арналған бюджет санаттарын құру үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-152">Follow these steps to create budget categories for the estimated costs.</span></span>

1. <span data-ttu-id="09935-153">**Жобаларды басқару және есепке алу** \> **Жобалар** \> **Барлық жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-153">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="09935-154">**Барлық жобалар** бетінде қажет жобаны таңдап, ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-154">On the **All projects** page, select and open the project that you want.</span></span>
3. <span data-ttu-id="09935-155">**Жобалар** бетіндегі әрекеттер тақтасында, **Жоспар** қойыншасындағы **Бюджет** тобынан **Жоба бюджеті** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-155">On the **Projects** page, on the Action Pane, on the **Plan** tab, in the **Budget** group, select **Project budget**.</span></span>
4. <span data-ttu-id="09935-156">**Жоба бюджеті** бетінде жобадағы әр санат үшін болжамды құнын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-156">On the **Project budget** page, enter an estimated cost for each category in the project.</span></span>

## <a name="create-billing-rules-for-progress-billings"></a><span data-ttu-id="09935-157">Ұсынылатын шоттар үшін шот ұсыну ережелерін жасау</span><span class="sxs-lookup"><span data-stu-id="09935-157">Create billing rules for progress billings</span></span>

1. <span data-ttu-id="09935-158">**Жобаларды басқару және есепке алу** \> **Жобалар** \> **Жоба келісім-шарттары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-158">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="09935-159">**Жоба келісім-шарттары** бетінде жоба келісім-шартын таңдап, ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-159">On the **Project contracts** page, select and open a project contract.</span></span>
3. <span data-ttu-id="09935-160">Жоба келісім-шарты бетіндегі **Шот ұсыну ережелері** FastTab қойыншасынан **Қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-160">On the project contract page, on the **Billing rules** FastTab, select **Add**.</span></span>
4. <span data-ttu-id="09935-161">**Шот ұсыну ережесі** бетінде, **Жол түрі** өрісінен **Орындалу барысы** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-161">On the **Billing rule** page, in the **Line type** field, select **Progress**.</span></span>
5. <span data-ttu-id="09935-162">**Шот ұсыну ережесі жолының мәліметтері** FastTab қойыншасындағы **Келісім-шарт мәні** өрісіне келісім-шарттың жалпы мәнін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-162">On the **Billing rule line details** FastTab, in the **Contract value** field, enter the total value of the contract.</span></span>
6. <span data-ttu-id="09935-163">**Санат** өрісінде ақы транзакциясын орналастыратын санатты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-163">In the **Category** field, select the category to post the fee transaction to.</span></span>
7. <span data-ttu-id="09935-164">**Жоба** өрісінде осы шот ұсыну ережесін қолданатын жобаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-164">In the **Project** field, select the project that uses this billing rule.</span></span>
8. <span data-ttu-id="09935-165">Қосымша: шот ұсыну ережесін қосымша жобаларға тағайындаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-165">Optional: Assign the billing rule to additional projects.</span></span> <span data-ttu-id="09935-166">**Жоба** FastTab қойыншасындағы **Қолжетімді жобалар** бөлімінен жобаны таңдаңыз, содан кейін жобаны **Таңдалған жобалар** бөліміне қосу үшін оң жақ көрсеткіні таңдаңыз басыңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-166">On the **Project** FastTab, in the **Available projects** section, select a project, and then select the right arrow button to add the project to the **Selected projects** section.</span></span>
9. <span data-ttu-id="09935-167">Қосымша: тұтынушы есеп-шоттағы төлемдерден ұстап қалатын пайыздық соманы есептеңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-167">Optional: Calculate the percentage amount that the customer withholds from payments on an invoice.</span></span> <span data-ttu-id="09935-168">**Төлемді сақтау шарттары** FastTab қойыншасында, қаржыландыру көзін таңдаңыз, содан кейін **Сақтау пайызы** өрісіне сақтау пайызын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="09935-168">On the **Payment retention terms** FastTab, select the funding source, and then, in the **Retention percentage** field, enter the retention percentage.</span></span>
10. <span data-ttu-id="09935-169">Жоба келісім-шарты үшін қосымша шот ұсыну ережелерін жасау үшін осы қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="09935-169">Repeat these steps to create additional billing rules for the project contract.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]