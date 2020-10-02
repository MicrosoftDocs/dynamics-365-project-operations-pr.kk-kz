---
title: Бағалар өлшемдеріне шолу
description: Осы тақырыпта Dynamics 365 Project Operations бағдарламасындағы бағалау өлшемдері туралы ақпарат ұсынылған.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: fe2ab3a1b12c00e346e27709d66b5a0cb81a3b56
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898223"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="30591-103">Бағалар өлшемдеріне шолу</span><span class="sxs-lookup"><span data-stu-id="30591-103">Pricing dimensions overview</span></span>

<span data-ttu-id="30591-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="30591-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="30591-105">Бағалар мен шығындарды белгілеу үшін кадрлар ресурстарында қолданылатын өлшемдер екі санатқа бөлінеді:</span><span class="sxs-lookup"><span data-stu-id="30591-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="30591-106">Адамдар</span><span class="sxs-lookup"><span data-stu-id="30591-106">People</span></span>
- <span data-ttu-id="30591-107">Жоспарланған жұмыс</span><span class="sxs-lookup"><span data-stu-id="30591-107">Planned work</span></span>

<span data-ttu-id="30591-108">Осы себептен, бағалау өлшемі мәндерінің екі түрі қолжетімді:</span><span class="sxs-lookup"><span data-stu-id="30591-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="30591-109">**Параметр жинақтары**: Мәндер жинағы үшін бекітілген нөмірлеу болып табылатын өлшемдер.</span><span class="sxs-lookup"><span data-stu-id="30591-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="30591-110">**Нысан негізіндегі мәндер**: Әртүрлі мәндер жинағы бола алатын өлшемдер.</span><span class="sxs-lookup"><span data-stu-id="30591-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="30591-111">Бағалар өлшемдері</span><span class="sxs-lookup"><span data-stu-id="30591-111">Pricing dimensions</span></span>

<span data-ttu-id="30591-112">Dynamics 365 Project Operations бағдарламасы бағалау өлшемдерінің әдепкі жинағымен жеткізіледі.</span><span class="sxs-lookup"><span data-stu-id="30591-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="30591-113">Бағалау өлшемдерін **Project Operations** > **Параметрлер** тармағы бойынша өту арқылы көруге болады.</span><span class="sxs-lookup"><span data-stu-id="30591-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="30591-114">Параметр жазбасындағы **Сомаға негізделген бағалар өлшемдері** қойыншасында рөлді тексеріңіз, **msdyn_resourcecategory** және ресурстық бөлімше, **msdyn_organizationalunit** параметрінің **Иә** мәніне орнатылған бар **Сатуға қолданылады** және **Құны үшін қолданылады** өрістері бар.</span><span class="sxs-lookup"><span data-stu-id="30591-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="30591-115">Осы өрістер іске қосылған кезде, әрбір рөл мен ұйымдық бірлік тіркесімі үшін баға мен шығынды орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="30591-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

<span data-ttu-id="30591-116">Егер қосымша атрибуттарды қолдана отырып, ресурстарыңыздың бағасын немесе құнын анықтау қажет болса, реттелген өрістерді, нысандарды және өлшемдерді жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="30591-116">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span>

## <a name="pricing-human-resource-time"></a><span data-ttu-id="30591-117">Кадрлық ресурс уақытының құнын белгілеу</span><span class="sxs-lookup"><span data-stu-id="30591-117">Pricing human resource time</span></span>
<span data-ttu-id="30591-118">Ұйымның кадрлық ресурс уақытының құнын белгілеу жолы көбінесе ұйымның табыстылығына тікелей әсер ететін маңызды стратегиялық фактор болып табылады.</span><span class="sxs-lookup"><span data-stu-id="30591-118">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="30591-119">Ұйымыңыз кадрлық ресурс уақытына арналған пайыздық мөлшерлеме мен құн мөлшерлемесін реттеу жолын анықтауға дайын болған кезде, қаржылық топтармен және тәжірибе жетекшілерімен жұмыс жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="30591-119">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="30591-120">Баға белгілеуге қатысты ұсыныстар қазіргі уақытта бағалар өлшемдері болып табылмайтын, бірақ ұйымыңыз үшін бағалар өлшемі ретінде қолданылатын өрістерді немесе нысандарды қайта пайдалану қажеттігін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="30591-120">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="30591-121">**Транзакция санаты** (**msdyn_transactioncategory**) және **Резервтеу үшін қолжетімді ресурс** (**bookableresource**) өрістері кандидат өлшемдерінің мысалдары болып табылады.</span><span class="sxs-lookup"><span data-stu-id="30591-121">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="30591-122">Бағалау өлшемі кесте немесе параметр жинағы болуы керек екенін қарастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="30591-122">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="30591-123">Егер сіз 10 немесе 12-ден асатын өлшем мәндерінің өзгерістерін болжасаңыз және осы мәндерге қосымша атрибуттар қажет болса, параметрлер жиынын емес, нысанды жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="30591-123">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="30591-124">Мәндерді қосу немесе жою сияқты параметрлер жиынын сақтау үшін әкімші немесе әзірлеуші қажет, ал кестеге жаңа жолдар қосу әрекетін көптеген пайдаланушылар орындай алады.</span><span class="sxs-lookup"><span data-stu-id="30591-124">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="30591-125">Төмендегі мысалда ресурстар тиесілі рөл мен ресурстық бөлімше негізінде құрылған пайыздық мөлшерлемелер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="30591-125">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="30591-126">Құн мөлшерлемелері, әдетте, қызметкердің жалақы деңгейіне және құрамына кіретін бөлімшеге негізделеді.</span><span class="sxs-lookup"><span data-stu-id="30591-126">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="30591-127">Бұл мысалда вексель мен құн мөлшерлемесі кестелері келесідей болады.</span><span class="sxs-lookup"><span data-stu-id="30591-127">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="30591-128">**Үлгілі вексель мөлшерлемелері**</span><span class="sxs-lookup"><span data-stu-id="30591-128">**Sample bill rates**</span></span>

| <span data-ttu-id="30591-129">Рөл</span><span class="sxs-lookup"><span data-stu-id="30591-129">Role</span></span>        | <span data-ttu-id="30591-130">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="30591-130">Org Unit</span></span>    |<span data-ttu-id="30591-131">Бірлік</span><span class="sxs-lookup"><span data-stu-id="30591-131">Unit</span></span>      |<span data-ttu-id="30591-132">Баға</span><span class="sxs-lookup"><span data-stu-id="30591-132">Price</span></span>      |<span data-ttu-id="30591-133">Валюта</span><span class="sxs-lookup"><span data-stu-id="30591-133">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="30591-134">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="30591-134">Developer</span></span>   | <span data-ttu-id="30591-135">Contoso АҚШ</span><span class="sxs-lookup"><span data-stu-id="30591-135">Contoso US</span></span>  |<span data-ttu-id="30591-136">Hour</span><span class="sxs-lookup"><span data-stu-id="30591-136">Hour</span></span> | <span data-ttu-id="30591-137">200</span><span class="sxs-lookup"><span data-stu-id="30591-137">200</span></span>|<span data-ttu-id="30591-138">USD</span><span class="sxs-lookup"><span data-stu-id="30591-138">USD</span></span>     |
| <span data-ttu-id="30591-139">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="30591-139">Developer</span></span>   | <span data-ttu-id="30591-140">Contoso India</span><span class="sxs-lookup"><span data-stu-id="30591-140">Contoso India</span></span> |<span data-ttu-id="30591-141">Hour</span><span class="sxs-lookup"><span data-stu-id="30591-141">Hour</span></span>|   <span data-ttu-id="30591-142">112</span><span class="sxs-lookup"><span data-stu-id="30591-142">112</span></span>|<span data-ttu-id="30591-143">USD</span><span class="sxs-lookup"><span data-stu-id="30591-143">USD</span></span>     |


<span data-ttu-id="30591-144">**Үлгілі құн мөлшерлемелері**</span><span class="sxs-lookup"><span data-stu-id="30591-144">**Sample cost rates**</span></span>

| <span data-ttu-id="30591-145">Жалақы деңгейі</span><span class="sxs-lookup"><span data-stu-id="30591-145">Salary Band</span></span>     | <span data-ttu-id="30591-146">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="30591-146">Org Unit</span></span>    |<span data-ttu-id="30591-147">Бірлік</span><span class="sxs-lookup"><span data-stu-id="30591-147">Unit</span></span>      |<span data-ttu-id="30591-148">Баға</span><span class="sxs-lookup"><span data-stu-id="30591-148">Price</span></span>      |<span data-ttu-id="30591-149">Валюта</span><span class="sxs-lookup"><span data-stu-id="30591-149">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="30591-150">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="30591-150">My company_Band1</span></span> | <span data-ttu-id="30591-151">Contoso АҚШ</span><span class="sxs-lookup"><span data-stu-id="30591-151">Contoso US</span></span>  |<span data-ttu-id="30591-152">Hour</span><span class="sxs-lookup"><span data-stu-id="30591-152">Hour</span></span> | <span data-ttu-id="30591-153">145</span><span class="sxs-lookup"><span data-stu-id="30591-153">145</span></span>|<span data-ttu-id="30591-154">USD</span><span class="sxs-lookup"><span data-stu-id="30591-154">USD</span></span>     |
| <span data-ttu-id="30591-155">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="30591-155">My company_Band2</span></span> | <span data-ttu-id="30591-156">Contoso India</span><span class="sxs-lookup"><span data-stu-id="30591-156">Contoso India</span></span> |<span data-ttu-id="30591-157">Hour</span><span class="sxs-lookup"><span data-stu-id="30591-157">Hour</span></span>|   <span data-ttu-id="30591-158">67</span><span class="sxs-lookup"><span data-stu-id="30591-158">67</span></span>|<span data-ttu-id="30591-159">USD</span><span class="sxs-lookup"><span data-stu-id="30591-159">USD</span></span>     |
