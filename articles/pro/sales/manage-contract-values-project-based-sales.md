---
title: Жобаға негізделген келісім-шарт жолдарына шолу
description: Бұл тақырыпта жобаға негізделген келісім-шарт жолдарымен жұмыс істеу туралы ақпарат берілген.
author: rumant
ms.date: 10/28/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8af32b0475650db9c5862ea23d185588a631ade6
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003143"
---
# <a name="project-based-contract-lines-overview"></a><span data-ttu-id="66ab5-103">Жобаға негізделген келісім-шарт жолдарына шолу</span><span class="sxs-lookup"><span data-stu-id="66ab5-103">Project-based contract lines overview</span></span>

<span data-ttu-id="66ab5-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="66ab5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="66ab5-105">Dynamics 365 Project Operations бағдарламасындағы жобаға негізделген келісім-шарт жолдары келісім бойынша жоба жұмысының нақты құрамдастары үшін болжам және төлем келісімдерін сақтауға арналған.</span><span class="sxs-lookup"><span data-stu-id="66ab5-105">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="66ab5-106">Жобаға негізделген келісім-шарт жолының құрылымы жобаның болжам және төлем сценарийлері үшін келесі тұжырымдамалармен кеңейтілген:</span><span class="sxs-lookup"><span data-stu-id="66ab5-106">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="66ab5-107">Төлем әдісі</span><span class="sxs-lookup"><span data-stu-id="66ab5-107">Billing method</span></span>
- <span data-ttu-id="66ab5-108">Жоба мен тапсырманы салыстыру</span><span class="sxs-lookup"><span data-stu-id="66ab5-108">Project and task mapping</span></span>
- <span data-ttu-id="66ab5-109">Қамтылған транзакция кластары</span><span class="sxs-lookup"><span data-stu-id="66ab5-109">Included transaction classes</span></span>
- <span data-ttu-id="66ab5-110">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="66ab5-110">Not-to-exceed limit</span></span>
- <span data-ttu-id="66ab5-111">Төлем қабілеттілігін орнату</span><span class="sxs-lookup"><span data-stu-id="66ab5-111">Chargeability setup</span></span>
- <span data-ttu-id="66ab5-112">Келісім-шарт жолдары туралы мәліметтерді пайдаланатын болжамдар</span><span class="sxs-lookup"><span data-stu-id="66ab5-112">Estimates using contract line details</span></span>
- <span data-ttu-id="66ab5-113">Келісім-шарт жолы тұтынушылары</span><span class="sxs-lookup"><span data-stu-id="66ab5-113">Contract line customers</span></span>

<span data-ttu-id="66ab5-114">Келесі кестеде жобаға негізделген жұмыстардың толық, негізгі болжам және төлем реттеулері үшін негізді орнатуға көмектесетін жобаға негізделген келісім-шарт жолдарының **Жалпы мәліметтер** қойыншасындағы өрістер қамтылған.</span><span class="sxs-lookup"><span data-stu-id="66ab5-114">The following table includes the fields on the **General** tab of project–based contract lines that help set up the basis for a detailed, ground–up estimate and billing arrangements for project–based work.</span></span>

| <span data-ttu-id="66ab5-115">Өріс</span><span class="sxs-lookup"><span data-stu-id="66ab5-115">Field</span></span> | <span data-ttu-id="66ab5-116">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="66ab5-116">Description</span></span> | <span data-ttu-id="66ab5-117">Төменгі әсер</span><span class="sxs-lookup"><span data-stu-id="66ab5-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="66ab5-118">**Атауы**</span><span class="sxs-lookup"><span data-stu-id="66ab5-118">**Name**</span></span> | <span data-ttu-id="66ab5-119">Келісім-шарт жолының атауы.</span><span class="sxs-lookup"><span data-stu-id="66ab5-119">Name of the contract line.</span></span> <span data-ttu-id="66ab5-120">Бұл бағаланатын келісім-шарттың дискретті құрамдасын анықтайды.</span><span class="sxs-lookup"><span data-stu-id="66ab5-120">This identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="66ab5-121">Баға ұсынудан жасалған жоба келісім-шарты үшін бұл мән жобаға негізделген баға ұсыну жолының сәйкес мәнінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="66ab5-121">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="66ab5-122">Атауы есеп-шот жасалған кезде осы келісім-шарт жолынан жасалған жоба есеп-шоты жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="66ab5-122">The name copied over to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="66ab5-123">**Есепшот ұсыну әдісі**</span><span class="sxs-lookup"><span data-stu-id="66ab5-123">**Billing Method**</span></span> | <span data-ttu-id="66ab5-124">Баға ұсынудан жасалған жоба келісім-шартында бұл мән баға ұсыну жолындағы сәйкес өрістен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="66ab5-124">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="66ab5-125">Бұл Project Operations қолдайтын екі негізгі келісім-шарттық үлгілерді ұсынатын параметрлер жиыны:</span><span class="sxs-lookup"><span data-stu-id="66ab5-125">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="66ab5-126">- **Бекітілген баға**</span><span class="sxs-lookup"><span data-stu-id="66ab5-126">- **Fixed Price**</span></span></br><span data-ttu-id="66ab5-127">- **Уақыт және материал**</span><span class="sxs-lookup"><span data-stu-id="66ab5-127">- **Time and Material**</span></span> | <span data-ttu-id="66ab5-128">Сілтеме жасалған келісім-шарт жолының төлем әдісі негізінде нақты транзакция өңделеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-128">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="66ab5-129">Егер нақты мән арқылы сілтеме жасалған келісім-шарт жолында уақыт пен материалдық есеп-шот ұсыну әдісі болса, құн мен төлем жасалмаған сатылымның нақты жазбалары жасалады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-129">If the contract line referenced by the actual has a time and material billing method, cost and unbilled sales actual records are created.</span></span> <span data-ttu-id="66ab5-130">Егер нақты мән арқылы сілтеме жасалған келісім-шарт жолында белгіленген баға бойынша есеп-шот ұсыну әдісі болса, тек нақты өзіндік құн жасалады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-130">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="66ab5-131">**Project**</span><span class="sxs-lookup"><span data-stu-id="66ab5-131">**Project**</span></span> | <span data-ttu-id="66ab5-132">Бұл өрісті осы келісім бойынша жұмысты орындау үшін пайдаланылатын жобаны анықтау үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="66ab5-132">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="66ab5-133">Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жазбаны бағалау үшін **Қосылған тапсырмалар** және **Қосылған транзакциялар санаттары** опцияларымен бірге пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-133">This value will be used in conjunction with **Included Tasks** and **Included Transaction Classes** to resolve the contract line reference on an actual or estimate line record.</span></span> |
| <span data-ttu-id="66ab5-134">**Қосылған тапсырмалар**</span><span class="sxs-lookup"><span data-stu-id="66ab5-134">**Included Tasks**</span></span> | <span data-ttu-id="66ab5-135">Осы келісім-шарт жолына таңдалған жоба бойынша барлық жоба тапсырмалары немесе тапсырмалар жиыны ғана қосылғанын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-135">Indicates if this contract line includes all project tasks for the selected project or only a subset of the tasks.</span></span> <span data-ttu-id="66ab5-136">Бұл келесі мүмкін мәндерге ие параметрлер жиыны болып табылады:</span><span class="sxs-lookup"><span data-stu-id="66ab5-136">This is an option set that has the following possible values:</span></span></br><span data-ttu-id="66ab5-137">- **Барлық жоба тапсырмалары**</span><span class="sxs-lookup"><span data-stu-id="66ab5-137">- **All Project Tasks**</span></span></br><span data-ttu-id="66ab5-138">- **Тек таңдалған жоба тапсырмалары**.</span><span class="sxs-lookup"><span data-stu-id="66ab5-138">- **Selected Project Tasks Only**.</span></span> <span data-ttu-id="66ab5-139">Бұл өрістегі бос мән **Барлық жоба тапсырмалары** таңдауына тең.</span><span class="sxs-lookup"><span data-stu-id="66ab5-139">A blank value in this field is equal to selecting **All Project Tasks**.</span></span> | <span data-ttu-id="66ab5-140">Егер **Тек таңдалған тапсырмалар** таңдалған болса, сіз нақты тапсырмаларды таңдап, оларды **Жоба** бетіндегі **Тапсырма шотын ұсынуды реттеу** қойыншасындағы келісім-шарт жолымен байланыстыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="66ab5-140">If **Selected Tasks Only** is selected, you can select specific tasks and associate them to this contract line on the **Task Billing Setup** tab on the **Project** page.</span></span> <span data-ttu-id="66ab5-141">Бұл мән келісім-шарттың нақты немесе болжамды жол жазбасына сілтеме жасау үшін **Жоба** және **Қамтылған транзакция** кластарымен бірге пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-141">The value will be used in conjunction with **Project** and **Included Transaction** classes to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="66ab5-142">**Уақытпен қоса**</span><span class="sxs-lookup"><span data-stu-id="66ab5-142">**Include Time**</span></span> | <span data-ttu-id="66ab5-143">**Иә**/**Жоқ** мәні таңдалған жобадағы уақыт транзакцияларының немесе еңбек шығындарының осы келісім-шарт жолына кіретінін не кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-143">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="66ab5-144">**Жоқ** мәні уақыт транзакциялары немесе еңбек құны осы келісім-шарт жолына қосылмайтынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-144">A **No** value indicates that the time transactions or labor cost will not be included on this contract line.</span></span> <span data-ttu-id="66ab5-145">**Иә** мәні олардың қосылатынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-145">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="66ab5-146">Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жол жазбасын бағалау үшін жобамен бірге пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-146">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="66ab5-147">**Шығыспен қоса**</span><span class="sxs-lookup"><span data-stu-id="66ab5-147">**Include Expense**</span></span> | <span data-ttu-id="66ab5-148">**Иә**/**Жоқ** мәні таңдалған жобадағы шығындардың осы келісім-шарт жолына кіретінін не кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-148">A **Yes**/**No** value indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="66ab5-149">**Жоқ** мәні шығыс құны осы келісім-шарт жолына қосылмайтынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-149">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="66ab5-150">**Иә** мәні қосылатынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-150">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="66ab5-151">Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жол жазбасын бағалау үшін жобамен бірге пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-151">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="66ab5-152">**Материалдармен қоса**</span><span class="sxs-lookup"><span data-stu-id="66ab5-152">**Include Materials**</span></span> | <span data-ttu-id="66ab5-153">**Иә**/**Жоқ** мәні таңдалған жобадағы материалдың осы келісім-шарт жолына кіретінін не кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-153">A **Yes**/**No** value indicates if material costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="66ab5-154">**Жоқ** мәні материал шығындарының осы келісім-шарт жолына кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-154">A **No** value indicates that the material costs will not be included on this contract line.</span></span> <span data-ttu-id="66ab5-155">**Иә** мәні қосылатынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-155">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="66ab5-156">Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жол жазбасын бағалау үшін жобамен бірге пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-156">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="66ab5-157">**Ақымен қоса**</span><span class="sxs-lookup"><span data-stu-id="66ab5-157">**Include Fee**</span></span> | <span data-ttu-id="66ab5-158">**Иә**/**Жоқ** мәні таңдалған жобадағы ақылардың осы келісім-шарт жолына кіретінін не кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-158">A **Yes**/**No** value indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="66ab5-159">**Жоқ** мәні ақы осы келісім-шарт жолына қосылмайтынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-159">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="66ab5-160">**Иә** мәні олардың қосылатынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-160">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="66ab5-161">Бұл мән нақты көрсеткіштегі келісім-шарт жолының анықтамасын шешу үшін немесе жол жазбасын бағалау үшін жобамен бірге пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-161">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="66ab5-162">**Келісім-шарт сомасы**</span><span class="sxs-lookup"><span data-stu-id="66ab5-162">**Contracted Amount**</span></span> | <span data-ttu-id="66ab5-163">Белгіленген баға келісім-шарты жолы бойынша, бұл сома тұтынушыға осы келісім-шарт жолымен байланысты барлық жұмыс құрамдастары үшін есеп-шот ұсынылатын келісілген мән болып табылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-163">On a fixed price contract line, this amount is the agreed-on value that will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="66ab5-164">Уақыт және материал бойынша келісім-шарт жолы бойынша, бұл сома тұтынушыға осы келісім-шарт жолымен байланысты барлық жұмыс құрамдастары үшін есеп-шот ұсынылатын болжалды мән болып табылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-164">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="66ab5-165">Баға ұсынудан жасалған жоба келісім-шарты бойынша, бұл мән баға ұсыну жолындағы сәйкес өрістен көшірілген.</span><span class="sxs-lookup"><span data-stu-id="66ab5-165">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="66ab5-166">Жобаға негізделген келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл өріс өңдеу үшін құлыпталады және келісім-шарт жолы туралы мәліметтердегі сомадан жинақталады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-166">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="66ab5-167">Келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл мәнді жол туралы мәліметтердегі сомаларды өзгерту арқылы өзгертуге болады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-167">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="66ab5-168">Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді шот ұсыну кезеңдеріне салық алдында соманы құру үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-168">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="66ab5-169">**Болжалды салық**</span><span class="sxs-lookup"><span data-stu-id="66ab5-169">**Estimated Tax**</span></span> | <span data-ttu-id="66ab5-170">Пайдаланушы бұл өрісті келісім-шарт жолына болжалды салық сомасын енгізу үшін өңдей алады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-170">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="66ab5-171">Жобаға негізделген келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл өріс өңдеу үшін құлыпталады және келісім-шарт жолы туралы мәліметтердегі салық сомасынан жинақталады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-171">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="66ab5-172">Келісім-шарт жолында жол туралы мәліметтер болған кезде, бұл мәнді жол туралы мәліметтердегі салық сомаларын өзгерту арқылы өзгертуге болады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-172">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="66ab5-173">Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді төлем жасау кезеңдеріне салық салу үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-173">On a fixed price contract line, this value is used to generate the tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="66ab5-174">**Салықтан кейінгі келісім-шарт сомасы**</span><span class="sxs-lookup"><span data-stu-id="66ab5-174">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="66ab5-175">Салықтан кейінгі келісім-шарт жолының сомасы.</span><span class="sxs-lookup"><span data-stu-id="66ab5-175">The contract line amount after tax.</span></span> <span data-ttu-id="66ab5-176">Бұл өріс тек оқуға арналған және **Келісім-шарт сомасы + салық** ретінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="66ab5-176">This field is read only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="66ab5-177">Белгіленген баға келісім-шарты жолы бойынша, бұл мән мерзімді төлем жасау кезеңдерін құру үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-177">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="66ab5-178">**Асырмау шегі**</span><span class="sxs-lookup"><span data-stu-id="66ab5-178">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="66ab5-179">Пайдаланушы бұл өрісті өңдей алады және ол тек шот ұсыну әдісін уақыт пен материал ретінде орнатқан жобаға негізделген келісім-шарт жолдарында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-179">The user can edit this field and it is only available on project-based contract lines that have the billing method set as time and material.</span></span> | <span data-ttu-id="66ab5-180">Пайдаланушы бұл өрісті өңдей алады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-180">The user can edit this field.</span></span> <span data-ttu-id="66ab5-181">Уақыт пен материалға арналған нақты көрсеткіштер осы келісім-шарт жолына уақыт пен материал үшін сілтеме жасаған кезде, нақты сома осы келісім-шарт жолындағы асырмау шегімен бағаланады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-181">When an actual for time and material references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on the contract line.</span></span> <span data-ttu-id="66ab5-182">Бұл бағалау жұмсалған және жасалған сомалар есепке алынғаннан кейін аяқталады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-182">This evaluation is completed after  the already spent and committed amounts are accounted for.</span></span> |
| <span data-ttu-id="66ab5-183">**Тұтынушы бюджеті**</span><span class="sxs-lookup"><span data-stu-id="66ab5-183">**Customer Budget**</span></span> | <span data-ttu-id="66ab5-184">Бұл өрісті өңдеуге болады және келісім-шарт баға ұсынудан жасалған болса, баға ұсыну жолындағы сәйкес өрістен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="66ab5-184">This field is editable and is copied from the corresponding field on the quote line if the contract was created from a quote.</span></span> | <span data-ttu-id="66ab5-185">Бұл өріс тек ақпарат алу үшін пайдаланылады және бұл өрісте ағынның маңыздылығы жоқ.</span><span class="sxs-lookup"><span data-stu-id="66ab5-185">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="66ab5-186">Жобаға негізделген келісім-шарт жолдарының Жалпы қойыншасындағы опцияларға арналған тексеру ережелері</span><span class="sxs-lookup"><span data-stu-id="66ab5-186">Validation rules for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="66ab5-187">1-ереже: **Қосылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** опциясына орнатылса, жобаның барлық тапсырмалары келісім-шарт жолына қосылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-187">Rule 1: If the **Included Tasks** field is blank or set to **All Project Tasks**, all tasks of the project are included on the contract line.</span></span>

<span data-ttu-id="66ab5-188">2-ереже: **Қосылған тапсырмалар** өрісі бос болған кезде немесе нақты **Барлық жоба тапсырмалары** опциясына орнатылған кезде, жоба мен белгілі бір транзакция класын тек келісім-шарттың бір жобаға негізделген келісім-шарт жолына қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-188">Rule 2: When the **Included Tasks** field is blank or explicitly set to **All Project Tasks**, a project and a certain transaction class can only be included on one project-based contract line of a contract.</span></span>

<span data-ttu-id="66ab5-189">3-ереже: **Қосылған тапсырмалар** өрісі **Тек таңдалған жоба тапсырмалары** опциясына орнатылған кезде, жоба мен белгілі бір транзакция класын тек келісім-шарттың бірнеше жобаға негізделген келісім-шарт жолдарына қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-189">Rule 3: When the **Included Tasks** field is set to **Selected Project Tasks Only**, a project and a certain transaction class can be included on multiple project-based contract lines of a contract.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p><span data-ttu-id="66ab5-190">
                    <strong>Келісімшарт</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-190">
                    <strong>Contract</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="66ab5-191">
                    <strong>Келісім-шарт жолы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-191">
                    <strong>Contract line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="66ab5-192">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-192">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="67" valign="top">
                <p><span data-ttu-id="66ab5-193">
                    <strong>Қамтылған тапсырмалар</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-193">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="66ab5-194">
                    <strong>Уақытпен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-194">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="66ab5-195">
                    <strong>Шығыспен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-195">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="66ab5-196">
                    <strong>Материалдармен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-196">
                    <strong>Include Materials</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="66ab5-197">
                    <strong>Қамту</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-197">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="66ab5-198">
                    <strong>Құн</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-198">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="53" valign="top">
                <p><span data-ttu-id="66ab5-199">
                    <strong>Жарамды/ Жарамсыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-199">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="250" valign="top">
                <p><span data-ttu-id="66ab5-200">
                    <strong>Себеп</strong>
                </span><span class="sxs-lookup"><span data-stu-id="66ab5-200">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-201">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-201">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-202">CL1</span><span class="sxs-lookup"><span data-stu-id="66ab5-202">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-203">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-203">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-204">Бос</span><span class="sxs-lookup"><span data-stu-id="66ab5-204">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-205">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-205">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-206">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-206">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-207">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-207">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-208">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-208">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-209">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="66ab5-209">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-210">№2 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="66ab5-210">Violation of Rule #2.</span></span> <span data-ttu-id="66ab5-211">Р1 жобасындағы уақыт, шығын , материалдар және төлемдер CL1 және CL2 келісім-шарт жолдарына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="66ab5-211">Time, Expense, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-212">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-212">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-213">CL2</span><span class="sxs-lookup"><span data-stu-id="66ab5-213">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-214">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-214">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-215">Бос</span><span class="sxs-lookup"><span data-stu-id="66ab5-215">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-216">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-216">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-217">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-217">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-218">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-218">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-219">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-219">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-220">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-220">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-221">CL1</span><span class="sxs-lookup"><span data-stu-id="66ab5-221">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-222">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-222">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-223">Бос</span><span class="sxs-lookup"><span data-stu-id="66ab5-223">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-224">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-224">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-225">No</span><span class="sxs-lookup"><span data-stu-id="66ab5-225">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-226">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-226">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-227">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-227">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-228">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="66ab5-228">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-229">№2 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="66ab5-229">Violation of Rule #2.</span></span> <span data-ttu-id="66ab5-230">Р1 жобасындағы уақыт, материалдар және төлемдер CL1 және CL2 келісім-шарт жолдарына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="66ab5-230">Time, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-231">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-231">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-232">CL2</span><span class="sxs-lookup"><span data-stu-id="66ab5-232">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-233">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-233">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-234">Бос</span><span class="sxs-lookup"><span data-stu-id="66ab5-234">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-235">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-235">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-236">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-236">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-237">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-237">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-238">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-238">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-239">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-239">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-240">CL1</span><span class="sxs-lookup"><span data-stu-id="66ab5-240">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-241">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-241">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-242">Бос</span><span class="sxs-lookup"><span data-stu-id="66ab5-242">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-243">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-243">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-244">No</span><span class="sxs-lookup"><span data-stu-id="66ab5-244">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-245">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-245">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-246">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-246">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-247">Жарамды</span><span class="sxs-lookup"><span data-stu-id="66ab5-247">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-248">Р1 жобасындағы уақыт, материалдар және төлемдер CL1 баға ұсыну жолына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="66ab5-248">Time, Materials, and Fees on P1 project are included on CL1.</span></span>
                </p>
                <ul>
                    <li>
<span data-ttu-id="66ab5-249">P1 жобасындағы шығыс CL2 баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="66ab5-249">Expense on P1 project is included on CL2.</span></span>
                    </li>
                </ul>
                <p>
<span data-ttu-id="66ab5-250">Әрбір келісім-шарт жолына кіретін ешнәрсе қабаттаспайды, сондықтан жарамды болып табылады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-250">No overlap in what is being included on each Contract line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-251">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-251">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-252">CL2</span><span class="sxs-lookup"><span data-stu-id="66ab5-252">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-253">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-253">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-254">Бос</span><span class="sxs-lookup"><span data-stu-id="66ab5-254">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-255">No</span><span class="sxs-lookup"><span data-stu-id="66ab5-255">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-256">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-257">No</span><span class="sxs-lookup"><span data-stu-id="66ab5-257">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-258">No</span><span class="sxs-lookup"><span data-stu-id="66ab5-258">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-259">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-259">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-260">CL1</span><span class="sxs-lookup"><span data-stu-id="66ab5-260">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-261">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-261">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-262">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="66ab5-262">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-263">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-263">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-264">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-264">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-265">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-266">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-266">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-267">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="66ab5-267">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-268">№2 ережені бұзу</span><span class="sxs-lookup"><span data-stu-id="66ab5-268">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="66ab5-269">C1 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығындағы уақытты, материалдарды, шығындар мен ақыларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="66ab5-269">C1 includes Time, Materials, Expenses and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="66ab5-270">CL2 жолына бүкіл P1 жобасы үшін уақыт, материалдар, шығын және төлем қосылған, сондықтан C1 жолында қамтылғанмен қабаттасады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-270">CL2 includes Time, Materials, Expenses and Fees for the whole project P1 and therefore overlaps with what is included on C1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-271">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-271">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-272">CL2</span><span class="sxs-lookup"><span data-stu-id="66ab5-272">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-273">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-273">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-274">Бос</span><span class="sxs-lookup"><span data-stu-id="66ab5-274">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-275">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-275">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-276">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-276">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-277">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-278">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-278">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-279">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-279">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-280">CL1</span><span class="sxs-lookup"><span data-stu-id="66ab5-280">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-281">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-281">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-282">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="66ab5-282">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-283">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-283">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-284">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-284">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-285">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-285">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-286">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-286">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-287">Жарамды</span><span class="sxs-lookup"><span data-stu-id="66ab5-287">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="66ab5-288">№3 ережеге сәйкес</span><span class="sxs-lookup"><span data-stu-id="66ab5-288">Per Rule #3</span></span> </p>
                <p>
<span data-ttu-id="66ab5-289">C1 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығындағы уақытты, шығындарды, материалдар мен төлемдерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="66ab5-289">C1 includes Time, Expenses, Materials, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="66ab5-290">CL2 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығы үшін уақытты, материалдарды, шығындар мен төлемдерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="66ab5-290">CL2 includes Time, Expenses, Materials, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="66ab5-291">Жалғыз қосымша тексеру CL1 бойынша тапсырмалар жиынтығының айналасында болады, бұл CL2 бойынша тапсырмалар жиынтығынан ерекшеленеді, осылайша қабаттасудың болмауын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="66ab5-291">The only additional validation is around the subset of tasks on CL1 is different from the subset of tasks on CL2 to ensure that there are no overlaps there.</span></span> <span data-ttu-id="66ab5-292">Бұл тапсырмалар байланыстырылған кезде жүйе тарапынан жасалады.</span><span class="sxs-lookup"><span data-stu-id="66ab5-292">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="66ab5-293">C1</span><span class="sxs-lookup"><span data-stu-id="66ab5-293">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="66ab5-294">CL2</span><span class="sxs-lookup"><span data-stu-id="66ab5-294">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-295">P1</span><span class="sxs-lookup"><span data-stu-id="66ab5-295">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="66ab5-296">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="66ab5-296">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-297">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-297">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="66ab5-298">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-298">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-299">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-299">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="66ab5-300">Иә</span><span class="sxs-lookup"><span data-stu-id="66ab5-300">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
