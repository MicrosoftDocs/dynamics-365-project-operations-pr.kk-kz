---
title: Шығыстар үшін құн мен сатылым мөлшерлемелерін орнату
description: Бұл тақырыпта операция және шығыс санаттары үшін құн мен сатылым мөлшерлемелерін орнату жолдары туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e5a2402a2c1059ff11dbe1a331a028da77958235
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079579"
---
# <a name="set-up-cost-and-sales-rates-for-expenses"></a><span data-ttu-id="41972-103">Шығыстар үшін құн мен сатылым мөлшерлемелерін орнату</span><span class="sxs-lookup"><span data-stu-id="41972-103">Set up cost and sales rates for expenses</span></span>

<span data-ttu-id="41972-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="41972-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="41972-105">Dynamics 365 Project Operations ішінде операциялар санаттары үшін шығындар мен сатылым бағаларын орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="41972-105">You can set up cost and sales prices for transaction categories in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="41972-106">Шығындар мен сатылым бағалары шығыстарға арналғандықтан, оларды қамтитын әрбір операция санаты да шығындар санаты ретінде белгіленуі керек.</span><span class="sxs-lookup"><span data-stu-id="41972-106">Because the cost and sales prices are designed for Expenses, each transaction category that includes these, must also be set up as an expense category.</span></span> <span data-ttu-id="41972-107">Бұл параметр төменгі функционалдылықта дәлдікті қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="41972-107">This set up ensures accuracy in downstream functionality.</span></span> <span data-ttu-id="41972-108">Операциялық санаттар үшін өзіндік құн мен сату бағасы бағатізбе тақырыбындағы валюта болуы қажет тек бір валютада көрсетілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="41972-108">Cost and sales prices for transaction categories can only be listed in one currency, which must be the currency on the price list header.</span></span>

<span data-ttu-id="41972-109">Операциялық санаттар үшін шығындар мен сату мөлшерлемелерін орнату үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="41972-109">To set up cost and sales rates for transaction categories, complete the following steps.</span></span> 

1. <span data-ttu-id="41972-110">Бағатізбе тақырыбы негізінде бағатізбе жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="41972-110">Create a price list based on the price list header.</span></span> 
2. <span data-ttu-id="41972-111">**Санат бағалары** параметрінде ішкі тор мәзірінде **+ Жаңа санат бағасы** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="41972-111">On the **Category Prices** , on the sub-grid menu, select **+ New Category Price**.</span></span> 
3. <span data-ttu-id="41972-112">**Жылдам жасау** бетінде жаңа бағаны құратын операция санаты мен бірлігін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="41972-112">On the **Quick Create** page, enter the transaction category and unit that you are creating the new price for.</span></span>

<span data-ttu-id="41972-113">Келесі кестеде **Жалпы** қойыншасындағы өрістер мен сатылым немесе құн бағатізбесінде санат бағаларын жасаған кезде назар аудару қажет санат бағасының **Жылдам жасау** беті қамтылған.</span><span class="sxs-lookup"><span data-stu-id="41972-113">The following table lists the fields on the **General** tab and **Quick Create** page of a category price line that you should keep in mind as you create category prices on a sales or cost price list.</span></span>

| <span data-ttu-id="41972-114">Өріс</span><span class="sxs-lookup"><span data-stu-id="41972-114">Field</span></span> | <span data-ttu-id="41972-115">Орналасқан жері</span><span class="sxs-lookup"><span data-stu-id="41972-115">Location</span></span> | <span data-ttu-id="41972-116">Маңыздылық, мақсаты және нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="41972-116">Relevance, purpose, and guidance</span></span> | <span data-ttu-id="41972-117">Төменгі әсер</span><span class="sxs-lookup"><span data-stu-id="41972-117">Downstream impact</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="41972-118">Транзакция санаты</span><span class="sxs-lookup"><span data-stu-id="41972-118">Transaction Category</span></span> | <span data-ttu-id="41972-119">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="41972-119">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="41972-120">Сату немесе құн бағасы жасалатын операциялар санатын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="41972-120">Select the transaction category you are creating a sales or cost price for.</span></span> | <span data-ttu-id="41972-121">Шығысқа арналған кіріс болжамы мен нақты жолдағы операция санаты оның құн немесе сатылым мөлшерлемесін әдепкі бойынша орнату үшін осы жолмен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="41972-121">The transaction category on the incoming estimate or actual for Expense will be matched against this line to default the cost or sales rate of the transaction category.</span></span> |
| <span data-ttu-id="41972-122">Бірлік кестесі</span><span class="sxs-lookup"><span data-stu-id="41972-122">Unit Schedule</span></span> | <span data-ttu-id="41972-123">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="41972-123">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="41972-124">Әдепкі өлшем бірліктерінің кестесі операция санатының өлшем бірліктерінің кестесінен анықталады.</span><span class="sxs-lookup"><span data-stu-id="41972-124">The unit schedule defaults from the unit schedule of the transaction category.</span></span> | <span data-ttu-id="41972-125">Бұл өрістен төменгі әсері жоқ.</span><span class="sxs-lookup"><span data-stu-id="41972-125">There is no downstream impact from this field.</span></span> |
| <span data-ttu-id="41972-126">Бірлік</span><span class="sxs-lookup"><span data-stu-id="41972-126">Unit</span></span> | <span data-ttu-id="41972-127">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="41972-127">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="41972-128">Мөлшерлемелер орнатылатын бірлікті таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="41972-128">Select the unit for which the rates are being set up.</span></span> | <span data-ttu-id="41972-129">Шығындарды немесе нақты бағалау үшін мөлшерлемені пайдалану үшін кіріс немесе нақты бағалаудағы өлшем бірлігі осы жолдағы өлшем бірлігімен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="41972-129">The unit on the incoming estimate or actual is matched against the unit on this line to default the rate on the expense estimate or actual.</span></span> |
| <span data-ttu-id="41972-130">Бағаны бекіту әдісі</span><span class="sxs-lookup"><span data-stu-id="41972-130">Pricing Method</span></span> | <span data-ttu-id="41972-131">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="41972-131">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="41972-132">**Баға әдісі** өрісінің ықтимал мәндері – **Бірлік бойынша бағасы** , **Құны бойынша** және **Құн бойынша үстеме баға**.</span><span class="sxs-lookup"><span data-stu-id="41972-132">Possible values of the **Pricing Method** field are, **Price Per Unit** , **At Cost** , and **Markup Over Cost**.</span></span> | <span data-ttu-id="41972-133">Бағаны орнату кезінде **Бірлік бойынша бағасы** санат бағасы жолындағы **Пайыз** өрісін құлыптайды.</span><span class="sxs-lookup"><span data-stu-id="41972-133">During price setup, selecting **Price Per Unit** locks the **Percent** field on the category price line.</span></span> <span data-ttu-id="41972-134">**Өзіндік құны бойынша** таңдалса , **Бағасы** және **Пайыз** өрістері сату бағаларының тізімінде құлыпталады.</span><span class="sxs-lookup"><span data-stu-id="41972-134">If **At cost** is selected, the **Price** and **Percent** fields are locked on the sales price list.</span></span> <span data-ttu-id="41972-135">**Құн бойынша үстеме баға** құлыптайды сату бағасы тізіміндегі **Бағасы** өрісін құлыптайды.</span><span class="sxs-lookup"><span data-stu-id="41972-135">Selecting **Markup Over Cost** locks the **Price** field on the sales price list.</span></span> <span data-ttu-id="41972-136">Шығыстарға арналған нақты кіріс сызығында **Өзіндік құны бойынша** немесе **Құн бойынша үстеме баға** баға белгілеу әдісі сәйкес сатылмаған сату сызығына нақты өзіндік құн бағасына тең немесе бағадан үстеме ретінде есептелген баға тағайындалуына әкеледі.</span><span class="sxs-lookup"><span data-stu-id="41972-136">On an incoming actual line for expense, the **At cost** or **Markup Over Cost** pricing method results in the corresponding unbilled sales line being assigned a price that is equal to the price on the cost actual or calculated as a markup over the price.</span></span> |
| <span data-ttu-id="41972-137">Баға</span><span class="sxs-lookup"><span data-stu-id="41972-137">Price</span></span> | <span data-ttu-id="41972-138">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="41972-138">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="41972-139">Операция санаты мен бірлік комбинациясы үшін бірлік мөлшерлемесін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="41972-139">Set up a per unit rate for the transaction category and unit combination.</span></span> <span data-ttu-id="41972-140">Мысалы, жүгіріс мөлшерлемесі – бір миль үшін 10 доллар және бір километр үшін 8 доллар.</span><span class="sxs-lookup"><span data-stu-id="41972-140">For example, the rate for mileage is 10 USD per mile and 8 USD per Kilometer.</span></span> | <span data-ttu-id="41972-141">Жүгіріс мөлшерлемесі — шығыс транзакция класы үшін кіріс болжамының немесе нақты жолдың бірлік бағасына немесе құнына арналған әдепкі құн мөлшерлемесі.</span><span class="sxs-lookup"><span data-stu-id="41972-141">The mileage rate will be the rate that defaults on the per unit price or cost of the incoming estimate or actual line for an expense transaction class.</span></span>|
| <span data-ttu-id="41972-142">Пайыз</span><span class="sxs-lookup"><span data-stu-id="41972-142">Percent</span></span> | <span data-ttu-id="41972-143">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="41972-143">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="41972-144">Операция санаты мен бірлік комбинациясы үшін құнынан асатын пайызды орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="41972-144">Set up percent over cost for the transaction category and unit combination.</span></span> <span data-ttu-id="41972-145">Мысалы, авиабилеттерді сату тарифі авиа ұшуға жұмсалған шығыстар құнынан 10 пайызға жоғары белгіленуі тиіс.</span><span class="sxs-lookup"><span data-stu-id="41972-145">For example, the airfare sales rate should be marked up 10 percent over the cost of the incurred airfare expense.</span></span> | <span data-ttu-id="41972-146">Өзіндік құнынан жоғары бұл пайыз, егер баға белгілеу әдісі **Құны бойынша үстеме бағасы** таңдалған болса, сату бағатізбесінде ғана қолданылады.</span><span class="sxs-lookup"><span data-stu-id="41972-146">This percent over cost is only applicable on a sales price list when the pricing method selected is **Markup Over Cost**.</span></span> |
| <span data-ttu-id="41972-147">Валюта</span><span class="sxs-lookup"><span data-stu-id="41972-147">Currency</span></span> | <span data-ttu-id="41972-148">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="41972-148">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="41972-149">Әдепкі бойынша, бұл мән бағатізбе тақырыбындағы валютадан келеді.</span><span class="sxs-lookup"><span data-stu-id="41972-149">By default, this value comes from the currency on the header of the price list.</span></span> <span data-ttu-id="41972-150">Операция санатындағы баға үшін валютаны болдырмау мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="41972-150">For transaction category pricing, the currency can't be overridden.</span></span> | <span data-ttu-id="41972-151">Әдепкі бойынша, бұл валюта өзіндік құн мен сату бойынша шығындар класы үшін кіріс нақты жолдың бірлігіне бағаны пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="41972-151">This currency defaults on the per unit price of the incoming actual line for the expense transaction class for cost and sales.</span></span> |

## <a name="pricing-methods-for-expenses"></a><span data-ttu-id="41972-152">Шығындарға баға белгілеу әдістері</span><span class="sxs-lookup"><span data-stu-id="41972-152">Pricing methods for expenses</span></span>

<span data-ttu-id="41972-153">Шығындарды белгілеу жағдайында ғана сәйкес келетін санаттағы бағаларды орнатқан кезде, сіз келесі үш баға әдістерінің бірін пайдалана аласыз:</span><span class="sxs-lookup"><span data-stu-id="41972-153">When you set up category prices that are only relevant in the context of expense pricing, you can use one of the following three pricing methods:</span></span>

- <span data-ttu-id="41972-154">**Бірлік бағасы**</span><span class="sxs-lookup"><span data-stu-id="41972-154">**Price per unit**</span></span>
- <span data-ttu-id="41972-155">**Барлық құн**</span><span class="sxs-lookup"><span data-stu-id="41972-155">**At cost**</span></span>
- <span data-ttu-id="41972-156">**Құны бойынша үстеме баға**</span><span class="sxs-lookup"><span data-stu-id="41972-156">**Markup over cost**</span></span>

### <a name="price-per-unit"></a><span data-ttu-id="41972-157">Бірлік бағасы</span><span class="sxs-lookup"><span data-stu-id="41972-157">Price per unit</span></span>
<span data-ttu-id="41972-158">Бұл баға әдісі сатылым бағалары тізіміне байланысты санаттағы баға сызығында таңдалғанда, баға санаттағы және бірліктегі санаттағы бірліктердің тіркесімі үшін әдепкі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="41972-158">When this pricing method is selected on a category price line that is linked to a sales price list, the price defaults for the category and unit combination in both the estimate and the actual.</span></span> <span data-ttu-id="41972-159">Бағалау шығыстарға арналған жобалық бағалау жолдарына, ұсыныс жолын нақтылауға және шығыстарға арналған келісім-шарт жолын нақтылауға жатады.</span><span class="sxs-lookup"><span data-stu-id="41972-159">Estimate refers to the project estimate lines for expenses, the quote line detail, and the contract line detail for expenses.</span></span>

### <a name="at-cost"></a><span data-ttu-id="41972-160">Барлық құн</span><span class="sxs-lookup"><span data-stu-id="41972-160">At cost</span></span>
<span data-ttu-id="41972-161">Егер бұл баға белгілеу әдісі сату тізімімен байланысты санат бағасының жолында таңдалса, онда санат пен өлшем бірлігінің тіркесімі үшін әдепкі баға тек нақты шығындар үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="41972-161">When this pricing method is selected on the category price line that is linked to a sales price list, the price defaults for the category and unit combination only for the expense actual.</span></span> <span data-ttu-id="41972-162">Мысалы, шығын операциясы класы үшін төленбеген нақты сату деректері.</span><span class="sxs-lookup"><span data-stu-id="41972-162">For example, unbilled sales actuals for the expense transaction class.</span></span> <span data-ttu-id="41972-163">Бірлік бағасы осы шығын үшін нақты шығындар негізінде бірліктің бағасынан есеп-шотсыз нақты сату негізінде белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="41972-163">The unit price is set on the unbilled sales actual from the unit price on the cost actual for that expense.</span></span> <span data-ttu-id="41972-164">Өзіндік құн негізіндегі бағаның әдепкі мәні шығыстардың жобалық бағалауында немесе баға белгілеу жолында және шығыстар үшін келісім-шарт жолының бөлшектерінде орындалмайды.</span><span class="sxs-lookup"><span data-stu-id="41972-164">Price defaulting based on cost isn't done on project estimates for expenses or the quote line and contract line details for expenses.</span></span>

### <a name="markup-over-cost"></a><span data-ttu-id="41972-165">Құны бойынша үстеме баға</span><span class="sxs-lookup"><span data-stu-id="41972-165">Markup over cost</span></span>
<span data-ttu-id="41972-166">Егер бұл баға белгілеу әдісі сату тізімімен байланысты санат бағасының жолында таңдалса, онда санат пен өлшем бірлігінің тіркесімі үшін әдепкі баға тек нақты шығындар үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="41972-166">When this pricing method is selected on the category price line that is linked to a sales price list, the price defaults for the category and unit combination only for an expense actual.</span></span> <span data-ttu-id="41972-167">Мысалы, шығын операциясы класы үшін төленбеген нақты сату деректері.</span><span class="sxs-lookup"><span data-stu-id="41972-167">For example, unbilled sales actuals for the expense transaction class.</span></span> <span data-ttu-id="41972-168">Бірліктің бұл бағасы белгілі бір үстеме пайызды қолданғаннан кейін осы шығын үшін нақты шығындар бірлігінің бағасынан есептік мәнге дейін шот-фактурасыз нақты сату үшін белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="41972-168">This unit price is set on the unbilled sales actual to a calculated value from the unit price on the cost actual for that expense after the defined markup percent is applied.</span></span> <span data-ttu-id="41972-169">Өзіндік құн негізіндегі бағаның әдепкі мәні шығыстардың жобалық бағалауында немесе баға белгілеу жолында және шығыстар үшін келісім-шарт жолының бөлшектерінде орындалмайды.</span><span class="sxs-lookup"><span data-stu-id="41972-169">Price defaulting based on cost isn't done in on project estimates for expenses or quote line and contract line details for expenses.</span></span>