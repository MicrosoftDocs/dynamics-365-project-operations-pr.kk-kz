---
title: Сіздегі орналастыру түрін анықтау
description: Бұл тақырыпта компанияңыздың жоба операцияларының тиісті орналастыру түрін анықтауға көмектесу үшін ақпарат береді.
author: stsporen
manager: Annbe
ms.date: 03/15/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 1aae04230104d27db2f62db8e674697fd83460ac
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948113"
---
# <a name="determine-your-deployment-type"></a><span data-ttu-id="b7294-103">Сіздегі орналастыру түрін анықтау</span><span class="sxs-lookup"><span data-stu-id="b7294-103">Determine your deployment type</span></span>

<span data-ttu-id="b7294-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="b7294-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b7294-105">Лицензияны сатып алғаннан кейін, [Қадамдық орнату ағыны](https://aka.ms/provisionprojectoperations) арқылы Dynamics 365 Project Operations ең жақсы орналастыру үлгісін анықтау үшін осы жерден бастаңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-105">After you purchase the license, start here to determine the best deployment model of Dynamics 365 Project Operations using the [Guided installation flow](https://aka.ms/provisionprojectoperations).</span></span>
> <span data-ttu-id="b7294-106">Басқарылатын орнату ағынын аяқтағаннан кейін орнатуды аяқтау үшін тиісті басқару порталына бағытталасыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-106">After you have finshed the Guided installation flow, you will be directed to the correct management portal to complete your installation.</span></span> <span data-ttu-id="b7294-107">Орнатуды аяқтау үшін орналастыру мәліметтерін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-107">See the deployment details to complete the installation.</span></span>


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a><span data-ttu-id="b7294-108">Dynamics 365 Project Service Automation арқылы Dynamics жүйесінің бар тұтынушылары</span><span class="sxs-lookup"><span data-stu-id="b7294-108">Existing customers of Dynamics using Dynamics 365 Project Service Automation</span></span>
<span data-ttu-id="b7294-109">Project Operations жүйесі Project Service Automation көмегімен жеткізілген мүмкіндіктерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="b7294-109">Project Operations includes the capabilities that shipped with Project Service Automation.</span></span> <span data-ttu-id="b7294-110">2021 жылдың 1-толқынында тұтынушылар үшін жаңарту жолы шығарылады.</span><span class="sxs-lookup"><span data-stu-id="b7294-110">An upgrade path will be released for these customers in the 2021 release wave 1.</span></span>

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a><span data-ttu-id="b7294-111">Жобалық басқару және есеп бойынша Dynamics 365 Finance бар тұтынушылары</span><span class="sxs-lookup"><span data-stu-id="b7294-111">Existing customers of Dynamics 365 Finance using Project management and accounting</span></span> 

<span data-ttu-id="b7294-112">Жобалық басқару және есеп мүмкіндіктерін пайдаланатын Finance бағдарламасының бұрыннан бар тұтынушылары оны сол күйінде пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="b7294-112">Existing customers of Finance who use the Project management and accounting functionality can continue to use it as is.</span></span> <span data-ttu-id="b7294-113">[Қосалқы/өндіріс тапсырысы сценарийлеріне арналған Project Operations](#pma) қараңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-113">See [Project Operations for stocked/production order scenarios](#pma).</span></span>


## <a name="deployment-regions"></a><span data-ttu-id="b7294-114">Орналастыру аймақтары</span><span class="sxs-lookup"><span data-stu-id="b7294-114">Deployment regions</span></span>
<span data-ttu-id="b7294-115">Project Operations бағдарламасын орналастыруға қолдау көрсететін аймақтарды анықтау үшін [Dynamics 365 және Power Platform есебіне арналған географиялық қолжетімділік](https://dynamics.microsoft.com/en-us/geographic-availability/) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-115">To determine which regions support Project Operations deployment, see [Geographical availability for Dynamics 365 and Power Platform report](https://dynamics.microsoft.com/en-us/geographic-availability/).</span></span> <span data-ttu-id="b7294-116">**Есепті қарау** параметрін таңдап, қолдау көрсетілетін аймақтарды көру үшін **Dynamics 365> Operations бағдарламалары > Dynamics 365 Project Operations** тармағын кеңейтіңіз.</span><span class="sxs-lookup"><span data-stu-id="b7294-116">Select **View Report**, and expand **Dynamics 365 > Operations Apps > Dynamics 365 Project Operations** to view the supported regions.</span></span>

## <a name="deployment-types"></a><span data-ttu-id="b7294-117">Орналастыру түрлері</span><span class="sxs-lookup"><span data-stu-id="b7294-117">Deployment types</span></span>
<span data-ttu-id="b7294-118">Project Operations сіздің қажеттіліктеріңізге сәйкес бірнеше орналастыру нұсқаларын қолдайды.</span><span class="sxs-lookup"><span data-stu-id="b7294-118">Project Operations supports multiple deployment options to match your requirements.</span></span> <span data-ttu-id="b7294-119">Сіз Dynamics 365 жаңа немесе қолданыстағы тұтынушысы болсаңыз да, Project Operations сіздің қажеттіліктеріңізді қолдай алады.</span><span class="sxs-lookup"><span data-stu-id="b7294-119">Whether you're a new or existing Dynamics 365 customer, Project Operations can support your needs.</span></span>

<span data-ttu-id="b7294-120">Біздің[ Орналастыруға арналған сауалнама](https://aka.ms/provisionprojectoperations) дұрыс орналастыруды анықтауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="b7294-120">Our [Deployment questionnaire](https://aka.ms/provisionprojectoperations) will help you determine the right deployment.</span></span> <span data-ttu-id="b7294-121">Нәтижелер сізді келесі орналастыру түрлеріне бағыттайды:</span><span class="sxs-lookup"><span data-stu-id="b7294-121">The results will guide you toward one of the following deployment types:</span></span>

- [<span data-ttu-id="b7294-122">Жеңілдетілген орналастыру – проформа-шотын ұсыну мәмілесі</span><span class="sxs-lookup"><span data-stu-id="b7294-122">Lite deployment – deal to proforma invoicing</span></span>](#lite)
- [<span data-ttu-id="b7294-123">Ресурс/биржадан тыс сценарийлерге арналған Project Operations</span><span class="sxs-lookup"><span data-stu-id="b7294-123">Project Operations for resource/non-stocked scenarios</span></span>](#integrated)
- [<span data-ttu-id="b7294-124">Қосалқы/өндіріс тапсырысы сценарийлеріне арналған Project Operations</span><span class="sxs-lookup"><span data-stu-id="b7294-124">Project Operations for stocked/production order scenarios</span></span>](#pma)

<span data-ttu-id="b7294-125">Project Operations заңды тұлға деңгейіндегі конфигурациялар арқылы бір ортада қосалқы/өндіріс тапсырыстың сценарийлерін және қосалқы емес/ресурстарға негізделген сценарийлерді қолдайды.</span><span class="sxs-lookup"><span data-stu-id="b7294-125">Project Operations support stocked/production order scenarios and non-stocked/resource-based scenarios on the same environment through legal entity-level configurations.</span></span> <span data-ttu-id="b7294-126">Мысалы, Contoso қосалқы/өндірістік тапсырыстың мүмкіндіктерін АҚШ-тың өндірістік мекемесінде пайдалана алады (заңды тұлға = Contoso Америка Құрама Штаттарындағы өндірістік мекемесі).</span><span class="sxs-lookup"><span data-stu-id="b7294-126">For example, Contoso can use the stocked/production order capabilities in their US manufacturing facility (Legal entity = Contoso Manufacturing United States).</span></span> <span data-ttu-id="b7294-127">Contoso қосалқы емес/ресурстарға негізделген мүмкіндіктерді Contoso Ұлыбританиядағы Robotics Arms қызмет көрсететін мекемеде (заңды тұлға = Contoso Robotics, Ұлыбритания) пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="b7294-127">Contoso can use the non-stocked/resource-based capabilities in their Contoso Robotics Arms servicing facility in UK (Legal entity = Contoso Robotics United Kingdom).</span></span>

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a><span data-ttu-id="b7294-128">Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі</span><span class="sxs-lookup"><span data-stu-id="b7294-128">Lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="b7294-129">Қарапайым орналастыру келесі мүмкіндіктерді қамтиды:</span><span class="sxs-lookup"><span data-stu-id="b7294-129">The lite deployment includes the following capabilities:</span></span>

- <span data-ttu-id="b7294-130">Dynamics 365 Sales бағдарламасының тәжірибелерін кеңейтетін жобалардың сату үрдісі</span><span class="sxs-lookup"><span data-stu-id="b7294-130">Sales process for projects that extends Dynamics 365 Sales application experiences</span></span>
- <span data-ttu-id="b7294-131">Вебке арналған Microsoft Project жобасын жоспарлау</span><span class="sxs-lookup"><span data-stu-id="b7294-131">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="b7294-132">Көпөлшемді баға белгілеу</span><span class="sxs-lookup"><span data-stu-id="b7294-132">Multi-dimensional pricing</span></span>
- <span data-ttu-id="b7294-133">Бірыңғай ресурстық басқару</span><span class="sxs-lookup"><span data-stu-id="b7294-133">Unified resource management</span></span>
- <span data-ttu-id="b7294-134">Уақытты бақылау</span><span class="sxs-lookup"><span data-stu-id="b7294-134">Time tracking</span></span>
- <span data-ttu-id="b7294-135">Негізгі шығыс</span><span class="sxs-lookup"><span data-stu-id="b7294-135">Basic expense</span></span>
- <span data-ttu-id="b7294-136">Жоба менеджерінің шолуы мен өңдеуі үшін арналған проформа шоты</span><span class="sxs-lookup"><span data-stu-id="b7294-136">Proforma invoicing for Project manager's review and edits</span></span> 

#### <a name="deployment-steps"></a><span data-ttu-id="b7294-137">Орналастыру қадамдары</span><span class="sxs-lookup"><span data-stu-id="b7294-137">Deployment steps</span></span>
<span data-ttu-id="b7294-138">[Орналастыру бойынша сауалнама](https://aka.ms/provisionprojectoperations) көмегімен Project Operations жүйесінің ең тиімді орналастыру үлгісін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-138">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="b7294-139">Бұл орналастыру үшін [Алдын ала қарау жазылымдарына арналған тіркелу](lite-preview-subscription-sign-up.md) және [Жаңа ортаны дайындау](lite-deployment.md) бөлімдерін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-139">For this deployment, see [Sign-up for preview subscriptions](lite-preview-subscription-sign-up.md) and [Provision new environment](lite-deployment.md).</span></span> 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a><span data-ttu-id="b7294-140">Ресурс/биржадан тыс сценарийлерге арналған Project Operations</span><span class="sxs-lookup"><span data-stu-id="b7294-140">Project Operations for resource/non-stocked scenarios</span></span>
<span data-ttu-id="b7294-141">Ресурстық/қосалқы емес сценарийлерге арналған Project Operations жүйесі келесі мүмкіндіктерді қамтиды:</span><span class="sxs-lookup"><span data-stu-id="b7294-141">The Project Operations for resource/non-stocked scenarios includes the following capabilities:</span></span>
 
- <span data-ttu-id="b7294-142">Dynamics 365 Sales бағдарламасын кеңейтетін жобалардың сату үрдісі</span><span class="sxs-lookup"><span data-stu-id="b7294-142">Sales process for projects that extends the Dynamics 365 Sales application</span></span>
- <span data-ttu-id="b7294-143">Вебке арналған Microsoft Project жобасын жоспарлау</span><span class="sxs-lookup"><span data-stu-id="b7294-143">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="b7294-144">Көпөлшемді баға белгілеу</span><span class="sxs-lookup"><span data-stu-id="b7294-144">Multi-dimensional pricing</span></span>
- <span data-ttu-id="b7294-145">Бірыңғай ресурстық басқару</span><span class="sxs-lookup"><span data-stu-id="b7294-145">Unified resource management</span></span>
- <span data-ttu-id="b7294-146">Уақытты бақылау</span><span class="sxs-lookup"><span data-stu-id="b7294-146">Time tracking</span></span>
- <span data-ttu-id="b7294-147">Негізгі шығыс</span><span class="sxs-lookup"><span data-stu-id="b7294-147">Basic expense</span></span>
- <span data-ttu-id="b7294-148">Толық шығыс</span><span class="sxs-lookup"><span data-stu-id="b7294-148">Full expense</span></span>
- <span data-ttu-id="b7294-149">ТҚР түбіртегі</span><span class="sxs-lookup"><span data-stu-id="b7294-149">Receipt OCR</span></span>
- <span data-ttu-id="b7294-150">Проформа және тұтынушыға арналған шот-фактуралар</span><span class="sxs-lookup"><span data-stu-id="b7294-150">Proforma and customer-facing invoicing</span></span> 
- <span data-ttu-id="b7294-151">Жобалар бойынша табысты тану</span><span class="sxs-lookup"><span data-stu-id="b7294-151">Revenue recognition for projects</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="b7294-152">Орналастыру қадамдары</span><span class="sxs-lookup"><span data-stu-id="b7294-152">Deployment steps</span></span>
<span data-ttu-id="b7294-153">[Орналастыру бойынша сауалнама](https://aka.ms/provisionprojectoperations) көмегімен Project Operations жүйесінің ең тиімді орналастыру үлгісін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-153">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="b7294-154">Бұл орналастыру үшін [Алдын ала қарау жазылымдарына арналған тіркелу](resource-sign-up-preview-subscription.md) және [Жаңа ортаны дайындау](resource-provision-new-environment.md) бөлімдерін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-154">For this deployment, see [Sign-up for preview subscriptions](resource-sign-up-preview-subscription.md) and [Provision new environment](resource-provision-new-environment.md).</span></span> 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a><span data-ttu-id="b7294-155">Қосалқы/өндіріс тапсырысы сценарийлеріне арналған Project Operations</span><span class="sxs-lookup"><span data-stu-id="b7294-155">Project Operations for stocked/production order scenarios</span></span>

- <span data-ttu-id="b7294-156">WBS бойынша жобаны жоспарлау</span><span class="sxs-lookup"><span data-stu-id="b7294-156">Project planning using WBS</span></span>
- <span data-ttu-id="b7294-157">Ресурстарды басқару</span><span class="sxs-lookup"><span data-stu-id="b7294-157">Resource management</span></span>
- <span data-ttu-id="b7294-158">Уақытты бақылау</span><span class="sxs-lookup"><span data-stu-id="b7294-158">Time tracking</span></span>
- <span data-ttu-id="b7294-159">Толық шығыс</span><span class="sxs-lookup"><span data-stu-id="b7294-159">Full expense</span></span>
- <span data-ttu-id="b7294-160">ТҚР түбіртегі</span><span class="sxs-lookup"><span data-stu-id="b7294-160">Receipt OCR</span></span>
- <span data-ttu-id="b7294-161">Толық шот-фактура</span><span class="sxs-lookup"><span data-stu-id="b7294-161">Full invoicing</span></span>
- <span data-ttu-id="b7294-162">Табысты тану</span><span class="sxs-lookup"><span data-stu-id="b7294-162">Revenue recognition</span></span>
- <span data-ttu-id="b7294-163">Өндірістік тапсырыстар</span><span class="sxs-lookup"><span data-stu-id="b7294-163">Production orders</span></span>
- <span data-ttu-id="b7294-164">Қойма қамтамасыз етілген қосалқы материалдар</span><span class="sxs-lookup"><span data-stu-id="b7294-164">Stocked materials support with inventory</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="b7294-165">Орналастыру қадамдары</span><span class="sxs-lookup"><span data-stu-id="b7294-165">Deployment steps</span></span>
<span data-ttu-id="b7294-166">[Орналастыру бойынша сауалнама](https://aka.ms/provisionprojectoperations) көмегімен Project Operations жүйесінің ең тиімді орналастыру үлгісін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-166">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="b7294-167">Бұл орналастыру үшін [Алдын ала қарау жазылымдарына арналған тіркелу](/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=%2fdynamics365%2ffinance%2ftoc.json) және [Жаңа ортаны дайындау](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=%2fdynamics365%2ffinance%2ftoc.json) бөлімдерін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="b7294-167">For this deployment, see [Sign-up for preview subscriptions](/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=%2fdynamics365%2ffinance%2ftoc.json) and [Provision new environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=%2fdynamics365%2ffinance%2ftoc.json).</span></span> 



[!INCLUDE[footer-include](../includes/footer-banner.md)]