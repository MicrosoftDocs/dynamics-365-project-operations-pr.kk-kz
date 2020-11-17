---
title: Сатылым процесі барысында жоба үшін жұмыс болжамдарын қамтамасыз ету
description: Project Service жүйесіндегі сатылым процесі барысында жобаның жұмыс болжамдарын беру жолы
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 7bd83b6872d437f1d074d6ea2336c751bdfdd9e6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120595"
---
# <a name="provide-work-estimates-for-a-project-during-the-sales-process-project-service"></a><span data-ttu-id="e5c05-103">Сатылым процесі барысында жұмыс болжамдарын қамтамасыз ету (Project Service)</span><span class="sxs-lookup"><span data-stu-id="e5c05-103">Provide work estimates for a project during the sales process (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="e5c05-104">Сатылым процесі барысында баға ұсыну жолдарымен жерден сатылым болжамдарымен жұмыс істеуге болады.</span><span class="sxs-lookup"><span data-stu-id="e5c05-104">During the sales process, you can work out sales estimates from the ground up with quote lines.</span></span> [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] <span data-ttu-id="e5c05-105">жүйесіндегі [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] мүмкіндіктері жұмыс элементтерін үзумен және жұмыс декомпозициясының құрылымындағы жоба болжамдарымен іскерлесетін қатысты төлсипаттарды байланыстырумен сатылым болжамдарының ғылыми және анықтамалы жолын береді.</span><span class="sxs-lookup"><span data-stu-id="e5c05-105">capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] provide a more scientific and deterministic way of coming up with sales estimates by breaking down work items and associating relevant attributes that contribute toward the estimates for the project in the work breakdown structure.</span></span>  
  
 <span data-ttu-id="e5c05-106">Сатылымды жеңген кезде жобаның сәтті аяқталуын қажетінше анықтаумен жоба жоспарындағы байланысты жұмыс декомпозициясының құрылымын пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="e5c05-106">Once you win the sale, you can use the associated work breakdown structure in your project plan, refining it as necessary for successful completion of your project.</span></span>  
  
## <a name="link-a-project-to-a-quote-line"></a><span data-ttu-id="e5c05-107">Жобаны баға ұсыну жолымен байланыстыру</span><span class="sxs-lookup"><span data-stu-id="e5c05-107">Link a project to a quote line</span></span>  
 <span data-ttu-id="e5c05-108">Жоба негізіндегі баға ұсыну жолын жасау кезінде баға ұсыну жолынан жаңа жоба жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="e5c05-108">When creating a project-based quote line, you can create a new project from the quote line.</span></span> <span data-ttu-id="e5c05-109">Алдын ала теңшелген стандартты жоба жоспарлары және ұйымның жалпы қаржылық болжамдары болып табылатын жоба үлгілерін пайдалануға немесе өткен жоба жоспарын және болжамдарын көшіруге болады.</span><span class="sxs-lookup"><span data-stu-id="e5c05-109">You can then use project templates, which are either pre-configured standard project plans and financial estimates common to your organization, or a copy of a project plan and estimates from a past project.</span></span> <span data-ttu-id="e5c05-110">Жоба жасаған кезде жоба үлгісін таңдау жоба жоспарын, болжамдарын және рөл талаптарын анықтау негізін береді.</span><span class="sxs-lookup"><span data-stu-id="e5c05-110">When you create a project, choosing a project template provides a basis to refine the project plan, estimates, and role requirements.</span></span> <span data-ttu-id="e5c05-111">Баға ұсынудан жоба жасау кезінде жоба автоматты түрде баға ұсыну жолымен байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="e5c05-111">By creating your project from the quote, the project is automatically associated with the quote line.</span></span>  
  
## <a name="project-estimate-components"></a><span data-ttu-id="e5c05-112">Жоба болжамы құрамдастары</span><span class="sxs-lookup"><span data-stu-id="e5c05-112">Project estimate components</span></span>  
 <span data-ttu-id="e5c05-113">Жобадағы жұмыс декомпозициясының құрылымы жұмысты тапсырмаларға бөліп, тапсырмалар иерархиясын сақтап, әрбір тапсырманы аяқтауға талап етілетін талпыныс болжамын белгілеу жолын береді.</span><span class="sxs-lookup"><span data-stu-id="e5c05-113">The work breakdown structure in a project provides a way to break down work into tasks, maintain a hierarchy of tasks, and assign an estimate of effort required to complete each task.</span></span> <span data-ttu-id="e5c05-114">Сонымен қатар, тапсырманы және кестені аяқтауға талап етілетін ресурс түрі болжамын көрсету үшін рөлдерді тапсырмаға байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="e5c05-114">You can also associate roles to a task to indicate an estimate of the type of resource required to complete a task and a schedule.</span></span>  
  
 <span data-ttu-id="e5c05-115">Жұмыс декомпозициясының құрылымы жұмыс талпынысын және кесте болжамдарын анықтауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="e5c05-115">The work breakdown structure helps you determine work effort and schedule estimates.</span></span> <span data-ttu-id="e5c05-116">Әдепкі бойынша жобада бұрын анықталған әдепкі бағатізбелер пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e5c05-116">By default, the project uses default price lists that you defined earlier.</span></span> <span data-ttu-id="e5c05-117">Бағатізбелерде анықталған құн және сатылым бағалары жобаның жұмыс декомпозициясының қаржылық болжамдарын анықтауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="e5c05-117">The cost and sales prices defined in the price lists help determine financial estimates for the project’s work breakdown.</span></span>  
  
 <span data-ttu-id="e5c05-118">Егер жоба баға ұсынумен байланыстырылса және баға ұсынуда әр түрлі әдепкі бағатізбе болса, баға ұсыну бағатізбегі қаржылық болжамдарға пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e5c05-118">If your project is associated with a quote, and the quote has a different price list from the default, the quote’s price list is used for financial estimates.</span></span>  
  
## <a name="import-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="e5c05-119">Жоба болжамдарын баға ұсынуға импорттау</span><span class="sxs-lookup"><span data-stu-id="e5c05-119">Import estimates from a project into a quote</span></span>  
 <span data-ttu-id="e5c05-120">Жобада жоба болжамдары болса, осы болжамдарды баға ұсыну жолына импорттауға болады:</span><span class="sxs-lookup"><span data-stu-id="e5c05-120">Once you have project estimates in the project, you can import these estimates into the quote line:</span></span>  
  
-   <span data-ttu-id="e5c05-121">**Баға ұсыну жолы мәліметтері** ішінде **Болжамдардан импорттау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="e5c05-121">In **Quote Line Details**, click **Import from estimates**.</span></span> 

-   <span data-ttu-id="e5c05-122">Транзакция түрі, рөлі немесе жұмыс декомпозициясының құрылымы түйіні деңгейі бойынша қорытындыланған жоба болжамдарын импорттауды таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e5c05-122">Select whether to import project estimates summarized by transaction type, role, or work breakdown structure node level.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="e5c05-123">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="e5c05-123">See Also</span></span>  
 [<span data-ttu-id="e5c05-124">Жоба менеджерінің нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="e5c05-124">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
