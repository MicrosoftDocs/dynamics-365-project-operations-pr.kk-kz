---
title: Жобаға негізделген баға ұсыну жолдарына шолу
description: Бұл тақырыпта Project Operations бағдарламасындағы жоба жұмысына арналған жобаға негізделген баға ұсыну жолын пайдалану туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ea54d83b1e26d1ee3520dbfab9ba56ffd1191dc9
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181864"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="8c4ff-103">Жобаға негізделген баға ұсыну жолдарына шолу</span><span class="sxs-lookup"><span data-stu-id="8c4ff-103">Project-based quote lines overview</span></span>

<span data-ttu-id="8c4ff-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="8c4ff-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8c4ff-105">Жобаға негізделген баға ұсыну жолдары жоба жұмысын бағалауға көмектесуге арналған.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="8c4ff-106">Жобаға негізделген баға ұсыну жолының құрылымы жоба болжамдары үшін келесі тұжырымдамалармен кеңейтілген:</span><span class="sxs-lookup"><span data-stu-id="8c4ff-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="8c4ff-107">Есепшот ұсыну әдісі</span><span class="sxs-lookup"><span data-stu-id="8c4ff-107">Billing Method</span></span>
- <span data-ttu-id="8c4ff-108">Жобаны салыстыру</span><span class="sxs-lookup"><span data-stu-id="8c4ff-108">Project Mapping</span></span>
- <span data-ttu-id="8c4ff-109">Қамтылған транзакция кластары</span><span class="sxs-lookup"><span data-stu-id="8c4ff-109">Included Transaction classes</span></span>
- <span data-ttu-id="8c4ff-110">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="8c4ff-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="8c4ff-111">Төлем қабілеттілігін орнату</span><span class="sxs-lookup"><span data-stu-id="8c4ff-111">Chargeability setup</span></span>
- <span data-ttu-id="8c4ff-112">Баға ұсыну жолының мәліметтері көмегімен бағалау</span><span class="sxs-lookup"><span data-stu-id="8c4ff-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="8c4ff-113">Баға ұсыну жолының тұтынушылары</span><span class="sxs-lookup"><span data-stu-id="8c4ff-113">Quote line Customers</span></span>

<span data-ttu-id="8c4ff-114">Келесі кестеде жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасындағы өрістері туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="8c4ff-115">Бұл өрістер жоба жұмысын егжей-тегжейлі, алдын ала болжам негізін орнатуға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="8c4ff-116">**Өріс**</span><span class="sxs-lookup"><span data-stu-id="8c4ff-116">**Field**</span></span> | <span data-ttu-id="8c4ff-117">**Сипаттамасы**</span><span class="sxs-lookup"><span data-stu-id="8c4ff-117">**Description**</span></span> | <span data-ttu-id="8c4ff-118">**Төменгі әсер**</span><span class="sxs-lookup"><span data-stu-id="8c4ff-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8c4ff-119">Атауы</span><span class="sxs-lookup"><span data-stu-id="8c4ff-119">Name</span></span> | <span data-ttu-id="8c4ff-120">Бағаланатын баға ұсынудың жеке компонентін анықтауға көмектесетін баға ұсыну жолының атауы.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="8c4ff-121">Баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-122">Есепшот ұсыну әдісі</span><span class="sxs-lookup"><span data-stu-id="8c4ff-122">Billing Method</span></span> | <span data-ttu-id="8c4ff-123">Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолының сәйкес өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="8c4ff-124">Бұл өрісте Dynamics 365 Project Operations тарапынан қолдау көрсетілетін екі негізгі келісілген үлгілер қамтылған:</span><span class="sxs-lookup"><span data-stu-id="8c4ff-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="8c4ff-125">- Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="8c4ff-125">- Fixed price</span></span></br><span data-ttu-id="8c4ff-126">- Уақыт және материал.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-126">- Time and material.</span></span>| <span data-ttu-id="8c4ff-127">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-128">Project</span><span class="sxs-lookup"><span data-stu-id="8c4ff-128">Project</span></span> | <span data-ttu-id="8c4ff-129">Осы қосымша өрісті осы келісім бойынша жұмысты орындау мақсатында пайдаланылатын жобаны анықтау үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="8c4ff-130">Жоба баға ұсыну жолымен байланыстырылған кезде, ақылы тапсырмаларды орнатуға, сондай-ақ баға ұсыну жолын баға ұсыну жолының мәліметтері ретінде жоба негізінде болжауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="8c4ff-131">Жоба жобаға негізделген баға ұсыну жолымен салыстырылмаған кезде, баға әр баға ұсыну жолының мәліметтерін құру арқылы қолмен жасалуы керек.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="8c4ff-132">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-133">Уақытпен қоса</span><span class="sxs-lookup"><span data-stu-id="8c4ff-133">Include Time</span></span> | <span data-ttu-id="8c4ff-134">Таңдалған жобадағы уақыт транзакциялары немесе еңбек құны осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="8c4ff-135">Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="8c4ff-136">Баға ұсыну жолындағы болжамға уақыт транзакциялары немесе еңбек құны қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="8c4ff-137">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-138">Шығыспен қоса</span><span class="sxs-lookup"><span data-stu-id="8c4ff-138">Include Expense</span></span> | <span data-ttu-id="8c4ff-139">Таңдалған жобадағы шығыс құны осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="8c4ff-140">Баға ұсыну жолындағы болжамға шығыс құны қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="8c4ff-141">Баға ұсыну жолындағы болжамға шығыс құны қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="8c4ff-142">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-143">Ақымен қоса</span><span class="sxs-lookup"><span data-stu-id="8c4ff-143">Include Fee</span></span> | <span data-ttu-id="8c4ff-144">Таңдалған жобадағы төлемдер осы баға ұсыну жолындағы болжамға қосылатын жағдайда **Иә**/**Жоқ** жалаушасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="8c4ff-145">Баға ұсыну жолындағы болжамға төлемдер қосылмайтын болған жағдайда, **Жоқ** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="8c4ff-146">Баға ұсыну жолындағы болжамға төлемдер қосылатын жағдайда, **Иә** мәні көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="8c4ff-147">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-148">Баға ұсынылған көлем</span><span class="sxs-lookup"><span data-stu-id="8c4ff-148">Quoted Amount</span></span> | <span data-ttu-id="8c4ff-149">Бұл тұтынушыға осы жобаға негізделген баға ұсыну жолы бойынша болжамдалған барлық жұмыстар үшін ұсынылатын сома.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="8c4ff-150">Мүмкіндіктен баға ұсынысы жасалған кезде, бұл мән мүмкіндік жолындағы **Тұтынушы бюджеті** өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="8c4ff-151">Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі мөлшерден жинақталады.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="8c4ff-152">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-153">Болжалды салық</span><span class="sxs-lookup"><span data-stu-id="8c4ff-153">Estimated Tax</span></span> | <span data-ttu-id="8c4ff-154">Бұл пайдаланушыға баға ұсыну жолына салықтың есептелген мөлшерін қосатын өңделетін өріс.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="8c4ff-155">Жобаға негізделген баға ұсыну жолында жол мәліметтері болған кезде, бұл өріс өңдеу үшін бұғатталады және баға ұсыну жолындағы мәліметтердегі салық мөлшерінен жинақталады.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="8c4ff-156">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-157">Салықтан кейінгі баға ұсыну сомасы</span><span class="sxs-lookup"><span data-stu-id="8c4ff-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="8c4ff-158">Бұл өріс салықтан кейінгі баға ұсыну жолының сомасы болып табылады және тек оқуға арналған.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="8c4ff-159">Бұл өрістегі сома *Ұсынылған сома + Салық* ретінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="8c4ff-160">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-161">Асырмау шегі</span><span class="sxs-lookup"><span data-stu-id="8c4ff-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="8c4ff-162">Бұл өрісті өңдеуге болады және тек **Уақыт және материал** төлем әдісіне ие жобаға негізделген баға ұсыну жолдарында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="8c4ff-163">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="8c4ff-164">Тұтынушы бюджеті</span><span class="sxs-lookup"><span data-stu-id="8c4ff-164">Customer Budget</span></span> | <span data-ttu-id="8c4ff-165">Бұл өрісті өңдеуге болады және мүмкіндіктен баға ұсынуы жасалған жағдайда, мүмкіндік жолындағы сәйкес өрісінен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="8c4ff-166">Бұл өріс мәні баға ұсынуын ұтып алған кезде, осы баға ұсыну жолынан жасалған жоба келісімшартының жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="8c4ff-167">Жобаға негізделген баға ұсыну жолдарының Жалпы қойыншасындағы өрістерді тексеру ережелері</span><span class="sxs-lookup"><span data-stu-id="8c4ff-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="8c4ff-168">**1-ереже** : Таңдалған жоба бойынша белгілі бір транзакция класын тек бір баға ұсыныстарының жобаға негізделген баға ұсыну жолына енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="8c4ff-169">**2-ереже**: Егер мүмкіндікте бірнеше баға ұсыныстары болса, онда барлығы бірдей жобаға сілтеме жасайтын және бір транзакция класын қамтитын әртүрлі баға ұсыныстарында баға ұсыну жолдары болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="8c4ff-170">**3-ереже**: Егер баға ұсыныстары бірдей мүмкіндікке тиесілі болмаса, олар бірдей жоба мен транзакция класын қамтуы мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="8c4ff-171">
                    <strong>Мүмкіндік</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="8c4ff-172">
                    <strong>Баға ұсынысы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="8c4ff-173">
                    <strong>Баға ұсыну жолы</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="8c4ff-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="8c4ff-175">
                    <strong>Уақытпен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="8c4ff-176">
                    <strong>Шығыспен қоса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="8c4ff-177">
                    <strong>Қамту</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="8c4ff-178">
                    <strong>төлем</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="8c4ff-179">
                    <strong>Жарамды/ Жарамсыз</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="8c4ff-180">
                    <strong>Себеп</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8c4ff-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="8c4ff-181">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-182">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-183">QL1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-184">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-185">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-186">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-187">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-188">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="8c4ff-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-189">№1 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-189">Violation of Rule #1.</span></span> <span data-ttu-id="8c4ff-190">Р1 жобасындағы уақыт, шығыс және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="8c4ff-191">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-192">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-193">QL2</span><span class="sxs-lookup"><span data-stu-id="8c4ff-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-194">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-195">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-196">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-197">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-197">Yes</span></span> </p>
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
<span data-ttu-id="8c4ff-198">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-199">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-200">QL1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-201">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-202">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-203">№</span><span class="sxs-lookup"><span data-stu-id="8c4ff-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-204">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-205">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="8c4ff-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-206">№1 ережені бұзу.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-206">Violation of Rule #1.</span></span> <span data-ttu-id="8c4ff-207">Р1 жобасындағы уақыт және төлемдер QL1 және QL2 баға ұсыну жолдарына бірдей енгізілген.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="8c4ff-208">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-209">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-210">QL2</span><span class="sxs-lookup"><span data-stu-id="8c4ff-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-211">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-212">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-213">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-214">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-214">Yes</span></span> </p>
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
<span data-ttu-id="8c4ff-215">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-216">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-217">QL1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-218">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-219">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-220">№</span><span class="sxs-lookup"><span data-stu-id="8c4ff-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-221">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-222">Жарамды</span><span class="sxs-lookup"><span data-stu-id="8c4ff-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="8c4ff-223">P1 жобасындағы уақыт және төлемдер QL1 баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="8c4ff-224">P1 жобасындағы шығыс QL2 баға ұсыну жолына енгізілген.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="8c4ff-225">Әр баға ұсыну жолына енгізілгенде қабаттасу жоқ, сондықтан ол жарамды.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="8c4ff-226">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-227">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-228">QL2</span><span class="sxs-lookup"><span data-stu-id="8c4ff-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-229">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-230">№</span><span class="sxs-lookup"><span data-stu-id="8c4ff-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-231">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-232">№</span><span class="sxs-lookup"><span data-stu-id="8c4ff-232">No</span></span> </p>
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
<span data-ttu-id="8c4ff-233">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-234">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-235">QL1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-236">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-237">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-238">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-239">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-240">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="8c4ff-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-241">Жоғарыдағы №1 ережені бұзу</span><span class="sxs-lookup"><span data-stu-id="8c4ff-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="8c4ff-242">Q1 бүкіл Р1 жобасына арналған уақыт, шығыстар мен төлемдерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="8c4ff-243">QL2 бүкіл P1 жобасына арналған уақыт, шығыстар және төлемдерді қамтиды және Q1 баға ұсыну жолына енгізілгендермен қабаттасады.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="8c4ff-244">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-245">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-246">QL2</span><span class="sxs-lookup"><span data-stu-id="8c4ff-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-247">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-248">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-249">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-250">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-250">Yes</span></span> </p>
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
<span data-ttu-id="8c4ff-251">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-252">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-253">QL1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-254">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-255">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-256">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-257">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="8c4ff-258">Жарамды</span><span class="sxs-lookup"><span data-stu-id="8c4ff-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-259">№2 ереже негізінде, Q1 және Q2 - бір мүмкіндіктегі екі баға ұсыну жолы, сондықтан екеуі де жобаның бірдей компоненттерін бағалай алады.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="8c4ff-260">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-261">Q2</span><span class="sxs-lookup"><span data-stu-id="8c4ff-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-262">Q2 баға ұсыну жолындағы QL1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-263">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-264">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-265">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-266">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-266">Yes</span></span> </p>
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
<span data-ttu-id="8c4ff-267">O1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-268">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-269">QL1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-270">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-271">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-272">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-273">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="8c4ff-274">Жарамды</span><span class="sxs-lookup"><span data-stu-id="8c4ff-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8c4ff-275">№3 ереже негізінде, Q1 және Q2 - әртүрлі мүмкіндіктегі екі баға ұсыну жолы, сондықтан екеуі де бірдей жобаның бірдей компоненттерін бағалай алмайды.</span><span class="sxs-lookup"><span data-stu-id="8c4ff-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="8c4ff-276">O2</span><span class="sxs-lookup"><span data-stu-id="8c4ff-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="8c4ff-277">Т1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-278">QL1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-279">P1</span><span class="sxs-lookup"><span data-stu-id="8c4ff-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-280">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8c4ff-281">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8c4ff-282">Иә</span><span class="sxs-lookup"><span data-stu-id="8c4ff-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="8c4ff-283">Жарамсыз</span><span class="sxs-lookup"><span data-stu-id="8c4ff-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

