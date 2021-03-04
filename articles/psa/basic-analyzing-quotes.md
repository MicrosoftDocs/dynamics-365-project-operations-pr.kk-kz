---
title: Жобаның баға ұсыныстарын талдау
description: Бұл тақырыпта жобаның баға ұсыныстарын талдау туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 361a940261811467c46222c3d58c9504434ec882
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145230"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="24aeb-103">Жобаның баға ұсыныстарын талдау</span><span class="sxs-lookup"><span data-stu-id="24aeb-103">Analysis of project quotes</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="24aeb-104">Dynamics 365 Project Service Automation қызметі табыстылықты болжау үшін жобаның баға ұсыныстарын талдайды.</span><span class="sxs-lookup"><span data-stu-id="24aeb-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="24aeb-105">Сондай-ақ ол баға ұсыныстары тұтынушының жеткізілу күніне немесе аяқталу күніне және бюджетке қатысты болжамдарына қаншалықты сәйкес келетінін талдайды.</span><span class="sxs-lookup"><span data-stu-id="24aeb-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="24aeb-106">Табыстылық талдауы</span><span class="sxs-lookup"><span data-stu-id="24aeb-106">Profitability analysis</span></span>

<span data-ttu-id="24aeb-107">Project Service Automation қызметі жиынтық пайда мен реттелген жиынтық пайданы пайдалану арқылы табыстылықты талдайды.</span><span class="sxs-lookup"><span data-stu-id="24aeb-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="24aeb-108">Жиынтық пайда келесі формула бойынша есептеледі:</span><span class="sxs-lookup"><span data-stu-id="24aeb-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="24aeb-109">Реттелген жиынтық пайда келесі формула бойынша есептеледі:</span><span class="sxs-lookup"><span data-stu-id="24aeb-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="24aeb-110">Егер жиынтық пайда мен реттелген жиынтық пайда мәндері айтарлықтай өзгешеленсе, баға ұсынудағы жұмыстың көбі ақылы емес ретінде жіктеледі.</span><span class="sxs-lookup"><span data-stu-id="24aeb-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="24aeb-111">Тұтынушы болжамдарын талдау</span><span class="sxs-lookup"><span data-stu-id="24aeb-111">Analysis of customer expectations</span></span>

<span data-ttu-id="24aeb-112">Келесі өрістер үшін мәндерді енгізу арқылы баға ұсыныстарын талдап, тұтынушының кесте мен бюджетке қатысты болжамдары үшін диаграммалар жасауға болады:</span><span class="sxs-lookup"><span data-stu-id="24aeb-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="24aeb-113">Баға ұсыну тақырыбындағы **Сұралған жеткізу күні** өрісі.</span><span class="sxs-lookup"><span data-stu-id="24aeb-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="24aeb-114">Әр баға ұсыну жолының **Тұтынушы бюджеті** өрісі (жобаға негізделген жолдар және өнімге негізделген жолдар үшін).</span><span class="sxs-lookup"><span data-stu-id="24aeb-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="24aeb-115">Тұтынушының кестеге қатысты болжамдарын талдау баға ұсыну жолы мәліметінің соңғы аяқталу күні мен баға ұсынудағы барлық баға ұсыну жолдары бойынша сұралған жеткізу күнін салыстыру арқылы жасалады.</span><span class="sxs-lookup"><span data-stu-id="24aeb-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="24aeb-116">Тұтынушының бюджетке қатысты болжамдарын талдау жалпы тұтынушы бюджетінің сомасын барлық баға ұсыну жолдары бойынша баға ұсыну сомасымен салыстыру арқылы жасалады.</span><span class="sxs-lookup"><span data-stu-id="24aeb-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>
