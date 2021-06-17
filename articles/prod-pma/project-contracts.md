---
title: Жоба келісім-шарттары
description: Бұл тақырыпта әртүрлі жобалар мен қаржыландыру көздері үшін жасай алатын жоба келісім-шарттарының мысалдары, сондай-ақ келісім-шарттар мен есеп-шот жобасының тұтынушыларын басқара аласыз.
author: Yowelle
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a794ec38ac07c1418f9e95b741941a83492bb3d5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999768"
---
# <a name="project-contracts"></a><span data-ttu-id="317a1-103">Жоба келісім-шарттары</span><span class="sxs-lookup"><span data-stu-id="317a1-103">Project contracts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="317a1-104">Бұл мақалада әртүрлі жобалар мен қаржыландыру көздері үшін жасай алатын жоба келісім-шарттарының мысалдары, сондай-ақ келісім-шарттар мен есеп-шот жобасының тұтынушыларын басқара аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-104">This article provides examples of the project contracts that you can create for various types of projects and funding sources, and how you can manage contracts and invoice project customers.</span></span>

<span data-ttu-id="317a1-105">Жоба келісім-шарты үшін жасайтын жоба түрі жоба тұтынушыларына есеп-шот ұсыну әдісін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="317a1-105">The type of project that you create for a project contract determines the method that is used to invoice project customers.</span></span> <span data-ttu-id="317a1-106">Сіз жоба келісім-шартын және оған қатысты жобаны өзгерте аласыз, бірақ жоба түрін өзгерте алмайсыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-106">You can change a project contract and the related project, but you can't change the project type.</span></span> 

<span data-ttu-id="317a1-107">Жоба келісім-шартын пайдалану арқылы сіз бір немесе бірнеше жобаларға бір уақытта есеп-шот ұсына аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-107">By using a project contract, you can invoice one or more projects at the same time.</span></span> <span data-ttu-id="317a1-108">Жоба келісім-шарты сонымен қатар жоба құрылымындағы әрбір кіші жоба үшін дәйекті есеп-шот процедурасына кепілдік береді.</span><span class="sxs-lookup"><span data-stu-id="317a1-108">The project contract also helps guarantee a consistent invoicing procedure for every subproject in a project structure.</span></span> 

<span data-ttu-id="317a1-109">Есеп-шот ұсынылатын кез келген жоба келісім-шартымен байланысты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="317a1-109">Every project that will be invoiced must be associated with a project contract.</span></span> <span data-ttu-id="317a1-110">Жоба келісім-шартының параметрлері сол жоба келісім-шартымен байланысты барлық жобалар мен кіші жобаларға қолданылады.</span><span class="sxs-lookup"><span data-stu-id="317a1-110">The settings for a project contract apply to all projects and subprojects that are associated with that project contract.</span></span> 

<span data-ttu-id="317a1-111">Жоба келісім-шартында бір немесе бірнеше дереккөздер көрсетілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="317a1-111">A project contract can specify one or more sources of funding.</span></span> <span data-ttu-id="317a1-112">Сондықтан сіз төлемді бірнеше қаржыландырушылар арасында бөле аласыз, қаржыландыру көздері белгіленген мөлшерден артық болмайтындай етіп қаржыландыру шектеулерін белгілей аласыз және шығыстарды есептеу үшін қаржыландыру ережелерін конфигурациялай аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-112">Therefore, you can split the billing among multiple funders, set up funding limits so that funding sources are not billed more than a specified amount, and configure funding rules for charging expenditures.</span></span>

## <a name="funding-for-project-contracts"></a><span data-ttu-id="317a1-113">Жоба келісім-шарттарын қаржыландыру</span><span class="sxs-lookup"><span data-stu-id="317a1-113">Funding for project contracts</span></span>
<span data-ttu-id="317a1-114">Жобаның кейбір келісім-шарттарында бірнеше тараптар жобаның шығындарын қаржыландыру жауапкершілігін бөлетіндігі көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="317a1-114">Some project contracts specify that multiple parties share the responsibility for funding the project costs.</span></span> <span data-ttu-id="317a1-115">Мысалы:</span><span class="sxs-lookup"><span data-stu-id="317a1-115">Here are some examples:</span></span>

-   <span data-ttu-id="317a1-116">Бірнеше бөлімшелері бар ірі тұтынушы жобаны қаржыландыруды бөлу жолымен бөлуді сұрайды.</span><span class="sxs-lookup"><span data-stu-id="317a1-116">A large customer that has multiple divisions requests that funding of a project be split by division.</span></span>
-   <span data-ttu-id="317a1-117">Компанияңыз үлкен жобаның шығындарын сыртқы ұйыммен бөліседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-117">Your company shares the costs of a large project with an external organization.</span></span>
-   <span data-ttu-id="317a1-118">Жол жобасын екі муниципалитет қаржыландырады.</span><span class="sxs-lookup"><span data-stu-id="317a1-118">A  road project is co-funded by two municipalities.</span></span>
-   <span data-ttu-id="317a1-119">Көпір жобасы мемлекеттік грант пен жеке корпорация тарапынан қаржыландырылады.</span><span class="sxs-lookup"><span data-stu-id="317a1-119">A bridge project is funded by a government grant and a private corporation.</span></span>

<span data-ttu-id="317a1-120">Dynamics 365 Finance жүйесінде, бір транзакция немесе бүкіл жоба үшін төлемді бірнеше тұтынушылар, гранттар немесе ұйымдар арасында бөле аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-120">In Dynamics 365 Finance, you can split the billing for a single transaction or an entire project among multiple customers, grants, or organizations.</span></span> 

<span data-ttu-id="317a1-121">Бірнеше қаржыландырушысы бар жобаларда қаржыландырудың озық жобасын қаржыландыруға үлес қосатын барлық тараптар қаржыландыру көздері деп аталады.</span><span class="sxs-lookup"><span data-stu-id="317a1-121">In projects that have multiple funders, all parties that contribute to the funding of an advanced funding project are called funding sources.</span></span> <span data-ttu-id="317a1-122">Тұтынушы, ұйым немесе грант қаржыландыру көзі ретінде анықталғаннан кейін, оны қаржыландырудың бір немесе бірнеше ережелеріне тағайындауға болады.</span><span class="sxs-lookup"><span data-stu-id="317a1-122">After a customer, organization, or grant is defined as a funding source, it can be assigned to one or more funding rules.</span></span> <span data-ttu-id="317a1-123">Қаржыландыру ережелері жобаны қаржыландырудың түрлі көздеріне төлемдердің қалай бөлінетінін анықтайтын критерийлерден тұрады.</span><span class="sxs-lookup"><span data-stu-id="317a1-123">Funding rules contain the criteria that determines how charges are allocated to the various funding sources for a project.</span></span> 

<span data-ttu-id="317a1-124">Сатып алу сұрауларында және сатып алу тапсырыстарында пайда болатын биржалық заттарды бөлуге болмайтындықтан, шығын мөлшерін тарату кезінде бірнеше қаржыландыру көздері арасында бөлуге болмайды.</span><span class="sxs-lookup"><span data-stu-id="317a1-124">Because stocked items, such as those that appear on purchase requisitions and purchase orders, can't be split, the cost amount can't be split among multiple funding sources at the time of distribution.</span></span> <span data-ttu-id="317a1-125">Сондықтан, қаржыландыру көзінің мәні қорды сату есепке алынғанға дейін 0 (нөл) болып қалады.</span><span class="sxs-lookup"><span data-stu-id="317a1-125">Therefore, the funding source value remains 0 (zero) until the inventory issue is posted.</span></span> <span data-ttu-id="317a1-126">Қорды сату есепке алынған кезде, шығын мөлшері жобаның тіркелгі тарату ережелеріне сәйкес бөлінеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-126">When the inventory issue is posted, the cost amount is distributed according to the account distribution rules for the project.</span></span>

<span data-ttu-id="317a1-127">Төлемді бірнеше қаржыландыру көздері арасында бөлуді жеңілдету үшін келесі бірнеше қадамды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="317a1-127">Here are some steps that you can take to make it easier to split the billing among multiple funding sources:</span></span>

-   <span data-ttu-id="317a1-128">Жоба үшін жасалған барлық транзакциялар жоба келісім-шартымен бірдей сату валютасын қолданатынын көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-128">Specify that all transactions that are entered for a project use the same sales currency as the project contract.</span></span>
-   <span data-ttu-id="317a1-129">Қаржыландыру көзіне жоба бойынша белгіленген мөлшерден артық төлем жасалмайтындай етіп қаржыландыру шектеулерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-129">Set up funding limits, so that a funding source isn't invoiced more than a specified amount toward a project.</span></span>
-   <span data-ttu-id="317a1-130">Әр қызметкер, элемент, санат, санат тобы және транзакция түрі (немесе барлық операция түрлері) үшін қаржыландыру ережелері мен қаржыландыру шектеулерін конфигурациялаңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-130">Configure funding rules and funding limits for each worker, item, category, category group, and transaction type (or for all transaction types).</span></span>
-   <span data-ttu-id="317a1-131">Әр қаржыландыру ережесі жарамды болған кезеңді анықтау үшін қосымша басталу және аяқталу күндерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-131">Select optional start and end dates to define the period when each funding rule is valid.</span></span>
-   <span data-ttu-id="317a1-132">Әрбір қаржыландыру көзі жауапты пайыздық мөлшерді көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-132">Specify the percentage that each funding source is responsible for.</span></span>
-   <span data-ttu-id="317a1-133">Қаржыны бөлу есептеулерінен туындайтын айырмашылықтарды дөңгелектеу үшін қай қаржыландыру көзі жауапты екенін көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-133">Specify which funding source is responsible for rounding differences that are caused by funding allocation calculations.</span></span>
-   <span data-ttu-id="317a1-134">Жоба шығындарының сыртқы тұтынушыларға есептелу және ішкі ұйымдардан алыну жолын анықтайтын ережелер орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-134">Set up rules that determine how project costs are invoiced to external customers and charged to internal organizations.</span></span>
-   <span data-ttu-id="317a1-135">Қосымша қаржыландыру алынғанға дейін немесе компания ішіндегі шығындарды өтеуге шешім қабылдағанға дейін транзакцияларды тіркелген қаржыландыру шотына жазыңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-135">Record transactions in an on-hold funding account until additional funding can be obtained, or until you decide to bear the costs internally.</span></span>

<span data-ttu-id="317a1-136">Транзакциямен қандай салық тобын байланыстыру керектігін анықтау үшін жоба бойынша салық тобын тағайындау жүргізіледі.</span><span class="sxs-lookup"><span data-stu-id="317a1-136">To determine which tax group to associate with a transaction, the project is searched for a tax group assignment.</span></span> <span data-ttu-id="317a1-137">Егер жоба деңгейінде салық тобын тағайындау жүргізілмесе, жоба келісім-шартын іздеу орындалады.</span><span class="sxs-lookup"><span data-stu-id="317a1-137">If no tax group assignment has been made at the project level, the project contract is searched.</span></span>

### <a name="example-multiple-funding-sources-simple"></a><span data-ttu-id="317a1-138">Мысалы: бірнеше қаржыландыру көзі (қарапайым)</span><span class="sxs-lookup"><span data-stu-id="317a1-138">Example: Multiple funding sources (simple)</span></span>

<span data-ttu-id="317a1-139">Келесі кестеде бірнеше қаржыландыру көздері арасында қаржыландыруды бөлуді басқаруға арналған сценарийлер берілген.</span><span class="sxs-lookup"><span data-stu-id="317a1-139">The following table provides scenarios for managing funding allocation among multiple funding sources.</span></span> <span data-ttu-id="317a1-140">Бұл сценарийлер келесі болжамдарға негізделген:</span><span class="sxs-lookup"><span data-stu-id="317a1-140">These scenarios are based on the following assumptions:</span></span>

-   <span data-ttu-id="317a1-141">Басымдық параметрлері басқа қаржыландыру ережелері критерийлері қолданылғанға дейін қаражат бөлу кезінде ескеріледі.</span><span class="sxs-lookup"><span data-stu-id="317a1-141">Priority settings are factored into the allocation of funds before other funding rule criteria are applied.</span></span>
-   <span data-ttu-id="317a1-142">Қаржыландыру ережесі жарамды болған d кезеңін анықтайтын күндер ауқымы көрсетілмеген.</span><span class="sxs-lookup"><span data-stu-id="317a1-142">No date range has been specified to define the period d when the funding rule is valid.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="317a1-143"><strong>Сценарий</strong></span><span class="sxs-lookup"><span data-stu-id="317a1-143"><strong>Scenario</strong></span></span></td>
<td><span data-ttu-id="317a1-144"><strong>Қаржыландыру көзі</strong></span><span class="sxs-lookup"><span data-stu-id="317a1-144"><strong>Funding source</strong></span></span></td>
<td><span data-ttu-id="317a1-145"><strong>Бөлу пайызы</strong></span><span class="sxs-lookup"><span data-stu-id="317a1-145"><strong>Allocation percentage</strong></span></span></td>
<td><span data-ttu-id="317a1-146"><strong>Бөлу басымдығы</strong></span><span class="sxs-lookup"><span data-stu-id="317a1-146"><strong>Allocation priority</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="317a1-147">Шығындарды бір қаражат көзіне қаражаты біткенше бөлуді, екінші қаржыландыру көзіне қаражаты біткенше бөлуді және қалған шығындарды үшінші қаржыландыру көзіне бөлуді қалайсыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-147">You want to allocate costs to one funding source until its funds are exhausted, allocate costs to a second funding source until its funds are exhausted, and finally allocate the remaining costs to a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="317a1-148">1-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-148">Funding　source　1</span></span></li>
<li><span data-ttu-id="317a1-149">2-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-149">Funding　source　2</span></span></li>
<li><span data-ttu-id="317a1-150">3-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-150">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="317a1-151">100%</span><span class="sxs-lookup"><span data-stu-id="317a1-151">100%</span></span></li>
<li><span data-ttu-id="317a1-152">100%</span><span class="sxs-lookup"><span data-stu-id="317a1-152">100%</span></span></li>
<li><span data-ttu-id="317a1-153">100%</span><span class="sxs-lookup"><span data-stu-id="317a1-153">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="317a1-154">1</span><span class="sxs-lookup"><span data-stu-id="317a1-154">1</span></span></li>
<li><span data-ttu-id="317a1-155">2</span><span class="sxs-lookup"><span data-stu-id="317a1-155">2</span></span></li>
<li><span data-ttu-id="317a1-156">3</span><span class="sxs-lookup"><span data-stu-id="317a1-156">3</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="317a1-157">Сіз шығындардың 75 пайызын бір қаржыландыру көзіне, 25 пайызын екінші қаржыландыру көзіне бөлгіңіз келеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-157">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="317a1-158">Қаржыландыру көздерінің екеуі де таусылғанда, қалған шығындарды үшінші қаржыландыру көзінен өтегіңіз келеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-158">When either of those funding sources is exhausted, you want to pay the remaining costs from a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="317a1-159">1-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-159">Funding　source　1</span></span></li>
<li><span data-ttu-id="317a1-160">2-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-160">Funding　source　2</span></span></li>
<li><span data-ttu-id="317a1-161">3-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-161">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="317a1-162">75%</span><span class="sxs-lookup"><span data-stu-id="317a1-162">75%</span></span></li>
<li><span data-ttu-id="317a1-163">25%</span><span class="sxs-lookup"><span data-stu-id="317a1-163">25%</span></span></li>
<li><span data-ttu-id="317a1-164">100%</span><span class="sxs-lookup"><span data-stu-id="317a1-164">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="317a1-165">1</span><span class="sxs-lookup"><span data-stu-id="317a1-165">1</span></span></li>
<li><span data-ttu-id="317a1-166">1</span><span class="sxs-lookup"><span data-stu-id="317a1-166">1</span></span></li>
<li><span data-ttu-id="317a1-167">2</span><span class="sxs-lookup"><span data-stu-id="317a1-167">2</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="317a1-168">Сіз шығындардың 75 пайызын бір қаржыландыру көзіне, 25 пайызын екінші қаржыландыру көзіне бөлгіңіз келеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-168">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="317a1-169">Қаржыландыру көздерінің екеуі де таусылғанда, үшінші қаржыландыру көзі мен төртінші қаржыландыру көзінің арасындағы қалған шығындарды бөлгіңіз келеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-169">When either of those funding sources is exhausted, you want to split the remaining costs between a third funding source and a fourth funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="317a1-170">1-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-170">Funding　source　1</span></span></li>
<li><span data-ttu-id="317a1-171">2-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-171">Funding　source　2</span></span></li>
<li><span data-ttu-id="317a1-172">3-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-172">Funding　source　3</span></span></li>
<li><span data-ttu-id="317a1-173">4-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-173">Funding　source　4</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="317a1-174">75%</span><span class="sxs-lookup"><span data-stu-id="317a1-174">75%</span></span></li>
<li><span data-ttu-id="317a1-175">25%</span><span class="sxs-lookup"><span data-stu-id="317a1-175">25%</span></span></li>
<li><span data-ttu-id="317a1-176">50%</span><span class="sxs-lookup"><span data-stu-id="317a1-176">50%</span></span></li>
<li><span data-ttu-id="317a1-177">50%</span><span class="sxs-lookup"><span data-stu-id="317a1-177">50%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="317a1-178">1</span><span class="sxs-lookup"><span data-stu-id="317a1-178">1</span></span></li>
<li><span data-ttu-id="317a1-179">1</span><span class="sxs-lookup"><span data-stu-id="317a1-179">1</span></span></li>
<li><span data-ttu-id="317a1-180">2</span><span class="sxs-lookup"><span data-stu-id="317a1-180">2</span></span></li>
<li><span data-ttu-id="317a1-181">2</span><span class="sxs-lookup"><span data-stu-id="317a1-181">2</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="317a1-182">Сіз шығындардың алғашқы 25 пайызын бір қаржыландыру көзіне, қалғанын екінші қаржыландыру көзіне бөлгіңіз келеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-182">You want to allocate the first 25 percent of costs to one funding source and the rest to a second funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="317a1-183">1-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-183">Funding　source　1</span></span></li>
<li><span data-ttu-id="317a1-184">2-қаржыландыру көзі</span><span class="sxs-lookup"><span data-stu-id="317a1-184">Funding　source　2</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="317a1-185">25%</span><span class="sxs-lookup"><span data-stu-id="317a1-185">25%</span></span></li>
<li><span data-ttu-id="317a1-186">100%</span><span class="sxs-lookup"><span data-stu-id="317a1-186">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="317a1-187">1</span><span class="sxs-lookup"><span data-stu-id="317a1-187">1</span></span></li>
<li><span data-ttu-id="317a1-188">2</span><span class="sxs-lookup"><span data-stu-id="317a1-188">2</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a><span data-ttu-id="317a1-189">Мысалы: бірнеше қаржыландыру көзі (күрделі)</span><span class="sxs-lookup"><span data-stu-id="317a1-189">Example: Multiple funding sources (complex)</span></span>

<span data-ttu-id="317a1-190">Сізде келесі тәртіпте пайдаланғыңыз келетін үш қаржыландыру көзі бар:</span><span class="sxs-lookup"><span data-stu-id="317a1-190">You have three funding sources that you want to use in the following order:</span></span>

1.  <span data-ttu-id="317a1-191">2-қаржыландыру көзі мен 3-қаржыландыру көзін 2-қаржыландыру көзі таусылғанша теңдей пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-191">Use funding source 2 and funding source 3 equally until funding source 2 is exhausted.</span></span>
2.  <span data-ttu-id="317a1-192">3-қаржыландыру көзі таусылғанға дейін оны пайдалануды жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-192">Continue to use funding source 3 until it is exhausted.</span></span>
3.  <span data-ttu-id="317a1-193">3-қаржыландыру көзі таусылғаннан кейін 1-қаржыландыру көзін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-193">Use funding source 1 after funding source 3 is exhausted.</span></span>

<span data-ttu-id="317a1-194">Осы мақсатты орындау үшін келесі әрекеттерді орындау керек:</span><span class="sxs-lookup"><span data-stu-id="317a1-194">To accomplish this goal, you must do the following:</span></span>

-   <span data-ttu-id="317a1-195">2-қаржыландыру көзі мен 3-қаржыландыру көзі үшін тиісті мөлшерде қаржыландыру шектеулерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-195">Set up funding limits for funding source 2 and funding source 3, for their respective amounts.</span></span>
-   <span data-ttu-id="317a1-196">Келесі қаржыландыру ережелерін жасаңыз:</span><span class="sxs-lookup"><span data-stu-id="317a1-196">Create the following funding rules:</span></span>
    -   <span data-ttu-id="317a1-197">1-ереже (1-басымдық): транзакциялардың 50 пайызын 2-қаржыландыру көзіне және 50 пайызын 3-қаржыландыру көзіне бөліңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-197">Rule 1 (Priority 1): Allocate 50 percent of transactions to funding source 2 and 50 percent to funding source 3.</span></span>
    -   <span data-ttu-id="317a1-198">2-ереже (2-басымдық): транзакциялардың 100 пайызын 3-қаржыландыру көзіне бөліңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-198">Rule 2 (Priority 2): Allocate 100 percent of transactions to funding source 3.</span></span>
    -   <span data-ttu-id="317a1-199">3-ереже (3-басымдық): транзакциялардың 100 пайызын 1-қаржыландыру көзіне бөліңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-199">Rule 3 (Priority 3): Allocate 100 percent of transactions to funding source 1.</span></span>

<span data-ttu-id="317a1-200">Бұл орнату жұмыс істейді, себебі транзакциялар олардың кез келгенінің транзакцияға қатыстылығын анықтау үшін ережелер мен шектеулерге сәйкес тексеріледі.</span><span class="sxs-lookup"><span data-stu-id="317a1-200">This setup works because transactions are checked against rules and limits to determine whether any of them apply to the transaction.</span></span> <span data-ttu-id="317a1-201">Егер транзакцияға арнайы ережелер мен шектеулер қолданылмаса, барлық транзакция ережелері қолданылады.</span><span class="sxs-lookup"><span data-stu-id="317a1-201">If no specific rules or limits apply to the transaction, the All transactions rule applies.</span></span> <span data-ttu-id="317a1-202">Барлық транзакция ережелері барлық транзакцияға сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-202">The All transactions rule matches all transactions.</span></span> 

<span data-ttu-id="317a1-203">Егер транзакцияға сәйкес келетін ереже табылса, алдымен осы ережеде бөлінген пайыздық мөлшер қолданылады, бірақ сәйкестіктер орнатылған шектеулермен тексерілгеннен кейін ғана.</span><span class="sxs-lookup"><span data-stu-id="317a1-203">If a rule is found that matches a transaction, the percentage that has been allocated in that rule is applied first, but only after the matches are checked against any limits that have been set up.</span></span> <span data-ttu-id="317a1-204">Егер шектеу орындалса және қаржыландыру көзінің қаражаты таусылса, қаржыландыру шектеуімен байланысты қаржыландыру ережесі ескерілмейді және бағдарлама келесі қолданылатын ережені тексереді.</span><span class="sxs-lookup"><span data-stu-id="317a1-204">If a limit has been met, and a funding source’s funds are exhausted, the funding rule that is associated with the funding limit is disregarded, and the program checks for the next rule that applies.</span></span> 

<span data-ttu-id="317a1-205">Кейбір жағдайларда транзакцияның тек бір бөлігін ережеге сәйкес бөлуге болады.</span><span class="sxs-lookup"><span data-stu-id="317a1-205">In some cases, only part of a transaction can be allocated under a rule.</span></span> <span data-ttu-id="317a1-206">Бұл транзакция бөлінген кезде шегіне жету үшін орын алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="317a1-206">This might happen because a limit is reached when the transaction is allocated.</span></span> <span data-ttu-id="317a1-207">Бұл жағдайда сол ережеге сәйкес белгілі бір сома ғана бөлінеді, мысалы әр қаржыландыру көзіне 50 пайыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-207">In this case, only a certain amount is allocated according to that rule, such as 50 percent to each funding source.</span></span> <span data-ttu-id="317a1-208">Бұл осы бөлімде бұрын сипатталған 1-ережеге қатысты.</span><span class="sxs-lookup"><span data-stu-id="317a1-208">This is the case in rule 1, which is described earlier in this section.</span></span> <span data-ttu-id="317a1-209">Қалған бөлігі кезектегі келесі ережеге сәйкес бөлінеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-209">The remainder is allocated according to the next rule in the sequence.</span></span> 

<span data-ttu-id="317a1-210">Келесі кестеде осы сценарий толығырақ қарастырылған.</span><span class="sxs-lookup"><span data-stu-id="317a1-210">The following table examines this scenario in more detail.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="317a1-211"><strong>Фокус</strong></span><span class="sxs-lookup"><span data-stu-id="317a1-211"><strong>Focus</strong></span></span></td>
<td><span data-ttu-id="317a1-212"><strong>Мәліметтер</strong></span><span class="sxs-lookup"><span data-stu-id="317a1-212"><strong>Details</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="317a1-213">Қаржыландыру ережелері</span><span class="sxs-lookup"><span data-stu-id="317a1-213">Funding rules</span></span></td>
<td><ul>
<li><span data-ttu-id="317a1-214">1-ереже (1-басымдық): Барлық транзакция.</span><span class="sxs-lookup"><span data-stu-id="317a1-214">Rule 1 (Priority 1): All transactions.</span></span> <span data-ttu-id="317a1-215">2-қаржыландыру көзін 50%-ға және 3-қаржыландыру көзін 50%-ға бөліңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-215">Allocate funding source 2 at 50% and funding source 3 at 50%.</span></span></li>
<li><span data-ttu-id="317a1-216">2-ереже (2-басымдық): Барлық транзакция.</span><span class="sxs-lookup"><span data-stu-id="317a1-216">Rule 2 (Priority 2): All transactions.</span></span> <span data-ttu-id="317a1-217">3-қаржыландыру көзін 100%-ға бөліңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-217">Allocate funding source 3 at 100%.</span></span></li>
<li><span data-ttu-id="317a1-218">3-ереже (2-басымдық): Барлық транзакция.</span><span class="sxs-lookup"><span data-stu-id="317a1-218">Rule 3 (Priority 2): All transactions.</span></span> <span data-ttu-id="317a1-219">1-қаржыландыру көзін 100%-ға бөліңіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-219">Allocate funding source 1 at 100%.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="317a1-220">Қаржыландыру шектеулері</span><span class="sxs-lookup"><span data-stu-id="317a1-220">Funding limits</span></span></td>
<td><ul>
<li><span data-ttu-id="317a1-221">1-қаржыландыру көзінің шегі = 10000,00</span><span class="sxs-lookup"><span data-stu-id="317a1-221">Funding source 1 limit = 10,000.00</span></span></li>
<li><span data-ttu-id="317a1-222">2-қаржыландыру көзінің шегі = 500,00</span><span class="sxs-lookup"><span data-stu-id="317a1-222">Funding source 2 limit = 500.00</span></span></li>
<li><span data-ttu-id="317a1-223">3-қаржыландыру көзінің шегі = 750,00</span><span class="sxs-lookup"><span data-stu-id="317a1-223">Funding source 3 limit = 750.00</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="317a1-224">Транзакция 1</span><span class="sxs-lookup"><span data-stu-id="317a1-224">Transaction 1</span></span></td>
<td><span data-ttu-id="317a1-225"><strong>Транзакция сомасы:</strong> 100,00 <strong>Қаржыландыру:</strong> Транзакция тек 1-ережеге сәйкес төленеді, себебі 1-ереже қолданылғаннан кейін транзакция толық төленеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-225"><strong>Transaction amount:</strong> 100.00<strong>Funding:</strong> The transaction is paid according to rule 1 only, because the transaction is fully paid after rule 1 is applied.</span></span> <span data-ttu-id="317a1-226">Транзакция 2-қаржыландыру көзі мен 3-қаржыландыру көзі арасында тең мөлшерде қаржыландырылады.</span><span class="sxs-lookup"><span data-stu-id="317a1-226">The transaction is funded equally between funding source 2 and funding source 3.</span></span>
<ul>
<li><span data-ttu-id="317a1-227">2-қаржыландыру көзі: 50,00</span><span class="sxs-lookup"><span data-stu-id="317a1-227">Funding source 2: 50.00</span></span></li>
<li><span data-ttu-id="317a1-228">3-қаржыландыру көзі: 50,00</span><span class="sxs-lookup"><span data-stu-id="317a1-228">Funding source 3: 50.00</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="317a1-229">Транзакция 2</span><span class="sxs-lookup"><span data-stu-id="317a1-229">Transaction 2</span></span></td>
<td><span data-ttu-id="317a1-230"><strong>Транзакция сомасы:</strong> 5000,00 <strong>Қаржыландыру:</strong> Транзакция барлық үш ережеге сәйкес төленеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-230"><strong>Transaction amount:</strong> 5,000.00<strong>Funding:</strong> The transaction is paid according to all three rules.</span></span> <span data-ttu-id="317a1-231"><strong>1-ереже</strong>
</span><span class="sxs-lookup"><span data-stu-id="317a1-231"><strong>Rule 1</strong>
</span></span><ul>
<li><span data-ttu-id="317a1-232">2-қаржыландыру көзі: 450,00</span><span class="sxs-lookup"><span data-stu-id="317a1-232">Funding source 2: 450.00</span></span></li>
<li><span data-ttu-id="317a1-233">3-қаржыландыру көзі: 450,00</span><span class="sxs-lookup"><span data-stu-id="317a1-233">Funding source 3: 450.00</span></span></li>
</ul><span data-ttu-id="317a1-234">
<strong>2-ереже</strong>
</span><span class="sxs-lookup"><span data-stu-id="317a1-234">
<strong>Rule 2</strong>
</span></span><ul>
<li><span data-ttu-id="317a1-235">3-қаржыландыру көзі: 250,00 (= 750,00 – 50,00 – 450,00)</span><span class="sxs-lookup"><span data-stu-id="317a1-235">Funding source 3: 250.00 (= 750.00 – 50.00 – 450.00)</span></span></li>
</ul><span data-ttu-id="317a1-236">
<strong>3-ереже</strong>
</span><span class="sxs-lookup"><span data-stu-id="317a1-236">
<strong>Rule 3</strong>
</span></span><ul>
<li><span data-ttu-id="317a1-237">1-қаржыландыру көзі: 3850,00 (= 5000,00 – 450,00 – 450,00 – 250,00)</span><span class="sxs-lookup"><span data-stu-id="317a1-237">Funding source 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="317a1-238">Әр қаржыландыру көзі бойынша бөлінген қаражаттың жалпы мөлшері</span><span class="sxs-lookup"><span data-stu-id="317a1-238">Total funds that are distributed for each funding source</span></span></td>
<td><ul>
<li><span data-ttu-id="317a1-239">1-қаржыландыру көзі: 3850,00</span><span class="sxs-lookup"><span data-stu-id="317a1-239">Funding source 1: 3,850.00</span></span></li>
<li><span data-ttu-id="317a1-240">2-қаржыландыру көзі: 500,00</span><span class="sxs-lookup"><span data-stu-id="317a1-240">Funding source 2: 500.00</span></span></li>
<li><span data-ttu-id="317a1-241">3-қаржыландыру көзі: 750,00</span><span class="sxs-lookup"><span data-stu-id="317a1-241">Funding source 3: 750.00</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a><span data-ttu-id="317a1-242">Төлем ережелері</span><span class="sxs-lookup"><span data-stu-id="317a1-242">Billing rules</span></span>
<span data-ttu-id="317a1-243">Тұтынушымен жоба келісім-шартын жасасқанда, сіз тұтынушыға жоба бойынша жұмыс жасау үшін есеп-шотты қалай және қашан ұсына алатыныңызды анықтайсыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-243">When you negotiate a project contract with a customer, you define how and when you can invoice the customer for work on a project.</span></span> <span data-ttu-id="317a1-244">Жоба келісім-шартын және жобаны орнатқаннан кейін, сіз жоба үшін төлем ережелерін орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-244">After you set up the project contract and the project, you can set up billing rules for the project.</span></span> <span data-ttu-id="317a1-245">Төлем ережелері жоба келісім-шартында көрсетілген жоба шарттарына негізделген.</span><span class="sxs-lookup"><span data-stu-id="317a1-245">Billing rules are based on the project terms that are specified in the project contract.</span></span> <span data-ttu-id="317a1-246">Жасаға болатын төлем ережелері жоба келісім-шартының талаптарына және уақыт пен материал немесе төлем ережесімен байланыстыратын белгіленген баға сияқты жобаның түріне байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="317a1-246">The billing rules that you can create depend on the terms of the project contract and the project type, such as Time and material or Fixed-price, that you associate with the billing rule.</span></span> <span data-ttu-id="317a1-247">Жоба келісім-шарты үшін бірнеше төлем ережелерін жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-247">You can create more than one billing rule for a project contract.</span></span> <span data-ttu-id="317a1-248">Сондай-ақ төлем ережесін бір жоба келісім-шартымен байланысты және төлем шарттары ұқсас бірнеше жобаларға тағайындай аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-248">You can also assign a billing rule to multiple projects that are associated with the same project contract and have similar billing terms.</span></span> 

<span data-ttu-id="317a1-249">Сіз төлем ережелерінің келесі түрлерін орната аласыз:</span><span class="sxs-lookup"><span data-stu-id="317a1-249">You can set up the following types of billing rules:</span></span>

-   <span data-ttu-id="317a1-250">**Жеткізу бірлігі** – Жеткізу бірлігін аяқтаған кезде тұтынушыға есеп-шот ұсыныңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-250">**Unit of delivery** – Invoice a customer when you complete a unit of delivery.</span></span> <span data-ttu-id="317a1-251">Келісім-шартта жеткізу бірліктерін анықтайсыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-251">You define the units of delivery in the contract.</span></span>
-   <span data-ttu-id="317a1-252">**Орындалу барысы** – жобаның белгіленген пайызын аяқтаған кезде тұтынушыға есеп-шот ұсыныңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-252">**Progress** – Invoice a customer when you complete a specified percentage of the project.</span></span> <span data-ttu-id="317a1-253">Аяқталған жұмыс пайызын автоматты түрде есептеу үшін төлем ережесін орната аласыз немесе аяқталған жұмыс пайызын және тұтынушыға есеп-шот ұсынуға болатын соманы қолмен есептей аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-253">You can set up a billing rule to automatically calculate the percentage of work completed, or you can manually calculate the percentage of work completed and the amount to invoice the customer.</span></span>
-   <span data-ttu-id="317a1-254">**Кезең** – кезеңге жеткен кезде тұтынушыға жоба кезеңінің толық сомасына есеп-шот ұсыныңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-254">**Milestone** – Invoice a customer for the full amount of a project milestone when the milestone is reached.</span></span>
-   <span data-ttu-id="317a1-255">**Ақы** – қызметтеріңіз үшін, сонымен қатар әдетте қызметтер құнының пайызын құрайтын басқару ақысы үшін тұтынушыға есеп-шот ұсыныңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-255">**Fee** – Invoice a customer for your services plus a management fee, which is typically a percentage of the cost of services.</span></span>
-   <span data-ttu-id="317a1-256">**Уақыт және материал** – жобада пайдаланылатын уақыт пен материалдар құны үшін тұтынушыға есеп-шот ұсыныңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-256">**Time and material** – Invoice a customer for the value of time and materials that are used on a project.</span></span>

<span data-ttu-id="317a1-257">Төлем ережелерінің барлық түрлері үшін тұтынушы есеп-шоттарынан жоба келісілген кезеңге жеткенге дейін сақтау пайызын көрсете аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-257">For all types of billing rules, you can specify a retention percentage that is deducted from customer invoices until a project reaches an agreed-upon stage.</span></span> <span data-ttu-id="317a1-258">Төлемді сақтау пайызы жобаның келісім-шартында көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="317a1-258">The payment retention percentage is specified in the project contract.</span></span> <span data-ttu-id="317a1-259">Бұл сома тұтынушы есеп-шотындағы жолдардың жалпы мәніне сүйене отырып есептеледі.</span><span class="sxs-lookup"><span data-stu-id="317a1-259">The amount is calculated based on, and subtracted from, the total value of the lines in a customer invoice.</span></span> 

<span data-ttu-id="317a1-260">**Уақыт және материал** және **Орындалу барысы** төлем ережелері үшін ақылы санаттар тағайындай аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-260">For **Time and material** and **Progress** billing rules, you can assign chargeable categories.</span></span> <span data-ttu-id="317a1-261">Ақылы санаттар тұтынушы есеп-шотына енуі керек транзакцияларды көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="317a1-261">Chargeable categories indicate the transactions that should be included in customer invoices.</span></span> 

<span data-ttu-id="317a1-262">Тұтынушыға есеп-шот ұсынуға дайын болған кезде, жобаның есеп-шот сомасы төлем ережелері негізінде есептеледі және жоба бойынша есеп-шот ұсынысы жасалады.</span><span class="sxs-lookup"><span data-stu-id="317a1-262">When you are ready to invoice the customer, the amount to invoice for the project is calculated based on the billing rules, and a project invoice proposal is generated.</span></span> 

<span data-ttu-id="317a1-263">Келесі бөлімдерде жобаның төлем ережелерін орнату және басқару жолдары көрсетілген мысалдар келтірілген.</span><span class="sxs-lookup"><span data-stu-id="317a1-263">The following sections provide examples that show how to set up and manage billing rules for a project.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a><span data-ttu-id="317a1-264">Мысалы: жеткізілген бірліктер санына негізделген төлем ережесін жасау</span><span class="sxs-lookup"><span data-stu-id="317a1-264">Example: Create a billing rule that is based on the number of units delivered</span></span>

<span data-ttu-id="317a1-265">Ұйымыңыз тұтынушының қызметкерлеріне бір оқыту сеансы 10000 тұратын жалпы бес оқыту сеансын беру туралы келісімге отырады.</span><span class="sxs-lookup"><span data-stu-id="317a1-265">Your organization enters into an agreement to provide a total of five training sessions to a customer’s employees at a cost of 10,000 per training session.</span></span> <span data-ttu-id="317a1-266">Әр оқыту сеансынан кейін тұтынушыға есеп-шот ұсынасыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-266">You invoice the customer after each training session.</span></span> 

<span data-ttu-id="317a1-267">Келісім-шарт бойынша төлем ережелерін орнатқан кезде, келесі мәндерді қолданасыз:</span><span class="sxs-lookup"><span data-stu-id="317a1-267">When you set up the billing rules for the contract, you use the following values:</span></span>

-   <span data-ttu-id="317a1-268">Жеткізу бірлігі – бір оқыту сеансы.</span><span class="sxs-lookup"><span data-stu-id="317a1-268">The unit of delivery is one training session.</span></span>
-   <span data-ttu-id="317a1-269">Бірліктің бағасы – әр оқыту сеансы үшін 10000.</span><span class="sxs-lookup"><span data-stu-id="317a1-269">The unit price is 10,000 per training session.</span></span>
-   <span data-ttu-id="317a1-270">Бірліктердің жалпы саны бес оқыту сеансын құрайды.</span><span class="sxs-lookup"><span data-stu-id="317a1-270">The total number of units is five training sessions.</span></span>

<span data-ttu-id="317a1-271">Бір оқыту сеансын аяқтағаннан кейін, жеткізілген бірінші бірлік үшін 10000 сомаға есеп-шот жасап, оны тұтынушыға жібере аласыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-271">When you have completed one training session, you can create an invoice for 10,000, for the first unit that was delivered, and send the invoice to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a><span data-ttu-id="317a1-272">Мысалы: жобаның аяқталған пайызына негізделген төлем ережесін жасау (қолмен есептеу)</span><span class="sxs-lookup"><span data-stu-id="317a1-272">Example: Create a billing rule that is based on a specified percentage of project completion (manual calculation)</span></span>

<span data-ttu-id="317a1-273">Ұйымыңыз, бағдарламалық жасақтама бойынша кеңес беруші ұйым, тұтынушы әзірлейтін өнімнің бір бөлігін әзірлеу туралы тұтынушымен келісімге отырады.</span><span class="sxs-lookup"><span data-stu-id="317a1-273">Your organization, a software consulting firm, enters into an agreement with a customer to develop part of a product that the customer is developing.</span></span> <span data-ttu-id="317a1-274">Ұйымыңыз бағдарламалық жасақтама кодын алты ай ішінде жеткізуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-274">Your organization agrees to deliver the software code over a period of six months.</span></span> <span data-ttu-id="317a1-275">Тұтынушы ұйымыңызға жұмыс үшін жалпы 100000 төлеуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-275">The customer agrees to pay your organization a total of 100,000 for the work.</span></span> <span data-ttu-id="317a1-276">Келісім-шартта көрсетілгендей, жобада аяқталған жұмыс пайызы негізінде тұтынушыға есеп-шот ұсыну үшін төлем ережесін жасайсыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-276">You create a billing rule to invoice the customer based on the percentage of work that is completed on the project, as specified in the contract.</span></span>

-   <span data-ttu-id="317a1-277">Бірінші айдың соңында, аяқталған жұмыс пайызын анықтау үшін тұтынушымен кездесесіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-277">At the end of the first month, you meet with the customer to determine the percentage of work completed.</span></span> <span data-ttu-id="317a1-278">Тұтынушымен бірге жобаны қарап шыққаннан кейін, жобаның 15 пайызы аяқталды деп шешесіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-278">After you and the customer review the project, you decide that the project is 15 percent completed.</span></span>
-   <span data-ttu-id="317a1-279">15000 (100000-ның 15 пайызы) сомаға есеп-шот жасап, оны тұтынушыға жібересіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-279">You create an invoice for 15,000 (15 percent of 100,000) and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a><span data-ttu-id="317a1-280">Мысалы: жобаның аяқталған пайызына негізделген төлем ережесін жасау (автоматты есептеу)</span><span class="sxs-lookup"><span data-stu-id="317a1-280">Example: Create a billing rule that is based on a specified percentage of project completion (automatic calculation)</span></span>

<span data-ttu-id="317a1-281">Ұйымыңыз, бағдарламалық жасақтама әзірлеуші ұйым, тұтынушының 30000 сома үшін ақы төлеуді есепке алу пакетін жасауға келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-281">Your organization, a software development firm, agrees to develop a payroll accounting package for a customer for 30,000.</span></span> <span data-ttu-id="317a1-282">Тұтынушы ұйымыңызға аяқталған жұмыс пайызы негізінде төлеуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-282">The customer agrees to pay your organization based on the percentage of work completed.</span></span> <span data-ttu-id="317a1-283">Жобаның құны 20000 құрайды деп есептейсіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-283">You estimate that the project costs are 20,000.</span></span> <span data-ttu-id="317a1-284">Жоба келісім-шартында төлем процесінде пайдаланатын жұмыс санаттары көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="317a1-284">The project contract specifies the categories of work that you use in the billing process.</span></span> <span data-ttu-id="317a1-285">Әр санат үшін аяқталған жұмыс пайызына есеп-шот сомаларын автоматты түрде есептейтін төлем ережелерін орнаттыңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-285">You set up billing rules that automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="317a1-286">Сіз әр санат үшін бюджет орнатасыз:</span><span class="sxs-lookup"><span data-stu-id="317a1-286">You set up a budget for each category:</span></span>

-   <span data-ttu-id="317a1-287">**Әзірлеу** – құны 15000 және кірісі 20000</span><span class="sxs-lookup"><span data-stu-id="317a1-287">**Development** – Cost of 15,000 and revenue of 20,000</span></span>
-   <span data-ttu-id="317a1-288">**Орнату** – құны 5000 және кірісі 10000</span><span class="sxs-lookup"><span data-stu-id="317a1-288">**Installation** – Cost of 5,000 and revenue of 10,000</span></span>

<span data-ttu-id="317a1-289">Тұтынушы есеп-шотын бірінші рет жасаған кезде есеп-шот сомасы келесі ақпарат негізінде автоматты түрде есептеледі:</span><span class="sxs-lookup"><span data-stu-id="317a1-289">When you create a customer invoice for the first time, the invoice amount is automatically calculated based on the following information:</span></span>

-   <span data-ttu-id="317a1-290">Бір айдан кейін жобадағы қызметкер жұмыс кестесін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="317a1-290">After a month, the worker on the project submits a timesheet for the project.</span></span> <span data-ttu-id="317a1-291">Қызметкер сағаттарының құны әзірлеу үшін 5000, орнату жұмыстары үшін 1000 құрайды.</span><span class="sxs-lookup"><span data-stu-id="317a1-291">The cost of the worker’s hours is 5,000 for development and 1,000 for installation.</span></span> <span data-ttu-id="317a1-292">Әзірлеу жұмысының 33 пайызы аяқталды (5000 нақты шығын/15000 бюджеттік шығын), ал орнату жұмыстарының 20 пайызы аяқталды (1000 нақты шығын/5000 бюджеттік шығын).</span><span class="sxs-lookup"><span data-stu-id="317a1-292">The development work is 33 percent completed (5,000 actual cost/15,000 budget cost), and the installation work is 20 percent completed (1,000 actual cost/5,000 budget cost).</span></span>
-   <span data-ttu-id="317a1-293">8667 есеп-шот сомасы автоматты түрде есептеледі (20000-ның 33 пайызы + 10000-ның 20 пайызы).</span><span class="sxs-lookup"><span data-stu-id="317a1-293">The invoice amount of 8,667 is automatically calculated (33 percent of 20,000 + 20 percent of 10,000).</span></span>
-   <span data-ttu-id="317a1-294">8667 сомаға есеп-шот жасап, оны тұтынушыға жібересіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-294">You create an invoice for 8,667 and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a><span data-ttu-id="317a1-295">Мысалы: келісілген кезеңдерге негізделген төлем ережесін жасау</span><span class="sxs-lookup"><span data-stu-id="317a1-295">Example: Create a billing rule that is based on agreed-upon milestones</span></span>

<span data-ttu-id="317a1-296">Ұйымыңыз, басқарушылық бойынша кеңес беруші ұйым, тұтынушы сатуды жоспарлап отырған тұтыну өнімі үшін нарықтық зерттеулер жүргізуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-296">Your organization, a management consulting firm, agrees to conduct market research for a consumer product that the customer plans to sell.</span></span> <span data-ttu-id="317a1-297">Тұтынушы сіздің қызметтеріңізді наурыз айынан бастап үш ай бойы пайдалануға және ұйымыңызға 50000 төлеуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-297">The customer agrees to use your services for a period of three months, starting in March, and agrees to pay your organization 50,000.</span></span> <span data-ttu-id="317a1-298">Жоба үш кезеңнен тұрады:</span><span class="sxs-lookup"><span data-stu-id="317a1-298">The project has three milestones:</span></span>

-   <span data-ttu-id="317a1-299">1 кезең: тұтынушы деректерін жинау – 31 наурыз</span><span class="sxs-lookup"><span data-stu-id="317a1-299">Milestone 1: Collect consumer data – March 31</span></span>
-   <span data-ttu-id="317a1-300">2 кезең: тұтынушы деректерін талдау – 30 сәуір</span><span class="sxs-lookup"><span data-stu-id="317a1-300">Milestone 2: Analyze consumer data – April 30</span></span>
-   <span data-ttu-id="317a1-301">3 кезең: өнімнің жарамдылық мерзімі туралы ұсыныс жасау - 31 мамыр</span><span class="sxs-lookup"><span data-stu-id="317a1-301">Milestone 3: Present a product viability proposal – May 31</span></span>

<span data-ttu-id="317a1-302">Тұтынушы ұйымыңызға бірінші кезең үшін 10000, екінші кезең үшін 20000, үшінші кезең үшін 20000 төлеуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-302">The customer agrees to pay your organization 10,000 for the first milestone, 20,000 for the second milestone, and 20,000 for the third milestone.</span></span> 

<span data-ttu-id="317a1-303">Жоба келісім-шартын жасаған кезде, тұтынушымен аяқталған кезең негізінде есеп айырысуға келісесіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-303">When you set up the project contract, you agree to bill the customer based on the milestone that has been completed.</span></span> <span data-ttu-id="317a1-304">Төлем ережесін орнату келесі қадамдарды қамтиды:</span><span class="sxs-lookup"><span data-stu-id="317a1-304">The billing rule setup includes the following steps:</span></span>

-   <span data-ttu-id="317a1-305">Жоба кезеңдерін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-305">Define the project milestones.</span></span>
-   <span data-ttu-id="317a1-306">Әр кезең аяқталған кезде тұтынушыға ұсынылатын есеп-шот сомасын анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-306">Define the amount to invoice the customer when each milestone is completed.</span></span>

<span data-ttu-id="317a1-307">31 наурызда бірінші кезең аяқталған кезде, кезең аяқталды деп белгілейсіз, содан кейін 10000 сомаға есеп-шот жасап, оны тұтынушыға жібересіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-307">When the first milestone is completed on March 31, you mark the milestone as completed, and then create an invoice for 10,000 and send it to the customer.</span></span> <span data-ttu-id="317a1-308">Кезең аяқталған деп белгілемейінше, есеп-шот жасау мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="317a1-308">You can’t create an invoice for a milestone until you have marked the milestone as completed.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a><span data-ttu-id="317a1-309">Мысалы: қызметтер мен басқару ақысына негізделген төлем ережесін жасау</span><span class="sxs-lookup"><span data-stu-id="317a1-309">Example: Create a billing rule that is based on services plus a management fee</span></span>

<span data-ttu-id="317a1-310">Ұйымыңыз, басқарушылық бойынша кеңес беруші ұйым, тұтынушы, бөлшек сауда компаниясы әзірлейтін өнімнің жарамдылық мерзімін бағалау үшін нарықтық зерттеулер жүргізуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-310">Your organization, a management consulting firm, agrees to conduct market research to evaluate the viability of a product that the customer, a retail company, is developing.</span></span> <span data-ttu-id="317a1-311">Келісім шарттарында зерттеуді уақытылы және материалды негізде жүргізетін үш басқарушылық кеңесші қызметтерін көрсететіндігіңіз көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="317a1-311">The terms of the agreement specify that you will provide the services of your top three management consultants, who will conduct the research on a time-and-materials basis.</span></span> <span data-ttu-id="317a1-312">Тұтынушы сағатына 100 төлеуге келіседі, сонымен бірге жобаға есептелген кеңес беру сағаттары үшін 10 пайыздық басқару ақысын төлейді.</span><span class="sxs-lookup"><span data-stu-id="317a1-312">The customer agrees to pay 100 per hour, plus a 10 percent management fee for the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="317a1-313">Жоба келісім-шартын жасаған кезде, жоба үшін есептелген кеңес беру сағаттарына 10 пайыздық басқару ақысын қосу үшін төлем ережесін жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-313">When you set up the project contract, create a billing rule to add a 10 percent management fee to the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="317a1-314">Тұтынушыға есеп-шот жасаған кезде, тұтынушыдан 10 пайыздық басқару ақысы және кеңес беру сағатының құны алынады.</span><span class="sxs-lookup"><span data-stu-id="317a1-314">When you create an invoice for the customer, the customer is billed a 10 percent management fee plus the cost of the consulting hours.</span></span> <span data-ttu-id="317a1-315">Мысалы, егер үш кеңесші жобада жалпы 200 сағат жұмыс істеген болса, келесі есеп негізінде 22000 сомаға есеп-шот жасалады:</span><span class="sxs-lookup"><span data-stu-id="317a1-315">For example, if the three consultants worked a total of 200 hours on the project, an invoice for 22,000 is created based on the following calculation:</span></span>

-   <span data-ttu-id="317a1-316">Сағатына 100 болғанда 200 сағат = 20000</span><span class="sxs-lookup"><span data-stu-id="317a1-316">200 hours at 100 per hour = 20,000</span></span>
-   <span data-ttu-id="317a1-317">10 пайыздық басқару ақысы = 2000</span><span class="sxs-lookup"><span data-stu-id="317a1-317">10 percent management fee = 2,000</span></span>
-   <span data-ttu-id="317a1-318">Жалпы есеп-шот сомасы = 22000</span><span class="sxs-lookup"><span data-stu-id="317a1-318">Total invoice amount = 22,000</span></span>

<span data-ttu-id="317a1-319">Егер тұтынушыға салық салынатын болса және сіз жоба келісім-шартында сату салығы тобын таңдасаңыз, сатылым салығы тобы автоматты түрде ақысы үшін төлем ережесіне енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="317a1-319">If fees are taxable to a customer, and you select a sales tax group in the project contract, the sales tax group is automatically entered in a billing rule for fees.</span></span>

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a><span data-ttu-id="317a1-320">Мысалы: уақыт пен материалдардың құны үшін төлем ережесін жасау</span><span class="sxs-lookup"><span data-stu-id="317a1-320">Example: Create a billing rule for the value of time and materials</span></span>

<span data-ttu-id="317a1-321">Ұйымыңыз, бағдарламалық жасақтама бойынша кеңес беруші ұйым, келесі алты ай ішінде тұтынушыға бағдарламалық жасақтама жасау жобасында жұмыс жасау үшін бес техникалық кеңесшіні қамтамасыз етуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-321">Your organization, a software consulting firm, agrees to provide five technical consultants to work on a software development project for a customer for the next six months.</span></span> <span data-ttu-id="317a1-322">Тұтынушы әр кеңес беру сағаты үшін кеңсе керек-жарақтарының құнын қосқанда 150 төлеуге келіседі.</span><span class="sxs-lookup"><span data-stu-id="317a1-322">The customer agrees to pay 150 for each consulting hour, plus the cost of office supplies.</span></span> <span data-ttu-id="317a1-323">Ұйымыңыз әр айдың соңында тұтынушыға есеп-шот жібереді.</span><span class="sxs-lookup"><span data-stu-id="317a1-323">Your organization sends an invoice to the customer at the end of each month.</span></span> 

<span data-ttu-id="317a1-324">Жоба келісім-шартын жасаған кезде, тұтынушыға ай сайын уақыт пен жоба үшін ақы төлеуге келісесіз.</span><span class="sxs-lookup"><span data-stu-id="317a1-324">When you set up the project contract, you agree to bill the customer each month for time and materials on the project.</span></span> <span data-ttu-id="317a1-325">Келесі ақпаратты қамтитын төлем ережесін жасайсыз:</span><span class="sxs-lookup"><span data-stu-id="317a1-325">You create a billing rule that includes the following information:</span></span>

-   <span data-ttu-id="317a1-326">Келісім-шарт мерзімі – алты ай.</span><span class="sxs-lookup"><span data-stu-id="317a1-326">The contract period is six months.</span></span>
-   <span data-ttu-id="317a1-327">Кеңес беру уақыты сағатына 150 жылдамдықпен есептеледі.</span><span class="sxs-lookup"><span data-stu-id="317a1-327">Consulting time is calculated at a rate of 150 per hour.</span></span>
-   <span data-ttu-id="317a1-328">Кеңсе керек-жарақтары өзіндік құны бойынша есеп-шотпен жазылады, ал жобаның жалпы құны 10000-нан аспауы керек.</span><span class="sxs-lookup"><span data-stu-id="317a1-328">Office supplies are invoiced at cost, and the total cost for the project must not exceed 10,000.</span></span>
-   <span data-ttu-id="317a1-329">Сіз жоба барысында әр күнтізбелік айдың соңында тұтынушыға есеп-шот ұсынасыз.</span><span class="sxs-lookup"><span data-stu-id="317a1-329">You create a customer invoice at the end of each calendar month during the project.</span></span>

<span data-ttu-id="317a1-330">Бірінші айда жобадағы кеңесшілер тарапынан жалпы 800 сағат жазылады.</span><span class="sxs-lookup"><span data-stu-id="317a1-330">During the first month, a total of 800 hours are recorded by the consultants on the project.</span></span> <span data-ttu-id="317a1-331">Жоба бойынша алынатын кеңсе керек-жарақтарының құны 2000 құрайды.</span><span class="sxs-lookup"><span data-stu-id="317a1-331">The cost of office supplies that are charged to the project is 2,000.</span></span> <span data-ttu-id="317a1-332">Сондықтан, айдың соңында 122000 сомаға есеп-шот жасайсыз, ол сағатына 150 болғанда 800 сағат деп есептеледі және кеңсе керек-жарақтары үшін 2000 қосылады.</span><span class="sxs-lookup"><span data-stu-id="317a1-332">Therefore, at the end of the month, you create an invoice for 122,000, which is calculated as 800 hours at 150 per hour, plus 2,000 for office supplies.</span></span>





[!INCLUDE[footer-include](../includes/footer-banner.md)]