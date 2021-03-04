---
title: Жоба кезеңдері бизнес процесінің ағынын қалай теңшеуге болады?
description: Жоба кезеңдері бизнес процесінің ағынын реттеу жолы туралы жалпы ақпарат.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
ms.topic: article
author: JohnPBurrows
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d0168f187e6b0880713aac04bd87dbc2209197d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149010"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a><span data-ttu-id="5331d-103">Жоба кезеңдері бизнес процесінің ағынын қалай теңшеуге болады?</span><span class="sxs-lookup"><span data-stu-id="5331d-103">How do I customize the Project Stages business process flow?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

<span data-ttu-id="5331d-104">Жоба кезеңдері бизнес процесінің ағынындағы кезеңдер аттары болжалды ағылшын атауларына (**Quote**, **Plan**, **Close**) сәйкес болуы керек Project Service бағдарламасының бұрынғы нұсқаларында белгілі шектеу бар.</span><span class="sxs-lookup"><span data-stu-id="5331d-104">There's a known limitation in earlier versions of the Project Service application that the names of the stages in the Project Stages business process flow must exactly match the expected English names (**Quote**, **Plan**, **Close**).</span></span> <span data-ttu-id="5331d-105">Болмаса, ағылшын кезең атауларына байланысты бизнес логикасы болжанғандай жұмыс істемейді.</span><span class="sxs-lookup"><span data-stu-id="5331d-105">Otherwise, the business logic, which relies on the English stage names, doesn't work as expected.</span></span> <span data-ttu-id="5331d-106">Сол себепті, жоба пішінінде қолжетімді **Процесті ауыстыру** немесе **Процесті өңдеу** сияқты таныс әрекеттерді көрмейсіз және бизнес процесінің ағынын теңшеу орындалмайды.</span><span class="sxs-lookup"><span data-stu-id="5331d-106">That's why you don't see familiar actions such as **Switch Process** or **Edit Process** available on the project form, and customizing the business process flow isn't encouraged.</span></span> 

<span data-ttu-id="5331d-107">Бұл шектеу 2.4.5.48 және кейінгі нұсқада қарастырылған.</span><span class="sxs-lookup"><span data-stu-id="5331d-107">This limitation has been addressed in version 2.4.5.48 and later.</span></span> <span data-ttu-id="5331d-108">Әдепкі бизнес процесі ағынын алдыңғы нұсқалар үшін реттеу керек болса, бұл мақалада ұсынылған уақытша шешімдер берілген.</span><span class="sxs-lookup"><span data-stu-id="5331d-108">This article provides suggested workarounds if you need to customize the default business process flow for earlier versions.</span></span>  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a><span data-ttu-id="5331d-109">Бизнес логика ағылшын кезең атауларымен нақты сәйкестікті талап етеді</span><span class="sxs-lookup"><span data-stu-id="5331d-109">Business logic requires an exact match with English stage names</span></span>

<span data-ttu-id="5331d-110">Жоба кезеңдері бизнес процесінің ағынына бағдарламадағы келесі әрекеттерге әкелетін бизнес логика кіреді:</span><span class="sxs-lookup"><span data-stu-id="5331d-110">The Project Stages business process flow includes business logic that drives the following behaviors in the app:</span></span>
- <span data-ttu-id="5331d-111">Жоба баға ұсынумен байланысты болса, код бизнес процесінің ағынын **Баға ұсыну** кезеңіне орнатады.</span><span class="sxs-lookup"><span data-stu-id="5331d-111">When the project is associated with a quote, the code sets the business process flow to the **Quote** stage.</span></span>
- <span data-ttu-id="5331d-112">Жоба баға келісім-шартпен байланысты болса, код бизнес процесінің ағынын **Жоспар** кезеңіне орнатады.</span><span class="sxs-lookup"><span data-stu-id="5331d-112">When the project is associated with a contract, the code sets the business process flow to the **Plan** stage.</span></span>
- <span data-ttu-id="5331d-113">Бизнес процесінің ағыны **Жабу** кезеңіне ауыстырылса, жоба жазбасы өшіріледі.</span><span class="sxs-lookup"><span data-stu-id="5331d-113">When the business process flow is advanced to the **Close** stage, the project record is deactivated.</span></span> <span data-ttu-id="5331d-114">Жоба өшірілсе, жоба пішіні мен жұмыс декомпозициясының құрылымы (WBS) тек оқуға арналған күйіне орнатылады, аты бар ресурс тапсырыстары шығарылады және байланысты бағатізбелер өшіріледі.</span><span class="sxs-lookup"><span data-stu-id="5331d-114">When the project is deactivated, the project form and work breakdown structure (WBS) are set to read-only, the named resource bookings are released, and any associated price lists are deactivated.</span></span>

<span data-ttu-id="5331d-115">Бұл бизнес логикасы жоба кезеңдерінің ағылшын атауларына байланысты.</span><span class="sxs-lookup"><span data-stu-id="5331d-115">This business logic relies on the English names for the project stages.</span></span> <span data-ttu-id="5331d-116">Ағылшын кезең атауларындағы осы тәуелділік Жоба кезеңдері бизнес процесінің ағынының теңшелмеуінің негізгі себебі болғандықтан, жоба нысанында **Процесті ауыстыру** немесе **Процесті өңдеу** сияқты жалпы бизнес процесінің ағыны әрекеттерін көрмейсіз.</span><span class="sxs-lookup"><span data-stu-id="5331d-116">This dependency on the English stage names is the main reason why customization of the Project Stages business process flow isn't encouraged, as well as why you don’t see the common business process flow actions like **Switch Process** or **Edit Process** on the project entity.</span></span>

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a><span data-ttu-id="5331d-117">Кезең атаулары ағылшын атауларына сәйкес келмеген жағдайда не орын алады?</span><span class="sxs-lookup"><span data-stu-id="5331d-117">What happens if the stage names don't match the English names?</span></span>

<span data-ttu-id="5331d-118">8.2 платформасындағы Project Service бағдарламасының 1.x нұсқасында бизнес процесінің ағынындағы кезең атаулары ағылшын кезең атауларына нақты сәйкес келмесе, баға ұсынулар немесе келісім-шарттар үшін дұрыс кезеңді орнататын немесе жобаны жабатын бизнес логикасы еленбейді.</span><span class="sxs-lookup"><span data-stu-id="5331d-118">In the Project Service app version 1.x on the 8.2 platform, when the stage names in the business process flow don’t match the English stage names exactly, the business logic that sets the right stage for quotes or contracts, or that closes the project, is skipped.</span></span> <span data-ttu-id="5331d-119">Ешбір қате туралы хабарлар көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="5331d-119">No error messages are displayed.</span></span> <span data-ttu-id="5331d-120">Сол себепті, Жоба кезеңдері бизнес процесінің ағынын теңшей алатыныңызды көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="5331d-120">Therefore it appears that you are able to customize the Project Stages business process flow.</span></span> <span data-ttu-id="5331d-121">Дегенмен, баға ұсынулар, келісім-шарттар және жоба жабу үшін жұмыс істейтін автоматты процестерді көрмейсіз.</span><span class="sxs-lookup"><span data-stu-id="5331d-121">However, you won’t see any of the automatic processes working for quotes, contracts, and project close.</span></span>

<span data-ttu-id="5331d-122">9.0 платформасындағы Project Service бағдарламасының 2.4.4.30 немесе одан бұрынғы нұсқасында бизнес процесінің ағынының бизнес логикасын қайта жазуды талап ететін бизнес процесінің ағындарына айтарлықтай құрылымдық өзгеріс жасалды.</span><span class="sxs-lookup"><span data-stu-id="5331d-122">In the Project Service app version 2.4.4.30 or earlier on the 9.0 platform, there was a significant architectural change to business process flows, which required a re-write of the business process flow business logic.</span></span> <span data-ttu-id="5331d-123">Нәтижесінде, процесс кезеңі атаулары болжалды ағылшын атауларына сәйкес келмесе, қате туралы хабар аласыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-123">As a result, if the process stage names don’t match the expected English names, you do receive an error message.</span></span> 

<span data-ttu-id="5331d-124">Сол себепті, жоба нысаны үшін Жоба кезеңі бизнес процесінің ағынын теңшеу керек болса, **Баға ұсыну**, **Жоспар** және **Жабу** кезеңдерін сол күйінде сақтай отырып жоба нысанының әдепкі бизнес процесінің ағынына брендтің жаңа кезеңдерін ғана қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-124">Therefore, if you want to customize the Project Stages business process flow for the project entity, you can only add brand new stages to the default business process flow for the project entity, while keeping the **Quote**, **Plan**, and **Close** stages as-is.</span></span> <span data-ttu-id="5331d-125">Бұл шектеу бизнес процесінің ағынында ағылшын кезең атауларын күтетін бизнес логикасынан ешбір қателер алмағаныңызды қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="5331d-125">This restriction ensures that you don’t get errors from the business logic that expects the English stage names in the business process flow.</span></span>

<span data-ttu-id="5331d-126">2.4.5.48 немесе кейінгі нұсқада осы мақалада сипатталған бизнес логикасы жоба нысанының әдепкі бизнес процесі ағынынан алынып тасталған.</span><span class="sxs-lookup"><span data-stu-id="5331d-126">In version 2.4.5.48 or later, the business logic described in this article has been removed from the default business process flow for the project entity.</span></span> <span data-ttu-id="5331d-127">Осы немесе одан кейінгі нұсқаға жаңарту әдепкі бизнес процесінің ағынын біреуімен теңшеуге немесе ауыстыруға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="5331d-127">Upgrading to that version or later will let you customize or replace the default business process flow with one of your own.</span></span> 

## <a name="workarounds-for-earlier-versions"></a><span data-ttu-id="5331d-128">Бұрынғы нұсқаларының уақытша шешімдері</span><span class="sxs-lookup"><span data-stu-id="5331d-128">Workarounds for earlier versions</span></span>

<span data-ttu-id="5331d-129">Жаңарту опциясы болмаса, жоба нысанының Жоба кезеңдері бизнес процесінің ағынын осы екі жолдың біреуімен теңшей аласыз:</span><span class="sxs-lookup"><span data-stu-id="5331d-129">If upgrading isn't an option, you can customize the Project Stages business process flow for the project entity in one of these two ways:</span></span>

1. <span data-ttu-id="5331d-130">**Баға ұсыну**, **Жоспар** және **Жабу** ағылшын кезең атауларын сақтай отырып, әдепкі конфигурацияға қосымша кезеңдер қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-130">Add additional stages to the default configuration, while retaining the English stage names for **Quote**, **Plan**, and **Close**.</span></span>


![Әдепкі конфигурацияға кезеңдер қосу скриншоты](media/FAQ-Customize-BPF-1.png)
 
2. <span data-ttu-id="5331d-132">Жеке бизнес процесінің ағынын жасау және жоба нысанының негізгі бизнес процесінің ағынын жасау кез келген қажетті кезең атауларын иелену мүмкіндігін береді.</span><span class="sxs-lookup"><span data-stu-id="5331d-132">Create your own business process flow and make it the primary business process flow for the project entity, which lets you have any stage names you want.</span></span> <span data-ttu-id="5331d-133">Дегенмен, **Баға ұсыну**, **Жоспар** және **Жабу** стандартты жоба кезеңдерін пайдалану керек болса, теңшелетін кезең атауларынан ауытқытатын кейбір теңшеулерді орындауды керек етеді.</span><span class="sxs-lookup"><span data-stu-id="5331d-133">However, if you want to use the same standard project stages **Quote**, **Plan**, and **Close**, you need to do some customizations that are driven off your custom stage names.</span></span> <span data-ttu-id="5331d-134">Ең кешенді логикасы - жобаны жабу, яғни жоба жазбасын өшіру арқылы іске қоса аласыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-134">The more complex logic is in the closing of the project, which you can still trigger by just deactivating the project record.</span></span>

![BPF реттеуі](media/FAQ-Customize-BPF-2.png)

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a><span data-ttu-id="5331d-136">9.0 платформасындағы Project Service бағдарламасының 2.4.4.30 немесе одан бұрынғы нұсқасының қосымша ескертпелері</span><span class="sxs-lookup"><span data-stu-id="5331d-136">Additional considerations for Project Service app version 2.4.4.30 or earlier on platform 9.0</span></span>

<span data-ttu-id="5331d-137">9.0 платформасындағы Project Service 2.4.4.30 немесе одан бұрынғы нұсқасында **Кезең бойынша жобалау** сызбасында пайдаланылатын жоба нысанындағы **Кезең аты** өрісінің теңшелетін бизнес процесінің ағыны және жобалар тізімі жаңартылмайды, себебі ол әдепкі Процесс кезеңдері бизнес процесінің ағынымен байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="5331d-137">In Project Service 2.4.4.30 or earlier on platform 9.0, with a custom business process flow the **Stage Name** field on the project entity used in the **Project By Stage** chart and project list views won’t update, because it’s coupled to the default Project Stages business process flow.</span></span> <span data-ttu-id="5331d-138">Бұл мәселені келесі қадамдармен жібере аласыз:</span><span class="sxs-lookup"><span data-stu-id="5331d-138">You can address this issue with the following steps:</span></span>

- <span data-ttu-id="5331d-139">Ағымдағы бизнес процесінің ағыны кезеңі пайдаланушы арқылы теңшелетін бизнес процесінің ағыны көмегімен алу үшін үшін теңшелетін өрісті қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-139">Add a custom field to capture the current business process flow stage that is updated as the user advances through the custom business process flow.</span></span>

- <span data-ttu-id="5331d-140">Әдепкі конфигурация орнына теңшелетін өріспен жұмыс істеу үшін **Кезең бойынша жобалау** сызбасын өзгертіңіз.</span><span class="sxs-lookup"><span data-stu-id="5331d-140">Modify the **Project By Stage** chart to work with your custom field instead of the default configuration.</span></span>

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a><span data-ttu-id="5331d-141">Жоба нысанының жеке бизнес процесінің ағынын жасау қадамдары</span><span class="sxs-lookup"><span data-stu-id="5331d-141">Steps to create your own business process flow for the project entity</span></span>

<span data-ttu-id="5331d-142">Жоба нысанының жеке бизнес процесінің ағынын жасау үшін келесі әрекеттерді орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="5331d-142">To create your own business process flow for the project entity do the following:</span></span>

1. <span data-ttu-id="5331d-143">**Параметрлер** > **Процесс орталығы** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="5331d-143">Go to **Settings** > **Process Center**.</span></span> <span data-ttu-id="5331d-144">Project Service бизнес логикасының көшірмелеріне байланысты процесс кезеңдері бизнес процесінің ағынын көшіруге болмайды.</span><span class="sxs-lookup"><span data-stu-id="5331d-144">Don’t copy the Project Stages business process flow because that also copies the Project Service business logic.</span></span>

  ![Процессті жасау](media/FAQ-Customize-BPF-3.png)

2. <span data-ttu-id="5331d-146">Қажетті кезең атауларын жасау үшін Процесс құрастырушысын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-146">Use the Process Designer to create the stage names you want.</span></span> <span data-ttu-id="5331d-147">**Баға ұсыну**, **Жоспар** және **Жабу** әдепкі кезеңдері ретінде бір функция қажет болса, теңшелетін бизнес процесінің ағыны кезеңі атаулары негізінде жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-147">If you want the same functionality as the default stages for **Quote**, **Plan**, and **Close**, you’ll have to create that based on your custom business process flow’s stage names.</span></span>

   ![BPF теңшеуге пайдаланылатын процесс құрастырушысының скриншоты](media/FAQ-Customize-BPF-4.png) 

3. <span data-ttu-id="5331d-149">Процесс құрастырушысында Жоба кезеңдері бизнес процесінің ағынын тізім үстіне жылжыту арқылы жоба нысанының теңшелетін бизнес процесінің ағынын, негізгі бизнес процесс ағынын жасау үшін **Процесс ағынын реттеу** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-149">In the Process Designer, click **Order Process Flow** to make the custom business process flow the primary business process flow for the project entity by moving it above the Project Stages business process flow to the top of the list.</span></span>


   [<span data-ttu-id="5331d-150">Процесс ағынын реттеу пәрменін қолдану скриншоты</span><span class="sxs-lookup"><span data-stu-id="5331d-150">Screenshot of using Order Process Flow</span></span>](media/FAQ-Customize-BPF-5-720.png)

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a><span data-ttu-id="5331d-151">Келесі қадамдар 9.0 платформасындағы Project Service бағдарламасының 2.4.4.30 немесе одан бұрынғы нұсқасына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="5331d-151">The following steps apply to Project Service app 2.4.4.30 or earlier on the 9.0 platform</span></span>

4. <span data-ttu-id="5331d-152">Теңшелетін бизнес процесінің ағынындағы теңшелетін кезеңдерді қамту үшін жоба нысанына жаңа теңшелетін өріс қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="5331d-152">Add a new custom field to the project entity to capture the custom stages in your custom business process flow.</span></span> <span data-ttu-id="5331d-153">Теңшелетін бизнес процесінің ағынындағы кезең жаңартылса, осы өрісті жаңарту үшін бизнес логикасын (қосылатын модулін/жұмыс ағынын) қосу керек болады.</span><span class="sxs-lookup"><span data-stu-id="5331d-153">You’ll need to add business logic (plugin/workflow) to update this field when the stage on the custom business process flow is updated.</span></span>

   ![Жоба нысанын теңшеу скриншоты](media/FAQ-Customize-BPF-6-720.png)

5. <span data-ttu-id="5331d-155">Кезеңдердің жаңа теңшелетін өрісін пайдалану үшін **Кезең бойынша жобалау** сызбасын өзгертіңіз.</span><span class="sxs-lookup"><span data-stu-id="5331d-155">Modify the **Project By Stage** chart to use your new custom field for stages.</span></span>

   ![Кезең бойынша жобалау сызбасын пайдалану скриншоты](media/FAQ-Customize-BPF-7-720.png)

6. <span data-ttu-id="5331d-157">Кезеңдердің жаңа теңшелетін өрісін қосу үшін жоба нысаны көріністерін өзгертіңіз.</span><span class="sxs-lookup"><span data-stu-id="5331d-157">Modify any views for the project entity to include your new custom field for stages.</span></span>

   ![Жоба нысаны көріністерін өзгерту скриншоты](media/FAQ-Customize-BPF-8-720.png)

