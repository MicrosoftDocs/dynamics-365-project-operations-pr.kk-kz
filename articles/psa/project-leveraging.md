---
title: Сатылымы бойынша болжамдар және жобалар
description: Бұл тақырыпта сату процесіндегі кесте мен болжамдарды пайдалану жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: d8bb380519759659dc1b4151b62228a626ee7a26
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120685"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="67208-103">Сатылымы бойынша болжамдар және жобалар</span><span class="sxs-lookup"><span data-stu-id="67208-103">Sales estimates and projects</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="67208-104">Сату процесінде жобаны сатылым баға ұсынысымен байланыстыру арқылы сатылым болжамдарын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="67208-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="67208-105">Осылайша, жобаны жоспарлау және бағалау мүмкіндіктерін пайдалану үшін детерминистік болжам пайда болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="67208-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="67208-106">Егер сату жүзеге асса, сатылымды бағалау мақсаттарында пайдаланылған кестені жоба жоспарын одан әрі нақтылау үшін негіз ретінде қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="67208-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="67208-107">Жобаны баға ұсыну жолымен байланыстыру</span><span class="sxs-lookup"><span data-stu-id="67208-107">Linking a project to a quote line</span></span>

<span data-ttu-id="67208-108">Жобаға негізделген баға ұсыну жолын құрған кезде, жаңа жоба жасауға немесе **Баға ұсыну жолы** бетіндегі бұрыннан бар жобаны байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="67208-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![Баға ұсыну жолының пішіні](media/project-8.png)
 
<span data-ttu-id="67208-110">Баға ұсыну жолының мәліметтерінде жаңа жоба жасағанда, жоба үлгілерінің артықшылығын пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="67208-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="67208-111">Жоба үлгілері — бұл стандартты жоба жоспарларын көрсететін үлгілі жобалар және ұйымға тән қаржылық болжамдар.</span><span class="sxs-lookup"><span data-stu-id="67208-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="67208-112">Олар сонымен қатар жоба жоспарларының көшірмелерін және өткен жобалардың болжамдарын ұсына алады.</span><span class="sxs-lookup"><span data-stu-id="67208-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![Баға ұсыну жолы мәліметтері](media/project-9.png)
  
<span data-ttu-id="67208-114">Баға ұсынысынан жоба жасаған кезде, жоба автоматты түрде баға ұсыну жолымен байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="67208-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="67208-115">Жобадағы болжамдар компоненттері</span><span class="sxs-lookup"><span data-stu-id="67208-115">Components of estimates in a project</span></span>

<span data-ttu-id="67208-116">Кесте тапсырмаларды бөлуге, тапсырмалардың иерархиясын сақтауға, тапсырманы орындау үшін қандай ресурстар қажет екенін анықтауға және тапсырманы орындау үшін қажет қарқындылық бағасын тағайындауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="67208-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="67208-117">**Жоба** бетінің **Кесте** қойыншасындағы өрістерді қолдана отырып, жұмыс қарқындылығын және кесте болжамдарын анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="67208-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="67208-118">Бағатізбе жобамен байланысты болғандықтан, қаржылық болжамдар бағатізбеде анықталған құн мен сатылым бағаларын қолдану арқылы есептеледі.</span><span class="sxs-lookup"><span data-stu-id="67208-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="67208-119">Жоба болжамдарын баға ұсынысына импорттау</span><span class="sxs-lookup"><span data-stu-id="67208-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="67208-120">Жоба болжамдарын анықтағаннан кейін, оларды баға ұсыну жолына импорттай аласыз.</span><span class="sxs-lookup"><span data-stu-id="67208-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="67208-121">Жоба болжамдарын транзакция түрі, рөлі немесе тапсырма деңгейі бойынша қорытындылау үшін, **Баға ұсыну жолы мәліметтері** бетіндегі таспадан **Болжамдардан импорттау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="67208-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>
