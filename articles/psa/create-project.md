---
title: Жоба жасау
description: Project Service жүйесінде жобаны жасау жолы
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/13/2020
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
ms.openlocfilehash: 93958f8e7654ebc4cb038ba7ca0c5e4e02f39937
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148875"
---
# <a name="create-a-project-project-service"></a><span data-ttu-id="54106-103">Жоба жасау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="54106-103">Create a project (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="54106-104">Жоба негізіндегі қызметтер үшін мүмкіндік, баға ұсыну немесе келісімшарт жасау керек кезде [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] ішіндегі [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] мүмкіндіктерін пайдаланумен жоба жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="54106-104">Create a project using the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] when you want to create an opportunity, quote, or contract for project-based services.</span></span> <span data-ttu-id="54106-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] мүмкіндіктері жобаны мүмкіндіктен бастап аяқтауға дейін басқаруға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="54106-105">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities help you manage your project from opportunity through completion.</span></span> <span data-ttu-id="54106-106">Жобаны жасау кезінде баға ұсынуларға, шығын болжамдарына және ресурс басқармасына кері әсер ететін жұмыс декомпозициясының құрылымын жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="54106-106">When you create a project, you’ll also create a work breakdown structure, which affects your quotes, cost estimates, and resource management.</span></span>  
  
1.  <span data-ttu-id="54106-107">**Project Service > Жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="54106-107">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="54106-108">**Жаңа жоба** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="54106-108">Click **New Project**.</span></span>  
  
3.  <span data-ttu-id="54106-109">**Қорытынды** аймағында жоба атын енгізіп, барынша көп мәліметтер толтырыңыз.</span><span class="sxs-lookup"><span data-stu-id="54106-109">In the **Summary** area, enter a name for your project, and then fill in as many of the details as you can.</span></span> <span data-ttu-id="54106-110">Қызыл жұлдызшамен (\*) белгіленген элементтер талап етіледі.</span><span class="sxs-lookup"><span data-stu-id="54106-110">Items marked with a red asterisk (\*) are required.</span></span>  
  
4.  <span data-ttu-id="54106-111">Өңдеуді жалғастыра алу үшін жобаны жасау үшін **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="54106-111">Click **Save** to create your project so you can continue editing it.</span></span>  
  
<span data-ttu-id="54106-112">Одан кейін жобаға қажет тапсырмаларды, уақытты және ресурс рөлдерін анықтау үшін жұмыс декомпозициясының құрылымын жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="54106-112">Next, you’ll create a work breakdown structure for your project to define the tasks, timing, and resource roles needed for the project.</span></span>  

> [!NOTE]
> <span data-ttu-id="54106-113">Жоспарлау кезінде, Project Service Automation қолданылған **Жұмыс сағаты** үлгісінің уақыт белдеуін сақтайды.</span><span class="sxs-lookup"><span data-stu-id="54106-113">When scheduling, Project Service Automation respects the time zone of the applied **Work Hour** template.</span></span> <span data-ttu-id="54106-114">Алайда, кесте тапсырмаларын қарау кезінде, тапсырманың басталу және аяқталу күндері пайдаланушының уақыт белдеуінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="54106-114">However, when viewing the schedule tasks, the start and end dates of a task will be displayed in the user's time zone.</span></span> <span data-ttu-id="54106-115">Бұл **Жоба** пішінінде басқа уақыт кезеңіндегі көріністерге қолданылады.</span><span class="sxs-lookup"><span data-stu-id="54106-115">This applies to other time-phased views in the **Project** form.</span></span> <span data-ttu-id="54106-116">Егер пайдаланушының уақыт белдеуі жобаға қолданылатын жұмыс сағаты үлгісінің уақыт белдеуіне сәйкес келмесе, айырмашылықты түсіндіретін ескерту пайда болады.</span><span class="sxs-lookup"><span data-stu-id="54106-116">If the user's time zone does not match the time zone of the work hour template applied to the project, a warning which explains the difference will occur.</span></span> 
  
### <a name="see-also"></a><span data-ttu-id="54106-117">Сонымен қатар келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="54106-117">See Also</span></span>  
 [<span data-ttu-id="54106-118">Жоба менеджерінің нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="54106-118">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
