---
title: Қауіпсіздік үлгісі
description: Бұл тақырып Dynamics 365 Project Operations жүйесіндегі қауіпсіздік үлгісі туралы ақпарат береді.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 3f65d13809fef342be8bec682c11d95c4d9e9b19
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276805"
---
# <a name="security-model"></a><span data-ttu-id="55832-103">Қауіпсіздік үлгісі</span><span class="sxs-lookup"><span data-stu-id="55832-103">Security Model</span></span>

<span data-ttu-id="55832-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="55832-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="55832-105">Microsoft Dynamics 365 Project Operations бағдарламасы Microsoft Office топтарымен бірге жұмыс істейтін рөлге негізделген бизнес-қауіпсіздік үлгісіне мүмкіндік беретін бірегей қауіпсіздік үлгісін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="55832-105">Microsoft Dynamics 365 Project Operations contains a unique security model that allows for a role-based business security model that collaborates with Microsoft Office Groups.</span></span> 


## <a name="security-roles"></a><span data-ttu-id="55832-106">Қауіпсіздік рөлдері</span><span class="sxs-lookup"><span data-stu-id="55832-106">Security roles</span></span>
<span data-ttu-id="55832-107">Project Operations жүйесінің алдыңғы мүмкіндіктері келесі рөлдерді қамтиды:</span><span class="sxs-lookup"><span data-stu-id="55832-107">Project Operations front-end capabilities include the following roles:</span></span>

| <span data-ttu-id="55832-108">Рөл</span><span class="sxs-lookup"><span data-stu-id="55832-108">Role</span></span>                          | <span data-ttu-id="55832-109">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="55832-109">Description</span></span>                                                                                                                                                                 | <span data-ttu-id="55832-110">Scope</span><span class="sxs-lookup"><span data-stu-id="55832-110">Scope</span></span> |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| <span data-ttu-id="55832-111">Тәжірибе басқарушысы</span><span class="sxs-lookup"><span data-stu-id="55832-111">Practice manager</span></span>              | <span data-ttu-id="55832-112">Жобааралық есеп беруді қолдайды.</span><span class="sxs-lookup"><span data-stu-id="55832-112">Supports cross-project reporting.</span></span>                                                                                                            | <span data-ttu-id="55832-113">Бөлімше</span><span class="sxs-lookup"><span data-stu-id="55832-113">Business unit</span></span>              |
| <span data-ttu-id="55832-114">Жоба бекітушісі</span><span class="sxs-lookup"><span data-stu-id="55832-114">Project approver</span></span>              | <span data-ttu-id="55832-115">Жоба бойынша уақытты және шығыстарды бекітеді.</span><span class="sxs-lookup"><span data-stu-id="55832-115">Approves time and expenses against a project.</span></span>                                                                                                                              | <span data-ttu-id="55832-116">Бөлімше</span><span class="sxs-lookup"><span data-stu-id="55832-116">Business unit</span></span> |
| <span data-ttu-id="55832-117">Жобаны ұсынатын әкімші</span><span class="sxs-lookup"><span data-stu-id="55832-117">Project billing administrator</span></span> | <span data-ttu-id="55832-118">Шот-фактура ұсынысын жасайды.</span><span class="sxs-lookup"><span data-stu-id="55832-118">Creates the invoice proposal.</span></span>                                                                                                                                                 | <span data-ttu-id="55832-119">Бөлімше</span><span class="sxs-lookup"><span data-stu-id="55832-119">Business unit</span></span> |
| <span data-ttu-id="55832-120">Жоба менеджері</span><span class="sxs-lookup"><span data-stu-id="55832-120">Project manager</span></span>               | <span data-ttu-id="55832-121">Жоба жоспарын жасайды және ресурстарға сұраныс жасайды.</span><span class="sxs-lookup"><span data-stu-id="55832-121">Creates the project plan and requests resources.</span></span>                                                                                                                              | <span data-ttu-id="55832-122">Бөлімше</span><span class="sxs-lookup"><span data-stu-id="55832-122">Business unit</span></span> |
| <span data-ttu-id="55832-123">Жоба ресурсы</span><span class="sxs-lookup"><span data-stu-id="55832-123">Project resource</span></span>              | <span data-ttu-id="55832-124">Тапсырыс беруге болатын және уақыт туралы есеп беретін топ мүшелері.</span><span class="sxs-lookup"><span data-stu-id="55832-124">Team members who can be booked and report time.</span></span>                                                                                                          | <span data-ttu-id="55832-125">Бөлімше</span><span class="sxs-lookup"><span data-stu-id="55832-125">Business unit</span></span>|
| <span data-ttu-id="55832-126">Ресурс менеджері</span><span class="sxs-lookup"><span data-stu-id="55832-126">Resource manager</span></span>              | <span data-ttu-id="55832-127">Ресурстарды басқарудың барлық функциялары, мысалы, гибридті жоба менеджері + Ресурс менеджерінің конфигурациясы және бірыңғай және орталықтандырылған Ресурстар менеджері рөлін қолдау үшін бөлінген ресурстық сұраныстар мен тапсырыс беруді орындау.</span><span class="sxs-lookup"><span data-stu-id="55832-127">All resource management functions, such as fulfill resource requests and bookings, separated to support a hybrid Project manager + Resource manager configuration and a single and centralized Resource manager role.</span></span> | <span data-ttu-id="55832-128">Бөлімше</span><span class="sxs-lookup"><span data-stu-id="55832-128">Business unit</span></span> |


<span data-ttu-id="55832-129">Интернетке арналған Microsoft Project келесі рөлдерді қамтиды:</span><span class="sxs-lookup"><span data-stu-id="55832-129">Microsoft Project for the Web includes the following roles:</span></span>

| <span data-ttu-id="55832-130">Рөл</span><span class="sxs-lookup"><span data-stu-id="55832-130">Role</span></span>           | <span data-ttu-id="55832-131">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="55832-131">Description</span></span>                                                                                                        | <span data-ttu-id="55832-132">Scope</span><span class="sxs-lookup"><span data-stu-id="55832-132">Scope</span></span>  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| <span data-ttu-id="55832-133">Жоба пайдаланушысы</span><span class="sxs-lookup"><span data-stu-id="55832-133">Project user</span></span>   | <span data-ttu-id="55832-134">Өз жобаларын жасауға және олармен бөліскен кез келген жобаларды көруге қабілетті жобаның бірлескен пайдаланушысы.</span><span class="sxs-lookup"><span data-stu-id="55832-134">Collaborative user of Project   who is able to create their own projects and view any projects shared with   them.</span></span> | <span data-ttu-id="55832-135">Пайдаланушы</span><span class="sxs-lookup"><span data-stu-id="55832-135">User</span></span>   |
| <span data-ttu-id="55832-136">Жоба жүйесі</span><span class="sxs-lookup"><span data-stu-id="55832-136">Project system</span></span> | <span data-ttu-id="55832-137">Бағдарлама контекстінде пайдаланылатын рөл.</span><span class="sxs-lookup"><span data-stu-id="55832-137">Role used for application   context.</span></span> <span data-ttu-id="55832-138">Тұтынушылар бұл жүйенің рөлін пайдаланбауы тиіс.</span><span class="sxs-lookup"><span data-stu-id="55832-138">Customers should not use this system role.</span></span>                                    | <span data-ttu-id="55832-139">Глобалдық</span><span class="sxs-lookup"><span data-stu-id="55832-139">Global</span></span> |

## <a name="security-enforcement"></a><span data-ttu-id="55832-140">Қауіпсіздікті қамтамасыз ету</span><span class="sxs-lookup"><span data-stu-id="55832-140">Security enforcement</span></span>
<span data-ttu-id="55832-141">Жоба деңгейінде орындалатын әрекеттер кірген пайдаланушының контекстінде орындалады.</span><span class="sxs-lookup"><span data-stu-id="55832-141">Actions that are performed at the project level are performed in the context of the logged in user.</span></span> <span data-ttu-id="55832-142">Бұл дегеніміз, жобаны құру, ашу немесе жою үшін пайдаланушыға CDS қызметінде қолжетімділік қажет.</span><span class="sxs-lookup"><span data-stu-id="55832-142">This means that in order to create, open, or delete a project, the user is required to have access available in CDS.</span></span> <span data-ttu-id="55832-143">CDS қызметіне қолжетімділік платформаға енгізілген кез келген мүмкін механизмдер арқылы берілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="55832-143">Access in CDS may be granted through any of the possible mechanisms included in the platform.</span></span> <span data-ttu-id="55832-144">Мысалы, егер пайдаланушыға рұқсат беретін нақты жобаны бөлісу әрекеті орындалса, ауқымы кеңірек пайдаланушы жобаға кіре алады.</span><span class="sxs-lookup"><span data-stu-id="55832-144">For example, a user with a larger scope may access the project or if an explicit project share action has been performed which grants the user access.</span></span>

<span data-ttu-id="55832-145">Project Operations жүйесінде жобаларды жасау кезінде осыны ескеру маңызды.</span><span class="sxs-lookup"><span data-stu-id="55832-145">It's important to consider this when creating projects in Project Operations.</span></span>

## <a name="modern-group-collaboration-with-project-operations"></a><span data-ttu-id="55832-146">Project Operations жүйесімен заманауи топтық бірлескен жұмыс</span><span class="sxs-lookup"><span data-stu-id="55832-146">Modern group collaboration with Project Operations</span></span>
<span data-ttu-id="55832-147">Вебке арналған жоба және Project Operations бірге жұмыс істеу үшін заманауи топтарды қолдайды.</span><span class="sxs-lookup"><span data-stu-id="55832-147">Project for the Web and Project Operations support modern groups for collaboration.</span></span> <span data-ttu-id="55832-148">Топ арқылы жобаға қосылған пайдаланушылар жоба жоспарын өңдей алады.</span><span class="sxs-lookup"><span data-stu-id="55832-148">Users added to the project through a group are able to edit the project plan.</span></span>

<span data-ttu-id="55832-149">Вебке арналған жоба тағайындалған кезде пайдаланушыларды автоматты түрде топқа қосады.</span><span class="sxs-lookup"><span data-stu-id="55832-149">Project for the Web adds users to the group automatically upon assignment.</span></span>

<span data-ttu-id="55832-150">Топтар жобаның рұқсаттарын және бірлескен артефактілерді бірлесіп өңдеуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="55832-150">Groups allow the permissions of the project and supporting collaboration artifacts to be worked on collaboratively.</span></span> <span data-ttu-id="55832-151">Төмендегі диаграмма топтарды тағайындау кезінде болатын оқиғалар мен күйлерді бейнелейді.</span><span class="sxs-lookup"><span data-stu-id="55832-151">The following diagram depicts the events and state changes that happen during the group assignment process.</span></span>

<span data-ttu-id="55832-152">Project Operations жүйесі топты жасырын әрекеттер арқылы жасамайды және тек басу топтарының айқын әрекеті арқылы жасайды.</span><span class="sxs-lookup"><span data-stu-id="55832-152">Project Operations does not create a group through implicit action and only does so through the explicit action of pressing groups.</span></span>

<span data-ttu-id="55832-153">**Топты басқару** диалогтік терезесіндегі топ мүшесі ортаның қауіпсіздік тобының бөлігі ретінде белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="55832-153">Group member search in the **Group management** dialog, is limited to those who are set as part of the environment's security group.</span></span> <span data-ttu-id="55832-154">Қосымша ақпаратты [Пайдаланушының орталарға қатынасын басқарыңыз: қауіпсіздік топтары және лицензиялар](https://docs.microsoft.com/power-platform/admin/control-user-access) бөлімінде қараңыз.</span><span class="sxs-lookup"><span data-stu-id="55832-154">For more information, see [Control user access to environments: security groups and licenses](https://docs.microsoft.com/power-platform/admin/control-user-access).</span></span>

![Топ режимі](./media/groupsmode.png)

1. <span data-ttu-id="55832-156">Жоба жасалған және жасаушы пайдаланушыға тиесілі.</span><span class="sxs-lookup"><span data-stu-id="55832-156">The Project is created and owned by the creating User.</span></span>
2. <span data-ttu-id="55832-157">Жоба иесі топқа жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="55832-157">The Project owner is updated to the team.</span></span>
3. <span data-ttu-id="55832-158">Иеленуші топ көрсетілген немесе жасалған Office тобымен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="55832-158">The Owner team is mapped to the specified or created Office Group.</span></span>
4. <span data-ttu-id="55832-159">Жобаның негізгі иесі Office тобына қосылды.</span><span class="sxs-lookup"><span data-stu-id="55832-159">The original owner of the Project is added to the Office Group.</span></span>

## <a name="deployment-recommendation"></a><span data-ttu-id="55832-160">Орналастыру ұсынысы</span><span class="sxs-lookup"><span data-stu-id="55832-160">Deployment recommendation</span></span>
<span data-ttu-id="55832-161">Office тобының бірлесіп жұмыс істеу үлгісі дамып келе жатқанда, уақыт өте келе толығырақ бақылауды қамтамасыз ететін функционалдылық қосылады.</span><span class="sxs-lookup"><span data-stu-id="55832-161">As the Office group collaboration model evolves, functionality will be added to provide more detailed control over time.</span></span> <span data-ttu-id="55832-162">Project Operations жүйесін орналастыратын тұтынушыларға бүгінгі таңда Microsoft Dynamics 365 дәстүрлі қауіпсіздік үлгісіне назар аудару ұсынылады.</span><span class="sxs-lookup"><span data-stu-id="55832-162">Customers that deploy Project Operations today are encouraged to focus on a traditional Microsoft Dynamics 365 security model.</span></span>

<span data-ttu-id="55832-163">Толығырақ ақпарат алу үшін [Common Data Service қызметіндегі қауіпсіздік](https://docs.microsoft.com/power-platform/admin/wp-security) тақырыбын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="55832-163">For more information, see [Security in Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).</span></span>

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a><span data-ttu-id="55832-164">Project Operations және Microsoft Dynamics 365 Finance қауіпсіздігі</span><span class="sxs-lookup"><span data-stu-id="55832-164">Project Operations and Microsoft Dynamics 365 Finance security</span></span>
<span data-ttu-id="55832-165">Project Operations келесі рөлдерді қамтиды:</span><span class="sxs-lookup"><span data-stu-id="55832-165">Project Operations includes the following roles:</span></span>

- <span data-ttu-id="55832-166">Жоба менеджері</span><span class="sxs-lookup"><span data-stu-id="55832-166">Project manager</span></span>
- <span data-ttu-id="55832-167">Жоба бухгалтері</span><span class="sxs-lookup"><span data-stu-id="55832-167">Project accountant</span></span>

<span data-ttu-id="55832-168">Finance бөліміндегі қауіпсіздік туралы қосымша ақпаратты мына жерден қараңыз[Рөлдік қауіпсіздік](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span><span class="sxs-lookup"><span data-stu-id="55832-168">For more information about security in Finance, see [Role-based security](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]