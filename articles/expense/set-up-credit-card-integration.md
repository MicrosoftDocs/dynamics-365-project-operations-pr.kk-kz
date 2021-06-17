---
title: Несие картасы біріктіруін орнату
description: Бұл тақырыпта шығындарға байланысты несиелік карта транзакцияларымен жұмыс істеу жолы түсіндіріледі.
author: suvaidya
ms.date: 04/02/2021
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 3555e894e206c2aafb30b0df1e52efadd69b0713
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001831"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="f4948-103">Несие картасы біріктіруін орнату</span><span class="sxs-lookup"><span data-stu-id="f4948-103">Set up credit card integration</span></span>

<span data-ttu-id="f4948-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="f4948-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f4948-105">Шығыспен байланысты несиелік карта транзакциялары автоматты түрде қайталанатын кесте бойынша импортталатын етіп орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="f4948-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="f4948-106">Сонымен қатар қажет болған жағдайда транзакцияларды қолмен импорттауға болады.</span><span class="sxs-lookup"><span data-stu-id="f4948-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="f4948-107">Несиелік карта бойынша транзакциялар несиелік карта бойынша транзакция деректері заңды тұлға арқылы импортталады.</span><span class="sxs-lookup"><span data-stu-id="f4948-107">The credit card transactions are imported through the credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="f4948-108">Несие картасының транзакцияларын импорттау</span><span class="sxs-lookup"><span data-stu-id="f4948-108">Import credit card transactions</span></span>

<span data-ttu-id="f4948-109">Несиелік карта транзакцияларын импорттау үшін келесі әрекеттерді орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="f4948-109">To import credit card transactions, follow these steps:</span></span>

1. <span data-ttu-id="f4948-110">**Несие картасының транзакциялары** бетінде **Транзакцияларды импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="f4948-111">Егер сіз деректерді басқаруды бірінші рет ашып отырсаңыз, жалғастыру үшін жүйе деректер нысандарының тізімін жаңартуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="f4948-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="f4948-112">**Атау** өрісіне импорттау тапсырмасы үшін бір мәнді сипаттаманы енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f4948-112">In the **Name** field, enter a unique description for the import job.</span></span>
3. <span data-ttu-id="f4948-113">**Дереккөз пішімі** өрісінде импортталатын несие картасының транзакцияларын қамтитын файл пішімін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="f4948-114">**Жүктеп салу** түймесін таңдап, жүктеп салғыңыз келетін файлды тауып, тізімнен таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="f4948-115">Файл жүктеліп салынғаннан кейін, плиткадағы **Картаны қарау** сілтемесін таңдау арқылы несие картасымен жасалған транзакция файлының картасын және несие картасының транзакция деректерін салыстыру бағандарын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="f4948-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="f4948-116">Егер салыстыру қателіктері болса немесе салыстыруды өзгерту керек болса, **Салыстыруды визуализациялау** қойыншасынан немесе **Салыстыру мәліметтері** қойыншасынан өзгертуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="f4948-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="f4948-117">Несие карталарының транзакцияларын автоматтандыру үшін **Қайталанатын деректер тапсырмасын жасау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="f4948-118">Содан кейін несиелік картаның транзакциялары қаншалықты жиі импортталатынын анықтайтын қайталануды орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="f4948-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="f4948-119">Аяқтаған кезде **OK** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="f4948-120">Таңдалған файлды қазір импорттау үшін **Import** (Импорттау) опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="f4948-121">Импорттау кезінде қателер орын алса, сәтті импортты қамтамасыз ету мақсатында түзету қажет қателерді көру үшін орындау журналын немесе кезеңдік деректерді қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="f4948-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help ensure a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="f4948-122">Бірнеше файл пішімін импорттау қажет болса, әр пішім түрі үшін бөлек импорттау тапсырмаларын жасауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="f4948-122">If you need to import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="f4948-123">Қызметі тоқтатылған жұмысшылар үшін несиелік карта транзакцияларын қайта тағайындаңыз</span><span class="sxs-lookup"><span data-stu-id="f4948-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="f4948-124">Жұмысшының жазбасы тоқтатылғаннан кейін жұмысшының Active Directory Domain Services (AD DS) тіркелгісі өшіріледі.</span><span class="sxs-lookup"><span data-stu-id="f4948-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="f4948-125">Дегенмен несиелік карта белсенді транзакциялар болуы мүмкін, олар әлі де шығындарға жазылып, өтелуі керек.</span><span class="sxs-lookup"><span data-stu-id="f4948-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="f4948-126">**Несиелік карта транзакциялары** бетінде қызметкерді байланысты қызметкер тоқтатылған кез келген несиелік картасы транзакциясына қайта тағайындай аласыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-126">On the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="f4948-127">Несие картасымен бір немесе бірнеше транзакцияны таңдаңыз, содан кейін **Транзакцияларды қайта тағайындау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="f4948-128">Содан кейін несие картасымен транзакцияларды тағайындау үшін басқа жұмыскерді таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="f4948-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="f4948-129">Несиелік карта транзакциялары қайта тағайындалғаннан кейін оларды шығыс туралы есеп үшін таңдап алуға болады және шығысты өтеу үшін әдеттегі процесс арқылы төлеуге болады.</span><span class="sxs-lookup"><span data-stu-id="f4948-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>

## <a name="delete-credit-card-transactions"></a><span data-ttu-id="f4948-130">Несиелік карта транзакцияларын жою</span><span class="sxs-lookup"><span data-stu-id="f4948-130">Delete credit card transactions</span></span> 

<span data-ttu-id="f4948-131">Кейде несиелік карта транзакциялары импортталғаннан кейін белгілі бір операцияларды жою қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f4948-131">Sometimes, after credit card transactions are imported, certain transactions may need to be deleted.</span></span> <span data-ttu-id="f4948-132">Бұл транзакциялардың көшірмесі болғандықтан немесе деректер дәл болмауынан болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f4948-132">This could be because the transactions are duplicates or because the data might isn't accurate.</span></span> <span data-ttu-id="f4948-133">Әкімшілер **Несиелік карта операцияларын жою** несиелік картаның шығын есебіне **тіркелмеген** транзакцияларын таңдау және жою үшін пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="f4948-133">Admins can use the **"Delete credit card transactions"** feature to select and delete credit card transactions that are **not attached** to an expense report.</span></span> 

1. <span data-ttu-id="f4948-134">**Кезеңдік тапсырмалар** > **Несиелік карта транзакциялары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f4948-134">Go to **Periodic tasks** > **Delete credit card transactions**.</span></span>
2. <span data-ttu-id="f4948-135">**Сүзгі** опциясын таңдап, енгізу керек жазбаларды анықтау үшін ақпарат беріңіз.</span><span class="sxs-lookup"><span data-stu-id="f4948-135">Select **Filter** and provide information to identify the records to include.</span></span>
3. <span data-ttu-id="f4948-136">Жазбаларды жою үшін **OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4948-136">Select **OK** to delete the records.</span></span> 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
