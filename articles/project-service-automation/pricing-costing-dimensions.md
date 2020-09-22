---
title: Бағалар және шығын өлшемдерінің басты бет
description: Бұл тақырыпта бағалау өлшемдері туралы жалпы мәліметтер беріледі.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 425d7bb8-9015-4f67-b9c9-cf3602e9afe8
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 2379d0d2e038f28a1a8df87a851e9bf7db7fe33f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753047"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="5c0e2-103">Бағалар және шығын өлшемдерінің басты бет</span><span class="sxs-lookup"><span data-stu-id="5c0e2-103">Pricing and costing dimensions home page</span></span>

<span data-ttu-id="5c0e2-104">Бағалар мен шығындарды белгілеу үшін кадрлар ресурстарында қолданылатын өлшемдер екі санатқа бөлінеді:</span><span class="sxs-lookup"><span data-stu-id="5c0e2-104">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="5c0e2-105">Адамдар</span><span class="sxs-lookup"><span data-stu-id="5c0e2-105">People</span></span>
- <span data-ttu-id="5c0e2-106">Жоспарланған жұмыс</span><span class="sxs-lookup"><span data-stu-id="5c0e2-106">Planned work</span></span>

<span data-ttu-id="5c0e2-107">Осыған байланысты, Project Service Automation (PSA) бағдарламасында бағалар өлшемі мәндерінің екі түрі бар:</span><span class="sxs-lookup"><span data-stu-id="5c0e2-107">Because of this, there are two types of pricing dimension values available in Project Service Automation (PSA):</span></span> 

- <span data-ttu-id="5c0e2-108">**Параметрлер жиындары** - мәндер жиынтығы үшін бекітілген тізімдер болып табылатын өлшемдер.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-108">**Option sets** - Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="5c0e2-109">**Нысан негізіндегі мәндер** - әртүрлі мәндер жиынтығы бола алатын өлшемдер.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-109">**Entity-based values** - Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="5c0e2-110">Бағалар өлшемдері</span><span class="sxs-lookup"><span data-stu-id="5c0e2-110">Pricing dimensions</span></span>

<span data-ttu-id="5c0e2-111">PSA бағдарламасы әдепкі бағалар өлшемдерінің жиынтығымен жеткізіледі.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="5c0e2-112">Мұны **Project Service** > **Параметрлер** тармағына өту арқылы көре аласыз.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="5c0e2-113">Параметр жазбасындағы **Сомаға негізделген бағалар өлшемдері** қойыншасында рөлді тексеріңіз, **msdyn_resourcecategory** және ресурстық бөлімше, **msdyn_organizationalunit** параметрінің **Иә** мәніне орнатылған бар **Сатуға қолданылады** және **Құны үшін қолданылады** өрістері бар.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="5c0e2-114">Бұл әр рөл мен бірлік тіркесімінің бағасы мен құнын белгілеуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

!["Сатылымға қолданбалы" параметрі бөлектелген Project Service параметрлерінің скриншоты](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="5c0e2-116">Егер сіз PSA 3 нұсқасына дейін бағалар өлшемдері ретінде рөл мен ұйымдық бөлімшенің дайын өрістерін қолданған болсаңыз, елеулі өзгерістер болмайды.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="5c0e2-117">Project Service қызметін әдеттегідей пайдалануды жалғастыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="5c0e2-118">Егер қосымша атрибуттарды қолдана отырып, ресурстарыңыздың бағасын немесе құнын анықтау қажет болса, реттелген өрістерді, нысандарды және өлшемдерді жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="5c0e2-119">Қосымша ақпарат алу үшін, келесі тақырыптарды қараңыз, бірақ процедураларды төменде көрсетілген ретпен орындау керектігін ескеріңіз:</span><span class="sxs-lookup"><span data-stu-id="5c0e2-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="5c0e2-120">Реттелетін өрістер мен нысандарды жасау</span><span class="sxs-lookup"><span data-stu-id="5c0e2-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="5c0e2-121">Баға орнатуы және транзакциялық нысандарға реттелетін өрістер қосу</span><span class="sxs-lookup"><span data-stu-id="5c0e2-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="5c0e2-122">Бағалар өлшемдері ретінде реттелетін өрістерді реттеу</span><span class="sxs-lookup"><span data-stu-id="5c0e2-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="5c0e2-123">Жаңа бағалар өлшемдерін қосу үшін қосылатын модуль атрибуттарын жаңарту</span><span class="sxs-lookup"><span data-stu-id="5c0e2-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="5c0e2-124">Кадрлық ресурс уақытының құнын белгілеу</span><span class="sxs-lookup"><span data-stu-id="5c0e2-124">Pricing human resource time</span></span>
<span data-ttu-id="5c0e2-125">Ұйымның кадрлық ресурс уақытының құнын белгілеу жолы көбінесе ұйымның табыстылығына тікелей әсер ететін маңызды стратегиялық фактор болып табылады.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="5c0e2-126">Ұйымыңыз кадрлық ресурс уақытына арналған пайыздық мөлшерлеме мен құн мөлшерлемесін реттеу жолын анықтауға дайын болған кезде, қаржылық топтармен және тәжірибе жетекшілерімен жұмыс жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="5c0e2-127">Баға белгілеуге қатысты ұсыныстар қазіргі уақытта бағалар өлшемдері болып табылмайтын, бірақ ұйымыңыз үшін бағалар өлшемі ретінде қолданылатын өрістерді немесе нысандарды қайта пайдалану қажеттігін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="5c0e2-128">**Транзакция санаты** (**msdyn_transactioncategory**) және **Резервтеу үшін қолжетімді ресурс** (**bookableresource**) өрістері кандидат өлшемдерінің мысалдары болып табылады.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="5c0e2-129">Сонымен қатар бағалар өлшемінің кесте немесе параметрлер жиыны болуы керектігін ескеруіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-129">You should also consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="5c0e2-130">Егер сіз 10 немесе 12-ден асатын өлшем мәндерінің өзгерістерін болжасаңыз және осы мәндерге қосымша атрибуттар қажет болса, параметрлер жиынын емес, нысанды жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="5c0e2-131">Мәндерді қосу немесе жою сияқты параметрлер жиынын сақтау үшін әкімші немесе әзірлеуші қажет, ал кестеге жаңа жолдар қосу әрекетін көптеген пайдаланушылар орындай алады.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="5c0e2-132">Төмендегі мысалда ресурстар тиесілі рөл мен ресурстық бөлімше негізінде құрылған пайыздық мөлшерлемелер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="5c0e2-133">Құн мөлшерлемелері, әдетте, қызметкердің жалақы деңгейіне және құрамына кіретін бөлімшеге негізделеді.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="5c0e2-134">Бұл мысалда вексель мен құн мөлшерлемесі кестелері келесідей болады.</span><span class="sxs-lookup"><span data-stu-id="5c0e2-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="5c0e2-135">**Үлгілі вексель мөлшерлемелері**</span><span class="sxs-lookup"><span data-stu-id="5c0e2-135">**Sample bill rates**</span></span>

| <span data-ttu-id="5c0e2-136">Рөл</span><span class="sxs-lookup"><span data-stu-id="5c0e2-136">Role</span></span>        | <span data-ttu-id="5c0e2-137">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="5c0e2-137">Org Unit</span></span>    |<span data-ttu-id="5c0e2-138">Бірлік</span><span class="sxs-lookup"><span data-stu-id="5c0e2-138">Unit</span></span>      |<span data-ttu-id="5c0e2-139">Баға</span><span class="sxs-lookup"><span data-stu-id="5c0e2-139">Price</span></span>      |<span data-ttu-id="5c0e2-140">Валюта</span><span class="sxs-lookup"><span data-stu-id="5c0e2-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="5c0e2-141">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="5c0e2-141">Developer</span></span>   | <span data-ttu-id="5c0e2-142">Contoso АҚШ</span><span class="sxs-lookup"><span data-stu-id="5c0e2-142">Contoso US</span></span>  |<span data-ttu-id="5c0e2-143">Hour</span><span class="sxs-lookup"><span data-stu-id="5c0e2-143">Hour</span></span> | <span data-ttu-id="5c0e2-144">200</span><span class="sxs-lookup"><span data-stu-id="5c0e2-144">200</span></span>|<span data-ttu-id="5c0e2-145">USD</span><span class="sxs-lookup"><span data-stu-id="5c0e2-145">USD</span></span>     |
| <span data-ttu-id="5c0e2-146">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="5c0e2-146">Developer</span></span>   | <span data-ttu-id="5c0e2-147">Contoso India</span><span class="sxs-lookup"><span data-stu-id="5c0e2-147">Contoso India</span></span> |<span data-ttu-id="5c0e2-148">Hour</span><span class="sxs-lookup"><span data-stu-id="5c0e2-148">Hour</span></span>|   <span data-ttu-id="5c0e2-149">112</span><span class="sxs-lookup"><span data-stu-id="5c0e2-149">112</span></span>|<span data-ttu-id="5c0e2-150">USD</span><span class="sxs-lookup"><span data-stu-id="5c0e2-150">USD</span></span>     |


<span data-ttu-id="5c0e2-151">**Үлгілі құн мөлшерлемелері**</span><span class="sxs-lookup"><span data-stu-id="5c0e2-151">**Sample cost rates**</span></span>

| <span data-ttu-id="5c0e2-152">Жалақы деңгейі</span><span class="sxs-lookup"><span data-stu-id="5c0e2-152">Salary Band</span></span>     | <span data-ttu-id="5c0e2-153">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="5c0e2-153">Org Unit</span></span>    |<span data-ttu-id="5c0e2-154">Бірлік</span><span class="sxs-lookup"><span data-stu-id="5c0e2-154">Unit</span></span>      |<span data-ttu-id="5c0e2-155">Баға</span><span class="sxs-lookup"><span data-stu-id="5c0e2-155">Price</span></span>      |<span data-ttu-id="5c0e2-156">Валюта</span><span class="sxs-lookup"><span data-stu-id="5c0e2-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="5c0e2-157">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="5c0e2-157">My company_Band1</span></span> | <span data-ttu-id="5c0e2-158">Contoso АҚШ</span><span class="sxs-lookup"><span data-stu-id="5c0e2-158">Contoso US</span></span>  |<span data-ttu-id="5c0e2-159">Hour</span><span class="sxs-lookup"><span data-stu-id="5c0e2-159">Hour</span></span> | <span data-ttu-id="5c0e2-160">145</span><span class="sxs-lookup"><span data-stu-id="5c0e2-160">145</span></span>|<span data-ttu-id="5c0e2-161">USD</span><span class="sxs-lookup"><span data-stu-id="5c0e2-161">USD</span></span>     |
| <span data-ttu-id="5c0e2-162">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="5c0e2-162">My company_Band2</span></span> | <span data-ttu-id="5c0e2-163">Contoso India</span><span class="sxs-lookup"><span data-stu-id="5c0e2-163">Contoso India</span></span> |<span data-ttu-id="5c0e2-164">Hour</span><span class="sxs-lookup"><span data-stu-id="5c0e2-164">Hour</span></span>|   <span data-ttu-id="5c0e2-165">67</span><span class="sxs-lookup"><span data-stu-id="5c0e2-165">67</span></span>|<span data-ttu-id="5c0e2-166">USD</span><span class="sxs-lookup"><span data-stu-id="5c0e2-166">USD</span></span>     |
