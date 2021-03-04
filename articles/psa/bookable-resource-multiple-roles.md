---
title: Тапсырыс беруге болатын ресурс жоба үшін рөлді орындаған кезде, жоба сатылымдары мен шығындарын болжау
description: Бұл тақырып жобада бірнеше рөлді орындайтын ресурс үшін баға мен шығындарды қолдау үшін баға өлшемдерін пайдалану жолы туралы ақпаратты қамтиды.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 67e24156e960b9b09cf92f7f0cd77f6c74a982b8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145050"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-for-a-project"></a><span data-ttu-id="7cc2b-103">Тапсырыс беруге болатын ресурс жоба үшін рөлді орындаған кезде, жоба сатылымдары мен шығындарын болжау</span><span class="sxs-lookup"><span data-stu-id="7cc2b-103">Estimate project sales and costs when a bookable resource fills multiple roles for a project</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="7cc2b-104">Жобаға негізделген компаниялар көбінесе жобада бірнеше рөлді орындау үшін бір ресурсты қажет етеді.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-104">Project-based companies often have the need for one resource to perform multiple roles on a project.</span></span> <span data-ttu-id="7cc2b-105">Осы рөлдердің әрқайсысы әртүрлі бағалануы және әртүрлі болуы мүмкін, яғни жобадағы бірдей ресурстың уақыты төлемге және рөлдердің әрқайсысының шығын мөлшеріне байланысты әртүрлі қаржылық бағалау ала алады.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-105">Each of these roles could be priced and costed differently, which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="7cc2b-106">Project Service Automation аталған ресурс үшін топ мүшелерінің жазбасындағы мәндерді орнатуға мүмкіндік береді және топ мүшесіне тағайындалған әр тапсырма бойынша әртүрлі қайта анықтау әрекеттеріне мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="7cc2b-107">Келесі мысалда осы мәнді қарапайым қайта анықтау ресурстарға жобада әртүрлі шығындар мен төлем өлшемдерімен бірнеше рөлге ие болуға мүмкіндік беретіндігі түсіндірілген.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="7cc2b-108">Тапсырмаларды жасау</span><span class="sxs-lookup"><span data-stu-id="7cc2b-108">Create tasks</span></span>
<span data-ttu-id="7cc2b-109">Әрқайсысы 40 сағаттан екі жоба тапсырмасын жасаңыз, А және В тапсырмалары. В тапсырмасының алдындағысы ретінде А тапсырмасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="7cc2b-110">Жалпы жоба тобының мүшесі үшін "Рөл" және "Бөлімше" құрыңыз</span><span class="sxs-lookup"><span data-stu-id="7cc2b-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="7cc2b-111">**Кесте** бетінде, А тапсырмасы үшін **Тапсырма** қатарын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="7cc2b-112">**Ресурстар** өрісінде, ашылмалы тізімнен **Жасау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="7cc2b-113">**Топ мүшесін жылдам жасау** бетінде, осы тапсырманы орындай алатын жалпы топ мүшесінің төлсипаттарын көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="7cc2b-114">Тиісті рөл мен бөлімшені таңдап, содан кейін **Сақтау және жабу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="7cc2b-115">Бұл тапсырмаға жалпы топ мүшесі құрылады және тағайындалады.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="7cc2b-116">В тапсырмасы үшін осы әрекеттерді қайталаңыз және В тапсырмасы үшін құрылған жалпы топ мүшесіндегі рөл мен бөлімше А тапсырмасынан өзгеше екеніне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="7cc2b-117">Жоба тапсырмасы үшін рөл және бөлімше құрыңыз</span><span class="sxs-lookup"><span data-stu-id="7cc2b-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="7cc2b-118">А тапсырмасын жасағаннан кейін, тапсырманы таңдап, содан кейін **Тапсырманы өңдеу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="7cc2b-119">**Тапсырма туралы мәліметтер** бетінде, **Рөл** және **Бөлімше** өрістерін тауып, осы тапсырманы орындай алатын ресурстарға қажет мәндерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="7cc2b-120">Егер осы сценарийлерді Project Service Automation демо-деректерін пайдаланып толтырсаңыз, рөл үшін **Кеңес беруші ықтимал тұтынушы** және бөлімше ретінде **Fabrikam US** таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="7cc2b-121">В тапсырмасын таңдап, содан кейін **Тапсырманы өңдеу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="7cc2b-122">**Тапсырма туралы мәліметтер** бетінде, **Рөл** және **Бөлімше** өрістерін тауып, осы тапсырманы орындай алатын ресурстарға қажет мәндерді қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="7cc2b-123">**Рөл** және **Ұйымдық бірлік** өрістеріндегі мәндердің B тапсырмасы үшін А тапсырмасының мәндерінен өзгеше екендігін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from the values for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="7cc2b-124">Егер осы сценарийлерді Project Service Automation демо-деректерін пайдаланып толтырсаңыз, рөл үшін **Желі технигі** және бөлімше ретінде **Fabrikam US** таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="7cc2b-125">**Тапсырма туралы мәліметтер** бетін сақтап, жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behavior"></a><span data-ttu-id="7cc2b-126">Топ мүшесі және болжамдар әрекеті</span><span class="sxs-lookup"><span data-stu-id="7cc2b-126">Team member and estimates behavior</span></span> 

1. <span data-ttu-id="7cc2b-127">**Тапсырма туралы мәліметтер** бетіндегі **Топ мүшесі** өрісінде, екі жалпы топ мүшелерін таңдап, содан кейін **Талаптарды құру** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-127">On the **Task Details** page, on the **Team Member**, select the two generic team Members and then select **Generate Requirements**.</span></span> 
2. <span data-ttu-id="7cc2b-128">**Кеңес беруші ықтимал тұтынушы** үшін топ мүшесінің жолын таңдаңыз, содан кейін **Брондау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-128">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="7cc2b-129">Кесте тақтасы ашылып, сол талап үшін ресурсты брондайды.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-129">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="7cc2b-130">**Желі технигі** үшін топ мүшесінің жолын таңдап, **Брондау** пәрменін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-130">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="7cc2b-131">Кесте тақтасы ашылып, сол талапта бірдей ресурсты брондайды.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-131">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="7cc2b-132">Топ мүшесі торы</span><span class="sxs-lookup"><span data-stu-id="7cc2b-132">Team Member grid</span></span> 
<span data-ttu-id="7cc2b-133">**Топ мүшесі** торында, екі жалпы топ мүшесінің жазбалары жойылғанын және бір ресурспен алмастырылғанын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-133">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="7cc2b-134">**Рөл** және **Бөлімше** үшін әдепкі мәндер жиынтығын көрсететін ресурсқа арналған бір мәндер жиынтығы бар.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-134">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="7cc2b-135">Топ мүшесі жазбасының жолын кеңейткен кезде, топ мүшесінің жазбасында осы тапсырмалардың екеуіне де арналған бөлек тағайындауларды көруге болады.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-135">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="7cc2b-136">Әрбір тағайындау жолында **Рөл** және **Ұйымдық бірлік** үшін тапсырмаға сәйкес мәндер бар.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-136">Each assignment row has task-specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="7cc2b-137">Болжамдар торы</span><span class="sxs-lookup"><span data-stu-id="7cc2b-137">Estimates grid</span></span> 
<span data-ttu-id="7cc2b-138">**Болжамдар** торына өткен кезде, бір ресурсқа арналған тағайындаулардың екеуі де әртүрлі бағаланғанын байқайсыз.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-138">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="7cc2b-139">А тапсырмасындағы ресурсқа арналған тағайындау **Кеңес беруші ықтимал тұтынушы** параметрінің **Рөл** төлсипат мәні арқылы бағаланады.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-139">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="7cc2b-140">В тапсырмасындағы бірдей ресурсқа арналған тағайындау **Желі технигі** параметрінің **Рөл** төлсипат мәні арқылы бағаланады.</span><span class="sxs-lookup"><span data-stu-id="7cc2b-140">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>

