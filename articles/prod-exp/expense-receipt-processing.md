---
title: Шығыс түбіртегін өңдеу
description: Осы тақырып түсімдерге таңбаларды оптикалық түрде тану (OCR) өңдеуі туралы ақпаратты ұсынады. Бұл мүмкіндік шығыс туралы есептер Microsoft Dynamics 365 Finance жүйесінде жасалған кезде пайдаланушы тәжірибесін жақсартуға арналған.
author: stsporen
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: ed9c97ba9cc505106599c2896dc2112358d0c408
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993513"
---
# <a name="expense-receipt-processing"></a><span data-ttu-id="4017e-104">Шығыс түбіртегін өңдеу</span><span class="sxs-lookup"><span data-stu-id="4017e-104">Expense receipt processing</span></span>

<span data-ttu-id="4017e-105">Шығыс жазбасы түсімдерге таңбаларды оптикалық түрде тану (OCR) өңдеуді кірістіру арқылы жақсартылды.</span><span class="sxs-lookup"><span data-stu-id="4017e-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="4017e-106">Бұл мүмкіндік шығыс туралы есептер жасалған кезде пайдаланушы тәжірибесін жақсартуға арналған.</span><span class="sxs-lookup"><span data-stu-id="4017e-106">This feature is designed to improve the user experience when expense reports are created.</span></span>

## <a name="key-features"></a><span data-ttu-id="4017e-107">Негізгі мүмкіндіктер</span><span class="sxs-lookup"><span data-stu-id="4017e-107">Key features</span></span>

- <span data-ttu-id="4017e-108">Сатушы аты, күні және жалпы сомасы түбіртектерден алынады.</span><span class="sxs-lookup"><span data-stu-id="4017e-108">The merchant name, date, and total amount are extracted from receipts.</span></span>
- <span data-ttu-id="4017e-109">Мүмкіндік бекітілмеген түбіртектерді шығыс транзакциялармен сәйкестендіруге тырысады.</span><span class="sxs-lookup"><span data-stu-id="4017e-109">The feature tries to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="4017e-110">Пайдаланушылар қолмен енгізілген шығыс транзакцияларын түбіртектерден жасай алады.</span><span class="sxs-lookup"><span data-stu-id="4017e-110">Users can create manually entered expense transactions from receipts.</span></span>

## <a name="usage-examples"></a><span data-ttu-id="4017e-111">Пайдалану мысалдары</span><span class="sxs-lookup"><span data-stu-id="4017e-111">Usage examples</span></span>

<span data-ttu-id="4017e-112">Шығыс туралы есеп жасалған кезде кредиттік карта транзакцияларын қамтитын түбіртектерді автоматты түрде бекіту үшін келесі әрекеттерді орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="4017e-112">To automatically attach receipts that include credit card transactions when an expense report is created, do the following:</span></span>

  1. <span data-ttu-id="4017e-113">**Шығысты басқару** жұмыс кеңістігін ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="4017e-114">**Түсімдер** қойындысында тіркелмеген түсімдердің бар екенін растаңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="4017e-115">Түсімдерді **Түсімдер** қойыншасына да жүктей аласыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="4017e-116"> **Шығыстар** қойыншасында тіркелмеген шығыстардың бар екенін растаңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="4017e-117">Әдетте шығыс әкімшісі бұл шығыстарды несиелік карта жеткізушісінен импорттайды.</span><span class="sxs-lookup"><span data-stu-id="4017e-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="4017e-118">**Шығыс туралы есеп** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-118">Select **New expense report**.</span></span> <span data-ttu-id="4017e-119">Енді шығыс туралы есепті жасаған кезде шығыстарды, түсімдерді қоса алатыныңызды ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="4017e-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="4017e-120">Егер сіз шығындарды да, түбіртектерді де қоссаңыз, түсімдерді шығындармен автоматты түрде сәйкестендіру іске қосылады.</span><span class="sxs-lookup"><span data-stu-id="4017e-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

<span data-ttu-id="4017e-121">Шығын жасау немесе түбіртектен шығынды сәйкестендіру үшін келесі әрекеттерді орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="4017e-121">To create an expense, or match an expense from a receipt, do the following:</span></span>

  1. <span data-ttu-id="4017e-122">Шығыс туралы есепте **Түсімдер** қойындысында **Түсімдерді қосу** таңдау арқылы түсімді тіркеңіз.</span><span class="sxs-lookup"><span data-stu-id="4017e-122">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="4017e-123">Түсімнің жүктелген кескіні астында **Жасау** және **Сәйкестендіру** опцияларын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="4017e-123">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="4017e-124">Қолмен енгізілген шығыс операциясын жасау және түсімнен алынған мәндерді толтыру үшін **Жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-124">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="4017e-125">Егер **Сәйкестендіру** опциясы таңдалса, жүйе бар шығысты түсіммен сәйкестендіруге тырысады.</span><span class="sxs-lookup"><span data-stu-id="4017e-125">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="4017e-126">Орнату</span><span class="sxs-lookup"><span data-stu-id="4017e-126">Installation</span></span>

<span data-ttu-id="4017e-127">Бұл мүмкіндік шығыс тәжірибесін жеңілдетуге көмектесу үшін **Шығындар туралы есептер қайта қаралды** мүмкіндігімен тіркесімде жұмыс істейді.</span><span class="sxs-lookup"><span data-stu-id="4017e-127">This feature works in combination with the **Expense reports re-imagined** feature to help simplify the expense experience.</span></span> <span data-ttu-id="4017e-128">Бұл мүмкіндік тек сынақ данасын және өндіріс данасы деңгейіндегі 2-деңгейлі орталар үшін қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="4017e-128">This feature is only available for Tier 2+ environments, which are Sandbox and Production.</span></span>

<span data-ttu-id="4017e-129">Осы жетілдірілген шығыс мүмкіндіктерін пайдалану үшін Microsoft Dynamics 365 Finance бағдарламасы үшін шығысты басқару қызметі қондырмасын орнатыңыз және сіздің данаңыздағы мүмкіндіктерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-129">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="4017e-130">Microsoft Dynamics өмірлік цикл қызметтері (LCS) жүйесінде жобаңыздан қондырмаға кіруге болады.</span><span class="sxs-lookup"><span data-stu-id="4017e-130">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="4017e-131">LCS жүйесіне кіріп, қажетті ортаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-131">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="4017e-132">**Толық мәліметтер** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="4017e-132">Go to **Full details**.</span></span>
3. <span data-ttu-id="4017e-133">**Ұстау** түймесін таңдаңыз немесе **Орта қондырмалары** FastTab қойыншасына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="4017e-133">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="4017e-134">**Жаңа қондырманы орнату** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-134">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="4017e-135">**Шығысты басқару қызметі** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-135">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="4017e-136">Орнату нұсқаулығын ұстанып, шарттар мен талаптарға келісіңіз.</span><span class="sxs-lookup"><span data-stu-id="4017e-136">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="4017e-137">**Орнату** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-137">Select **Install**.</span></span>

<span data-ttu-id="4017e-138">**Мүмкіндікті басқару** жұмыс кеңістігінде келесі мүмкіндіктерді қосыңыз:</span><span class="sxs-lookup"><span data-stu-id="4017e-138">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="4017e-139">Шығыс туралы есептерге жаңа көзқарас</span><span class="sxs-lookup"><span data-stu-id="4017e-139">Expense reports re-imagined</span></span>
- <span data-ttu-id="4017e-140">Түсімдерден шығысты автоматты түрде сәйкестендіріңіз немесе жасаңыз</span><span class="sxs-lookup"><span data-stu-id="4017e-140">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="4017e-141">Осы мүмкіндіктерді қосқан кезде келесі әрекеттер орын алады:</span><span class="sxs-lookup"><span data-stu-id="4017e-141">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="4017e-142">Қолданыстағы **Шығысты басқару** жұмыс кеңістігі жаңа жұмыс кеңістігімен ауыстырылды.</span><span class="sxs-lookup"><span data-stu-id="4017e-142">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="4017e-143">Шығыс өрісінің көрінуіне арналған мәзірдің жаңа тармағы қосылды.</span><span class="sxs-lookup"><span data-stu-id="4017e-143">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="4017e-144">**Шығысты басқару > Менің шығыстарым > Шығыс туралы есептер** жолы арқылы бұрынғы **Шығыс туралы есеп** бетін аша аласыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-144">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="4017e-145">Жұмыс ағындары және кез келген растау сізді шығыс туралы есептер бетіне апарады.</span><span class="sxs-lookup"><span data-stu-id="4017e-145">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="4017e-146">Түсімдер Microsoft Azure Cognitive Services қызметі арқылы өңделеді және метадеректер алынып, қосылады.</span><span class="sxs-lookup"><span data-stu-id="4017e-146">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="4017e-147">Сәйкес тіркелмеген түбіртектерді қамтитын шығыс туралы есеп жасауға мүмкіндік беретін опция қосылды.</span><span class="sxs-lookup"><span data-stu-id="4017e-147">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="4017e-148">Шығыс туралы есептерге қосылатын опция түсімнен шығыс бабын жасауға мүмкіндік береді немесе бар түсімдерді қолданыстағы шығыс бабына сәйкестендіруге тырысады.</span><span class="sxs-lookup"><span data-stu-id="4017e-148">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

<span data-ttu-id="4017e-149">Шығыс туралы есептер қайта қаралды мүмкіндігі туралы қосымша ақпарат алу үшін [Шығыс туралы есептер қайта қаралды](ExpenseWorkspaceNew.md) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="4017e-149">For more information about the Expense reports re-imagined feature, see [Expense reports reimagined](ExpenseWorkspaceNew.md).</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="4017e-150">Жиі қойылатын сұрақтар</span><span class="sxs-lookup"><span data-stu-id="4017e-150">Frequently asked questions</span></span>

<span data-ttu-id="4017e-151">**Microsoft өз үлгілері үшін менің деректерімді пайдаланады ма?**</span><span class="sxs-lookup"><span data-stu-id="4017e-151">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="4017e-152">Жоқ, Microsoft түсімді өңдеу қызметі үшін жалпы машиналық оқыту үлгісін құрды.</span><span class="sxs-lookup"><span data-stu-id="4017e-152">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="4017e-153">Бұл үлгі сіз жүктеген түсімдерге негізделмеген.</span><span class="sxs-lookup"><span data-stu-id="4017e-153">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="4017e-154">**Бұл мүмкіндік қайда қолжетімді және қайда өңделеді?**</span><span class="sxs-lookup"><span data-stu-id="4017e-154">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="4017e-155">Қазіргі уақытта Америка Құрама Штаттарына қолдау көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4017e-155">Currently, the United States is supported.</span></span>

<span data-ttu-id="4017e-156">**Менің түсімдерім қайда жіберіледі?**</span><span class="sxs-lookup"><span data-stu-id="4017e-156">**Where do my receipts go?**</span></span>

<span data-ttu-id="4017e-157">Finance бағдарламасы өріс деректерін шығару үшін Cognitive Services қызметтерімен байланысады.</span><span class="sxs-lookup"><span data-stu-id="4017e-157">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="4017e-158">Cognitive Services өңдеу кезінде сіздің түсіміңіздің көшірмесін 24 сағатқа дейін сақтайды.</span><span class="sxs-lookup"><span data-stu-id="4017e-158">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="4017e-159">Өңдеу аяқталғаннан кейін Cognitive Services түсімдерді жояды.</span><span class="sxs-lookup"><span data-stu-id="4017e-159">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="4017e-160">Түбіртектер әлі де Finance жүйесінде сақталады.</span><span class="sxs-lookup"><span data-stu-id="4017e-160">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="4017e-161">Толық ақпарат алу үшін Form Recognizer қызметінің жаңа мүмкіндігімен түсімді түсінуді қосу бөліміне өтіңіз: [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="4017e-161">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]