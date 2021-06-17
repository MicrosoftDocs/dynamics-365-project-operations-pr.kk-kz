---
title: Жобаға негізделген баға ұсыну жолдарына шолу
description: Бұл тақырыпта Project Operations бағдарламасындағы жоба жұмысына арналған жобаға негізделген баға ұсыну жолын пайдалану туралы ақпарат берілген.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32337b05f09ef7c5b84fdff9870744d6367e2693
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994863"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="fe530-103">Жобаға негізделген баға ұсыну жолдарына шолу</span><span class="sxs-lookup"><span data-stu-id="fe530-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="fe530-104">_**Қолданылу аясы:** жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі, ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="fe530-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="fe530-105">Жобаға негізделген баға ұсыну жолдары жоба жұмысын бағалауға көмектесуге арналған.</span><span class="sxs-lookup"><span data-stu-id="fe530-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="fe530-106">Жобаға негізделген баға ұсыну жолының құрылымы жоба болжамдары үшін келесі тұжырымдамалармен кеңейтілген:</span><span class="sxs-lookup"><span data-stu-id="fe530-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="fe530-107">Есепшот ұсыну әдісі</span><span class="sxs-lookup"><span data-stu-id="fe530-107">Billing Method</span></span>
- <span data-ttu-id="fe530-108">Жоба мен тапсырманы салыстыру</span><span class="sxs-lookup"><span data-stu-id="fe530-108">Project and Task Mapping</span></span>
- <span data-ttu-id="fe530-109">Қамтылған транзакция кластары</span><span class="sxs-lookup"><span data-stu-id="fe530-109">Included Transaction classes</span></span>
- <span data-ttu-id="fe530-110">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="fe530-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="fe530-111">Төлем қабілеттілігін орнату</span><span class="sxs-lookup"><span data-stu-id="fe530-111">Chargeability setup</span></span>
- <span data-ttu-id="fe530-112">Баға ұсыну жолының мәліметтері көмегімен бағалау</span><span class="sxs-lookup"><span data-stu-id="fe530-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="fe530-113">Баға ұсыну жолының тұтынушылары</span><span class="sxs-lookup"><span data-stu-id="fe530-113">Quote line Customers</span></span>

<span data-ttu-id="fe530-114">Келесі кестеде жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасындағы өрістері туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="fe530-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="fe530-115">Бұл өрістер жоба жұмысын егжей-тегжейлі, алдын ала болжам негізін орнатуға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="fe530-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="fe530-116">**Өріс**</span><span class="sxs-lookup"><span data-stu-id="fe530-116">**Field**</span></span> | <span data-ttu-id="fe530-117">**Сипаттамасы**</span><span class="sxs-lookup"><span data-stu-id="fe530-117">**Description**</span></span> | <span data-ttu-id="fe530-118">**Төменгі әсер**</span><span class="sxs-lookup"><span data-stu-id="fe530-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="fe530-119">Атауы</span><span class="sxs-lookup"><span data-stu-id="fe530-119">Name</span></span> | <span data-ttu-id="fe530-120">Болжанатын баға ұсынысының дискреттік құрамдасын анықтауға көмектесетін баға ұсыну жолының атауы.</span><span class="sxs-lookup"><span data-stu-id="fe530-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="fe530-121">Баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-122">Есепшот ұсыну әдісі</span><span class="sxs-lookup"><span data-stu-id="fe530-122">Billing Method</span></span> | <span data-ttu-id="fe530-123">Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолының сәйкес өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="fe530-124">Бұл өріс Dynamics 365 Project Operations тарапынан қолдау көрсетілетін екі негізгі келісім-шарт үлгілерін қамтиды:</span><span class="sxs-lookup"><span data-stu-id="fe530-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="fe530-125">- Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="fe530-125">- Fixed price</span></span></br><span data-ttu-id="fe530-126">- Уақыт және материал.</span><span class="sxs-lookup"><span data-stu-id="fe530-126">- Time and material.</span></span>| <span data-ttu-id="fe530-127">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-128">Project</span><span class="sxs-lookup"><span data-stu-id="fe530-128">Project</span></span> | <span data-ttu-id="fe530-129">Осы қосымша өрісті осы келісім бойынша жұмысты орындау мақсатында пайдаланылатын жобаны анықтау үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe530-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="fe530-130">Жоба баға ұсыну жолымен байланыстырылған кезде, ақылы тапсырмаларды орнатуға, сондай-ақ баға ұсыну жолын баға ұсыну жолының мәліметтері ретінде жоба негізінде болжауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="fe530-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="fe530-131">Жоба жобаға негізделген баға ұсыну жолымен салыстырылмаған кезде, баға әр баға ұсыну жолының мәліметтерін құру арқылы қолмен жасалуы керек.</span><span class="sxs-lookup"><span data-stu-id="fe530-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="fe530-132">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="fe530-133">Қосылған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="fe530-133">Included Tasks</span></span> | <span data-ttu-id="fe530-134">Осы баға ұсыну жолының таңдалған жобаға арналған барлық немесе кейбір жоба тапсырмалары үшін пайдаланылатынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="fe530-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="fe530-135">Бұл өріс келесі мүмкін мәндерге ие:</span><span class="sxs-lookup"><span data-stu-id="fe530-135">This field has the following possible values:</span></span></br><span data-ttu-id="fe530-136">- Барлық жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="fe530-136">- All project tasks</span></span></br><span data-ttu-id="fe530-137">- Тек таңдалған жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="fe530-137">- Selected project tasks only</span></span></br><span data-ttu-id="fe530-138">Осы өрістегі бос мән **Барлық жоба тапсырмалары** опциясына балама болып табылады.</span><span class="sxs-lookup"><span data-stu-id="fe530-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="fe530-139">Жоба бетінде **Тек таңдалған жоба тапсырмалары** таңдалған кезде, **Тапсырма шотын ұсынуды реттеу** қойыншасы осы баға ұсыну жолымен байланыстыру үшін белгілі бір тапсырмаларды таңдауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="fe530-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="fe530-140">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-141">Уақытпен қоса</span><span class="sxs-lookup"><span data-stu-id="fe530-141">Include Time</span></span> | <span data-ttu-id="fe530-142">**Иә**/**Жоқ** мәні таңдалған жобадағы уақыт транзакцияларының немесе еңбек шығындарының осы баға ұсынысы жолының болжамына кіретінін не кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="fe530-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="fe530-143">Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="fe530-144">Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="fe530-145">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-146">Шығыспен қоса</span><span class="sxs-lookup"><span data-stu-id="fe530-146">Include Expense</span></span> | <span data-ttu-id="fe530-147">**Иә**/**Жоқ** мәні таңдалған жобадағы шығындардың осы баға ұсынысы жолының болжамына кіретінін не кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="fe530-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="fe530-148">Баға ұсыну жолындағы болжамға шығыс құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="fe530-149">Баға ұсыну жолындағы болжамға шығыс құны қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="fe530-150">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-151">Материалмен қоса</span><span class="sxs-lookup"><span data-stu-id="fe530-151">Include Material</span></span> | <span data-ttu-id="fe530-152">**Иә**/**Жоқ** мәні таңдалған жобадағы материал шығындарының осы баға ұсынысы жолының болжамына кіретінін не кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="fe530-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="fe530-153">**Жоқ** мәні материал шығындарының осы баға ұсынысы жолының болжамына кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="fe530-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="fe530-154">**Иә** мәні материал шығындарының осы баға ұсынысы жолының болжамына кіретінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="fe530-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="fe530-155">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-156">Ақымен қоса</span><span class="sxs-lookup"><span data-stu-id="fe530-156">Include Fee</span></span> | <span data-ttu-id="fe530-157">**Иә**/**Жоқ** мәні таңдалған жобадағы ақылардың осы баға ұсынысы жолының болжамына кіретінін не кірмейтінін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="fe530-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="fe530-158">Баға ұсыну жолындағы болжамға төлемдер қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="fe530-159">Баға ұсыну жолындағы болжамға төлемдер қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="fe530-160">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-161">Баға ұсынылған көлем</span><span class="sxs-lookup"><span data-stu-id="fe530-161">Quoted Amount</span></span> | <span data-ttu-id="fe530-162">Бұл тұтынушыға осы жобаға негізделген баға ұсыну жолы бойынша болжанған барлық жұмыс үшін ұсынылатын сома.</span><span class="sxs-lookup"><span data-stu-id="fe530-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="fe530-163">Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолындағы **Тұтынушы бюджеті** өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="fe530-164">Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі мөлшерден жинақталады.</span><span class="sxs-lookup"><span data-stu-id="fe530-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="fe530-165">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-166">Болжалды салық</span><span class="sxs-lookup"><span data-stu-id="fe530-166">Estimated Tax</span></span> | <span data-ttu-id="fe530-167">Бұл пайдаланушыға баға ұсыну жолына салықтың есептелген мөлшерін қосатын өңделетін өріс.</span><span class="sxs-lookup"><span data-stu-id="fe530-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="fe530-168">Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі салық мөлшерінен жинақталады.</span><span class="sxs-lookup"><span data-stu-id="fe530-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="fe530-169">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-170">Салықтан кейінгі баға ұсыну сомасы</span><span class="sxs-lookup"><span data-stu-id="fe530-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="fe530-171">Бұл өріс салықтан кейінгі баға ұсыну жолының сомасы болып табылады және тек оқуға арналған.</span><span class="sxs-lookup"><span data-stu-id="fe530-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="fe530-172">Бұл өрістегі сома *Ұсынылған сома + Салық* ретінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="fe530-173">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-174">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="fe530-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="fe530-175">Бұл өрісті өңдеуге болады және тек **Уақыт және материал** төлем әдісіне ие жобаға негізделген баға ұсыну жолдарында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="fe530-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="fe530-176">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="fe530-177">Тұтынушы бюджеті</span><span class="sxs-lookup"><span data-stu-id="fe530-177">Customer Budget</span></span> | <span data-ttu-id="fe530-178">Бұл өрісті өңдеуге болады және мүмкіндіктен баға ұсынуы жасалған жағдайда, мүмкіндік жолындағы сәйкес өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="fe530-179">Бұл мән баға ұсынысын ұтқан кезде осы баға ұсынысы жолынан жасалған жобаның келісім-шарт жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="fe530-180">Жобаға негізделген баға ұсыну жолдарының Жалпы қойыншасындағы өрістерді тексеру ережелері</span><span class="sxs-lookup"><span data-stu-id="fe530-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="fe530-181">**1-ереже**: Егер **Қамтылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** өрісіне орнатылған болса, жоба баға ұсыну жолына енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="fe530-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="fe530-182">**2-ереже**: Егер **Қаматылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** өрісіне орнатылған болса, жоба мен белгілі бір транзакция класын баға ұсыныстарының жобаға негізделген баға ұсыну жолына енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="fe530-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="fe530-183">**3-ереже**: Егер **Қаматылған тапсырмалар** өрісі **Тек таңдалған жоба тапсырмалары** өрісіне орнатылған болса, жоба мен белгілі бір транзакция класын баға ұсыныстарының бірнеше жобаға негізделген баға ұсыну жолдарына енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="fe530-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="fe530-184">**4-ереже**: Егер мүмкіндікте бірнеше баға ұсыныстары болса, онда барлығы бірдей жобаға сілтеме жасайтын және бір транзакция класын қамтитын әртүрлі баға ұсыныстарында баға ұсыну жолдары болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="fe530-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="fe530-185">**5-ереже**: Егер баға ұсыныстары бірдей мүмкіндікке тиесілі болмаса, олар бірдей жоба мен транзакция класын қамтуы мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="fe530-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="fe530-186">
                    <strong>Мүмкіндік</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="fe530-187">
                    <strong>Баға ұсынысы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="fe530-188">
                    <strong>Баға ұсыну жолы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="fe530-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="fe530-190">
                    <strong>Қамтылған тапсырмалар</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="fe530-191">
                    <strong>Уақытпен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="fe530-192">
                    <strong>Шығыспен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="fe530-193">
                    <strong>Материалмен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="fe530-194">
                    <strong>Қамту</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="fe530-195">
                    <strong>Құн</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="fe530-196">
                    <strong>Жарамды/ Жарамсыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="fe530-197">
                    <strong>Себеп</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fe530-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-198">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-199">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-200">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-201">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-202">Бос</span><span class="sxs-lookup"><span data-stu-id="fe530-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-203">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-204">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-205">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-206">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-207">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="fe530-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-208">№2 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="fe530-208">Violation of Rule #2.</span></span> <span data-ttu-id="fe530-209">Р1 жобасындағы уақыт, шығын және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген</span><span class="sxs-lookup"><span data-stu-id="fe530-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-210">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-211">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-212">QL2</span><span class="sxs-lookup"><span data-stu-id="fe530-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-213">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-214">Бос</span><span class="sxs-lookup"><span data-stu-id="fe530-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-215">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-216">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-217">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-218">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-218">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-219">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-220">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-221">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-222">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-223">Бос</span><span class="sxs-lookup"><span data-stu-id="fe530-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-224">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-225">No</span><span class="sxs-lookup"><span data-stu-id="fe530-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-226">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-227">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-228">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="fe530-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-229">№2 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="fe530-229">Violation of Rule #2.</span></span> <span data-ttu-id="fe530-230">Р1 жобасындағы уақыт, материал және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген</span><span class="sxs-lookup"><span data-stu-id="fe530-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-231">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-232">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-233">QL2</span><span class="sxs-lookup"><span data-stu-id="fe530-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-234">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-235">Бос</span><span class="sxs-lookup"><span data-stu-id="fe530-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-236">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-237">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-238">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-239">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-239">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-240">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-241">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-242">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-243">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-244">Бос</span><span class="sxs-lookup"><span data-stu-id="fe530-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-245">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-246">No</span><span class="sxs-lookup"><span data-stu-id="fe530-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-247">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-248">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-249">Жарамды</span><span class="sxs-lookup"><span data-stu-id="fe530-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-250">Р1 жобасындағы уақыт, материал және төлемдер QL1 баға ұсыну жолына бірдей енгізілген</span><span class="sxs-lookup"><span data-stu-id="fe530-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="fe530-251">P1 жобасындағы шығын QL2 баға ұсыну жолына енгізілген</span><span class="sxs-lookup"><span data-stu-id="fe530-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="fe530-252">Әрбір баға ұсыну жолына кіретін ешнәрсе қабаттаспайды, сондықтан жарамды болып табылады.</span><span class="sxs-lookup"><span data-stu-id="fe530-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-253">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-254">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-255">QL2</span><span class="sxs-lookup"><span data-stu-id="fe530-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-256">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-257">Бос</span><span class="sxs-lookup"><span data-stu-id="fe530-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-258">No</span><span class="sxs-lookup"><span data-stu-id="fe530-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-259">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-260">No</span><span class="sxs-lookup"><span data-stu-id="fe530-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-261">No</span><span class="sxs-lookup"><span data-stu-id="fe530-261">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-262">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-263">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-264">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-265">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-266">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="fe530-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-267">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-268">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-269">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-270">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-271">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="fe530-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-272">№2 ережені бұзу</span><span class="sxs-lookup"><span data-stu-id="fe530-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="fe530-273">Q1 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығындағы уақытты, материалды, шығындар мен ақыларды қамтиды</span><span class="sxs-lookup"><span data-stu-id="fe530-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="fe530-274">QL2 жолына бүкіл P1 жобасы үшін уақыт, шығын және ақы қосылған, сондықтан Q1 жолында қамтылғанмен қабаттасады.</span><span class="sxs-lookup"><span data-stu-id="fe530-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-275">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-276">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-277">QL2</span><span class="sxs-lookup"><span data-stu-id="fe530-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-278">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-279">Бос</span><span class="sxs-lookup"><span data-stu-id="fe530-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-280">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-281">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-282">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-283">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-283">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-284">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-285">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-286">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-287">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-288">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="fe530-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-289">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-290">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-291">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-292">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-293">Жарамды</span><span class="sxs-lookup"><span data-stu-id="fe530-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-294">№3 ережеге сәйкес,</span><span class="sxs-lookup"><span data-stu-id="fe530-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="fe530-295">Q1 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығындағы уақытты, материалды, шығындар мен ақыларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="fe530-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="fe530-296">QL2 баға ұсыну жолы P1 жобасы бойынша тапсырмалар жиынтығы үшін уақытты, материалды, шығындар мен ақыларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="fe530-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="fe530-297">Жалғыз қосымша тексеру QL1 бойынша тапсырмалар жиынтығының айналасында болады, бұл QL2 бойынша тапсырмалар жиынтығынан ерекшеленеді, осылайша қабаттасудың болмауын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="fe530-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="fe530-298">Бұл тапсырмалар байланыстырылған кезде жүйе тарапынан жасалады.</span><span class="sxs-lookup"><span data-stu-id="fe530-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-299">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-300">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-301">QL2</span><span class="sxs-lookup"><span data-stu-id="fe530-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-302">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-303">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="fe530-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-304">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-305">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-306">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-307">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-307">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-308">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-309">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-310">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-311">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-312">Барлық жоба тапсырмалары немесе бос</span><span class="sxs-lookup"><span data-stu-id="fe530-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-313">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-314">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-315">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-316">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-317">Жарамды</span><span class="sxs-lookup"><span data-stu-id="fe530-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-318">№5 ережеге сәйкес, Q1 және Q2 бірдей мүмкіндіктегі екі баға ұсыну жолы болып табылады, сондықтан да екеуі де жобаның бірдей құрамдастарын болжай алады.</span><span class="sxs-lookup"><span data-stu-id="fe530-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-319">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-320">Q2</span><span class="sxs-lookup"><span data-stu-id="fe530-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-321">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-322">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-323">Барлық жоба тапсырмалары немесе бос</span><span class="sxs-lookup"><span data-stu-id="fe530-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-324">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-325">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-326">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-327">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-327">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-328">O1</span><span class="sxs-lookup"><span data-stu-id="fe530-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-329">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-330">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-331">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-332">Барлық жоба тапсырмалары немесе бос</span><span class="sxs-lookup"><span data-stu-id="fe530-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-333">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-334">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-335">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-336">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-337">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="fe530-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fe530-338">№4 ережеге сәйкес, Q1 және Q2 әртүрлі мүмкіндіктегі екі баға ұсыну жолы болып табылады, сондықтан да олар бірдей жобаның бірдей құрамдастарын болжай алмайды.</span><span class="sxs-lookup"><span data-stu-id="fe530-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="fe530-339">O2</span><span class="sxs-lookup"><span data-stu-id="fe530-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="fe530-340">Т1</span><span class="sxs-lookup"><span data-stu-id="fe530-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="fe530-341">QL1</span><span class="sxs-lookup"><span data-stu-id="fe530-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-342">P1</span><span class="sxs-lookup"><span data-stu-id="fe530-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="fe530-343">Барлық жоба тапсырмалары немесе бос</span><span class="sxs-lookup"><span data-stu-id="fe530-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="fe530-344">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="fe530-345">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="fe530-346">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="fe530-347">Иә</span><span class="sxs-lookup"><span data-stu-id="fe530-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
