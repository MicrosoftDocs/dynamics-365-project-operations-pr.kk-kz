---
title: Жобаға негізделген баға ұсыну жолдары
description: Бұл тақырыпта Project Operations бағдарламасындағы жоба жұмысына арналған жобаға негізделген баға ұсыну жолын пайдалану туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 06a47c45dc3b3b174658e2fba14d3d2050aabf85
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079527"
---
# <a name="project-based-quote-lines"></a><span data-ttu-id="013db-103">Жобаға негізделген баға ұсыну жолдары</span><span class="sxs-lookup"><span data-stu-id="013db-103">Project-based quote lines</span></span>

<span data-ttu-id="013db-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="013db-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="013db-105">Жобаға негізделген баға ұсыну жолдары жоба жұмысын бағалауға көмектесуге арналған.</span><span class="sxs-lookup"><span data-stu-id="013db-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="013db-106">Жобаға негізделген баға ұсыну жолының құрылымы жоба болжамдары үшін келесі тұжырымдамалармен кеңейтілген:</span><span class="sxs-lookup"><span data-stu-id="013db-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="013db-107">Есепшот ұсыну әдісі</span><span class="sxs-lookup"><span data-stu-id="013db-107">Billing Method</span></span>
- <span data-ttu-id="013db-108">Жобаны салыстыру</span><span class="sxs-lookup"><span data-stu-id="013db-108">Project Mapping</span></span>
- <span data-ttu-id="013db-109">Қамтылған транзакция кластары</span><span class="sxs-lookup"><span data-stu-id="013db-109">Included Transaction classes</span></span>
- <span data-ttu-id="013db-110">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="013db-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="013db-111">Төлем қабілеттілігін орнату</span><span class="sxs-lookup"><span data-stu-id="013db-111">Chargeability setup</span></span>
- <span data-ttu-id="013db-112">Баға ұсыну жолының мәліметтері көмегімен бағалау</span><span class="sxs-lookup"><span data-stu-id="013db-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="013db-113">Баға ұсыну жолының тұтынушылары</span><span class="sxs-lookup"><span data-stu-id="013db-113">Quote line Customers</span></span>

<span data-ttu-id="013db-114">Келесі кестеде жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасындағы өрістері туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="013db-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="013db-115">Бұл өрістер жоба жұмысын егжей-тегжейлі, алдын ала болжам негізін орнатуға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="013db-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="013db-116">**Өріс**</span><span class="sxs-lookup"><span data-stu-id="013db-116">**Field**</span></span> | <span data-ttu-id="013db-117">**Маңыздылық, мақсаты және нұсқаулығы**</span><span class="sxs-lookup"><span data-stu-id="013db-117">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="013db-118">**Төменгі әсер**</span><span class="sxs-lookup"><span data-stu-id="013db-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="013db-119">Атауы</span><span class="sxs-lookup"><span data-stu-id="013db-119">Name</span></span> | <span data-ttu-id="013db-120">Бағаланатын баға ұсынудың жеке компонентін анықтауға көмектесетін баға ұсыну жолының атауы.</span><span class="sxs-lookup"><span data-stu-id="013db-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="013db-121">Баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-122">Есепшот ұсыну әдісі</span><span class="sxs-lookup"><span data-stu-id="013db-122">Billing Method</span></span> | <span data-ttu-id="013db-123">Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолының сәйкес өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="013db-124">Бұл өрісте Dynamics 365 Project Operations тарапынан қолдау көрсетілетін екі негізгі келісілген үлгілер қамтылған:</span><span class="sxs-lookup"><span data-stu-id="013db-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="013db-125">- Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="013db-125">- Fixed price</span></span></br><span data-ttu-id="013db-126">- Уақыт және материал.</span><span class="sxs-lookup"><span data-stu-id="013db-126">- Time and material.</span></span>| <span data-ttu-id="013db-127">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-128">Project</span><span class="sxs-lookup"><span data-stu-id="013db-128">Project</span></span> | <span data-ttu-id="013db-129">Осы қосымша өрісті осы келісім бойынша жұмысты орындау мақсатында пайдаланылатын жобаны анықтау үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="013db-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="013db-130">Жоба баға ұсыну жолымен байланыстырылған кезде, ақылы тапсырмаларды орнатуға, сондай-ақ баға ұсыну жолын баға ұсыну жолының мәліметтері ретінде жоба негізінде болжауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="013db-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="013db-131">Жоба жобаға негізделген баға ұсыну жолымен салыстырылмаған кезде, баға әр баға ұсыну жолының мәліметтерін құру арқылы қолмен жасалуы керек.</span><span class="sxs-lookup"><span data-stu-id="013db-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="013db-132">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-133">Уақытпен қоса</span><span class="sxs-lookup"><span data-stu-id="013db-133">Include Time</span></span> | <span data-ttu-id="013db-134">Таңдалған жобадағы уақыт транзакциялары немесе еңбек құны осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="013db-135">Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="013db-136">Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="013db-137">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-138">Шығыспен қоса</span><span class="sxs-lookup"><span data-stu-id="013db-138">Include Expense</span></span> | <span data-ttu-id="013db-139">Таңдалған жобадағы шығыс құны осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="013db-140">Баға ұсыну жолындағы болжамға шығыс құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="013db-141">Баға ұсыну жолындағы болжамға шығыс құны қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="013db-142">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-143">Ақымен қоса</span><span class="sxs-lookup"><span data-stu-id="013db-143">Include Fee</span></span> | <span data-ttu-id="013db-144">Таңдалған жобадағы төлемдер осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="013db-145">Баға ұсыну жолындағы болжамға төлемдер қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="013db-146">Баға ұсыну жолындағы болжамға төлемдер қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="013db-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="013db-147">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-148">Баға ұсынылған көлем</span><span class="sxs-lookup"><span data-stu-id="013db-148">Quoted Amount</span></span> | <span data-ttu-id="013db-149">Бұл тұтынушыға осы жобаға негізделген баға ұсыну жолы бойынша болжамдалған барлық жұмыстар үшін ұсынылатын сома.</span><span class="sxs-lookup"><span data-stu-id="013db-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="013db-150">Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолындағы **Тұтынушы бюджеті** өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="013db-151">Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі мөлшерден жинақталады.</span><span class="sxs-lookup"><span data-stu-id="013db-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="013db-152">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-153">Болжалды салық</span><span class="sxs-lookup"><span data-stu-id="013db-153">Estimated Tax</span></span> | <span data-ttu-id="013db-154">Бұл пайдаланушыға баға ұсыну жолына салықтың есептелген мөлшерін қосатын өңделетін өріс.</span><span class="sxs-lookup"><span data-stu-id="013db-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="013db-155">Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі салық мөлшерінен жинақталады.</span><span class="sxs-lookup"><span data-stu-id="013db-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="013db-156">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-157">Салықтан кейінгі баға ұсыну сомасы</span><span class="sxs-lookup"><span data-stu-id="013db-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="013db-158">Бұл өріс салықтан кейінгі баға ұсыну жолының сомасы болып табылады және тек оқуға арналған.</span><span class="sxs-lookup"><span data-stu-id="013db-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="013db-159">Бұл өрістегі сома *Ұсынылған сома + Салық* ретінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="013db-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="013db-160">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-161">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="013db-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="013db-162">Бұл өрісті өңдеуге болады және тек **Уақыт және материал** төлем әдісіне ие жобаға негізделген баға ұсыну жолдарында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="013db-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="013db-163">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="013db-164">Тұтынушы бюджеті</span><span class="sxs-lookup"><span data-stu-id="013db-164">Customer Budget</span></span> | <span data-ttu-id="013db-165">Бұл өрісті өңдеуге болады және мүмкіндіктен баға ұсынуы жасалған жағдайда, мүмкіндік жолындағы сәйкес өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="013db-166">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="013db-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="013db-167">Жобаға негізделген баға ұсыну жолдарының Жалпы қойыншасындағы өрістерді тексеру ережелері</span><span class="sxs-lookup"><span data-stu-id="013db-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="013db-168">**1-ереже** : Таңдалған жоба бойынша белгілі бір транзакция класын тек бір баға ұсыныстарының жобаға негізделген баға ұсыну жолына енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="013db-168">**Rule 1** : A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="013db-169">**2-ереже** : Егер мүмкіндікте бірнеше баға ұсыныстары болса, онда барлығы бірдей жобаға сілтеме жасайтын және бір транзакция класын қамтитын әртүрлі баға ұсыныстарында баға ұсыну жолдары болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="013db-169">**Rule 2** : If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="013db-170">**3-ереже** : Егер баға ұсыныстары бірдей мүмкіндікке тиесілі болмаса, олар бірдей жоба мен транзакция класын қамтуы мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="013db-170">**Rule 3** : If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="013db-171">
                    <strong>Мүмкіндік</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="013db-172">
                    <strong>Баға ұсынысы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="013db-173">
                    <strong>Баға ұсыну жолы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="013db-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="013db-175">
                    <strong>Уақытпен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="013db-176">
                    <strong>Шығыспен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="013db-177">
                    <strong>Қамту</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="013db-178">
                    <strong>төлем</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="013db-179">
                    <strong>Жарамды/ Жарамсыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="013db-180">
                    <strong>Себеп</strong>
                </span><span class="sxs-lookup"><span data-stu-id="013db-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="013db-181">O1</span><span class="sxs-lookup"><span data-stu-id="013db-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-182">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-183">QL1</span><span class="sxs-lookup"><span data-stu-id="013db-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-184">P1</span><span class="sxs-lookup"><span data-stu-id="013db-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-185">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-186">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-187">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-188">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="013db-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-189">№1 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="013db-189">Violation of Rule #1.</span></span> <span data-ttu-id="013db-190">Р1 жобасындағы уақыт, шығыс және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="013db-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="013db-191">O1</span><span class="sxs-lookup"><span data-stu-id="013db-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-192">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-193">QL2</span><span class="sxs-lookup"><span data-stu-id="013db-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-194">P1</span><span class="sxs-lookup"><span data-stu-id="013db-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-195">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-196">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-197">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-197">Yes</span></span> </p>
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
<span data-ttu-id="013db-198">O1</span><span class="sxs-lookup"><span data-stu-id="013db-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-199">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-200">QL1</span><span class="sxs-lookup"><span data-stu-id="013db-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-201">P1</span><span class="sxs-lookup"><span data-stu-id="013db-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-202">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-203">№</span><span class="sxs-lookup"><span data-stu-id="013db-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-204">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-205">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="013db-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-206">№1 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="013db-206">Violation of Rule #1.</span></span> <span data-ttu-id="013db-207">Р1 жобасындағы уақыт және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="013db-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="013db-208">O1</span><span class="sxs-lookup"><span data-stu-id="013db-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-209">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-210">QL2</span><span class="sxs-lookup"><span data-stu-id="013db-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-211">P1</span><span class="sxs-lookup"><span data-stu-id="013db-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-212">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-213">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-214">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-214">Yes</span></span> </p>
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
<span data-ttu-id="013db-215">O1</span><span class="sxs-lookup"><span data-stu-id="013db-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-216">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-217">QL1</span><span class="sxs-lookup"><span data-stu-id="013db-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-218">P1</span><span class="sxs-lookup"><span data-stu-id="013db-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-219">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-220">№</span><span class="sxs-lookup"><span data-stu-id="013db-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-221">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-222">Жарамды</span><span class="sxs-lookup"><span data-stu-id="013db-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="013db-223">P1 жобасындағы уақыт және төлемдер QL1 баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="013db-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="013db-224">P1 жобасындағы шығыс QL2 баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="013db-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="013db-225">Әр баға ұсыну жолына енгізілгенде қабаттасу жоқ, сондықтан ол жарамды.</span><span class="sxs-lookup"><span data-stu-id="013db-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="013db-226">O1</span><span class="sxs-lookup"><span data-stu-id="013db-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-227">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-228">QL2</span><span class="sxs-lookup"><span data-stu-id="013db-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-229">P1</span><span class="sxs-lookup"><span data-stu-id="013db-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-230">№</span><span class="sxs-lookup"><span data-stu-id="013db-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-231">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-232">№</span><span class="sxs-lookup"><span data-stu-id="013db-232">No</span></span> </p>
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
<span data-ttu-id="013db-233">O1</span><span class="sxs-lookup"><span data-stu-id="013db-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-234">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-235">QL1</span><span class="sxs-lookup"><span data-stu-id="013db-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-236">P1</span><span class="sxs-lookup"><span data-stu-id="013db-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-237">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-238">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-239">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-240">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="013db-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-241">Жоғарыдағы №1 ережені бұзу</span><span class="sxs-lookup"><span data-stu-id="013db-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="013db-242">Q1 бүкіл Р1 жобасына арналған уақыт, шығыстар мен төлемдерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="013db-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="013db-243">QL2 бүкіл P1 жобасына арналған уақыт, шығыстар және төлемдерді қамтиды және Q1 баға ұсыну жолына енгізілгендермен қабаттасады.</span><span class="sxs-lookup"><span data-stu-id="013db-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="013db-244">O1</span><span class="sxs-lookup"><span data-stu-id="013db-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-245">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-246">QL2</span><span class="sxs-lookup"><span data-stu-id="013db-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-247">P1</span><span class="sxs-lookup"><span data-stu-id="013db-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-248">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-249">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-250">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-250">Yes</span></span> </p>
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
<span data-ttu-id="013db-251">O1</span><span class="sxs-lookup"><span data-stu-id="013db-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-252">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-253">QL1</span><span class="sxs-lookup"><span data-stu-id="013db-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-254">P1</span><span class="sxs-lookup"><span data-stu-id="013db-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-255">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-256">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-257">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="013db-258">Жарамды</span><span class="sxs-lookup"><span data-stu-id="013db-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-259">№2 ереже негізінде, Q1 және Q2 - бір мүмкіндіктегі екі баға ұсыну жолы, сондықтан екеуі де жобаның бірдей компоненттерін бағалай алады.</span><span class="sxs-lookup"><span data-stu-id="013db-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="013db-260">O1</span><span class="sxs-lookup"><span data-stu-id="013db-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-261">Q2</span><span class="sxs-lookup"><span data-stu-id="013db-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-262">Q2 баға ұсыну жолындағы QL1</span><span class="sxs-lookup"><span data-stu-id="013db-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-263">P1</span><span class="sxs-lookup"><span data-stu-id="013db-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-264">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-265">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-266">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-266">Yes</span></span> </p>
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
<span data-ttu-id="013db-267">O1</span><span class="sxs-lookup"><span data-stu-id="013db-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-268">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-269">QL1</span><span class="sxs-lookup"><span data-stu-id="013db-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-270">P1</span><span class="sxs-lookup"><span data-stu-id="013db-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-271">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-272">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-273">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="013db-274">Жарамды</span><span class="sxs-lookup"><span data-stu-id="013db-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="013db-275">№3 ереже негізінде, Q1 және Q2 - әртүрлі мүмкіндіктегі екі баға ұсыну жолы, сондықтан екеуі де бірдей жобаның бірдей компоненттерін бағалай алмайды.</span><span class="sxs-lookup"><span data-stu-id="013db-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="013db-276">O2</span><span class="sxs-lookup"><span data-stu-id="013db-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="013db-277">Т1</span><span class="sxs-lookup"><span data-stu-id="013db-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-278">QL1</span><span class="sxs-lookup"><span data-stu-id="013db-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-279">P1</span><span class="sxs-lookup"><span data-stu-id="013db-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-280">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="013db-281">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="013db-282">Иә</span><span class="sxs-lookup"><span data-stu-id="013db-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="013db-283">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="013db-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

