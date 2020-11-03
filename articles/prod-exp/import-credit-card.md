---
title: Несиелік карта бойынша транзакцияларды импорттау және сақтау
description: Бұл тақырып шығыспен байланысты несиелік карта транзакцияларын қалай импорттау және ұстану туралы түсіндіреді. Бұл транзакциялар автоматты түрде қайталанатын кесте бойынша импортталатындай етіп орнатылуы мүмкін немесе қажет болған жағдайда қолмен импортталуы мүмкін.
author: KimANelson
manager: AnnBe
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPbsMainDataLines
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 274023
ms.assetid: 3605eda1-a7ed-4675-8031-5279c5a8f5e4
ms.search.region: Global
ms.author: suvaidya
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: 6cec15e436bc699e361577c970dd5845c6c68908
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079813"
---
# <a name="import-and-maintain-credit-card-transactions"></a><span data-ttu-id="2b16b-104">Несиелік карта бойынша транзакцияларды импорттау және сақтау</span><span class="sxs-lookup"><span data-stu-id="2b16b-104">Import and maintain credit card transactions</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="2b16b-105">Шығыспен байланысты несиелік карта транзакциялары автоматты түрде қайталанатын кесте бойынша импортталатын етіп орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="2b16b-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="2b16b-106">Сонымен қатар қажет болған жағдайда транзакцияларды қолмен импорттауға болады.</span><span class="sxs-lookup"><span data-stu-id="2b16b-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="2b16b-107">Несиелік карта бойынша транзакциялар несиелік карта бойынша транзакция деректері заңды тұлға арқылы импортталады.</span><span class="sxs-lookup"><span data-stu-id="2b16b-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

<span data-ttu-id="2b16b-108">Деректер нысандары туралы қосымша ақпаратты [Мәліметтер нысандары](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-108">For more information about data entities, see [Data entities](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="2b16b-109">Несие картасының транзакцияларын импорттау</span><span class="sxs-lookup"><span data-stu-id="2b16b-109">Import credit card transactions</span></span>

1. <span data-ttu-id="2b16b-110">**Несие картасының транзакциялары** бетінде **Транзакцияларды импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="2b16b-111">Егер сіз деректерді басқаруды бірінші рет ашып отырсаңыз, жалғастыру үшін жүйе деректер нысандарының тізімін жаңартуы тиіс.</span><span class="sxs-lookup"><span data-stu-id="2b16b-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="2b16b-112">**Атауы** өрісінде импорттау тапсырмасының бірегей сипаттамасын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-112">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="2b16b-113">**Дереккөз пішімі** өрісінде импортталатын несие картасының транзакцияларын қамтитын файл пішімін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="2b16b-114">**Жүктеп салу** түймесін таңдап, жүктеп салғыңыз келетін файлды тауып, тізімнен таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-114">Select **Upload** , and then find and select the file to import.</span></span>
5. <span data-ttu-id="2b16b-115">Файл жүктелініп салынғаннан кейін, плиткадағы **Картаны қарау** сілтемесін таңдау арқылы несие картасымен жасалған транзакция файлының картасын және несие картасының транзакция деректерін салыстыру бағандарын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="2b16b-116">Егер салыстыру қателіктері болса немесе салыстыруды өзгерту керек болса, **Салыстыруды визуализациялау** қойындысынан немесе **Салыстыру мәліметтері** қойындысынан өзгертуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="2b16b-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="2b16b-117">Несие карталарының транзакцияларын автоматтандыру үшін **Қайталанатын деректер тапсырмасын жасау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="2b16b-118">Содан кейін несиелік картаның транзакциялары қаншалықты жиі импортталатынын анықтайтын қайталануды орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="2b16b-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="2b16b-119">Аяқтаған кезде **OK** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="2b16b-120">Таңдалған файлды қазір импорттау үшін **Import** (Импорттау) опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="2b16b-121">Егер импорттау кезінде қателіктер орын алса, сәтті импорттауға кепілдік беру үшін түзету керек қателерді көру үшін орындау журналын немесе кезеңдік деректерді қарауға болады.</span><span class="sxs-lookup"><span data-stu-id="2b16b-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="2b16b-122">Егер сіз бірнеше файл пішімін импорттауыңыз керек болса, әр пішін түрі үшін бөлек импорттау тапсырмаларын жасауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="2b16b-122">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="2b16b-123">Қызметі тоқтатылған жұмысшылар үшін несиелік карта транзакцияларын қайта тағайындаңыз</span><span class="sxs-lookup"><span data-stu-id="2b16b-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="2b16b-124">Жұмысшының жазбасы тоқтатылғаннан кейін жұмысшының Active Directory Domain Services (AD DS) тіркелгісі өшіріледі.</span><span class="sxs-lookup"><span data-stu-id="2b16b-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="2b16b-125">Дегенмен несиелік карта белсенді транзакциялар болуы мүмкін, олар әлі де шығындарға жазылып, өтелуі керек.</span><span class="sxs-lookup"><span data-stu-id="2b16b-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="2b16b-126">**Несие картасының транзакциялары** бетінен байланысты жұмысшының тоқтатылған кез келген несие карта транзакциясы үшін жұмыскерді қайта тағайындай аласыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-126">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="2b16b-127">Несие картасымен бір немесе бірнеше транзакцияны таңдаңыз, содан кейін **Транзакцияларды қайта тағайындау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b16b-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="2b16b-128">Содан кейін несие картасымен транзакцияларды тағайындау үшін басқа жұмыскерді таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="2b16b-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="2b16b-129">Несиелік карта транзакциялары қайта тағайындалғаннан кейін оларды шығыс туралы есеп үшін таңдап алуға болады және шығысты өтеу үшін әдеттегі процесс арқылы төлеуге болады.</span><span class="sxs-lookup"><span data-stu-id="2b16b-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>
