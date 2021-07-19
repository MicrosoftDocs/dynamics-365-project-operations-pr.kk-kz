---
title: Бағалар және шығын өлшемдерінің басты бет
description: Бұл тақырыпта бағалау өлшемдері туралы жалпы мәліметтер беріледі.
author: rumant
ms.custom:
- dyn365-projectservice
- intro-internal
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 5c8c28839f5e7b3259afbea4ab400d0c4fca95fd
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368888"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="3a280-103">Бағалар және шығын өлшемдерінің басты бет</span><span class="sxs-lookup"><span data-stu-id="3a280-103">Pricing and costing dimensions home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="3a280-104">Жобаға негізделген ұйымдарда еңбекақы бағасын және өзіндік құнын белгілеу үшін қолданылатын өлшемдерге келесі төлсипаттар әсер етеді:</span><span class="sxs-lookup"><span data-stu-id="3a280-104">The dimensions used to set labor pricing and costing in project-based organizations are influenced by the following attributes:</span></span>

- <span data-ttu-id="3a280-105">Адамдар өздерінің тәжірибесіне, рөліне немесе географиясына ұқсас жұмыс істейді</span><span class="sxs-lookup"><span data-stu-id="3a280-105">People doing work similar to their experience, role, or geography</span></span>
- <span data-ttu-id="3a280-106">Оның күрделілігіне немесе тәулік уақытына ұқсас орындалатын жұмыс</span><span class="sxs-lookup"><span data-stu-id="3a280-106">Work to be performed similar to its complexity or time of day</span></span>

<span data-ttu-id="3a280-107">Жұмыстың осы төлсипаттарының және жұмысты орындауға қажетті адамдардың типтік сипатына сәйкес, Project Service Automation бағдарламасында баға өлшемі мәндерінің екі түрі бар:</span><span class="sxs-lookup"><span data-stu-id="3a280-107">Given the typical nature of these attrubutes of the work and the people required to perform the work, there are two types of pricing dimension values available in Project Service Automation:</span></span> 

- <span data-ttu-id="3a280-108">**Параметрлер жиындары** - мәндер жиынтығы үшін бекітілген тізімдер болып табылатын төлсипаттар.</span><span class="sxs-lookup"><span data-stu-id="3a280-108">**Option sets** - Attributes that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="3a280-109">**Нысанға негізделген мәндер** - шектеулі, бірақ уақыт өте өзгеруі мүмкін әртүрлі мәндер жиынына ие болатын төлсипаттар.</span><span class="sxs-lookup"><span data-stu-id="3a280-109">**Entity-based values** - Attributes that can have a varied set of values that are finite but can change over time.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="3a280-110">Бағалар өлшемдері</span><span class="sxs-lookup"><span data-stu-id="3a280-110">Pricing dimensions</span></span>

<span data-ttu-id="3a280-111">PSA бағдарламасы әдепкі бағалар өлшемдерінің жиынтығымен жеткізіледі.</span><span class="sxs-lookup"><span data-stu-id="3a280-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="3a280-112">Мұны **Project Service** > **Параметрлер** тармағына өту арқылы көре аласыз.</span><span class="sxs-lookup"><span data-stu-id="3a280-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="3a280-113">Параметр жазбасындағы **Сомаға негізделген бағалар өлшемдері** қойыншасында рөлді тексеріңіз, **msdyn_resourcecategory** және ресурстық бөлімше, **msdyn_organizationalunit** параметрінің **Иә** мәніне орнатылған бар **Сатуға қолданылады** және **Құны үшін қолданылады** өрістері бар.</span><span class="sxs-lookup"><span data-stu-id="3a280-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="3a280-114">Бұл әр рөл мен бірлік тіркесімінің бағасы мен құнын белгілеуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="3a280-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

!["Сатылымға қолданбалы" параметрі бөлектелген Project Service параметрлерінің скриншоты](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="3a280-116">Егер сіз PSA 3 нұсқасына дейін бағалар өлшемдері ретінде рөл мен ұйымдық бөлімшенің дайын өрістерін қолданған болсаңыз, елеулі өзгерістер болмайды.</span><span class="sxs-lookup"><span data-stu-id="3a280-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="3a280-117">Project Service қызметін әдеттегідей пайдалануды жалғастыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="3a280-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="3a280-118">Егер қосымша атрибуттарды қолдана отырып, ресурстарыңыздың бағасын немесе құнын анықтау қажет болса, реттелген өрістерді, нысандарды және өлшемдерді жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="3a280-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="3a280-119">Қосымша ақпарат алу үшін, келесі тақырыптарды қараңыз, бірақ процедураларды төменде көрсетілген ретпен орындау керектігін ескеріңіз:</span><span class="sxs-lookup"><span data-stu-id="3a280-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="3a280-120">Реттелетін өрістер мен нысандарды жасау</span><span class="sxs-lookup"><span data-stu-id="3a280-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="3a280-121">Баға орнатуы және транзакциялық нысандарға реттелетін өрістер қосу</span><span class="sxs-lookup"><span data-stu-id="3a280-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="3a280-122">Реттелетін өрістерді баға өлшемдері ретінде орнату </span><span class="sxs-lookup"><span data-stu-id="3a280-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="3a280-123">Жаңа бағалар өлшемдерін қосу үшін қосылатын модуль атрибуттарын жаңарту</span><span class="sxs-lookup"><span data-stu-id="3a280-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="3a280-124">Кадрлық ресурс уақытының құнын белгілеу</span><span class="sxs-lookup"><span data-stu-id="3a280-124">Pricing human resource time</span></span>
<span data-ttu-id="3a280-125">Ұйымның кадрлық ресурс уақытының құнын белгілеу жолы көбінесе ұйымның табыстылығына тікелей әсер ететін маңызды стратегиялық фактор болып табылады.</span><span class="sxs-lookup"><span data-stu-id="3a280-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="3a280-126">Ұйымыңыз кадрлық ресурс уақытына арналған пайыздық мөлшерлеме мен құн мөлшерлемесін реттеу жолын анықтауға дайын болған кезде, қаржылық топтармен және тәжірибе жетекшілерімен жұмыс жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="3a280-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="3a280-127">Баға белгілеуге қатысты ұсыныстар қазіргі уақытта бағалар өлшемдері болып табылмайтын, бірақ ұйымыңыз үшін бағалар өлшемі ретінде қолданылатын өрістерді немесе нысандарды қайта пайдалану қажеттігін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="3a280-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="3a280-128">**Транзакция санаты** (**msdyn_transactioncategory**) және **Резервтеу үшін қолжетімді ресурс** (**bookableresource**) өрістері кандидат өлшемдерінің мысалдары болып табылады.</span><span class="sxs-lookup"><span data-stu-id="3a280-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="3a280-129">Бағалау өлшемі кесте немесе параметр жинағы болуы керек екенін қарастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="3a280-129">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="3a280-130">Егер сіз 10 немесе 12-ден асатын өлшем мәндерінің өзгерістерін болжасаңыз және осы мәндерге қосымша төлсипаттар қажет болса, параметрлер жиынын емес, нысанды жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="3a280-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, create an entity rather than an option set.</span></span> <span data-ttu-id="3a280-131">Мәндерді қосу немесе жою сияқты параметрлер жиынын сақтау үшін әкімші немесе әзірлеуші қажет, ал кестеге жаңа жолдар қосу әрекетін көптеген іскери пайдаланушылар орындай алады.</span><span class="sxs-lookup"><span data-stu-id="3a280-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most business users.</span></span>

<span data-ttu-id="3a280-132">Төмендегі мысалда ресурстар тиесілі рөл мен ресурстық бөлімше негізінде құрылған пайыздық мөлшерлемелер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="3a280-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="3a280-133">Құн мөлшерлемелері, әдетте, қызметкердің жалақы деңгейіне және құрамына кіретін бөлімшеге негізделеді.</span><span class="sxs-lookup"><span data-stu-id="3a280-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="3a280-134">Бұл мысалда вексель мен құн мөлшерлемесі кестелері келесідей болады.</span><span class="sxs-lookup"><span data-stu-id="3a280-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="3a280-135">**Үлгілі вексель мөлшерлемелері**</span><span class="sxs-lookup"><span data-stu-id="3a280-135">**Sample bill rates**</span></span>

| <span data-ttu-id="3a280-136">Рөл</span><span class="sxs-lookup"><span data-stu-id="3a280-136">Role</span></span>        | <span data-ttu-id="3a280-137">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="3a280-137">Org Unit</span></span>    |<span data-ttu-id="3a280-138">Бірлік</span><span class="sxs-lookup"><span data-stu-id="3a280-138">Unit</span></span>      |<span data-ttu-id="3a280-139">Баға</span><span class="sxs-lookup"><span data-stu-id="3a280-139">Price</span></span>      |<span data-ttu-id="3a280-140">Валюта</span><span class="sxs-lookup"><span data-stu-id="3a280-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="3a280-141">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="3a280-141">Developer</span></span>   | <span data-ttu-id="3a280-142">Contoso (АҚШ)</span><span class="sxs-lookup"><span data-stu-id="3a280-142">Contoso US</span></span>  |<span data-ttu-id="3a280-143">Сағат</span><span class="sxs-lookup"><span data-stu-id="3a280-143">Hour</span></span> | <span data-ttu-id="3a280-144">200</span><span class="sxs-lookup"><span data-stu-id="3a280-144">200</span></span>|<span data-ttu-id="3a280-145">USD</span><span class="sxs-lookup"><span data-stu-id="3a280-145">USD</span></span>     |
| <span data-ttu-id="3a280-146">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="3a280-146">Developer</span></span>   | <span data-ttu-id="3a280-147">Contoso India</span><span class="sxs-lookup"><span data-stu-id="3a280-147">Contoso India</span></span> |<span data-ttu-id="3a280-148">Сағат</span><span class="sxs-lookup"><span data-stu-id="3a280-148">Hour</span></span>|   <span data-ttu-id="3a280-149">112</span><span class="sxs-lookup"><span data-stu-id="3a280-149">112</span></span>|<span data-ttu-id="3a280-150">USD</span><span class="sxs-lookup"><span data-stu-id="3a280-150">USD</span></span>     |


<span data-ttu-id="3a280-151">**Үлгілі құн мөлшерлемелері**</span><span class="sxs-lookup"><span data-stu-id="3a280-151">**Sample cost rates**</span></span>

| <span data-ttu-id="3a280-152">Жалақы деңгейі</span><span class="sxs-lookup"><span data-stu-id="3a280-152">Salary Band</span></span>     | <span data-ttu-id="3a280-153">Ұйымдық бөлімше</span><span class="sxs-lookup"><span data-stu-id="3a280-153">Org Unit</span></span>    |<span data-ttu-id="3a280-154">Бірлік</span><span class="sxs-lookup"><span data-stu-id="3a280-154">Unit</span></span>      |<span data-ttu-id="3a280-155">Баға</span><span class="sxs-lookup"><span data-stu-id="3a280-155">Price</span></span>      |<span data-ttu-id="3a280-156">Валюта</span><span class="sxs-lookup"><span data-stu-id="3a280-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="3a280-157">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="3a280-157">My company_Band1</span></span> | <span data-ttu-id="3a280-158">Contoso (АҚШ)</span><span class="sxs-lookup"><span data-stu-id="3a280-158">Contoso US</span></span>  |<span data-ttu-id="3a280-159">Сағат</span><span class="sxs-lookup"><span data-stu-id="3a280-159">Hour</span></span> | <span data-ttu-id="3a280-160">145</span><span class="sxs-lookup"><span data-stu-id="3a280-160">145</span></span>|<span data-ttu-id="3a280-161">USD</span><span class="sxs-lookup"><span data-stu-id="3a280-161">USD</span></span>     |
| <span data-ttu-id="3a280-162">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="3a280-162">My company_Band2</span></span> | <span data-ttu-id="3a280-163">Contoso India</span><span class="sxs-lookup"><span data-stu-id="3a280-163">Contoso India</span></span> |<span data-ttu-id="3a280-164">Сағат</span><span class="sxs-lookup"><span data-stu-id="3a280-164">Hour</span></span>|   <span data-ttu-id="3a280-165">67</span><span class="sxs-lookup"><span data-stu-id="3a280-165">67</span></span>|<span data-ttu-id="3a280-166">USD</span><span class="sxs-lookup"><span data-stu-id="3a280-166">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]