---
title: Жаңа жобаны жасау
description: Бұл тақырыпта жаңа жоба жасау жолы туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 727d287c571b2a64bf10b2393a87567093a420d2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079795"
---
# <a name="create-a-new-project"></a><span data-ttu-id="0b59c-103">Жаңа жобаны жасау</span><span class="sxs-lookup"><span data-stu-id="0b59c-103">Create a new project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="0b59c-104">Жаңа жоба жасау үшін келесі әрекеттерді орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-104">Complete the following steps to create a new project.</span></span>

1. <span data-ttu-id="0b59c-105">**Жобаны басқару** бетінде **Жаңа жоба** опциясын таңдаңыз да, келесі мәндерді енгізіңіз:</span><span class="sxs-lookup"><span data-stu-id="0b59c-105">On the **Project management** page, select **New project** , and enter the following values:</span></span>

    - <span data-ttu-id="0b59c-106">**Жоба түрі:** уақыт және материал</span><span class="sxs-lookup"><span data-stu-id="0b59c-106">**Project type:** Time and material</span></span>
    - <span data-ttu-id="0b59c-107">**Жоба атауы:** XYZ жаңартуының 2-кезеңі</span><span class="sxs-lookup"><span data-stu-id="0b59c-107">**Project name:** XYZ Upgrade Phase 2</span></span>
    - <span data-ttu-id="0b59c-108">**Жоба тобы:** TM\_WIP</span><span class="sxs-lookup"><span data-stu-id="0b59c-108">**Project group:** TM\_WIP</span></span>
    - <span data-ttu-id="0b59c-109">**Жоба келісім-шартының идентификаторы:** 00000002</span><span class="sxs-lookup"><span data-stu-id="0b59c-109">**Project contract ID:** 00000002</span></span>

2. <span data-ttu-id="0b59c-110">**Жоба жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-110">Select **Create project**.</span></span>

## <a name="assign-a-resource-to-a-project"></a><span data-ttu-id="0b59c-111">Ресурсты жобаға тағайындау</span><span class="sxs-lookup"><span data-stu-id="0b59c-111">Assign a resource to a project</span></span>

1. <span data-ttu-id="0b59c-112">**Жұмысшылар** тізіміндегі **Жұмысшылар** бетінен бұрын құзыреттіліктерді орнатқан жұмысшыға арналған жазбаны таңдап, жұмысшы жазбасын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-112">On the **Workers** page, in the **Workers** list, select the record for the worker that you previously set up competencies for, and open the worker record.</span></span>
2. <span data-ttu-id="0b59c-113">Әрекеттер тақтасындағы **Жоба** қойыншасынан **Орнату** тобындағы **Жобаларды тағайындау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-113">On the Action Pane, on the **Project** tab, in the **Setup** group, select **Assign projects**.</span></span>
3. <span data-ttu-id="0b59c-114">**Ресурсты тексеру жобасының тағайындамалары** бетіндегі **Жобалар** қойыншасында **Жобаны таңдалған жобаларға қосу** өрісіндегі **XYZ жаңартуының 2-кезеңі** жобасын сүзгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-114">On the **Resource validation project assignments** page, on the **Projects** tab, in the **Add the project to selected projects** field, filter on the **XYZ Upgrade Phase 2** project.</span></span>
4. <span data-ttu-id="0b59c-115">**Қалған жобалар** тақтасынан жобаны таңдап, содан кейін оны **Таңдалған жобалар** тақтасына қосу үшін көрсеткі түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-115">In the **Remaining projects** pane, select a project, and then select the arrow button to add it to the **Selected projects** pane.</span></span>

<span data-ttu-id="0b59c-116">Сондай-ақ ресурсқа санаттарды қажетінше тағайындауға болады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-116">You can also assign categories for a resource as you require.</span></span> <span data-ttu-id="0b59c-117">Санат түрі **Шығын** немесе **Табыс**.</span><span class="sxs-lookup"><span data-stu-id="0b59c-117">The category type is either **Cost** or **Revenue**.</span></span> <span data-ttu-id="0b59c-118">Санат түрін ұйым анықтайды.</span><span class="sxs-lookup"><span data-stu-id="0b59c-118">The category type is determined by your organization.</span></span> <span data-ttu-id="0b59c-119">Егер ресурсқа санаттар тағайындалмаса, Finance жүйесі шығын мен кірістің сағаттық бағалары үшін әдепкі санатты іздейді.</span><span class="sxs-lookup"><span data-stu-id="0b59c-119">If no categories are assigned for a resource, Finance looks up the default category on hour prices for cost and revenue.</span></span>

## <a name="set-up-project-resource-and-role-characteristics"></a><span data-ttu-id="0b59c-120">Жоба ресурсын және рөл сипаттарын орнату</span><span class="sxs-lookup"><span data-stu-id="0b59c-120">Set up project resource and role characteristics</span></span>

<span data-ttu-id="0b59c-121">Жоба менеджері жоба үшін қажетті рөлдерді жасау үшін жобаның ресурс функциясын қолдана алады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-121">A project manager can use the project resourcing functionality to create the roles that are required for the project.</span></span> <span data-ttu-id="0b59c-122">Рөлдерді ресурстар сақталған кезде расталған ресурстар әлі белгісіз болса пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-122">Roles can be used if confirmed resources are still unknown when resources are being reserved.</span></span> <span data-ttu-id="0b59c-123">Рөлдерді жоспарланған ресурстар ретінде уақытша сақтауға болады, осылайша жобаның жоспарлау кезеңдерін жалғастыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-123">Roles can be temporarily reserved as planned resources, so that you can continue the project planning stages.</span></span>

<span data-ttu-id="0b59c-124">[![Рөлдің мысалы](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span><span class="sxs-lookup"><span data-stu-id="0b59c-124">[![Example of a role](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span></span> 

<span data-ttu-id="0b59c-125">**Сценарий:** Contoso компаниясы бекітілген жобалық жарғысы бар "Уақыт және материалдар" жобасын аяқтау үшін жалданды.</span><span class="sxs-lookup"><span data-stu-id="0b59c-125">**Scenario:** Contoso was hired to complete a Time and material project that has an approved project charter.</span></span> <span data-ttu-id="0b59c-126">Кіші жоба менеджері жоба ауқымын әлі аяқтауда.</span><span class="sxs-lookup"><span data-stu-id="0b59c-126">The junior project manager is still completing the scope of the project.</span></span> <span data-ttu-id="0b59c-127">Ресурстар менеджері қазіргі уақытта жаңа жобада жұмыс істеу үшін сақталатын нақты ресурстарды анықтауда.</span><span class="sxs-lookup"><span data-stu-id="0b59c-127">The resource manager is currently identifying specific resources that will be reserved to work on the new project.</span></span> <span data-ttu-id="0b59c-128">Жобаның критикалық сипатына байланысты жоба демеушісі рөлдердің бірі ретінде аға жоба менеджерін сұрады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-128">Because of the critical nature of the project, the project sponsor requested Senior project manager as one of the roles.</span></span> <span data-ttu-id="0b59c-129">Кіші жоба менеджері жобаны жоспарлау кезінде ресурстар туралы ақпарат қажет болған жағдайда ресурс менеджері жаңа ресурсты алып, жүйеде рөлін анықтауы керек.</span><span class="sxs-lookup"><span data-stu-id="0b59c-129">The resource manager must acquire the new resource and define the role in the system in case the junior project manager requires the resource information during project planning.</span></span>

<span data-ttu-id="0b59c-130">Келесі қадамдарда ресурс менеджері аға жоба менеджері рөлін қалай орната алатындығы және онымен ресурстар сипаттамаларын байланыстыратыны көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="0b59c-130">The following steps show how the resource manager can set up the Senior project manager role and associate resource characteristics with it.</span></span> <span data-ttu-id="0b59c-131">Кейінірек бұл рөлді қажетті ресурс құзыреттілігіне сәйкес келетін қолжетімді ресурстарды табу үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-131">Later, the role can be used to search for available resources that match the required resource competencies.</span></span>

1. <span data-ttu-id="0b59c-132">**Рөлдерді орнату** бетінде **Жаңа** опциясын таңдаңыз да, келесі мәндерді енгізіңіз:</span><span class="sxs-lookup"><span data-stu-id="0b59c-132">On the **Setup roles** page, select **New** , and enter the following values:</span></span>

    - <span data-ttu-id="0b59c-133">**Рөл идентификаторы:** аға жоба менеджері</span><span class="sxs-lookup"><span data-stu-id="0b59c-133">**Role ID:** Senior Project Manager</span></span>
    - <span data-ttu-id="0b59c-134">**Сипаттама:** аға жоба менеджері</span><span class="sxs-lookup"><span data-stu-id="0b59c-134">**Description:** Senior Project Manager</span></span>

2. <span data-ttu-id="0b59c-135">**Жасау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-135">Select **Create**.</span></span>
3. <span data-ttu-id="0b59c-136">**Аға жоба менеджері** рөлін, содан кейін **Сипаттарды орнату** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-136">Select the **Senior Project Manager** role, and then select **Configure characteristics**.</span></span>
4. <span data-ttu-id="0b59c-137">**Сипаттамалар түрі** өрісінен **Дағды** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-137">In the **Characteristics type** field, select **Skill**.</span></span>
5. <span data-ttu-id="0b59c-138">**Қолжетімді сипаттамалар** өрісіне іздеу қажет дағдыны енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-138">In the **Available characteristics** field, enter the skill to search for.</span></span>
6. <span data-ttu-id="0b59c-139">**Сипаттама түрі** өрісінен **Куәлік** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-139">In the **Characteristic type** field, select **Certificate**.</span></span>
7. <span data-ttu-id="0b59c-140">**Қолжетімді сипаттамалар** өрісіне іздеу қажет куәлік түрін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-140">In the **Available characteristics** field, enter the certificate type to search for.</span></span>

## <a name="assign-a-project-resource-to-a-project"></a><span data-ttu-id="0b59c-141">Жоба ресурсын жобаға тағайындау</span><span class="sxs-lookup"><span data-stu-id="0b59c-141">Assign a project resource to a project</span></span>

1. <span data-ttu-id="0b59c-142">**Барлық жобалар** бетінен **XYZ жаңартуының 2-кезеңі** жобасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-142">On the **All projects** page, select the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="0b59c-143">**Жоба тобы және жоспарлау** қойыншасынан **Қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-143">On the **Project team and scheduling** tab, select **Add**.</span></span>
3. <span data-ttu-id="0b59c-144">**Рөл** өрісінен **Топ мүшесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-144">In the **Role** field, select **Team member**.</span></span>
4. <span data-ttu-id="0b59c-145">**Күнтізбеден тапсырыс беру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-145">Select **Book from calendar**.</span></span>
5. <span data-ttu-id="0b59c-146">**Ресурс қолжетімділігі** бетінен **Көрініс параметрлері** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-146">On the **Resource availability** page, select **View settings**.</span></span>
6. <span data-ttu-id="0b59c-147">**Көру параметрлерін реттеу** бетіне келесі мәндерді енгізіңіз:</span><span class="sxs-lookup"><span data-stu-id="0b59c-147">On the **Adjust view settings** page, enter the following values:</span></span>

    - <span data-ttu-id="0b59c-148">**Күндер ауқымы көрінісінің пішімі:** күн</span><span class="sxs-lookup"><span data-stu-id="0b59c-148">**Format for date range view:** Day</span></span>
    - <span data-ttu-id="0b59c-149">**Қолжетімділік сипаттамаларын көрсету:** иә</span><span class="sxs-lookup"><span data-stu-id="0b59c-149">**Display availability descriptions:** Yes</span></span>
    - <span data-ttu-id="0b59c-150">**Қалған сыйымдылықты көрсету:** иә</span><span class="sxs-lookup"><span data-stu-id="0b59c-150">**Display remaining capacity:** Yes</span></span>

7. <span data-ttu-id="0b59c-151">Ресурстар тізімінен ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-151">In the list of resources, select a resource.</span></span>
8. <span data-ttu-id="0b59c-152">**Қатты көшірме** және **Толық сыйымдылығы** тармақтарын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-152">Select **Hard book** and **Full capacity**.</span></span>

## <a name="assign-a-resource-to-a-default-role"></a><span data-ttu-id="0b59c-153">Ресурсты әдепкі рөлге тағайындау</span><span class="sxs-lookup"><span data-stu-id="0b59c-153">Assign a resource to a default role</span></span>

<span data-ttu-id="0b59c-154">Жоба немесе ресурстар менеджерлеріне көмектесу үшін олар жоба үшін сақталуы мүмкін ресурстарды тереңірек қарастыра алады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-154">To help project or resource managers can drill down further on the resources that can be reserved for a project.</span></span> <span data-ttu-id="0b59c-155">Әдепкі рөлді бұрыннан бар ресурспен немесе жаңадан алынған ресурспен байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-155">You can associate a default role with an existing resource or a newly acquired resource.</span></span> <span data-ttu-id="0b59c-156">Мысалы, Даниэлді жұмысқа қабылдаған кезде оның бизнес-аналитика рөлін орындау тәжірибесі мен дағдылары болды.</span><span class="sxs-lookup"><span data-stu-id="0b59c-156">For example, when Daniel was hired, he had the experience and skills to fill the Business analyst role.</span></span> <span data-ttu-id="0b59c-157">Ресурс менеджері бұл рөлді Даниелдің әдепкі рөліне тағайындады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-157">The resource manager assigned this role as Daniel's default role.</span></span> <span data-ttu-id="0b59c-158">Сондықтан ресурстар менеджері Даниэлді жобалармен жұмыс істеуге дайын бизнес-аналитиктер тобына қосты.</span><span class="sxs-lookup"><span data-stu-id="0b59c-158">Therefore, the resource manager added Daniel to a pool of business analysts who are available to work on projects.</span></span>

<span data-ttu-id="0b59c-159">Ресурстарды резервтеу кезінде жоба менеджерлері жобаларда жұмыс істеу үшін қолжетімді рөлдік ресурстарды сүзгілей алады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-159">During resource reservation, project managers can filter the role resources that are available to work on projects.</span></span> <span data-ttu-id="0b59c-160">Олар бұл ақпаратты ресурстарды орындау кезінде көп критерийлі шешімдерді талдау кезінде бір критерий ретінде қолдана алады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-160">They can use this information as one criterion when they perform multi-criteria decision analysis during resource fulfillment.</span></span> <span data-ttu-id="0b59c-161">Сонымен қатар олар берілген жоба үшін белгілі бір дағдыға, білімге және тәжірибеге ие ресурстарды табу үшін сүзгіге басқа ресурс сипаттамаларын қоса алады.</span><span class="sxs-lookup"><span data-stu-id="0b59c-161">They can also add other resource characteristics to the filter to search for resources that have specific skills, education, and experience for a given project.</span></span>

<span data-ttu-id="0b59c-162">**Сценарий:** бекітілген жоба басталды және жобаның аға менеджері рөлі жобаны жоспарлау кезеңінде жоспарланған ресурс ретінде сақталды.</span><span class="sxs-lookup"><span data-stu-id="0b59c-162">**Scenario:** An approved project has started, and the Senior project manager role was reserved as a planned resource during the project planning stage.</span></span> <span data-ttu-id="0b59c-163">Ресурс менеджері қазір аға жоба менеджері рөлін орындау үшін ресурс алды.</span><span class="sxs-lookup"><span data-stu-id="0b59c-163">The resource manager has now acquired a resource to fulfill the Senior project manager role.</span></span>

1. <span data-ttu-id="0b59c-164">**Ресурстар тізімі** бетінен **Даниэль Гольдшмидт** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-164">On the **Resources list** page, select **Daniel Goldschmidt**.</span></span>
2. <span data-ttu-id="0b59c-165">**Ресурс рөлі** бетінде **Жаңа** опциясын таңдаңыз да, келесі мәндерді енгізіңіз:</span><span class="sxs-lookup"><span data-stu-id="0b59c-165">On the **Resource role** page, select **New** , and enter the following values:</span></span>

    - <span data-ttu-id="0b59c-166">**Күшіне енеді:** ағымдағы күнді енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-166">**Effective:** Enter the current date.</span></span>
    - <span data-ttu-id="0b59c-167">**Жарамдылық мерзімінің бітуі:** **Ешқашан** мәнін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-167">**Expiration:** Enter **Never**.</span></span>
    - <span data-ttu-id="0b59c-168">**Рөл:** **Аға жоба менеджері** енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-168">**Role:** Enter **Senior Project Manager**.</span></span>

3. <span data-ttu-id="0b59c-169">**Сақтау** параметрін таңдап, бетті жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-169">Select **Save** , and then close the page.</span></span>
4. <span data-ttu-id="0b59c-170">**Құзыреттер** қойыншасына **ProjectMgmt** дағдысы мен **PMP** куәлігін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="0b59c-170">On the **Competencies** tab, add the **ProjectMgmt** skill and the **PMP** certificate.</span></span>
