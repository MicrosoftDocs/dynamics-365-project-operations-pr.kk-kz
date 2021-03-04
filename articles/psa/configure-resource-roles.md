---
title: Ресурс рөлдерін конфигурациялау
description: Project Service жүйесінде ресурс рөлдерін теңшеу жолы
author: JohnPBurrows
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
ms.openlocfilehash: deaff0977ebb50382a28494fba2a1c34ed5cc9b4
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144915"
---
# <a name="configure-resource-roles-project-service"></a><span data-ttu-id="fe5c9-103">Ресурс рөлдерін теңшеу (Project Service)</span><span class="sxs-lookup"><span data-stu-id="fe5c9-103">Configure resource roles (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="fe5c9-104">Ресурс талаптарын немесе жоба шығындарын анықтауда жобаны жоспарлау кезінде рөлдер маңызды рөл атқарады.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-104">Roles play an important part in project planning, when determining resource requirements or costs of a project.</span></span> <span data-ttu-id="fe5c9-105">Жобаларға талап етілетін әрбір рөл үшін ресурс рөлін жасап, біліктіліктер мен тиімділіктерді осы рөлмен байланыстыру керек.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-105">For each role your projects require, you need to create a resource role and associate skills and proficiencies to that role.</span></span> <span data-ttu-id="fe5c9-106">Мысалы, әзірлеуші, жоба менеджері немесе ойынды сынаушы рөлдерін жасау керек болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-106">For example, you might want to create roles for developer, project manager, or game tester.</span></span> <span data-ttu-id="fe5c9-107">Сонымен қатар рөлге талап етілетін біліктіліктер мен тиімділік деңгейлерін орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-107">You’ll also set the skills and proficiency levels required for the role.</span></span>  
  
 <span data-ttu-id="fe5c9-108">Ұйымыңыз үшін тиімді жоба бағалауын қамтамасыз ету үшін ресурс рөлдерін теңшеңіз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-108">Configure resource roles to ensure effective project estimation for your organization.</span></span>  <span data-ttu-id="fe5c9-109">Сонымен қатар шот ұсыну түрін дәл орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-109">Also make sure you accurately set the billing type.</span></span> <span data-ttu-id="fe5c9-110">Ақы алынбайтын шот ұсыну түрінен тұратын элементтер жиыны келісімшарт немесе баға ұсыну жолдарын көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-110">An item set with a non-chargeable billing type doesn’t show up on contract or quote lines.</span></span>  
  
 <span data-ttu-id="fe5c9-111">Ресурс рөлдері орнатылса, бағатізбемен құны мен сатылым бағаларын орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-111">Once you’ve set up resource roles, you can set up cost and sales prices with a price list.</span></span>  
  
 <span data-ttu-id="fe5c9-112">Қосу керек әрбір рөл үшін келесіні істеңіз:</span><span class="sxs-lookup"><span data-stu-id="fe5c9-112">For each role you want to add, do the following:</span></span>  
  
1.  <span data-ttu-id="fe5c9-113">**Project Service > Ресурс рөлдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-113">Go to **Project Service > Resource Roles**.</span></span>  
  
2.  <span data-ttu-id="fe5c9-114">**Жаңа** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-114">Click **New**.</span></span>  
  
3.  <span data-ttu-id="fe5c9-115">**Жалпы** аумағында **Атау** ішінде рөл атын енгізіп, басқа өрістерді қажетінше толтырыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-115">In the **General** area, enter a name for the role in **Name**, and then fill in the other fields as necessary.</span></span>  
  
4.  <span data-ttu-id="fe5c9-116">Өңдеуді жалғастыра алу үшін жазбаны жасауға **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-116">Click **Save** to create the record so you can continue editing it.</span></span>  
  
5.  <span data-ttu-id="fe5c9-117">**Біліктіліктер** аумағында біліктілік қосу үшін **+** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-117">In the **Skills** area, click **+** to add a skill.</span></span>  
  
6.  <span data-ttu-id="fe5c9-118">**Рөл біліктілігі талабы** тақтасында **Біліктілік** өрісін басып, **Іздеу** түймешігін басып, біліктілікті таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-118">In the **Role competency requirement** pane, click in the **Skill** field, click the **Search** button, and then select a skill.</span></span>  
  
7.  <span data-ttu-id="fe5c9-119">Біліктіліктің тиімділігін таңдап, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-119">Select a proficiency for that skill, and then click **Save**.</span></span>  
  
8.  <span data-ttu-id="fe5c9-120">Біліктіліктерді қосуды қажетінше жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-120">Continue adding skills as necessary.</span></span> <span data-ttu-id="fe5c9-121">Орындалған кезде экранның төменгі оң жақ бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-121">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
9. <span data-ttu-id="fe5c9-122">Пайдаланылатын жобаларға осы ресурс рөлін қолжетімді ету үшін **Белсендіру** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe5c9-122">To make this resource role available for projects to use, click **Activate**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="fe5c9-123">Сонымен қатар келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="fe5c9-123">See Also</span></span>  
 [<span data-ttu-id="fe5c9-124">Ресурстарды реттеу</span><span class="sxs-lookup"><span data-stu-id="fe5c9-124">Set up resources</span></span>](../psa/set-up-resources.md)
