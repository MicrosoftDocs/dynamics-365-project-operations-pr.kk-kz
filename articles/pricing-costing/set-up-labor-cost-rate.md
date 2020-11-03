---
title: Еңбектің құн мөлшерлемелерін орнату
description: Бұл тақырыпта Project Operations бағдарламасында еңбектің құн мөлшерлемелерін орнату әдісі туралы ақпарат берілген
author: rumant
manager: Annbe
ms.date: 10/12/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d17f266b6e34fc2a2743fe19fd18b15fb992ceef
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079557"
---
# <a name="set-up-labor-cost-rates"></a><span data-ttu-id="e4291-103">Еңбектің құн мөлшерлемелерін орнату</span><span class="sxs-lookup"><span data-stu-id="e4291-103">Set up labor cost rates</span></span>

<span data-ttu-id="e4291-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="e4291-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="e4291-105">Әрбір бағатізбеде бағатізбенің мазмұны және жарамдылық мерзімімен тураланған еңбек мөлшерлерінің (рөл бағалары) жиынтығы бар.</span><span class="sxs-lookup"><span data-stu-id="e4291-105">Each price list has a set of labor rates (role prices) that align with the content and date effectivity of the price list.</span></span>

1. <span data-ttu-id="e4291-106">Бағатізбені жасап, **Рөл бағасы** қойыншасында ішкі тордан **+ жаңа рөл бағасы** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e4291-106">Create a price list and on the **Role Price** tab, in the sub-grid, select **New Role**.</span></span>
2. <span data-ttu-id="e4291-107">**Жылдам жасау** бетінде рөл мен ұйымдық бөлімшені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e4291-107">On the **Quick Create** page, select the role and organization unit.</span></span>
3. <span data-ttu-id="e4291-108">Кез келген басқа қажетті өріс туралы ақпаратты енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="e4291-108">Enter any other required field information.</span></span>

<span data-ttu-id="e4291-109">Келесі кестеде құн бағатізбесінде еңбек мөлшерлерін жасау кезінде маңызды кейбір өрістер қамтылған.</span><span class="sxs-lookup"><span data-stu-id="e4291-109">The following table includes some of the fields that are important when creating labor rates on a cost price list.</span></span>

| <span data-ttu-id="e4291-110">Өріс</span><span class="sxs-lookup"><span data-stu-id="e4291-110">Field</span></span> | <span data-ttu-id="e4291-111">Орналасқан жері</span><span class="sxs-lookup"><span data-stu-id="e4291-111">Location</span></span> | <span data-ttu-id="e4291-112">Маңыздылық, мақсаты және нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="e4291-112">Relevance, purpose, and guidance</span></span> | <span data-ttu-id="e4291-113">Төменгі әсер</span><span class="sxs-lookup"><span data-stu-id="e4291-113">Downstream impact</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="e4291-114">Рөл</span><span class="sxs-lookup"><span data-stu-id="e4291-114">Role</span></span> | <span data-ttu-id="e4291-115">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="e4291-115">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="e4291-116">Құн мөлшері қолданылатын рөлді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e4291-116">Select the role that the cost rate applies to.</span></span> | <span data-ttu-id="e4291-117">Кіріс болжамы мен нақты жолдағы рөл рөлдің құнын әдепкі бойынша орнату үшін осы жолмен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="e4291-117">The role on the incoming estimate or actual will be matched against this line to default the cost of the role.</span></span> |
| <span data-ttu-id="e4291-118">Ресурс компаниясы</span><span class="sxs-lookup"><span data-stu-id="e4291-118">Resourcing Company</span></span> | <span data-ttu-id="e4291-119">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="e4291-119">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="e4291-120">Осы рөл тағайындалған заңды нысанды таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e4291-120">Select the legal entity that the role is assigned to.</span></span> <span data-ttu-id="e4291-121">Мысалы, Fabrikam India әзірлеушісі немесе Fabrikam USA әзірлеушісі.</span><span class="sxs-lookup"><span data-stu-id="e4291-121">For example, a developer from Fabrikam India or a developer from Fabrikam USA.</span></span> | <span data-ttu-id="e4291-122">Кіріс болжамы мен нақты жолдағы ресурс компаниясы рөлдің құн мөлшерлемесін әдепкі бойынша орнату үшін осы жолмен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="e4291-122">The resourcing company on the incoming estimate or actual will be matched against this line to default the cost rate of the role.</span></span> |
| <span data-ttu-id="e4291-123">Ресурс бірлігі</span><span class="sxs-lookup"><span data-stu-id="e4291-123">Resourcing Unit</span></span> | <span data-ttu-id="e4291-124">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="e4291-124">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="e4291-125">Осы рөл пайдаланылатын ұйымдық бөлімшені немесе компания бөлімін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e4291-125">Select the organizational unit or division of the company from where this role will be used.</span></span> <span data-ttu-id="e4291-126">Мысалы, Fabrikam India компаниясының Robotics бөлімінің әзірлеушісі немесе Fabrikam USA компаниясының Software бөлімінің әзірлеушісі.</span><span class="sxs-lookup"><span data-stu-id="e4291-126">For example, a developer from the Robotics division of Fabrikam India or a developer from the Software division of Fabrikam USA.</span></span> | <span data-ttu-id="e4291-127">Кіріс болжамы мен нақты жолдағы ресурс бірлігі рөлдің құн мөлшерлемесін әдепкі бойынша орнату үшін осы жолмен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="e4291-127">The resourcing unit on the incoming estimate or actual will be matched against this line to default the cost of the role.</span></span> |
| <span data-ttu-id="e4291-128">Баға</span><span class="sxs-lookup"><span data-stu-id="e4291-128">Price</span></span> | <span data-ttu-id="e4291-129">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="e4291-129">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="e4291-130">Рөл, ресурс компаниясы және ресурс бірлігі тіркесімі үшін құн мөлшерлемесін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4291-130">Set up the cost rate for the role, resourcing company, and resourcing unit combination.</span></span> <span data-ttu-id="e4291-131">Мысалы, Fabrikam India әзірлеушісінің құны - 1000 INR немесе Fabrikam USA әзірлеушісінің құны - 150 USD.</span><span class="sxs-lookup"><span data-stu-id="e4291-131">For example, a developer from Fabrikam India costs 1000 INR or a developer from Fabrikam USA costs 150 USD.</span></span> | <span data-ttu-id="e4291-132">Бұл баға — **Уақыт** транзакция класы үшін кіріс болжамының немесе нақты жолдың бірлік құнына арналған әдепкі құн мөлшерлемесі.</span><span class="sxs-lookup"><span data-stu-id="e4291-132">The price is the cost rate that defaults on the per unit cost of the incoming estimate or actual line for the **Time** transaction class.</span></span> |
| <span data-ttu-id="e4291-133">Валюта</span><span class="sxs-lookup"><span data-stu-id="e4291-133">Currency</span></span> | <span data-ttu-id="e4291-134">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="e4291-134">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="e4291-135">Әдепкі бойынша, валюта мәні құн бағатізбесінің тақырыбындағы валютадан келеді, бірақ оны алдын ала анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="e4291-135">By default, the currency value comes from the currency on the header of the cost price list but can be overridden.</span></span> <span data-ttu-id="e4291-136">Мысалы, Fabrikam India компаниясы әзірлеушісінің құны – 1000 INR.</span><span class="sxs-lookup"><span data-stu-id="e4291-136">For example, a developer from Fabrikam India costs 1000 INR.</span></span> <span data-ttu-id="e4291-137">Fabrikam USA компаниясы әзірлеушісінің құны – 150 USD.</span><span class="sxs-lookup"><span data-stu-id="e4291-137">A developer from Fabrikam USA costs 150 USD.</span></span> | <span data-ttu-id="e4291-138">Бұл валюта **Уақыт** транзакция класы үшін кіріс нақты шығын жолының бірлік құнына арналған әдепкі валюта болып табылады.</span><span class="sxs-lookup"><span data-stu-id="e4291-138">This currency defaults on the per unit cost of the incoming actual cost line for the **Time** transaction class.</span></span> <span data-ttu-id="e4291-139">Жоба болжамында валюта мәні жоба валютасына түрлендіріледі және болжамның уақыт кезеңіндегі көрінісінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="e4291-139">On a project estimate, the currency value is converted to the project currency and shown on the Time-phased view of the estimate.</span></span> |
| <span data-ttu-id="e4291-140">Бірлік кестесі</span><span class="sxs-lookup"><span data-stu-id="e4291-140">Unit Schedule</span></span> | <span data-ttu-id="e4291-141">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="e4291-141">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="e4291-142">Бірлік кестесі Уақыт класы үшін әдепкі болып табылады және Рөл бағасының нысанында өзгертілмейді, өйткені ол мөлшерлерді уақыт бірлігі бойынша көрсету үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e4291-142">The unit schedule defaults to Time and can't be changed on the Role price entity because it is used express rates by units of time.</span></span> | <span data-ttu-id="e4291-143">Төменгі әсері жоқ.</span><span class="sxs-lookup"><span data-stu-id="e4291-143">There is no downstream impact.</span></span> |
| <span data-ttu-id="e4291-144">Бірлік</span><span class="sxs-lookup"><span data-stu-id="e4291-144">Unit</span></span> | <span data-ttu-id="e4291-145">**Жалпы** қойыншасы және **Жылдам жасау** беттері</span><span class="sxs-lookup"><span data-stu-id="e4291-145">**General** tab and **Quick Create** pages</span></span> | <span data-ttu-id="e4291-146">Әдепкі бойынша, мән құн бағатізбесінің тақырыбындағы **Уақыт бірлігі** өрісінен келеді.</span><span class="sxs-lookup"><span data-stu-id="e4291-146">By default, the value comes from the **Time Unit** field on the header of the cost price list.</span></span> <span data-ttu-id="e4291-147">Мәнді алдын ала анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="e4291-147">The value can be overridden.</span></span> <span data-ttu-id="e4291-148">Мысалы, Fabrikam India компаниясы әзірлеушісінің **Үндістан күні** үшін құны 1000 INR мөлшерін құрайды.</span><span class="sxs-lookup"><span data-stu-id="e4291-148">For example, a developer from Fabrikam India costs 1000 INR per **India Day**.</span></span> <span data-ttu-id="e4291-149">Fabrikam USA компаниясы әзірлеушінің **АҚШ күні** үшін құны 150 USD мөлшерін құрайды.</span><span class="sxs-lookup"><span data-stu-id="e4291-149">A developer from Fabrikam USA costs 150 USD per **US Day**.</span></span> | <span data-ttu-id="e4291-150">Кіріс болжамында немесе нақты жолда бірлік бағасының әдепкі мәнін есептеу мақсатында жүйе бірлік құнын есептеу үшін бірліктер және түрлендіру жүйесін негізгі өлшем бірліктерінде пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e4291-150">The system uses the system of units and conversion in base units to compute a per unit cost to calculate the default price per unit on an incoming estimate or actual line.</span></span> <span data-ttu-id="e4291-151">Мысалы, Үндістаннан келген әзірлеуші үшін болжам 10 **Үндістан күні** жұмысы, ал **Үндістан күні** бірлігі 10 сағат ретінде анықталады.</span><span class="sxs-lookup"><span data-stu-id="e4291-151">For example, an estimate is for 10 **India Days** worth of work for a developer from India, and the unit, **India Day** is defined as 10 hours.</span></span> <span data-ttu-id="e4291-152">Болжам жолының құнын есептеу кезінде бағдарлама болжамдағы бірлік құнын есептейді: 1000 INR/10 сағат = сағатына 100 INR, ол АҚШ долларына түрлендірілген және **Жобалық болжамдар** бетінде бірлік құны ретінде көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="e4291-152">When costing that estimate line, the application calculates the unit cost on the estimate as: 1000 INR/ 10 hours = 100 INR per hour which is converted into USD and shown as the unit cost on the **Project Estimates** page.</span></span> |

## <a name="transfer-pricing-and-costs-for-resources-outside-of-your-division-or-legal-entity"></a><span data-ttu-id="e4291-153">Бөлімнен немесе заңды нысаннан тыс ресурстарға арналған тасымалдау бағалары мен құндар</span><span class="sxs-lookup"><span data-stu-id="e4291-153">Transfer pricing and costs for resources outside of your division or legal entity</span></span>

<span data-ttu-id="e4291-154">Жобаға негізделген компанияларда жобаларда әртүрлі заңды нысандардың немесе бөлімдердің қызметкерлерін пайдалану қалыпты жағдай болып табылады.</span><span class="sxs-lookup"><span data-stu-id="e4291-154">In project-based companies, it's common to use employees from different legal entities or divisions on projects.</span></span> <span data-ttu-id="e4291-155">Жоба белгілі бір заңды нысаннан орындалуы мүмкін, бірақ жобамен жұмыс жасайтын қызметкерлер немесе кеңесшілер сол заңды нысаннан немесе басқасынан немесе екеулерінің тіркесімінен келуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e4291-155">A project can be executed by one legal entity, but the employees or consultants that work on the project could come from the same legal entity or from a different one, or there may be a combination of both.</span></span> <span data-ttu-id="e4291-156">Dynamics 365 Project Operations бағдарламасында жобаны жеткізуді жүзеге асыратын заңды нысан **Иеленуші компания** деп, ал жеткізуді жүзеге асыратын бөлім **Келісім-шарт бірлігі** деп аталады.</span><span class="sxs-lookup"><span data-stu-id="e4291-156">In Dynamics 365 Project Operations, the legal entity that owns the delivery of the project is the **Owning Company** and the division that owns the delivery is the **Contracting Unit**.</span></span> <span data-ttu-id="e4291-157">Ресурстарды ұсынатын басқа заңды нысандар **Ресурс компаниялары** деп, ал ресурстарды қамтамасыз ететін бөлімдер **Ресурс бірліктері** деп аталады.</span><span class="sxs-lookup"><span data-stu-id="e4291-157">Other legal entities that provide resources are the **Resourcing companies** and divisions that provide resources are the **Resourcing Units**.</span></span> <span data-ttu-id="e4291-158">Көптеген елдерде компаниялар ресурстарды пайдаланғаны үшін ресурстарды ұсынатын заңды нысанға немесе бөлімге, иеленуші компанияға және келісім-шарт жасаушы бөлімге ақы төлеуін қамтамасыз етуге міндетті.</span><span class="sxs-lookup"><span data-stu-id="e4291-158">In most countries, companies are required to ensure that the resourcing legal entity or division, charge the owning company and the contracting unit for the use of resources.</span></span>

<span data-ttu-id="e4291-159">Мысалы, Fabrikam корпорациясы Fabrikam India-Robotics компаниясының Fabrikam US-Robotics немесе Fabrikam UK-Robotics компаниясымен келісілген құн мөлшерлемесі бар картасын қамтамасыз етуі керек.</span><span class="sxs-lookup"><span data-stu-id="e4291-159">For example, the Fabrikam corporation must ensure that Fabrikam India-Robotics has a negotiated a cost rate card with Fabrikam US-Robotics or Fabrikam UK-Robotics.</span></span>

<span data-ttu-id="e4291-160">Fabrikam India-Robotic компаниясының әзірлеушісі Fabrikam US-Robotics компаниясына қарыз берген кезде $100 және Fabrikam U-Robotics компаниясына қарыз бергенде $150 ақы төлейді.</span><span class="sxs-lookup"><span data-stu-id="e4291-160">A developer from Fabrikam India-Robotic charges $100 when lent to Fabrikam US-Robotics and $150 when lent to Fabrikam U-Robotics.</span></span>

### <a name="set-up-costs-for-outside-resources"></a><span data-ttu-id="e4291-161">Сыртқы ресурстарға құндарды орнату</span><span class="sxs-lookup"><span data-stu-id="e4291-161">Set up costs for outside resources</span></span>

1. <span data-ttu-id="e4291-162">*Fabrikam US-Robotics құн мөлшерлемелері* атты құн бағатізбесін жасаңыз және күннің тиімді ауқымын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4291-162">Create a cost price list called, *Fabrikam US-Robotics cost rates* and set a date effective range.</span></span>
2. <span data-ttu-id="e4291-163">Құн бағатізбесінде мөлшерлерді келесі кестедегі ақпаратты пайдалана отырып орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4291-163">In the cost price list, set up rates using information from the following table.</span></span> 

| <span data-ttu-id="e4291-164">Рөл</span><span class="sxs-lookup"><span data-stu-id="e4291-164">Role</span></span> | <span data-ttu-id="e4291-165">Ресурс компаниясы</span><span class="sxs-lookup"><span data-stu-id="e4291-165">Resourcing Company</span></span> | <span data-ttu-id="e4291-166">Ресурс бірлігі</span><span class="sxs-lookup"><span data-stu-id="e4291-166">Resourcing Unit</span></span> | <span data-ttu-id="e4291-167">Құн мөлшерлемесі</span><span class="sxs-lookup"><span data-stu-id="e4291-167">Cost rate</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="e4291-168">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="e4291-168">Developer</span></span> | <span data-ttu-id="e4291-169">Fabrikam India</span><span class="sxs-lookup"><span data-stu-id="e4291-169">Fabrikam India</span></span> | <span data-ttu-id="e4291-170">Fabrikam India-Robotics</span><span class="sxs-lookup"><span data-stu-id="e4291-170">Fabrikam India-Robotics</span></span> | <span data-ttu-id="e4291-171">$100</span><span class="sxs-lookup"><span data-stu-id="e4291-171">$100</span></span> |
| <span data-ttu-id="e4291-172">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="e4291-172">Developer</span></span> | <span data-ttu-id="e4291-173">Fabrikam Philippines</span><span class="sxs-lookup"><span data-stu-id="e4291-173">Fabrikam Philippines</span></span> | <span data-ttu-id="e4291-174">Fabrikam Philippines-Robotics</span><span class="sxs-lookup"><span data-stu-id="e4291-174">Fabrikam Philippines-Robotics</span></span> | <span data-ttu-id="e4291-175">$90</span><span class="sxs-lookup"><span data-stu-id="e4291-175">$90</span></span> |
| <span data-ttu-id="e4291-176">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="e4291-176">Developer</span></span> | <span data-ttu-id="e4291-177">Fabrikam US</span><span class="sxs-lookup"><span data-stu-id="e4291-177">Fabrikam US</span></span> | <span data-ttu-id="e4291-178">Fabrikam US-Robotics</span><span class="sxs-lookup"><span data-stu-id="e4291-178">Fabrikam US-Robotics</span></span> | <span data-ttu-id="e4291-179">$150</span><span class="sxs-lookup"><span data-stu-id="e4291-179">$150</span></span> |

3. <span data-ttu-id="e4291-180">Бұл құн бағатізбесін Fabrikam US-Robotics ұйымдық бөлімшесіне тіркеңіз.</span><span class="sxs-lookup"><span data-stu-id="e4291-180">Attach this cost price list to the Fabrikam US-Robotics organization unit.</span></span>

### <a name="set-up-transfer-pricing-for-a-resource-in-the-appropriate-currency"></a><span data-ttu-id="e4291-181">Тиісті валютадағы ресурс үшін тасымалдау бағасын орнату</span><span class="sxs-lookup"><span data-stu-id="e4291-181">Set up transfer pricing for a resource in the appropriate currency</span></span> 

<span data-ttu-id="e4291-182">Project Operations бағдарламасында ресурс бағасын кез келген валютада орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="e4291-182">In Project Operations, resource pricing can be set up in any currency.</span></span> <span data-ttu-id="e4291-183">Валюта бағатізбегіндегі тақырыпқа сәйкес келеді, бірақ оны өзгертуге болады.</span><span class="sxs-lookup"><span data-stu-id="e4291-183">The currency defaults to what is on the price list header, but can be changed.</span></span>

<span data-ttu-id="e4291-184">Тасымалдау бағасын орнату мысалын пайдаланып, ақпаратты келесіге өзгертуге болады:</span><span class="sxs-lookup"><span data-stu-id="e4291-184">Using the example for transfer price set up, the information could be changed to:</span></span>

<span data-ttu-id="e4291-185">Fabrikam корпорациясы Fabrikam India-Robotics компаниясының Fabrikam US-Robotics немесе Fabrikam UK-Robotics компаниясымен келісілген құн мөлшерлемесін қамтамасыз етуі керек.</span><span class="sxs-lookup"><span data-stu-id="e4291-185">Fabrikam corporation must ensure that Fabrikam India-Robotics has a negotiated a cost rate with Fabrikam US-Robotics or Fabrikam UK-Robotics.</span></span>

<span data-ttu-id="e4291-186">Fabrikam India-Robotics компаниясының әзірлеушісінің құны Fabrikam US-Robotics компаниясына қарыз берген кезде 5000 INR және Fabrikam U-Robotics компаниясына қарыз бергенде 5500 INR болады.</span><span class="sxs-lookup"><span data-stu-id="e4291-186">A developer from Fabrikam India-Robotics costs 5000 INR when lent to Fabrikam US-Robotics and 5500 INR when lent to Fabrikam UK-Robotics.</span></span>

<span data-ttu-id="e4291-187">Fabrikam US-Robotics құн бағатізбесінде құн мөлшерлемелері төмендегідей көрсетілуі мүмкін:</span><span class="sxs-lookup"><span data-stu-id="e4291-187">In the cost price list for Fabrikam US-Robotics, cost rates can be expressed as:</span></span>

| <span data-ttu-id="e4291-188">Рөл</span><span class="sxs-lookup"><span data-stu-id="e4291-188">Role</span></span> | <span data-ttu-id="e4291-189">Ресурс компаниясы</span><span class="sxs-lookup"><span data-stu-id="e4291-189">Resourcing Company</span></span> | <span data-ttu-id="e4291-190">Құны</span><span class="sxs-lookup"><span data-stu-id="e4291-190">Cost</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e4291-191">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="e4291-191">Developer</span></span> | <span data-ttu-id="e4291-192">Fabrikam India</span><span class="sxs-lookup"><span data-stu-id="e4291-192">Fabrikam India</span></span> | <span data-ttu-id="e4291-193">5000 INR</span><span class="sxs-lookup"><span data-stu-id="e4291-193">5000 INR</span></span> |
| <span data-ttu-id="e4291-194">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="e4291-194">Developer</span></span> | <span data-ttu-id="e4291-195">Fabrikam US</span><span class="sxs-lookup"><span data-stu-id="e4291-195">Fabrikam US</span></span> | <span data-ttu-id="e4291-196">115 USD</span><span class="sxs-lookup"><span data-stu-id="e4291-196">115 USD</span></span> |

<span data-ttu-id="e4291-197">Fabrikam UK-Robotics құн бағатізбесінде құн мөлшерлемелері төмендегідей көрсетілуі мүмкін:</span><span class="sxs-lookup"><span data-stu-id="e4291-197">In the cost price list for Fabrikam UK-Robotics, cost rates can be expressed below:</span></span>

| <span data-ttu-id="e4291-198">Рөл</span><span class="sxs-lookup"><span data-stu-id="e4291-198">Role</span></span> | <span data-ttu-id="e4291-199">Ресурс компаниясы</span><span class="sxs-lookup"><span data-stu-id="e4291-199">Resourcing company</span></span> | <span data-ttu-id="e4291-200">Құны</span><span class="sxs-lookup"><span data-stu-id="e4291-200">Cost</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e4291-201">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="e4291-201">Developer</span></span> | <span data-ttu-id="e4291-202">Fabrikam India</span><span class="sxs-lookup"><span data-stu-id="e4291-202">Fabrikam India</span></span> | <span data-ttu-id="e4291-203">5500 INR</span><span class="sxs-lookup"><span data-stu-id="e4291-203">5500 INR</span></span> |
| <span data-ttu-id="e4291-204">Әзірлеуші</span><span class="sxs-lookup"><span data-stu-id="e4291-204">Developer</span></span> | <span data-ttu-id="e4291-205">Fabrikam UK</span><span class="sxs-lookup"><span data-stu-id="e4291-205">Fabrikam UK</span></span> | <span data-ttu-id="e4291-206">115 GBP</span><span class="sxs-lookup"><span data-stu-id="e4291-206">115 GBP</span></span> |

<span data-ttu-id="e4291-207">Құн бағатізбесі еңбек мөлшерлерін бірнеше валютада қамтамасыз ете алады.</span><span class="sxs-lookup"><span data-stu-id="e4291-207">The cost price list can provide labor rates in multiple currencies.</span></span> <span data-ttu-id="e4291-208">Жоба бойынша құн болжамын құру кезінде Project Operations бағдарламасы осы құн мөлшерлемелерін жоба валютасына түрлендіреді және оны пайдаланушыға көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="e4291-208">When generating a cost estimate on the project, Project Operations will convert these cost rates into the project currency and display it to the user.</span></span> <span data-ttu-id="e4291-209">Уақыт жазбасы мақұлданған және нақты құн жасалған кезде, нақты құн сәйкес келетін рөл бағасы жолының валютасымен құн бағатізбесінде бағаланады.</span><span class="sxs-lookup"><span data-stu-id="e4291-209">When a time entry is approved and a cost actual is created, the cost actual is priced in the currency of that matching role price line on the cost price list.</span></span> <span data-ttu-id="e4291-210">Бір жоба бойынша нақты құн бірнеше валютада жазылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e4291-210">Cost actuals for time on a single project can be recorded in multiple currencies.</span></span> <span data-ttu-id="e4291-211">Алайда жоба деңгейіндегі нақты еңбек құндарын жинау немесе жинақтау кезінде Project Operations бағдарламасы барлық еңбек құндарының сомаларын пайдаланушы көре алатын жоба валютасына түрлендіреді.</span><span class="sxs-lookup"><span data-stu-id="e4291-211">However, when rolling up or summarizing the actual labor costs at the project level, Project Operations will convert all labor cost amounts into the project currency, which the user can view.</span></span>