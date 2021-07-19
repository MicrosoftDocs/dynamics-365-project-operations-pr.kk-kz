---
title: Қолда бар тауарлар
description: Бұл тақырыпта Microsoft Dynamics 365 Project Operations бағдарламасында нақты көрсеткіштермен жұмыс жасау жолы туралы ақпарат берілген.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: intro-internal
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9e046602a3005930c41ab8c50472d5b1a72303c6
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368618"
---
# <a name="actuals"></a><span data-ttu-id="e3282-103">Қолда бар тауарлар</span><span class="sxs-lookup"><span data-stu-id="e3282-103">Actuals</span></span> 

<span data-ttu-id="e3282-104">_**Қолданылу аясы:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="e3282-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e3282-105">Нақты көрсеткіштер жобаның қаралған және бекітілген қаржылық және жоспарлық барысын білдіреді.</span><span class="sxs-lookup"><span data-stu-id="e3282-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="e3282-106">Олар уақытты, шығынды, материалды пайдалану жазбаларын, журналдағы жазбалар мен есеп-шоттарды бекіту нәтижесінде жасалады.</span><span class="sxs-lookup"><span data-stu-id="e3282-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="e3282-107">Журнал жолдары және уақытты ұсыну</span><span class="sxs-lookup"><span data-stu-id="e3282-107">Journal lines and time submission</span></span>

<span data-ttu-id="e3282-108">Уақыт жазбасы туралы қосымша ақпаратты [Уақыт жазбасын шолу](../time/time-entry-overview.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="e3282-109">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="e3282-109">Time and materials</span></span>

<span data-ttu-id="e3282-110">Уақыт жазбасы уақыт және материалдар келісім-шарт жолына тағайындалған жобамен байланыстырылған кезде, жүйе екі журнал жолын жасайды, оның біреуі өзіндік құны, екіншісі шот ұсынылмаған сатылым.</span><span class="sxs-lookup"><span data-stu-id="e3282-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="e3282-111">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="e3282-111">Fixed price</span></span>

<span data-ttu-id="e3282-112">Бағасы бекітілген келісім-шарт жолына тағайындалған жобаға уақыт жазбасы жіберілген кезде, жүйе журнал жолын тек құн үшін жасайды.</span><span class="sxs-lookup"><span data-stu-id="e3282-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="e3282-113">Әдепкі баға</span><span class="sxs-lookup"><span data-stu-id="e3282-113">Default pricing</span></span>

<span data-ttu-id="e3282-114">Әдеттегі бағаларды жасау логикасы журнал жолында орналасқан.</span><span class="sxs-lookup"><span data-stu-id="e3282-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="e3282-115">Уақыт жазбасындағы өріс мәндері журнал жолына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="e3282-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="e3282-116">Бұл мәндер транзакция күнін, жоба тағайындалған келісім-шарт жолын және тиісті бағатізбедегі валютаны қамтиды.</span><span class="sxs-lookup"><span data-stu-id="e3282-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="e3282-117">**Рөл** және **Ресурс бірлігі** сияқты әдепкі бағаларды көрсететін өрістер журнал жолында тиісті бағаны анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e3282-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="e3282-118">Уақыт жазбасына реттелетін өрісті қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="e3282-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="e3282-119">Өріс мәнін нақты көрсеткіштерге тарату қажет болса, **Нақты көрсеткіштер** және **Журнал жолы** кестелерінде өріс жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="e3282-120">Таңдалған өріс мәнін транзакция көздерін пайдаланып журнал жолы арқылы "Уақыт жазбасынан" "Нақты көрсеткіштерге" тарату үшін реттелетін кодты пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="e3282-121">Транзакция көздері мен байланыстар туралы қосымша ақпарат алу үшін [Нақты көрсеткіштерді бастапқы жазбалармен байланыстыру](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="e3282-122">Журнал жолдары және негізгі шығысты жіберу</span><span class="sxs-lookup"><span data-stu-id="e3282-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="e3282-123">Шығыс жазбасы туралы қосымша ақпаратты [Шығыстарды шолу](../expense/expense-overview.md) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="e3282-124">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="e3282-124">Time and materials</span></span>

<span data-ttu-id="e3282-125">Негізгі шығыс жазбасы уақыт және материалдар келісім-шарт жолына тағайындалған жобамен байланыстырылған кезде, жүйе екі журнал жолын жасайды, оның біреуі өзіндік құны, екіншісі шот ұсынылмаған сатылым.</span><span class="sxs-lookup"><span data-stu-id="e3282-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="e3282-126">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="e3282-126">Fixed price</span></span>

<span data-ttu-id="e3282-127">Бағасы бекітілген келісім-шарт жолына тағайындалған жобамен жіберілген негізгі шығын жазбасы байланыстырылған кезде, жүйе құн үшін бір журнал жолын жасайды.</span><span class="sxs-lookup"><span data-stu-id="e3282-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="e3282-128">Әдепкі баға</span><span class="sxs-lookup"><span data-stu-id="e3282-128">Default pricing</span></span>

<span data-ttu-id="e3282-129">Шығыстар бойынша әдепкі бағаларды енгізу логикасы шығыстар санатына негізделген.</span><span class="sxs-lookup"><span data-stu-id="e3282-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="e3282-130">Транзакция жасалған күн, жоба тағайындалған келісім-шарт жолы және валюта тиісті бағатізбені анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e3282-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="e3282-131">**Транзакция санаты** және **Бірлік** сияқты әдепкі бағаларды көрсететін өрістер журнал жолында тиісті бағаны анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e3282-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="e3282-132">Алайда бұл бағатізбедегі баға әдісі **Бірлік бағасы** болған кезде ғана орындалады.</span><span class="sxs-lookup"><span data-stu-id="e3282-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="e3282-133">Егер бағалау әдісі **Барлық құн** немесе **Құн бойынша үстеме баға** болса, шығындар жазбасы жасалған кезде енгізілген баға құны үшін пайдаланылады және сатылым журнал жолы бойынша бағалау әдісі негізінде есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e3282-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="e3282-134">Шығын жазбасына реттелетін өрісті қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="e3282-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="e3282-135">Өріс мәнін нақты көрсеткіштерге тарату қажет болса, **Нақты көрсеткіштер** және **Журнал жолы** кестелерінде өріс жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="e3282-136">Таңдалған өріс мәнін транзакция көздерін пайдаланып журнал жолы арқылы "Уақыт жазбасынан" "Нақты көрсеткіштерге" тарату үшін реттелетін кодты пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="e3282-137">Транзакция көздері мен байланыстар туралы қосымша ақпарат алу үшін [Нақты көрсеткіштерді бастапқы жазбалармен байланыстыру](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="e3282-138">Журнал жолдары және материалды пайдалану журналын жіберу</span><span class="sxs-lookup"><span data-stu-id="e3282-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="e3282-139">Шығын жазбасы туралы қосымша ақпаратты мына жерден қараңыз: [Материалды пайдалану журналы](../material/material-usage-log.md).</span><span class="sxs-lookup"><span data-stu-id="e3282-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="e3282-140">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="e3282-140">Time and materials</span></span>

<span data-ttu-id="e3282-141">Жіберілген материалды пайдалану журналының жазбасы уақыт пен материалдар келісім-шарт жолымен салыстырылған жобамен байланыстырылған кезде, жүйе екі журнал жолын жасайды, оның біреуі құнға және екіншісі шот ұсынылмаған сатылымға арналған.</span><span class="sxs-lookup"><span data-stu-id="e3282-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="e3282-142">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="e3282-142">Fixed price</span></span>

<span data-ttu-id="e3282-143">Бағасы бекітілген келісім-шарт жолына тағайындалған жобамен жіберілген материалды пайдалану журналының жазбасы байланыстырылған кезде, жүйе құн үшін бір журнал жолын жасайды.</span><span class="sxs-lookup"><span data-stu-id="e3282-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="e3282-144">Әдепкі баға</span><span class="sxs-lookup"><span data-stu-id="e3282-144">Default pricing</span></span>

<span data-ttu-id="e3282-145">Материалдың әдепкі бағаларын енгізу логикасы өнім мен бірліктің тіркесіміне негізделген.</span><span class="sxs-lookup"><span data-stu-id="e3282-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="e3282-146">Транзакция жасалған күн, жоба тағайындалған келісім-шарт жолы және валюта тиісті бағатізбені анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e3282-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="e3282-147">**Өнім идентификаторы** және **Бірлік** сияқты әдепкі бағаларды көрсететін өрістер журнал жолында тиісті бағаны анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e3282-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="e3282-148">Алайда бұл тек каталог өнімдері үшін орындалады.</span><span class="sxs-lookup"><span data-stu-id="e3282-148">However, this only works for catalog products.</span></span> <span data-ttu-id="e3282-149">Енгізілген өнімдер үшін материалды пайдалану журналының жазбасы енгізілген кезде енгізілген баға журнал жолдарындағы шығындар мен сату бағасы үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e3282-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="e3282-150">**Материалды пайдалану журналы** жазбасына реттелетін өрісті қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="e3282-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="e3282-151">Өріс мәнін нақты көрсеткіштерге тарату қажет болса, **Нақты көрсеткіштер** және **Журнал жолы** кестелерінде өріс жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="e3282-152">Таңдалған өріс мәнін транзакция көздерін пайдаланып журнал жолы арқылы "Уақыт жазбасынан" "Нақты көрсеткіштерге" тарату үшін реттелетін кодты пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="e3282-153">Транзакция көздері мен байланыстар туралы қосымша ақпарат алу үшін [Нақты көрсеткіштерді бастапқы жазбалармен байланыстыру](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="e3282-154">Шығыстарды жазу үшін жазба журналдарын пайдалану</span><span class="sxs-lookup"><span data-stu-id="e3282-154">Use entry journals to record costs</span></span>

<span data-ttu-id="e3282-155">Құнды немесе материалдағы, алымдағы, уақыттағы, шығыстағы табысты немесе салық транзакцияларының кластарын жазу үшін жазба журналдарын пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="e3282-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="e3282-156">Журналдарды келесі мақсаттарда пайдалануға болады:</span><span class="sxs-lookup"><span data-stu-id="e3282-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="e3282-157">Транзакцияның нақты көрсеткіштерін басқа жүйеден Microsoft Dynamics 365 Project Operations бағдарламасына ауыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="e3282-158">Басқа жүйеде орын алған шығындарды жазыңыз.</span><span class="sxs-lookup"><span data-stu-id="e3282-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="e3282-159">Бұл құндар сатып алу немесе қосымша келісім-шарт құнын қамтуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e3282-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e3282-160">Бағдарлама журнал жолының түрін немесе журнал жолына енгізілген тиісті бағаны тексермейді.</span><span class="sxs-lookup"><span data-stu-id="e3282-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="e3282-161">Сондықтан, нақты көрсеткіштердің жобаға тигізетін бухгалтерлік есебінің әсерін толық білетін пайдаланушы ғана нақты көрсеткіштер жасау үшін жазба журналдарын пайдалануы керек.</span><span class="sxs-lookup"><span data-stu-id="e3282-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="e3282-162">Осы журнал түрінің әсеріне байланысты, жазба журналдарын жасауға кімнің рұқсаты бар екенін мұқият таңдау керек.</span><span class="sxs-lookup"><span data-stu-id="e3282-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="e3282-163">Жоба оқиғаларының негізінде нақты көрсеткіштерді жазу</span><span class="sxs-lookup"><span data-stu-id="e3282-163">Record actuals based on project events</span></span>

<span data-ttu-id="e3282-164">Project Operations жүйесі жоба барысында орын алатын барлық қаржылық операцияларды жазады.</span><span class="sxs-lookup"><span data-stu-id="e3282-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="e3282-165">Бұл операциялар нақты мәндер ретінде жазылады.</span><span class="sxs-lookup"><span data-stu-id="e3282-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="e3282-166">Төмендегі кестелерде жобаның уақыт және материалдық екеніне, бағасының бекітілгеніне, алдын ала сату кезеңінде екеніне немесе ішкі жоба екеніне байланысты жасалған әртүрлі нақты мәндер көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="e3282-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="e3282-167">Ресурс жобаның келісімшарт бірлігімен бірдей ұйымдық бөлімшеге тиесілі</span><span class="sxs-lookup"><span data-stu-id="e3282-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="e3282-168">Оқиға</span><span class="sxs-lookup"><span data-stu-id="e3282-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="e3282-169">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="e3282-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="e3282-170">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="e3282-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="e3282-171">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="e3282-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="e3282-172">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="e3282-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="e3282-173">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="e3282-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="e3282-174">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="e3282-174">Actuals</span></span></th>
<th><span data-ttu-id="e3282-175">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-175">Transaction currency</span></span></th>
<th><span data-ttu-id="e3282-176">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="e3282-176">Fixed price</span></span></th>
<th><span data-ttu-id="e3282-177">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="e3282-178">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="e3282-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="e3282-179">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="e3282-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-180">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="e3282-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="e3282-181">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="e3282-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e3282-182">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="e3282-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e3282-183">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-183">Cost actual</span></span></td>
<td><span data-ttu-id="e3282-184">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-185">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-186">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="e3282-187">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-188">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-189">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="e3282-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="e3282-190">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e3282-191">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="e3282-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e3282-192">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-192">Cost actual</span></span></td>
<td><span data-ttu-id="e3282-193">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-194">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-195">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-196">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-197">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-198">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="e3282-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e3282-199">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-200">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="e3282-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e3282-201">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e3282-202">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="e3282-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e3282-203">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e3282-204">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-205">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-206">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-207">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-208">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-209">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-209">Billed sales</span></span></td>
<td><span data-ttu-id="e3282-210">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e3282-211">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="e3282-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e3282-212">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e3282-213">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-214">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-215">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-216">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-217">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-218">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="e3282-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e3282-219">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-220">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="e3282-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e3282-221">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e3282-222">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="e3282-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e3282-223">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e3282-224">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="e3282-225">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="e3282-226">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="e3282-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="e3282-227">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e3282-228">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="e3282-229">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-230">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-230">Billed sales</span></span></td>
<td><span data-ttu-id="e3282-231">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e3282-232">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="e3282-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e3282-233">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e3282-234">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-235">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="e3282-236">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-237">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="e3282-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="e3282-238">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="e3282-239">Ресурс жобаның келісім-шарт бірлігінен өзгеше ұйымдық бөлімшеге тиесілі</span><span class="sxs-lookup"><span data-stu-id="e3282-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="e3282-240">Оқиға</span><span class="sxs-lookup"><span data-stu-id="e3282-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="e3282-241">Шот ұсынылатын немесе сатылған жоба</span><span class="sxs-lookup"><span data-stu-id="e3282-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="e3282-242">Алдын ала сатылым кезеңіндегі жоба</span><span class="sxs-lookup"><span data-stu-id="e3282-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="e3282-243">Ішкі жоба</span><span class="sxs-lookup"><span data-stu-id="e3282-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="e3282-244">Уақыт және материалдар</span><span class="sxs-lookup"><span data-stu-id="e3282-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="e3282-245">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="e3282-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="e3282-246">Нақты мәндер</span><span class="sxs-lookup"><span data-stu-id="e3282-246">Actuals</span></span></th>
<th><span data-ttu-id="e3282-247">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-247">Transaction currency</span></span></th>
<th><span data-ttu-id="e3282-248">Бекітілген баға</span><span class="sxs-lookup"><span data-stu-id="e3282-248">Fixed price</span></span></th>
<th><span data-ttu-id="e3282-249">Транзакция валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="e3282-250">Уақыт жазбасы жасалды.</span><span class="sxs-lookup"><span data-stu-id="e3282-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="e3282-251">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="e3282-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-252">Уақыт жазбасы жіберілді.</span><span class="sxs-lookup"><span data-stu-id="e3282-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="e3282-253">Нақты мәндер нысанында әрекет жоқ</span><span class="sxs-lookup"><span data-stu-id="e3282-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="e3282-254">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="e3282-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e3282-255">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-255">Cost actual</span></span></td>
<td><span data-ttu-id="e3282-256">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="e3282-257">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="e3282-258">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="e3282-259">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="e3282-260">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-261">Шот ұсынылмаған сатылымның нақты мәні – ақылы</span><span class="sxs-lookup"><span data-stu-id="e3282-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="e3282-262">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-263">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="e3282-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="e3282-264">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-265">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="e3282-266">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="e3282-267">Уақыт бекітілді және бекіту кезінде шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="e3282-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e3282-268">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-268">Cost actual</span></span></td>
<td><span data-ttu-id="e3282-269">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e3282-270">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="e3282-271">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e3282-272">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="e3282-273">Нақты құны</span><span class="sxs-lookup"><span data-stu-id="e3282-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-274">Ресурс бірлігінің құны</span><span class="sxs-lookup"><span data-stu-id="e3282-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="e3282-275">Ресурс бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-276">Ұйымаралық сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="e3282-277">Келісім-шарт бірлігінің валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-278">Шот ұсынылмаған сатылымның нақты мәні – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="e3282-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e3282-279">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-280">Шот ұсынылмаған сатылымның нақты мәні – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="e3282-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e3282-281">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e3282-282">Есепшот расталды және шот ұсыну сағаттары өзгертілген жоқ немесе көбейтілген жоқ.</span><span class="sxs-lookup"><span data-stu-id="e3282-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e3282-283">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e3282-284">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-285">Кезең үшін шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-286">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-287">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="e3282-288">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-289">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-289">Billed sales</span></span></td>
<td><span data-ttu-id="e3282-290">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e3282-291">Есепшот расталды және шот ұсыну сағаттарының азаюы орын алды.</span><span class="sxs-lookup"><span data-stu-id="e3282-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e3282-292">Шот ұсынылмаған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e3282-293">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-294">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-295">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-296">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e3282-297">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-298">Шот ұсынылған сатылым – жаңа мөлшері үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="e3282-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e3282-299">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-300">Шот ұсынылған сатылым – айырмашылығы үшін ақысыз</span><span class="sxs-lookup"><span data-stu-id="e3282-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e3282-301">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e3282-302">Есеп-шот ақылы санын көбейту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="e3282-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e3282-303">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e3282-304">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="e3282-305">Кезең үшін шот ұсынылған сатылымды кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="e3282-306">Кезең күйін <strong>Есеп-шот ұсынылған</strong> күйінен <strong>Есеп-шот ұсыну үшін дайын</strong> күйіне өзгертіңіз</span><span class="sxs-lookup"><span data-stu-id="e3282-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="e3282-307">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e3282-308">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="e3282-309">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="e3282-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-310">Шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-310">Billed sales</span></span></td>
<td><span data-ttu-id="e3282-311">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e3282-312">Есеп-шот ақылы санын азайту үшін түзетілді.</span><span class="sxs-lookup"><span data-stu-id="e3282-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e3282-313">Шот ұсынылған сатылым – кері бағыттау</span><span class="sxs-lookup"><span data-stu-id="e3282-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e3282-314">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-315">Жаңа мөлшерге арналған шот ұсынылған сатылым</span><span class="sxs-lookup"><span data-stu-id="e3282-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="e3282-316">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e3282-317">Шот ұсынылмаған сатылым – айырмашылығы үшін ақылы</span><span class="sxs-lookup"><span data-stu-id="e3282-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="e3282-318">Жоба келісім-шартының валютасы</span><span class="sxs-lookup"><span data-stu-id="e3282-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
