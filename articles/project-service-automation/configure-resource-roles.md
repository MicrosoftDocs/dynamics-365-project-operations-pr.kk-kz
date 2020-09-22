---
title: Ресурс рөлдерін конфигурациялау
description: Project Service жүйесінде ресурс рөлдерін теңшеу жолы
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0a180069-17d9-40fd-b4af-9b8d50f373ea
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 6a32ec4380e847b897931b6691fa8f9784d0cee7
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753030"
---
# <a name="configure-resource-roles-project-service"></a><span data-ttu-id="3ce20-103">Ресурс рөлдерін теңшеу (Project Service)</span><span class="sxs-lookup"><span data-stu-id="3ce20-103">Configure resource roles (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="3ce20-104">Ресурс талаптарын немесе жоба шығындарын анықтауда жобаны жоспарлау кезінде рөлдер маңызды рөл атқарады.</span><span class="sxs-lookup"><span data-stu-id="3ce20-104">Roles play an important part in project planning, when determining resource requirements or costs of a project.</span></span> <span data-ttu-id="3ce20-105">Жобаларға талап етілетін әрбір рөл үшін ресурс рөлін жасап, біліктіліктер мен тиімділіктерді осы рөлмен байланыстыру керек.</span><span class="sxs-lookup"><span data-stu-id="3ce20-105">For each role your projects require, you need to create a resource role and associate skills and proficiencies to that role.</span></span> <span data-ttu-id="3ce20-106">Мысалы, әзірлеуші, жоба менеджері немесе ойынды сынаушы рөлдерін жасау керек болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="3ce20-106">For example, you might want to create roles for developer, project manager, or game tester.</span></span> <span data-ttu-id="3ce20-107">Сонымен қатар, рөлге талап етілетін біліктіліктер мен тиімділік деңгейлерін орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="3ce20-107">You’ll also set the skills and proficiency levels required for the role.</span></span>  
  
 <span data-ttu-id="3ce20-108">Ұйымыңыз үшін тиімді жоба бағалауын қамтамасыз ету үшін ресурс рөлдерін теңшеңіз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-108">Configure resource roles to ensure effective project estimation for your organization.</span></span>  <span data-ttu-id="3ce20-109">Сонымен қатар, шот ұсыну түрін дәл орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-109">Also make sure you accurately set the billing type.</span></span> <span data-ttu-id="3ce20-110">Ақы алынбайтын шот ұсыну түрінен тұратын элементтер жиыны келісімшарт немесе баға ұсыну жолдарын көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="3ce20-110">An item set with a non-chargeable billing type doesn’t show up on contract or quote lines.</span></span>  
  
 <span data-ttu-id="3ce20-111">Ресурс рөлдері орнатылса, бағатізбемен құны мен сатылым бағаларын орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="3ce20-111">Once you’ve set up resource roles, you can set up cost and sales prices with a price list.</span></span>  
  
 <span data-ttu-id="3ce20-112">Қосу керек әрбір рөл үшін келесіні істеңіз:</span><span class="sxs-lookup"><span data-stu-id="3ce20-112">For each role you want to add, do the following:</span></span>  
  
1.  <span data-ttu-id="3ce20-113">**Project Service > Ресурс рөлдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-113">Go to **Project Service > Resource Roles**.</span></span>  
  
2.  <span data-ttu-id="3ce20-114">**Жаңа** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-114">Click **New**.</span></span>  
  
3.  <span data-ttu-id="3ce20-115">**Жалпы** аумағында **Атау** ішінде рөл атын енгізіп, басқа өрістерді қажетінше толтырыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-115">In the **General** area, enter a name for the role in **Name**, and then fill in the other fields as necessary.</span></span>  
  
4.  <span data-ttu-id="3ce20-116">Өңдеуді жалғастыра алу үшін жазбаны жасауға **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-116">Click **Save** to create the record so you can continue editing it.</span></span>  
  
5.  <span data-ttu-id="3ce20-117">**Біліктіліктер** аумағында біліктілік қосу үшін **+** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-117">In the **Skills** area, click **+** to add a skill.</span></span>  
  
6.  <span data-ttu-id="3ce20-118">**Рөл біліктілігі талабы** тақтасында **Біліктілік** өрісін басып, **Іздеу** түймешігін басып, біліктілікті таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-118">In the **Role competency requirement** pane, click in the **Skill** field, click the **Search** button, and then select a skill.</span></span>  
  
7.  <span data-ttu-id="3ce20-119">Біліктіліктің тиімділігін таңдап, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-119">Select a proficiency for that skill, and then click **Save**.</span></span>  
  
8.  <span data-ttu-id="3ce20-120">Біліктіліктерді қосуды қажетінше жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-120">Continue adding skills as necessary.</span></span> <span data-ttu-id="3ce20-121">Орындалған кезде экранның төменгі оң жақ бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-121">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
9. <span data-ttu-id="3ce20-122">Пайдаланылатын жобаларға осы ресурс рөлін қолжетімді ету үшін **Белсендіру** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="3ce20-122">To make this resource role available for projects to use, click **Activate**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="3ce20-123">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="3ce20-123">See Also</span></span>  
 [<span data-ttu-id="3ce20-124">Ресурстарды реттеу</span><span class="sxs-lookup"><span data-stu-id="3ce20-124">Set up resources</span></span>](../project-service/set-up-resources.md)
