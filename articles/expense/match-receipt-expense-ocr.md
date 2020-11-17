---
title: Түсімді шығысқа OCR арқылы сәйкестендіру
description: Осы тақырып түсімдерге таңбаларды оптикалық түрде тану (OCR) өңдеуі туралы ақпаратты ұсынады.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 55f63c8c092942b73a55c9d86d867bca600f42e5
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124330"
---
# <a name="match-a-receipt-to-an-expense-using-ocr"></a><span data-ttu-id="946d9-103">Түсімді шығысқа OCR арқылы сәйкестендіру</span><span class="sxs-lookup"><span data-stu-id="946d9-103">Match a receipt to an expense using OCR</span></span>

<span data-ttu-id="946d9-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="946d9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="946d9-105">Шығыс жазбасы түсімдерге таңбаларды оптикалық түрде тану (OCR) өңдеуді кірістіру арқылы жақсартылды.</span><span class="sxs-lookup"><span data-stu-id="946d9-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="946d9-106">Функционалдылық шығыс туралы есептерді жасаған кезде пайдаланушы тәжірибесін жақсартуға арналған.</span><span class="sxs-lookup"><span data-stu-id="946d9-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="946d9-107">Негізгі мүмкіндіктер</span><span class="sxs-lookup"><span data-stu-id="946d9-107">Key features</span></span>

- <span data-ttu-id="946d9-108">Жүйе түсімнен сатушы атын, күнді және жалпы соманы алады.</span><span class="sxs-lookup"><span data-stu-id="946d9-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="946d9-109">Жүйе тіркелмеген түсімдерді тіркелмеген түсімдер транзакцияларымен сәйкестендіруге тырысады.</span><span class="sxs-lookup"><span data-stu-id="946d9-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="946d9-110">Сіз қолмен енгізілген шығыс транзакцияларын түсімдерден жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="946d9-111">Түсімдерді шығыс есебіне тіркеңіз</span><span class="sxs-lookup"><span data-stu-id="946d9-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="946d9-112">Шығыс туралы есеп жасалған кезде несиелік карта транзакцияларын қамтитын түсімдерді автоматты түрде тіркеу үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="946d9-113">**Шығысты басқару** жұмыс кеңістігін ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="946d9-114">**Түсімдер** қойыншасында тіркелмеген түсімдердің бар екенін растаңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="946d9-115">Түсімдерді **Түсімдер** қойыншасына да жүктей аласыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="946d9-116"> **Шығыстар** қойыншасында тіркелмеген шығыстардың бар екенін растаңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="946d9-117">Әдетте шығыс әкімшісі бұл шығыстарды несиелік карта жеткізушісінен импорттайды.</span><span class="sxs-lookup"><span data-stu-id="946d9-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="946d9-118">**Шығыс туралы есеп** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-118">Select **New expense report**.</span></span> <span data-ttu-id="946d9-119">Енді шығыс туралы есепті жасаған кезде шығыстарды, түсімдерді қоса алатыныңызды ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="946d9-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="946d9-120">Егер сіз шығындарды да, түбіртектерді де қоссаңыз, түсімдерді шығындармен автоматты түрде сәйкестендіру іске қосылады.</span><span class="sxs-lookup"><span data-stu-id="946d9-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="946d9-121">Түсімдерді шығыс туралы есепке сәйкестендіріңіз немесе жасаңыз</span><span class="sxs-lookup"><span data-stu-id="946d9-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="946d9-122">Шығысты жасау немесе түсімнен шығысты сәйкестендіру үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="946d9-123">Шығыс туралы есепте **Түсімдер** қойыншасында **Түсімдерді қосу** таңдау арқылы түсімді тіркеңіз.</span><span class="sxs-lookup"><span data-stu-id="946d9-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="946d9-124">Түсімнің жүктелген кескіні астында **Жасау** және **Сәйкестендіру** опцияларын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="946d9-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="946d9-125">Қолмен енгізілген шығыс операциясын жасау және түсімнен алынған мәндерді толтыру үшін **Жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="946d9-126">Егер **Сәйкестендіру** опциясы таңдалса, жүйе бар шығысты түсіммен сәйкестендіруге тырысады.</span><span class="sxs-lookup"><span data-stu-id="946d9-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="946d9-127">Орнату</span><span class="sxs-lookup"><span data-stu-id="946d9-127">Installation</span></span>

<span data-ttu-id="946d9-128">Осы жетілдірілген шығыс мүмкіндіктерін пайдалану үшін Microsoft Dynamics 365 Finance бағдарламасы үшін шығысты басқару қызметі қондырмасын орнатыңыз және сіздің данаңыздағы мүмкіндіктерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="946d9-129">Microsoft Dynamics өмірлік цикл қызметтері (LCS) жүйесінде жобаңыздан қондырмаға кіруге болады.</span><span class="sxs-lookup"><span data-stu-id="946d9-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="946d9-130">LCS жүйесіне кіріп, қажетті ортаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="946d9-131">**Толық мәліметтер** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="946d9-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="946d9-132">**Ұстау** түймесін таңдаңыз немесе **Орта қондырмалары** FastTab қойыншасына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="946d9-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="946d9-133">**Жаңа қондырманы орнату** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="946d9-134">**Шығысты басқару қызметі** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="946d9-135">Орнату нұсқаулығын ұстанып, шарттар мен талаптарға келісіңіз.</span><span class="sxs-lookup"><span data-stu-id="946d9-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="946d9-136">**Орнату** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-136">Select **Install**.</span></span>

<span data-ttu-id="946d9-137">**Мүмкіндікті басқару** жұмыс кеңістігінде келесі мүмкіндіктерді қосыңыз:</span><span class="sxs-lookup"><span data-stu-id="946d9-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="946d9-138">Шығыс туралы есептерге жаңа көзқарас</span><span class="sxs-lookup"><span data-stu-id="946d9-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="946d9-139">Түсімдерден шығысты автоматты түрде сәйкестендіріңіз немесе жасаңыз</span><span class="sxs-lookup"><span data-stu-id="946d9-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="946d9-140">Осы мүмкіндіктерді қосқан кезде келесі әрекеттер орын алады:</span><span class="sxs-lookup"><span data-stu-id="946d9-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="946d9-141">Қолданыстағы **Шығысты басқару** жұмыс кеңістігі жаңа жұмыс кеңістігімен ауыстырылды.</span><span class="sxs-lookup"><span data-stu-id="946d9-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="946d9-142">Шығыс өрісінің көрінуіне арналған мәзірдің жаңа тармағы қосылды.</span><span class="sxs-lookup"><span data-stu-id="946d9-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="946d9-143">**Шығысты басқару > Менің шығыстарым > Шығыс туралы есептер** жолы арқылы бұрынғы **Шығыс туралы есеп** бетін аша аласыз.</span><span class="sxs-lookup"><span data-stu-id="946d9-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="946d9-144">Жұмыс ағындары және кез келген растау сізді шығыс туралы есептер бетіне апарады.</span><span class="sxs-lookup"><span data-stu-id="946d9-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="946d9-145">Түсімдер Microsoft Azure Cognitive Services қызметі арқылы өңделеді және метадеректер алынып, қосылады.</span><span class="sxs-lookup"><span data-stu-id="946d9-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="946d9-146">Сәйкес тіркелмеген түбіртектерді қамтитын шығыс туралы есеп жасауға мүмкіндік беретін опция қосылды.</span><span class="sxs-lookup"><span data-stu-id="946d9-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="946d9-147">Шығыс туралы есептерге қосылатын опция түсімнен шығыс бабын жасауға мүмкіндік береді немесе бар түсімдерді қолданыстағы шығыс бабына сәйкестендіруге тырысады.</span><span class="sxs-lookup"><span data-stu-id="946d9-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="946d9-148">Жиі қойылатын сұрақтар</span><span class="sxs-lookup"><span data-stu-id="946d9-148">Frequently asked questions</span></span>

<span data-ttu-id="946d9-149">**Microsoft өз үлгілері үшін менің деректерімді пайдаланады ма?**</span><span class="sxs-lookup"><span data-stu-id="946d9-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="946d9-150">Жоқ, Microsoft түсімді өңдеу қызметі үшін жалпы машиналық оқыту үлгісін құрды.</span><span class="sxs-lookup"><span data-stu-id="946d9-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="946d9-151">Бұл үлгі сіз жүктеген түсімдерге негізделмеген.</span><span class="sxs-lookup"><span data-stu-id="946d9-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="946d9-152">**Бұл мүмкіндік қайда қолжетімді және қайда өңделеді?**</span><span class="sxs-lookup"><span data-stu-id="946d9-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="946d9-153">Қазіргі уақытта Америка Құрама Штаттарына қолдау көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="946d9-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="946d9-154">**Менің түсімдерім қайда жіберіледі?**</span><span class="sxs-lookup"><span data-stu-id="946d9-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="946d9-155">Finance бағдарламасы өріс деректерін шығару үшін Cognitive Services қызметтерімен байланысады.</span><span class="sxs-lookup"><span data-stu-id="946d9-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="946d9-156">Cognitive Services өңдеу кезінде сіздің түсіміңіздің көшірмесін 24 сағатқа дейін сақтайды.</span><span class="sxs-lookup"><span data-stu-id="946d9-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="946d9-157">Өңдеу аяқталғаннан кейін Cognitive Services түсімдерді жояды.</span><span class="sxs-lookup"><span data-stu-id="946d9-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="946d9-158">Түбіртектер әлі де Finance жүйесінде сақталады.</span><span class="sxs-lookup"><span data-stu-id="946d9-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="946d9-159">Толық ақпарат алу үшін Form Recognizer қызметінің жаңа мүмкіндігімен түсімді түсінуді қосу бөліміне өтіңіз: [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="946d9-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>
