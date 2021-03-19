---
title: Жоба күйін бақылау
description: Project Service жүйесінде жоба күйін бақылау жолы
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
ms.openlocfilehash: d57f33cdf240db4cae1f33fe962173790fe0fe7f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281935"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="8b950-103">Жоба күйін бақылау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="8b950-103">Track a project’s status (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="8b950-104">Клиент жобасының орындалу барысын бақылау үшін [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] қызметін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="8b950-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="8b950-105">Қосу прогресстері ретінде жоба кезеңдерін жаңарту қосу кезеңіне әсер етеді:</span><span class="sxs-lookup"><span data-stu-id="8b950-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="8b950-106">**Жаңа**</span><span class="sxs-lookup"><span data-stu-id="8b950-106">**New**</span></span>    | <span data-ttu-id="8b950-107">Жоба жасаған кезде кезең **Жаңа** күйіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="8b950-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="8b950-108">Егер үлгіден жоба жасалса, осы кезеңде жобада кесте, болжамдар және топ деректері болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8b950-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="8b950-109">Болмаса, бұл жоба жоспары болады және жоба құрамдастарының қалған бөлігін қолмен енгізу керек.</span><span class="sxs-lookup"><span data-stu-id="8b950-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="8b950-110">**Баға ұсынысы**</span><span class="sxs-lookup"><span data-stu-id="8b950-110">**Quote**</span></span>   |      <span data-ttu-id="8b950-111">Жобаны баға ұсынысымен байланыстырғанда немесе баға ұсынысынан жасалғанда жоба кезеңі **Баға ұсыну** күйіне орнатылады және болжалды басталу және аяқталу күні жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="8b950-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="8b950-112">Жоба баға ұсыну кезеңінде болғанда **Жоба** бетіндегі **Sales** қойыншасында баға ұсыну мәліметтері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8b950-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="8b950-113">**Жоспар**</span><span class="sxs-lookup"><span data-stu-id="8b950-113">**Plan**</span></span>   |                                     <span data-ttu-id="8b950-114">Жобамен байланысты баға ұсыну жеңіп алған кезде және тапсырма келісімшарт кезеңіне өткенде жоба кезеңі **Жоспар** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="8b950-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="8b950-115">**Жоба** бетіндегі **Сатылым** қойыншасында келісімшарт мәліметтері көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8b950-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="8b950-116">**Аяқтау**</span><span class="sxs-lookup"><span data-stu-id="8b950-116">**Complete**</span></span> |                    <span data-ttu-id="8b950-117">Жоба жұмысы аяқталған кезде кезеңді **Аяқталды** күйіне ауыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="8b950-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="8b950-118">Жоба кезеңі аяқтау күйіне орнатылғанда жұмыстың 100% аяқталды деп түсініледі, бірақ жоба белгілі бір күту уақытына ашық сақталады және шығыс жазбалары жазылады.</span><span class="sxs-lookup"><span data-stu-id="8b950-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="8b950-119">**Жабу**</span><span class="sxs-lookup"><span data-stu-id="8b950-119">**Close**</span></span>   |           <span data-ttu-id="8b950-120">Барлық транзакциялар жобада жазылған кезде және ештеңені тіркеу керек емес кезде кезеңді **Жабық** күйіне қолмен орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="8b950-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="8b950-121">Жоба **Жабық** күйіне орнатылғанда жоба қосымша транзакциялар тіркеу мүмкін емес және жоба тек оқылады.</span><span class="sxs-lookup"><span data-stu-id="8b950-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="8b950-122">Жоба күйін бақылау үшін</span><span class="sxs-lookup"><span data-stu-id="8b950-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="8b950-123">**Project Service > Жобалар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="8b950-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="8b950-124">Жұмыс істеу керек жобаны басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8b950-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="8b950-125">Экран үстіндегі жолақтан жоба атынан кейінгі төмен көрсеткісін таңдап, **Жобаны бақылау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8b950-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="8b950-126">Тапсырмалар тізімі үстіндегі ашылмалы тізімнен **Талпынысты бақылау** немесе **Құнын бақылау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8b950-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="8b950-127">Өңделетін тапсырманы екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8b950-127">Double-click any task to edit it.</span></span> <span data-ttu-id="8b950-128">Сонымен қатар тапсырма уақыты мен прогресін өзгерту үшін Гант сызбасындағы жолақтарды жылжытуға немесе өлшемін өзгертуге болады.</span><span class="sxs-lookup"><span data-stu-id="8b950-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="8b950-129">Сонымен қатар келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="8b950-129">See Also</span></span>  
 [<span data-ttu-id="8b950-130">Жоба менеджерінің нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="8b950-130">Project Manager Guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]