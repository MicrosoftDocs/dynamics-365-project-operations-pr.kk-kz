---
title: Жоба тобын жасау
description: Бұл тақырыпта жоба топтарын жасау және басқару жолы туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kdwns
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 121a007d91c2da4f3b9951901781757b8bcca8fe
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270865"
---
# <a name="create-a-project-team"></a><span data-ttu-id="624ed-103">Жоба тобын жасау</span><span class="sxs-lookup"><span data-stu-id="624ed-103">Create a project team</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="624ed-104">Бұрын жобада орнатылған рөлдерді пайдалану үшін жоба менеджері рөлдерді жобамен байланыстыруы керек.</span><span class="sxs-lookup"><span data-stu-id="624ed-104">To use the roles that were previously set up in a project, a project manager must associate the roles with the project.</span></span> <span data-ttu-id="624ed-105">Жобаға бірнеше рөл тағайындауға болады.</span><span class="sxs-lookup"><span data-stu-id="624ed-105">Multiple roles can be assigned for a project.</span></span> <span data-ttu-id="624ed-106">Шатаспау үшін бұл рөлдер резервтеу кезінде автоматты түрде белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="624ed-106">To prevent confusion, these roles are automatically labeled during reservation.</span></span> <span data-ttu-id="624ed-107">Мысалы, егер жоба менеджеріне үш бағдарламалық жасақтама инженері қажет болса, **1-бағдарламалық жасақтама инженері**, **2-бағдарламалық жасақтама инженері** және **3-бағдарламалық жасақтама инженері** ретінде белгіленген үш бағдарламалық жасақтама инженерінің рөлі автоматты түрде құрылады.</span><span class="sxs-lookup"><span data-stu-id="624ed-107">For example, if the project manager requires three software engineers, three Software engineer roles that have **software engineer 1**, **software engineer 2**, and **software engineer 3** as their labels are automatically generated.</span></span> <span data-ttu-id="624ed-108">Егер рөл үшін рөл сипаттамалары бұрын анықталған болса, олар ресурстарды іздеу кезінде сүзгі ретінде қолданылады.</span><span class="sxs-lookup"><span data-stu-id="624ed-108">If role characteristics were previously set for the role, they are applied as a filter during searches for a resource.</span></span> <span data-ttu-id="624ed-109">Іздеуді одан әрі нақтылау үшін қажет болған жағдайда қосымша сипаттамаларды қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="624ed-109">Additional characteristics can be added as required to further refine the search.</span></span>

<span data-ttu-id="624ed-110">Ресурстың қолжетімділігін жақсырақ көру үшін көрініс параметрлерін де теңшеуге болады.</span><span class="sxs-lookup"><span data-stu-id="624ed-110">View settings can also be customized to give a better view of resource availability.</span></span> <span data-ttu-id="624ed-111">Бір сағаттық, күнделікті, апталық, айлық, тоқсандық және жылдық қолжетімділікті көрсетудің нұсқалары бар.</span><span class="sxs-lookup"><span data-stu-id="624ed-111">There are options to show hourly, daily, weekly, monthly, quarterly, and annual availability.</span></span> <span data-ttu-id="624ed-112">Сондай-ақ ресурстардың қолжетімді және қалған сыйымдылығын көрсетуге болады.</span><span class="sxs-lookup"><span data-stu-id="624ed-112">There is also an option to show available and remaining capacity on resources.</span></span> <span data-ttu-id="624ed-113">Бұл опция әрекеттер үшін қолжетімді уақытты немесе ресурстардың қолжетімділігін бағалау кезінде уақытты басқару үшін пайдалы.</span><span class="sxs-lookup"><span data-stu-id="624ed-113">This option is useful for time management, when you're estimating available time for activities or resource availability.</span></span>

<span data-ttu-id="624ed-114">Жоба менеджері беттегі рөлді таңдай алады, содан кейін талаптарға сай қолжетімді ресурс болса, рөлді толтыру үшін ресурсты резервтеуді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-114">The project manager can select a role on the page and then, if there is an available resource that fits the requirement, select to reserve a resource to fill the role.</span></span> <span data-ttu-id="624ed-115">Жоспарлаудың осы кезеңінде ресурстарды сақтаудың қажеті жоқ екенін ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="624ed-115">Note that the resources don't have to be reserved at this point in the planning stage.</span></span> <span data-ttu-id="624ed-116">WBS жасаған кезде, рөлдерді жобаға арналған жинақталған ресурстармен алмастыруға болады.</span><span class="sxs-lookup"><span data-stu-id="624ed-116">When you create a WBS, you can replace roles with staffed resources for the project.</span></span> <span data-ttu-id="624ed-117">Егер рөлдер WBS ішінде жинақталған ресурстармен ауыстырылса, ресурс орнатылымы автоматты түрде жоба тобының тізімі мен кестесін жаңартады.</span><span class="sxs-lookup"><span data-stu-id="624ed-117">If roles are replaced with staffed resources in the WBS, the resource setup automatically updates the project team listing and scheduling.</span></span>

<span data-ttu-id="624ed-118">[![Рөлдерді де, нақты ресурстарды да қамтитын жоба тобының тізімі](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span><span class="sxs-lookup"><span data-stu-id="624ed-118">[![Project team listing that includes both roles and actual resources](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span></span> 

<span data-ttu-id="624ed-119">Жоба менеджерінде жоба үшін ресурсқа тапсырыс берудің әртүрлі нұсқалары бар, мысалы, **Қалған сыйымдылық**, **Толық сыйымдылығы**, **Сыйымдылық пайызы** және **Сағат көрсету**.</span><span class="sxs-lookup"><span data-stu-id="624ed-119">The project manager has various options for booking a resource for a project, such as **Remaining capacity**, **Full capacity**, **Capacity percentage**, and **Specify hours**.</span></span> <span data-ttu-id="624ed-120">Ресурс тағайындамасы өзгерген жағдайда, бұл тапсырыс опцияларынан кез келген уақытта бас тартуға болады.</span><span class="sxs-lookup"><span data-stu-id="624ed-120">These booking options can be canceled at any time if resource assignments change.</span></span> <span data-ttu-id="624ed-121">Тапсырыстың екі түріне қолдау көрсетіледі:</span><span class="sxs-lookup"><span data-stu-id="624ed-121">Two types of booking are supported:</span></span>

- <span data-ttu-id="624ed-122">**Қатты көшірме** – ресурстарды резервтеу көрсетілген мерзімде тапсырма бойынша жұмыс істеуге бекітілді және расталды.</span><span class="sxs-lookup"><span data-stu-id="624ed-122">**Hard Book** – The resource reservation was approved and confirmed to work on the engagement for the specified duration.</span></span>
- <span data-ttu-id="624ed-123">**"Жұмақ тіркеу"** – ресурсты алдын ала резервтеу көрсетілген мерзімде тапсырма бойынша жұмыс істеуге конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="624ed-123">**Soft book** – The resource reservations was tentatively set to work on the engagement for the specified duration.</span></span>

<span data-ttu-id="624ed-124">Келесі процедурада жоба тобын қалай жасауға болатыны түсіндіріледі.</span><span class="sxs-lookup"><span data-stu-id="624ed-124">The following procedure explains how to create a project team.</span></span>

## <a name="create-a-project-team"></a><span data-ttu-id="624ed-125">Жоба тобын жасау</span><span class="sxs-lookup"><span data-stu-id="624ed-125">Create a project team</span></span>

1. <span data-ttu-id="624ed-126">**Барлық жобалар** тізім бетінен жобаны таңдап, **Өңдеу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-126">On the **All projects** list page, select a project, and then select **Edit**.</span></span>
2. <span data-ttu-id="624ed-127">**Кестесінің аяқталу күні** өрісіндегі **Жоба тобы және жоспарлау** қойыншасына кестенің басталу күні + бір айды енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="624ed-127">On the **Project team and scheduling** tab, in the **Schedule end date** field, enter the schedule start date plus one month.</span></span> <span data-ttu-id="624ed-128">Мысалы, кестенің басталу күні 2017 жылдың 24 маусымы (24/06/2017) болса, **24/07/2017** енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="624ed-128">For example, if the schedule start date is June 24, 2017 (24/06/2017), enter **24/07/2017**.</span></span>
3. <span data-ttu-id="624ed-129">**Қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-129">Select **Add**.</span></span>
4. <span data-ttu-id="624ed-130">**Жобаға рөлдер қосу** тақтасындағы **Рөл** өрісінде **Аға жоба менеджері** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-130">In the **Add roles to the project** pane, in the **Role** field, select **Senior Project Manager**.</span></span>
5. <span data-ttu-id="624ed-131">**Қажетті құзыреттіліктер** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-131">Select **Required competencies**.</span></span>
6. <span data-ttu-id="624ed-132">**Сипаттамаларды таңдау** бетінде жобаның аға менеджері рөлі үшін бұрын орнатқан сипаттамалар әдепкі бойынша таңдалады.</span><span class="sxs-lookup"><span data-stu-id="624ed-132">On the **Choose characteristics** page, the characteristics that you previously set for the Senior project manager role are selected by default.</span></span> <span data-ttu-id="624ed-133">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-133">Select **OK**.</span></span>
7. <span data-ttu-id="624ed-134">**Жобаға рөлдер қосу** бетіндегі **Ресурстар саны** өрісіне **1** мәнін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="624ed-134">On the **Add roles to project** page, in the **Number of resources** field, enter **1**.</span></span>
8. <span data-ttu-id="624ed-135">**Ресурс** өрісінде іздеу тармағы қажетті құзыреттіліктерді қамтитын барлық ресурстарды көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="624ed-135">In the **Resource** field, the lookup shows all resources that have the required competencies.</span></span> <span data-ttu-id="624ed-136">**Даниэль Гольдшмидт**, содан кейін **Жасау** параметрлерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-136">Select **Daniel Goldschmidt**, and then select **Create**.</span></span>
9. <span data-ttu-id="624ed-137">**Жоба** бетінде **Қосу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-137">On the **Project** page, select **Add**.</span></span>
10. <span data-ttu-id="624ed-138">**Жобаға рөлдер қосу** тақтасындағы **Рөл** өрісінде **Топ мүшесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-138">In the **Add roles to the project** pane, in the **Role** field, select **Team member**.</span></span> <span data-ttu-id="624ed-139">**Ресурстар саны** өрісіне **5** мәнін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="624ed-139">In the **Number of resources** field, enter **5**.</span></span>
11. <span data-ttu-id="624ed-140">**Жасау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-140">Select **Create**.</span></span>
12. <span data-ttu-id="624ed-141">**Жобалар** бетінен **Ресурсты орындау** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-141">On the **Projects** page, select **Fulfill resource**.</span></span>

## <a name="monitor-project-teams"></a><span data-ttu-id="624ed-142">Жоба топтарын бақылау</span><span class="sxs-lookup"><span data-stu-id="624ed-142">Monitor project teams</span></span>
1. <span data-ttu-id="624ed-143">**Барлық жобалар** бетінен **XYZ жаңартуының 2-кезеңі** жобасына арналған **Жоба идентификаторы** таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="624ed-143">On the **All projects** page, select the **Project ID** link for the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="624ed-144">**Жоба тобы және жоспарлау** FastTab ішінде тізімделген жоба ресурстарының дұрыстығын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="624ed-144">On the **Project team and scheduling** FastTab, verify that the project resources that are listed are correct.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]