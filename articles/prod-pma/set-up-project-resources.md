---
title: Жоба ресурстарын орнату
description: Бұл тақырыпта жоба ресурстарына сұрау орнату туралы ақпарат берілген.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 49e0ca6254518079d2e01d92ac2e31d119468c4b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997698"
---
# <a name="set-up-project-resources"></a><span data-ttu-id="e7dac-103">Жоба ресурстарын орнату</span><span class="sxs-lookup"><span data-stu-id="e7dac-103">Set up project resources</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e7dac-104">Күнтізбені орнатып, оны қызметкермен немесе жұмысшымен байланыстыру керек.</span><span class="sxs-lookup"><span data-stu-id="e7dac-104">You must set up a calendar and associate it with an employee or a worker.</span></span> <span data-ttu-id="e7dac-105">Күнтізбе жобаны және жоба үшін сақталған ресурстардың жұмыс уақытын жоспарлау үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="e7dac-105">The calendar is used to schedule the project and the working time of the resources that are reserved for the project.</span></span> <span data-ttu-id="e7dac-106">Күнтізбені теңшеу кезінде жоба менеджерлері ресурстарды оңтайландыру шеңберінде ресурстарды теңестіре алады.</span><span class="sxs-lookup"><span data-stu-id="e7dac-106">During calendar setup, project managers can do resource leveling as part of resource optimization.</span></span> <span data-ttu-id="e7dac-107">Күнтізбелік кесте негізінде ресурстар шектеулер қойылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e7dac-107">Based on the calendar schedule, restrictions can be put on resources.</span></span> <span data-ttu-id="e7dac-108">Күнтізбені **Күнтізбелер** бетінде орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="e7dac-108">You can set up a calendar on the **Calendars** page.</span></span>

<span data-ttu-id="e7dac-109">Жұмысшыны жоба ресурсы ретінде орнатқан кезде ресурстарды орнататын компанияда жұмыс істейтін жұмысшылардың ішінен таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="e7dac-109">When you set up a worker as a project resource, you can select from workers who work in the company that you're setting up resources for.</span></span> <span data-ttu-id="e7dac-110">Сонымен қатар, ұйымыңыздағы басқа компаниялардың жұмысшыларын таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-110">Alternatively, you can select workers from other companies in your organization.</span></span> <span data-ttu-id="e7dac-111">Бұл жұмысшылар компания ішіндегі ресурстар ретінде белгілі.</span><span class="sxs-lookup"><span data-stu-id="e7dac-111">These workers are known as intercompany resources.</span></span>

<span data-ttu-id="e7dac-112">Келесі процедураларда компанияңызда жұмысшыны жоба ресурсы ретінде орнату амалы және компанияаралық жоба ресурсын қалай орнату керектігі түсіндіріледі.</span><span class="sxs-lookup"><span data-stu-id="e7dac-112">The following procedures explain how to set up a worker as a project resource in your company and how to set up an intercompany project resource.</span></span>

## <a name="set-up-a-worker-as-a-project-resource"></a><span data-ttu-id="e7dac-113">Жұмысшыны жоба ресурсы ретінде орнатыңыз</span><span class="sxs-lookup"><span data-stu-id="e7dac-113">Set up a worker as a project resource</span></span>

1. <span data-ttu-id="e7dac-114">**Жұмысшылар** тізіміндегі **Жұмысшылар** бетінен жоба ресурсы ретінде қосатын жұмысшыны таңдап, жұмысшы жазбасын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-114">On the **Workers** page, in the **Workers** list, select the worker that you're adding as a project resource, and open the worker record.</span></span>
2. <span data-ttu-id="e7dac-115">Әрекеттер тақтасынан **Жоба** &gt; **Орнату** &gt; **Жобаны орнату** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-115">On the Action Pane, select **Project** &gt; **Setup** &gt; **Project setup**.</span></span>
3. <span data-ttu-id="e7dac-116">Күнтізбені таңдап, бетті жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-116">Select a calendar, and then close the page.</span></span>

<span data-ttu-id="e7dac-117">Сондай-ақ ресурс үшін әдепкі жобаларды алдын ала тағайындау түрі ретінде көрсетуге болады.</span><span class="sxs-lookup"><span data-stu-id="e7dac-117">You can also specify default projects for a resource as a type of pre-assignment.</span></span> <span data-ttu-id="e7dac-118">алдын ала тағайындауларды ресурс менеджері немесе жоба менеджері ресурстың қандай жобаларда жұмыс жасайтынын алдын ала білген кезде пайдалануына болады.</span><span class="sxs-lookup"><span data-stu-id="e7dac-118">Pre-assignments can be used when the resource manager or project manager knows which projects the resource will be working on in advance.</span></span> <span data-ttu-id="e7dac-119">Алдын ала тағайындаулар, сондай-ақ, жоба демеушісі немесе тұтынушының сұранысына негізделуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e7dac-119">Pre-assignments can also be based on the request of a project sponsor or customer.</span></span> <span data-ttu-id="e7dac-120">Жобаны алдын ала тағайындау үшін, **Жобаларды тағайындау** бетінен, **Жобалар** қойыншасындағы, **Қалған жобалар** тізімінен лайықты жобаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-120">To pre-assign a project, on the **Assign projects** page, on the **Projects** tab, in the **Remaining projects** list, select the appropriate project.</span></span>

## <a name="set-up-an-intercompany-resource"></a><span data-ttu-id="e7dac-121">Компанияаралық ресурсты орнатыңыз</span><span class="sxs-lookup"><span data-stu-id="e7dac-121">Set up an intercompany resource</span></span>

<span data-ttu-id="e7dac-122">Жұмысшыны компанияаралық ресурс ретінде орнатқан кезде, бұл параметрді несие беруші компания мен қарыз алушы компанияда орындау керек.</span><span class="sxs-lookup"><span data-stu-id="e7dac-122">When you set up a worker as an intercompany resource, you must complete the setup in both the lending company and the borrowing company.</span></span>

### <a name="in-the-lending-company"></a><span data-ttu-id="e7dac-123">Несиелік компанияда</span><span class="sxs-lookup"><span data-stu-id="e7dac-123">In the lending company</span></span>

1. <span data-ttu-id="e7dac-124">"Қаржы" бөлімінде несие беруші компанияның таңдалғанына көз жеткізіп, алдыңғы "Жұмысшыны жоба ресурсы ретінде орнату" бөліміндегі процедурасын орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-124">In Finance, verify that the lending company is selected, and then complete the procedure in the previous section, "Set up a worker as a project resource."</span></span>
2. <span data-ttu-id="e7dac-125">**Компанияаралық шот** бетінен **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-125">On the **Intercompany accounting** page, select **New**.</span></span>
3. <span data-ttu-id="e7dac-126">**Заңды нысан идентификаторы** өрісінен несиелік компанияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-126">In the **Legal entity ID** field, select the lending company.</span></span> <span data-ttu-id="e7dac-127">Қалған өрістерді сәйкесінше толтырып, **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-127">Fill in the remaining fields as appropriate, and then select **Save**.</span></span>
4. <span data-ttu-id="e7dac-128">**Тасымал құны** бетінен **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-128">On the **Transfer price** page, select **New**.</span></span>
5. <span data-ttu-id="e7dac-129">**Қарыз алушы заңды тұлға** өрісінен тиісті компанияны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-129">In the **Borrowing legal entity** field, select the appropriate company.</span></span>
6. <span data-ttu-id="e7dac-130">Қарыз алушы компанияға осы бөлімнің басында жасалған ресурсты ғана беру үшін **Ресурс** өрісінен жасалған ресурстың атауын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-130">To lend the borrowing company only the resource that you created at the beginning of this section, in the **Resource** field, select the name of the resource that you created.</span></span> <span data-ttu-id="e7dac-131">Несие беруші компанияның барлық ресурстарын қарыз алушы компанияға қолжетімді ету үшін **Ресурс** өрісін бос қалдырыңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-131">To make all resources in the lending company available to the borrowing company, leave the **Resource** field blank.</span></span>
7. <span data-ttu-id="e7dac-132">**Жобаны басқару және есеп параметрлері** бетіндегі **Компанияаралық** қойыншасынан **Компанияаралық ресурсты жоспарлауды және уақыт кестелерін іске қосу** опциясын **Иә** мәніне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-132">On the **Project management and accounting parameters** page, on the **Intercompany** tab, set the **Enable intercompany resource scheduling and timesheets** option to **Yes**.</span></span>

### <a name="in-the-borrowing-company"></a><span data-ttu-id="e7dac-133">Қарыз алушы компанияда</span><span class="sxs-lookup"><span data-stu-id="e7dac-133">In the borrowing company</span></span>

- <span data-ttu-id="e7dac-134">**Ресурстар тізімі** бетіндегі іздеу сүзгісіне қарыз алушы компанияның ресурстар тізіміне сол атаудың қосылуын қамтамасыз ету үшін несие беруші компания үшін жасалған ресурстың атын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-134">On the **Resources list** page, in the search filter, enter the name of the resource that you created for the lending company, to verify that the name is included in the resource list for the borrowing company.</span></span>

## <a name="request-project-resources"></a><span data-ttu-id="e7dac-135">Жоба ресурстарын сұрау</span><span class="sxs-lookup"><span data-stu-id="e7dac-135">Request project resources</span></span>
<span data-ttu-id="e7dac-136">Жоба ресурстарын жоспарлау мүмкіндігі ресурс менеджерлеріне жинақталған ресурстарды тек тапсырмаларға немесе жобаларға бөлуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="e7dac-136">The functionality for project resource scheduling only lets resource managers distribute staffed resources on engagements or projects.</span></span> <span data-ttu-id="e7dac-137">Бұл мүмкіндікті қосу үшін келесі тапсырмаларды орындаңыз немесе оларды орындағаныңызға көз жеткізіңіз:</span><span class="sxs-lookup"><span data-stu-id="e7dac-137">To enable this functionality, complete the following tasks, or verify that they have been completed:</span></span>

- <span data-ttu-id="e7dac-138">Тізбектер санын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-138">Set up number sequences.</span></span>
- <span data-ttu-id="e7dac-139">Жобаларды басқару және есепке алу жұмыс ағындарын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-139">Set up project management and accounting workflows.</span></span>
- <span data-ttu-id="e7dac-140">Ресурс сұрауы жұмыс ағындарын іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-140">Enable resource request workflows.</span></span>

<span data-ttu-id="e7dac-141">Алдыңғы тапсырмалар аяқталғаннан кейін қажет болған жағдайда келесі тапсырмаларды орындауға болады:</span><span class="sxs-lookup"><span data-stu-id="e7dac-141">After the preceding tasks have been completed, you can complete the following tasks as you require:</span></span>

- <span data-ttu-id="e7dac-142">Жұмсақ көшірмесі жасалған жинақталған ресурстан сұраныс жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-142">Create a resource request from a soft-booked staffed resource.</span></span>
- <span data-ttu-id="e7dac-143">Ресурс сұрауларын бақылаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-143">Monitor resource requests.</span></span>
- <span data-ttu-id="e7dac-144">Ресурс сұрауларын орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-144">Fulfill resource requests.</span></span>
- <span data-ttu-id="e7dac-145">WBS үлгісінен жинақталған ресурстарды сұраңыз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-145">Request a staffed resource from a WBS.</span></span>
- <span data-ttu-id="e7dac-146">Жобаға ресурстарды жинақталған ресурсты сұратпай-ақ резервтеңіз.</span><span class="sxs-lookup"><span data-stu-id="e7dac-146">Book resources to a project without having a request for a staffed resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]