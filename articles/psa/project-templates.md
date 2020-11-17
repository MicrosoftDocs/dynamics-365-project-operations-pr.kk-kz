---
title: Жоба үлгілері
description: Бұл тақырыпта жобаны жылдам орнату үшін жоба үлгілерін пайдалану жолы туралы ақпарат берілген.
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
ms.openlocfilehash: 4fd618e15524c5cef5b6da9b282f449e3dfb7973
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123027"
---
# <a name="project-templates"></a><span data-ttu-id="722a0-103">Жоба үлгілері</span><span class="sxs-lookup"><span data-stu-id="722a0-103">Project templates</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="722a0-104">Жоба үлгісі — бұл жобаны тез әрі оңай бастауға көмектесетін алдын ала анықталған инфрақұрылым.</span><span class="sxs-lookup"><span data-stu-id="722a0-104">A project template is a predefined framework that helps you quickly and easily start a project.</span></span> <span data-ttu-id="722a0-105">Жаңа жобаны тінтуірді бір-ақ рет басу арқылы жасау үшін, алдын ала анықталған үлгіні пайдалана аласыз.</span><span class="sxs-lookup"><span data-stu-id="722a0-105">You can use a predefined template to create a new project with a single click.</span></span> <span data-ttu-id="722a0-106">Жобаларға келетін болсақ, жоба үлгілерінің алғышарттарын анықтауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="722a0-106">As for projects, you must define the prerequisites for project templates.</span></span> <span data-ttu-id="722a0-107">Әрбір жоба үлгісіне арналған жоба күнтізбесін анықтауыңыз керек, ал рөлдер мен бағатізбелер ұйымда алдын ала анықталуы керек, сонда үлгінің компоненттері пайдалы деректерді қамтитын болады.</span><span class="sxs-lookup"><span data-stu-id="722a0-107">You must define a project calendar for each project template, and roles and price lists must be predefined in the organization, so that the components of the template have useful data.</span></span>

<span data-ttu-id="722a0-108">Жоба үлгісі үш компоненттен тұрады: кесте, жобаны болжамдары және жоба тобының мүшелері.</span><span class="sxs-lookup"><span data-stu-id="722a0-108">A project template consists of three components: a schedule, project estimates, and project team members.</span></span>

## <a name="schedule"></a><span data-ttu-id="722a0-109">Жоспарлау</span><span class="sxs-lookup"><span data-stu-id="722a0-109">Schedule</span></span>

<span data-ttu-id="722a0-110">Жоба үлгісіндегі кестеде жобадағы кесте сияқты элементтер жиынтығы бар.</span><span class="sxs-lookup"><span data-stu-id="722a0-110">A schedule in a project template has the same set of elements as a schedule in a project.</span></span> <span data-ttu-id="722a0-111">Тапсырма иерархиясын жасауға, рөлдерді тапсырмалармен байланыстыруға, кесте атрибуттарын анықтауға, тәуелділіктерді орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="722a0-111">You can create a task hierarchy, associate roles with tasks, define schedule attributes, and set dependencies.</span></span> <span data-ttu-id="722a0-112">Жоба үлгісіндегі кесте әр тапсырма үшін тапсырма режимдерін қолдайды.</span><span class="sxs-lookup"><span data-stu-id="722a0-112">A schedule in a project template also supports task modes for each task.</span></span> <span data-ttu-id="722a0-113">Сондықтан, ол жоспарлау механизмін қолдайды.</span><span class="sxs-lookup"><span data-stu-id="722a0-113">Therefore, it supports the scheduling engine.</span></span> <span data-ttu-id="722a0-114">Жоба күнтізбесін жобамен байланыстыруыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="722a0-114">You must associate a project calendar with the project.</span></span> <span data-ttu-id="722a0-115">Жұмыс кестесін жасаған кезде, жоба үлгісі және жоба арасында еш айырмашылық болмайды.</span><span class="sxs-lookup"><span data-stu-id="722a0-115">When you create a work schedule, there is no difference between a project template and a project.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="722a0-116">Жоба болжамдары</span><span class="sxs-lookup"><span data-stu-id="722a0-116">Project estimates</span></span>

<span data-ttu-id="722a0-117">Жоба үлгісіндегі жоба болжамдары жобадағы жоба болжамдары сияқты жұмыс істейді.</span><span class="sxs-lookup"><span data-stu-id="722a0-117">Project estimates in a project template work the same way as project estimates in a project.</span></span> <span data-ttu-id="722a0-118">Алайда, өзіндік құн мен сатылым бағалары параметрлерде анықталған әдепкі құн мен сатылым бағалары тізімдерінен алынады.</span><span class="sxs-lookup"><span data-stu-id="722a0-118">However, the cost and sales prices are pulled from the default cost and sales price lists that are defined in the parameters.</span></span>

## <a name="creating-a-project-from-a-template"></a><span data-ttu-id="722a0-119">Үлгіден жоба жасау</span><span class="sxs-lookup"><span data-stu-id="722a0-119">Creating a project from a template</span></span>
 
<span data-ttu-id="722a0-120">Жоба үлгісінен жобаны жасаудың бірнеше жолы бар:</span><span class="sxs-lookup"><span data-stu-id="722a0-120">There are several ways to create a project from a project template:</span></span>

- <span data-ttu-id="722a0-121">Жобаны баға ұсынысынан жасаған кезде, жоба үлгісін **Жылдам жасау: жоба** диалогтық терезесінен таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="722a0-121">When you create a project from a quote, you can select a project template in the **Quick Create: Project** dialog box.</span></span>

> !["Жылдам жасау: жоба" диалогтық терезесі](media/project-11.png)

- <span data-ttu-id="722a0-123">Жобаны **Жаңа жоба** параметрін таңдау арқылы жасаған кезде, **Жоба** беті жазба сақталғанға дейін пайда болады.</span><span class="sxs-lookup"><span data-stu-id="722a0-123">When you create a project by selecting **New Project**, the **Project** page appears before the record is saved.</span></span> <span data-ttu-id="722a0-124">**Үлгіні таңдау** өрісінде ұйымдағы алдын ала анықталған жоба үлгілерінің біреуін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="722a0-124">In the **Pick a Template** field, select one of the predefined project templates in the organization.</span></span>
- <span data-ttu-id="722a0-125">**Үлгі нысаны** бетіндегі **Үлгіден жоба жасау** параметрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="722a0-125">Use **Create Project from a Template** on the **Template Entity** page.</span></span>

## <a name="copying-components-of-template-to-project"></a><span data-ttu-id="722a0-126">Үлгі компоненттерін жобаға көшіру</span><span class="sxs-lookup"><span data-stu-id="722a0-126">Copying components of template to project</span></span>

<span data-ttu-id="722a0-127">Жоба үлгісінің компоненттерін жобаға көшіргенде, жобадағы параметрлерге байланысты бірнеше қайта жазулар орын алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="722a0-127">When you copy the components of a project template to a project, a few overrides can occur, depending on the settings in the project.</span></span>

### <a name="copying-the-schedule"></a><span data-ttu-id="722a0-128">Кестені көшіру</span><span class="sxs-lookup"><span data-stu-id="722a0-128">Copying the schedule</span></span>

<span data-ttu-id="722a0-129">Кестені жоба үлгісінен көшірген кезде, жобадағы күнтізбе үлгіден өзгеше болса, жоба күнтізбесіндегі жұмыс сағаттары тапсырмалар кестесіне қолданылады.</span><span class="sxs-lookup"><span data-stu-id="722a0-129">When you copy the schedule from a project template, if the project has a different project calendar than the template, work hours from the project's calendar are applied to the task schedule.</span></span> <span data-ttu-id="722a0-130">Бұл жағдайда кесте негізгі жоба күнтізбесіне сәйкес болу үшін реттеледі.</span><span class="sxs-lookup"><span data-stu-id="722a0-130">In this way, the schedule is adjusted to match the backing project calendar.</span></span> <span data-ttu-id="722a0-131">Осылайша, кестедегі бірінші тапсырма жобаның басталу күнін алады, ал қалған иерархияның кестесі үлгіде көрсетілген ұзақтық және тәуелділіктер негізінде жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="722a0-131">Similarly, the first task on the schedule takes the project's start date, and the schedule of the rest of the hierarchy is updated based on the duration and dependencies that are specified in the template.</span></span> 

### <a name="copying-project-estimates"></a><span data-ttu-id="722a0-132">Жоба болжамдарын көшіру</span><span class="sxs-lookup"><span data-stu-id="722a0-132">Copying project estimates</span></span> 

<span data-ttu-id="722a0-133">Жоба болжамдарының жолдары бойынша көшіргенде, бағатізбелер жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="722a0-133">When you copy across project estimate lines, the price lists are updated.</span></span> <span data-ttu-id="722a0-134">Шығындар тізімі үшін бұл жаңартулар жобаның тиесілі бірлігіне негізделеді.</span><span class="sxs-lookup"><span data-stu-id="722a0-134">For the cost price list, these updates are based on the owning unit of the project.</span></span> <span data-ttu-id="722a0-135">Сатылым бағатізбесі үшін олар тұтынушыға негізделеді.</span><span class="sxs-lookup"><span data-stu-id="722a0-135">For the sales price list, they are based on the customer.</span></span> <span data-ttu-id="722a0-136">Сатылым нысанымен байланысты жобалар үшін бірлік құны және сатылым бағалары бағатізбелер негізінде анықталады.</span><span class="sxs-lookup"><span data-stu-id="722a0-136">For projects that are associated with a sales entity, the unit cost and sales prices are determined based on these price lists.</span></span>

### <a name="copying-a-project-team"></a><span data-ttu-id="722a0-137">Жоба тобын көшіру</span><span class="sxs-lookup"><span data-stu-id="722a0-137">Copying a project team</span></span>

<span data-ttu-id="722a0-138">Жоба тобы жоба үлгісінен жобаға көшірілген кезде, әмбебап ресурстар үлгіде анықталған дағдылар мен біліктіліктермен бірге көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="722a0-138">When a project team is copied from a project template to a project, the generic resources are copied, together with the skills and proficiencies that are defined in the template.</span></span> <span data-ttu-id="722a0-139">Әмбебап ресурс тағайындаулары да жоба үлгісіндегі күйінде сақталады.</span><span class="sxs-lookup"><span data-stu-id="722a0-139">Generic resource assignments are also maintained as they were in the project template.</span></span> <span data-ttu-id="722a0-140">Аталған ресурстарға жоба үлгілерінде қолдау көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="722a0-140">Named resources aren't supported in project templates.</span></span>
