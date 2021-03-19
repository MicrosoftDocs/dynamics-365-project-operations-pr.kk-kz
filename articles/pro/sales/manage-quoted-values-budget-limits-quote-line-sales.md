---
title: Жобаға негізделген баға ұсыну жолдарына шолу - жеңілдетілген
description: Бұл тақырыпта Project Operations бағдарламасындағы жоба жұмысына арналған жобаға негізделген баға ұсыну жолын пайдалану туралы ақпарат берілген. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4865c06691fba09eacf5fe6449adfaf542444520
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272980"
---
# <a name="project-based-quote-lines-overview---lite"></a><span data-ttu-id="4cdb9-104">Жобаға негізделген баға ұсыну жолдарына шолу - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="4cdb9-104">Project-based quote lines overview - lite</span></span>

<span data-ttu-id="4cdb9-105">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="4cdb9-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4cdb9-106">Жобаға негізделген баға ұсыну жолдары жоба жұмысын бағалауға көмектесуге арналған.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="4cdb9-107">Жобаға негізделген баға ұсыну жолының құрылымы жоба болжамдары үшін келесі тұжырымдамалармен кеңейтілген:</span><span class="sxs-lookup"><span data-stu-id="4cdb9-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="4cdb9-108">Есепшот ұсыну әдісі</span><span class="sxs-lookup"><span data-stu-id="4cdb9-108">Billing Method</span></span>
- <span data-ttu-id="4cdb9-109">Жоба мен тапсырманы салыстыру</span><span class="sxs-lookup"><span data-stu-id="4cdb9-109">Project and Task Mapping</span></span>
- <span data-ttu-id="4cdb9-110">Қамтылған транзакция кластары</span><span class="sxs-lookup"><span data-stu-id="4cdb9-110">Included Transaction classes</span></span>
- <span data-ttu-id="4cdb9-111">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="4cdb9-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="4cdb9-112">Төлем қабілеттілігін орнату</span><span class="sxs-lookup"><span data-stu-id="4cdb9-112">Chargeability setup</span></span>
- <span data-ttu-id="4cdb9-113">Баға ұсыну жолының мәліметтері көмегімен бағалау</span><span class="sxs-lookup"><span data-stu-id="4cdb9-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="4cdb9-114">Баға ұсыну жолының тұтынушылары</span><span class="sxs-lookup"><span data-stu-id="4cdb9-114">Quote line Customers</span></span>

<span data-ttu-id="4cdb9-115">Келесі кестеде жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасындағы өрістері туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="4cdb9-116">Бұл өрістер жоба жұмысын егжей-тегжейлі, алдын ала болжам негізін орнатуға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="4cdb9-117">**Өріс**</span><span class="sxs-lookup"><span data-stu-id="4cdb9-117">**Field**</span></span> | <span data-ttu-id="4cdb9-118">**Сипаттамасы**</span><span class="sxs-lookup"><span data-stu-id="4cdb9-118">**Description**</span></span> | <span data-ttu-id="4cdb9-119">**Төменгі әсер**</span><span class="sxs-lookup"><span data-stu-id="4cdb9-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="4cdb9-120">Атауы</span><span class="sxs-lookup"><span data-stu-id="4cdb9-120">Name</span></span> | <span data-ttu-id="4cdb9-121">Бағаланатын баға ұсынудың жеке компонентін анықтауға көмектесетін баға ұсыну жолының атауы.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="4cdb9-122">Баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-123">Есепшот ұсыну әдісі</span><span class="sxs-lookup"><span data-stu-id="4cdb9-123">Billing Method</span></span> | <span data-ttu-id="4cdb9-124">Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолының сәйкес өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="4cdb9-125">Бұл өріс Dynamics 365 Project Operations тарапынан қолдау көрсетілетін екі негізгі келісім-шарт үлгілерін қамтиды:</span><span class="sxs-lookup"><span data-stu-id="4cdb9-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="4cdb9-126">- Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="4cdb9-126">- Fixed price</span></span></br><span data-ttu-id="4cdb9-127">- Уақыт және материал.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-127">- Time and material.</span></span>| <span data-ttu-id="4cdb9-128">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-129">Project</span><span class="sxs-lookup"><span data-stu-id="4cdb9-129">Project</span></span> | <span data-ttu-id="4cdb9-130">Осы қосымша өрісті осы келісім бойынша жұмысты орындау мақсатында пайдаланылатын жобаны анықтау үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="4cdb9-131">Жоба баға ұсыну жолымен байланыстырылған кезде, ақылы тапсырмаларды орнатуға, сондай-ақ баға ұсыну жолын баға ұсыну жолының мәліметтері ретінде жоба негізінде болжауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="4cdb9-132">Жоба жобаға негізделген баға ұсыну жолымен салыстырылмаған кезде, баға әр баға ұсыну жолының мәліметтерін құру арқылы қолмен жасалуы керек.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="4cdb9-133">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="4cdb9-134">Қосылған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="4cdb9-134">Included Tasks</span></span> | <span data-ttu-id="4cdb9-135">Осы баға ұсыну жолының таңдалған жобаға арналған барлық немесе кейбір жоба тапсырмалары үшін пайдаланылатынын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="4cdb9-136">Бұл өріс келесі мүмкін мәндерге ие:</span><span class="sxs-lookup"><span data-stu-id="4cdb9-136">This field has the following possible values:</span></span></br><span data-ttu-id="4cdb9-137">- Барлық жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="4cdb9-137">- All project tasks</span></span></br><span data-ttu-id="4cdb9-138">- Тек таңдалған жоба тапсырмалары</span><span class="sxs-lookup"><span data-stu-id="4cdb9-138">- Selected project tasks only</span></span></br><span data-ttu-id="4cdb9-139">Осы өрістегі бос мән **Барлық жоба тапсырмалары** опциясына балама болып табылады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="4cdb9-140">Жоба бетінде **Тек таңдалған жоба тапсырмалары** таңдалған кезде, **Тапсырма төлемін орнату** қойыншасы арнайы тапсырмаларды баға ұсыну жолымен байланыстыру үшін оларды таңдауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="4cdb9-141">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-142">Уақытпен қоса</span><span class="sxs-lookup"><span data-stu-id="4cdb9-142">Include Time</span></span> | <span data-ttu-id="4cdb9-143">Таңдалған жобадағы уақыт транзакциялары немесе еңбек құны осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="4cdb9-144">Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="4cdb9-145">Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="4cdb9-146">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-147">Шығыспен қоса</span><span class="sxs-lookup"><span data-stu-id="4cdb9-147">Include Expense</span></span> | <span data-ttu-id="4cdb9-148">Таңдалған жобадағы шығыс құны осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="4cdb9-149">Баға ұсыну жолындағы болжамға шығыс құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="4cdb9-150">Баға ұсыну жолындағы болжамға шығыс құны қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="4cdb9-151">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-152">Ақымен қоса</span><span class="sxs-lookup"><span data-stu-id="4cdb9-152">Include Fee</span></span> | <span data-ttu-id="4cdb9-153">Таңдалған жобадағы төлемдер осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="4cdb9-154">Баға ұсыну жолындағы болжамға төлемдер қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="4cdb9-155">Баға ұсыну жолындағы болжамға төлемдер қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="4cdb9-156">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-157">Баға ұсынылған көлем</span><span class="sxs-lookup"><span data-stu-id="4cdb9-157">Quoted Amount</span></span> | <span data-ttu-id="4cdb9-158">Бұл тұтынушыға осы жобаға негізделген баға ұсыну жолы бойынша болжамдалған барлық жұмыстар үшін ұсынылатын сома.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="4cdb9-159">Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолындағы **Тұтынушы бюджеті** өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="4cdb9-160">Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі мөлшерден жинақталады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="4cdb9-161">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-162">Болжалды салық</span><span class="sxs-lookup"><span data-stu-id="4cdb9-162">Estimated Tax</span></span> | <span data-ttu-id="4cdb9-163">Бұл пайдаланушыға баға ұсыну жолына салықтың есептелген мөлшерін қосатын өңделетін өріс.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="4cdb9-164">Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі салық мөлшерінен жинақталады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="4cdb9-165">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-166">Салықтан кейінгі баға ұсыну сомасы</span><span class="sxs-lookup"><span data-stu-id="4cdb9-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="4cdb9-167">Бұл өріс салықтан кейінгі баға ұсыну жолының сомасы болып табылады және тек оқуға арналған.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="4cdb9-168">Бұл өрістегі сома *Ұсынылған сома + Салық* ретінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="4cdb9-169">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-170">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="4cdb9-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="4cdb9-171">Бұл өрісті өңдеуге болады және тек **Уақыт және материал** төлем әдісіне ие жобаға негізделген баға ұсыну жолдарында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="4cdb9-172">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="4cdb9-173">Тұтынушы бюджеті</span><span class="sxs-lookup"><span data-stu-id="4cdb9-173">Customer Budget</span></span> | <span data-ttu-id="4cdb9-174">Бұл өрісті өңдеуге болады және мүмкіндіктен баға ұсынуы жасалған жағдайда, мүмкіндік жолындағы сәйкес өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="4cdb9-175">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="4cdb9-176">Жобаға негізделген баға ұсыну жолдарының Жалпы қойыншасындағы өрістерді тексеру ережелері</span><span class="sxs-lookup"><span data-stu-id="4cdb9-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="4cdb9-177">**1-ереже**: Егер **Қамтылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** өрісіне орнатылған болса, жоба баға ұсыну жолына енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="4cdb9-178">**2-ереже**: Егер **Қаматылған тапсырмалар** өрісі бос болса немесе **Барлық жоба тапсырмалары** өрісіне орнатылған болса, жоба мен белгілі бір транзакция класын баға ұсыныстарының жобаға негізделген баға ұсыну жолына енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="4cdb9-179">**3-ереже**: Егер **Қаматылған тапсырмалар** өрісі **Тек таңдалған жоба тапсырмалары** өрісіне орнатылған болса, жоба мен белгілі бір транзакция класын баға ұсыныстарының бірнеше жобаға негізделген баға ұсыну жолдарына енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="4cdb9-180">**4-ереже**: Егер мүмкіндікте бірнеше баға ұсыныстары болса, онда барлығы бірдей жобаға сілтеме жасайтын және бір транзакция класын қамтитын әртүрлі баға ұсыныстарында баға ұсыну жолдары болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="4cdb9-181">**5-ереже**: Егер баға ұсыныстары бірдей мүмкіндікке тиесілі болмаса, олар бірдей жоба мен транзакция класын қамтуы мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="4cdb9-182">
                    <strong>Мүмкіндік</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="4cdb9-183">
                    <strong>Баға ұсынысы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="4cdb9-184">
                    <strong>Баға ұсыну жолы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="4cdb9-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="4cdb9-186">
                    <strong>Қамтылған тапсырмалар</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="4cdb9-187">
                    <strong>Уақытпен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="4cdb9-188">
                    <strong>Шығыспен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="4cdb9-189">
                    <strong>Қамту</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="4cdb9-190">
                    <strong>Құн</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="4cdb9-191">
                    <strong>Жарамды/ Жарамсыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="4cdb9-192">
                    <strong>Себеп</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4cdb9-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-193">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-194">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-195">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-196">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-197">Бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-198">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-199">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-200">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-201">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="4cdb9-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-202">№2 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-202">Violation of Rule #2.</span></span> <span data-ttu-id="4cdb9-203">Р1 жобасындағы уақыт, шығыс және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-204">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-205">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-206">QL2</span><span class="sxs-lookup"><span data-stu-id="4cdb9-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-207">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-208">Бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-209">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-210">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-211">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-211">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-212">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-213">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-214">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-215">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-216">Бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-217">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-218">№</span><span class="sxs-lookup"><span data-stu-id="4cdb9-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-219">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-220">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="4cdb9-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-221">№2 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-221">Violation of Rule #2.</span></span> <span data-ttu-id="4cdb9-222">Р1 жобасындағы уақыт және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-223">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-224">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-225">QL2</span><span class="sxs-lookup"><span data-stu-id="4cdb9-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-226">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-227">Бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-228">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-229">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-230">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-230">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-231">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-232">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-233">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-234">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-235">Бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-236">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-237">№</span><span class="sxs-lookup"><span data-stu-id="4cdb9-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-238">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-239">Жарамды</span><span class="sxs-lookup"><span data-stu-id="4cdb9-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="4cdb9-240">P1 жобасындағы уақыт және төлемдер QL1 баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="4cdb9-241">P1 жобасындағы шығыс QL2 баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="4cdb9-242">Әр баға ұсыну жолына енгізілгенде қабаттасу жоқ және ол жарамды.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-243">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-244">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-245">QL2</span><span class="sxs-lookup"><span data-stu-id="4cdb9-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-246">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-247">Бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-248">№</span><span class="sxs-lookup"><span data-stu-id="4cdb9-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-249">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-250">№</span><span class="sxs-lookup"><span data-stu-id="4cdb9-250">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-251">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-252">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-253">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-254">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-255">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="4cdb9-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-256">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-257">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-258">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-259">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="4cdb9-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-260">Жоғарыдағы №2 ережені бұзу</span><span class="sxs-lookup"><span data-stu-id="4cdb9-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="4cdb9-261">Q1 Р1 жобасында тапсырмалар жиынындағы уақыт, шығыс және төлемдерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="4cdb9-262">QL2 бүкіл P1 жобасына арналған уақыт, шығыстар және төлемдерді қамтиды және Q1 баға ұсыну жолына енгізілгендермен қабаттасады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-263">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-264">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-265">QL2</span><span class="sxs-lookup"><span data-stu-id="4cdb9-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-266">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-267">Бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-268">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-269">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-270">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-270">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-271">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-272">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-273">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-274">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-275">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="4cdb9-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-276">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-277">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-278">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-279">Жарамды</span><span class="sxs-lookup"><span data-stu-id="4cdb9-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-280">Жоғарыдағы №3 ережеге сәйкес,</span><span class="sxs-lookup"><span data-stu-id="4cdb9-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="4cdb9-281">Q1 Р1 жобасында тапсырмалар жиынындағы уақыт, шығыс және төлемдерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="4cdb9-282">QL2 Р1 жобасында тапсырмалар жиынындағы уақыт, шығыс және төлемдерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="4cdb9-283">Жалғыз қосымша тексеру QL2 тапсырмаларының жиынынан ерекшеленетін QL1 тапсырмаларының жиыны шеңберінде болады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="4cdb9-284">Бұл қабаттасудың болмауын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="4cdb9-285">Бұл тапсырмалар байланыстырылған кезде жүйе тарапынан жасалады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-286">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-287">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-288">QL2</span><span class="sxs-lookup"><span data-stu-id="4cdb9-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-289">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-290">Тек таңдалған тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="4cdb9-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-291">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-292">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-293">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-293">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-294">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-295">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-296">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-297">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-298">Барлық жоба тапсырмалары немесе бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-299">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-300">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-301">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="4cdb9-302">Жарамды</span><span class="sxs-lookup"><span data-stu-id="4cdb9-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-303">№5 ереже негізінде, Q1 және Q2 - бір мүмкіндіктегі екі баға ұсыну жолы, сондықтан екеуі де жобаның бірдей компоненттерін бағалай алады.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-304">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-305">Q2</span><span class="sxs-lookup"><span data-stu-id="4cdb9-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-306">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-307">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-308">Барлық жоба тапсырмалары немесе бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-309">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-310">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-311">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-311">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-312">O1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-313">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-314">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-315">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-316">Барлық жоба тапсырмалары немесе бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-317">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-318">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-319">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="4cdb9-320">Жарамды</span><span class="sxs-lookup"><span data-stu-id="4cdb9-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4cdb9-321">№4 ереже негізінде, Q1 және Q2 - әртүрлі мүмкіндіктегі екі баға ұсыну жолы, сондықтан екеуі де бірдей жобаның бірдей компоненттерін бағалай алмайды.</span><span class="sxs-lookup"><span data-stu-id="4cdb9-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="4cdb9-322">O2</span><span class="sxs-lookup"><span data-stu-id="4cdb9-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="4cdb9-323">Т1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-324">QL1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-325">P1</span><span class="sxs-lookup"><span data-stu-id="4cdb9-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="4cdb9-326">Барлық жоба тапсырмалары немесе бос</span><span class="sxs-lookup"><span data-stu-id="4cdb9-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-327">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4cdb9-328">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4cdb9-329">Иә</span><span class="sxs-lookup"><span data-stu-id="4cdb9-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="4cdb9-330">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="4cdb9-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]