---
title: Бағалар өлшемдеріне шолу
description: Бұл тақырыпта Dynamics 365 Project Operations бағдарламасындағы бағалар өлшемдері туралы ақпарат берілген.
author: rumant
ms.date: 11/30/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: e8d62dcf9975e5427926210a881dec2c256f1b8b
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368483"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="7be9f-103">Бағалар өлшемдеріне шолу</span><span class="sxs-lookup"><span data-stu-id="7be9f-103">Pricing dimensions overview</span></span>

<span data-ttu-id="7be9f-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="7be9f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7be9f-105">Бағалар мен шығындарды белгілеу үшін кадрлар ресурстарында қолданылатын өлшемдер екі санатқа бөлінеді:</span><span class="sxs-lookup"><span data-stu-id="7be9f-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="7be9f-106">Адамдар</span><span class="sxs-lookup"><span data-stu-id="7be9f-106">People</span></span>
- <span data-ttu-id="7be9f-107">Жоспарланған жұмыс</span><span class="sxs-lookup"><span data-stu-id="7be9f-107">Planned work</span></span>

<span data-ttu-id="7be9f-108">Осы себептен, бағалау өлшемі мәндерінің екі түрі қолжетімді:</span><span class="sxs-lookup"><span data-stu-id="7be9f-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="7be9f-109">**Параметр жинақтары**: Мәндер жинағы үшін бекітілген нөмірлеу болып табылатын өлшемдер.</span><span class="sxs-lookup"><span data-stu-id="7be9f-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="7be9f-110">**Нысан негізіндегі мәндер**: Әртүрлі мәндер жинағы бола алатын өлшемдер.</span><span class="sxs-lookup"><span data-stu-id="7be9f-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="7be9f-111">Бағалар өлшемдері</span><span class="sxs-lookup"><span data-stu-id="7be9f-111">Pricing dimensions</span></span>

<span data-ttu-id="7be9f-112">Dynamics 365 Project Operations бағдарламасы әдепкі бағалар өлшемдерінің жиынтығымен жеткізіледі.</span><span class="sxs-lookup"><span data-stu-id="7be9f-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="7be9f-113">Бағалау өлшемдерін **Project Operations** > **Параметрлер** тармағы бойынша өту арқылы көруге болады.</span><span class="sxs-lookup"><span data-stu-id="7be9f-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="7be9f-114">Параметр жазбасындағы **Сомаға негізделген бағалар өлшемдері** қойыншасында рөлді тексеріңіз, **msdyn_resourcecategory** және ресурстық бөлімше, **msdyn_organizationalunit** параметрінің **Иә** мәніне орнатылған бар **Сатуға қолданылады** және **Құны үшін қолданылады** өрістері бар.</span><span class="sxs-lookup"><span data-stu-id="7be9f-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="7be9f-115">Осы өрістер іске қосылған кезде, әрбір рөл мен ұйымдық бірлік тіркесімі үшін баға мен шығынды орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="7be9f-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

!["Сатылымға қолданбалы" параметрі бөлектелген Project Service параметрлерінің скриншоты](media/PS-OOB-parameters.png)

<span data-ttu-id="7be9f-117">Егер қосымша атрибуттарды қолдана отырып, ресурстарыңыздың бағасын немесе құнын анықтау қажет болса, реттелген өрістерді, нысандарды және өлшемдерді жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="7be9f-117">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="7be9f-118">Қосымша ақпарат алу үшін келесі тақырыптарды қараңыз.</span><span class="sxs-lookup"><span data-stu-id="7be9f-118">For more information, see the following topics.</span></span> 
  
  > [!NOTE]
  > <span data-ttu-id="7be9f-119">Процедуралар тізімделген тәртіпте орындалуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="7be9f-119">The procedures must be completed in the order they are listed.</span></span>

1. [<span data-ttu-id="7be9f-120">Реттелетін баға өлшемдері үшін шешім жасау</span><span class="sxs-lookup"><span data-stu-id="7be9f-120">Create a solution for custom pricing dimensions</span></span>](../sales/create-solution-custompd.md)
2. [<span data-ttu-id="7be9f-121">Реттелетін өрістер мен нысандар жасау</span><span class="sxs-lookup"><span data-stu-id="7be9f-121">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md)
3. [<span data-ttu-id="7be9f-122">Баға параметрлері мен транзакциялық нысандарға реттелетін өрістерді қосу </span><span class="sxs-lookup"><span data-stu-id="7be9f-122">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
4. [<span data-ttu-id="7be9f-123">Реттелетін өрістерді баға өлшемдері ретінде орнату </span><span class="sxs-lookup"><span data-stu-id="7be9f-123">Set up custom fields as pricing dimensions</span></span>](set-up-custom-fields-pricing-dimensions.md)
5. [<span data-ttu-id="7be9f-124">Жаңа бағалар өлшемдерін қосу үшін қосылатын модуль атрибуттарын жаңарту</span><span class="sxs-lookup"><span data-stu-id="7be9f-124">Update plug-in attributes to include new pricing dimensions</span></span>](update-plugin-attributes-pd.md)


## <a name="pricing-human-resource-time"></a><span data-ttu-id="7be9f-125">Кадрлық ресурс уақытының құнын белгілеу</span><span class="sxs-lookup"><span data-stu-id="7be9f-125">Pricing human resource time</span></span>
<span data-ttu-id="7be9f-126">Ұйымның кадрлық ресурс уақытының құнын белгілеу жолы көбінесе ұйымның табыстылығына тікелей әсер ететін маңызды стратегиялық фактор болып табылады.</span><span class="sxs-lookup"><span data-stu-id="7be9f-126">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="7be9f-127">Ұйымыңыз кадрлық ресурс уақытына арналған пайыздық мөлшерлеме мен құн мөлшерлемесін реттеу жолын анықтауға дайын болған кезде, қаржылық топтармен және тәжірибе жетекшілерімен жұмыс жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="7be9f-127">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="7be9f-128">Баға белгілеуге қатысты ұсыныстар қазіргі уақытта бағалар өлшемдері болып табылмайтын, бірақ ұйымыңыз үшін бағалар өлшемі ретінде қолданылатын өрістерді немесе нысандарды қайта пайдалану қажеттігін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="7be9f-128">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="7be9f-129">**Транзакция санаты** (**msdyn_transactioncategory**) және **Резервтеу үшін қолжетімді ресурс** (**bookableresource**) өрістері кандидат өлшемдерінің мысалдары болып табылады.</span><span class="sxs-lookup"><span data-stu-id="7be9f-129">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="7be9f-130">Бағалау өлшемі кесте немесе параметр жинағы болуы керек екенін қарастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="7be9f-130">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="7be9f-131">Егер сіз 10 немесе 12-ден асатын өлшем мәндерінің өзгерістерін болжасаңыз және осы мәндерге қосымша атрибуттар қажет болса, параметрлер жиынын емес, нысанды жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="7be9f-131">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="7be9f-132">Мәндерді қосу немесе жою сияқты параметрлер жиынын сақтау үшін әкімші немесе әзірлеуші қажет, ал кестеге жаңа жолдар қосу әрекетін көптеген пайдаланушылар орындай алады.</span><span class="sxs-lookup"><span data-stu-id="7be9f-132">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="7be9f-133">Төмендегі мысалда ресурстар тиесілі рөл мен ресурстық бөлімше негізінде құрылған пайыздық мөлшерлемелер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="7be9f-133">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="7be9f-134">Құн мөлшерлемелері, әдетте, қызметкердің жалақы деңгейіне және құрамына кіретін бөлімшеге негізделеді.</span><span class="sxs-lookup"><span data-stu-id="7be9f-134">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="7be9f-135">Бұл мысалда вексель мен құн мөлшерлемесі кестелері келесідей болады.</span><span class="sxs-lookup"><span data-stu-id="7be9f-135">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="7be9f-136">**Үлгілі вексель мөлшерлемелері**</span><span class="sxs-lookup"><span data-stu-id="7be9f-136">**Sample bill rates**</span></span>

| <span data-ttu-id="7be9f-137">Рөл</span><span class="sxs-lookup"><span data-stu-id="7be9f-137">Role</span></span>        | <span data-ttu-id="7be9f-138">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="7be9f-138">Org Unit</span></span>    |<span data-ttu-id="7be9f-139">Бірлік</span><span class="sxs-lookup"><span data-stu-id="7be9f-139">Unit</span></span>      |<span data-ttu-id="7be9f-140">Баға</span><span class="sxs-lookup"><span data-stu-id="7be9f-140">Price</span></span>      |<span data-ttu-id="7be9f-141">Валюта</span><span class="sxs-lookup"><span data-stu-id="7be9f-141">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="7be9f-142">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="7be9f-142">Developer</span></span>   | <span data-ttu-id="7be9f-143">Contoso (АҚШ)</span><span class="sxs-lookup"><span data-stu-id="7be9f-143">Contoso US</span></span>  |<span data-ttu-id="7be9f-144">Сағат</span><span class="sxs-lookup"><span data-stu-id="7be9f-144">Hour</span></span> | <span data-ttu-id="7be9f-145">200</span><span class="sxs-lookup"><span data-stu-id="7be9f-145">200</span></span>|<span data-ttu-id="7be9f-146">USD</span><span class="sxs-lookup"><span data-stu-id="7be9f-146">USD</span></span>     |
| <span data-ttu-id="7be9f-147">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="7be9f-147">Developer</span></span>   | <span data-ttu-id="7be9f-148">Contoso India</span><span class="sxs-lookup"><span data-stu-id="7be9f-148">Contoso India</span></span> |<span data-ttu-id="7be9f-149">Сағат</span><span class="sxs-lookup"><span data-stu-id="7be9f-149">Hour</span></span>|   <span data-ttu-id="7be9f-150">112</span><span class="sxs-lookup"><span data-stu-id="7be9f-150">112</span></span>|<span data-ttu-id="7be9f-151">USD</span><span class="sxs-lookup"><span data-stu-id="7be9f-151">USD</span></span>     |


<span data-ttu-id="7be9f-152">**Үлгілі құн мөлшерлемелері**</span><span class="sxs-lookup"><span data-stu-id="7be9f-152">**Sample cost rates**</span></span>

| <span data-ttu-id="7be9f-153">Жалақы деңгейі</span><span class="sxs-lookup"><span data-stu-id="7be9f-153">Salary Band</span></span>     | <span data-ttu-id="7be9f-154">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="7be9f-154">Org Unit</span></span>    |<span data-ttu-id="7be9f-155">Бірлік</span><span class="sxs-lookup"><span data-stu-id="7be9f-155">Unit</span></span>      |<span data-ttu-id="7be9f-156">Баға</span><span class="sxs-lookup"><span data-stu-id="7be9f-156">Price</span></span>      |<span data-ttu-id="7be9f-157">Валюта</span><span class="sxs-lookup"><span data-stu-id="7be9f-157">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="7be9f-158">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="7be9f-158">My company_Band1</span></span> | <span data-ttu-id="7be9f-159">Contoso (АҚШ)</span><span class="sxs-lookup"><span data-stu-id="7be9f-159">Contoso US</span></span>  |<span data-ttu-id="7be9f-160">Сағат</span><span class="sxs-lookup"><span data-stu-id="7be9f-160">Hour</span></span> | <span data-ttu-id="7be9f-161">145</span><span class="sxs-lookup"><span data-stu-id="7be9f-161">145</span></span>|<span data-ttu-id="7be9f-162">USD</span><span class="sxs-lookup"><span data-stu-id="7be9f-162">USD</span></span>     |
| <span data-ttu-id="7be9f-163">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="7be9f-163">My company_Band2</span></span> | <span data-ttu-id="7be9f-164">Contoso India</span><span class="sxs-lookup"><span data-stu-id="7be9f-164">Contoso India</span></span> |<span data-ttu-id="7be9f-165">Сағат</span><span class="sxs-lookup"><span data-stu-id="7be9f-165">Hour</span></span>|   <span data-ttu-id="7be9f-166">67</span><span class="sxs-lookup"><span data-stu-id="7be9f-166">67</span></span>|<span data-ttu-id="7be9f-167">USD</span><span class="sxs-lookup"><span data-stu-id="7be9f-167">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]