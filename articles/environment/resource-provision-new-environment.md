---
title: Жаңа ортаны дайындау
description: Бұл тақырып жаңа Project Operations ортасын дайындау туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 45700371c50e3b5a840df45fc24fa8a5b4584b61
ms.sourcegitcommit: 87b7a8d793c19c50f3765b8d788cde24a6a0ca24
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949369"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="7c0e6-103">Жаңа ортаны дайындау</span><span class="sxs-lookup"><span data-stu-id="7c0e6-103">Provision a new environment</span></span>

<span data-ttu-id="7c0e6-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="7c0e6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="7c0e6-105">Бұл тақырып ресурстарға/қосалқы емес негіздегі сценарийлер үшін жаңа Dynamics 365 Project Operations ортасын дайындау жолы туралы ақпарат береді.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="7c0e6-106">LCS жобасында Project Operations автоматтандырылған дайындық жүргізу процесін қосу</span><span class="sxs-lookup"><span data-stu-id="7c0e6-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="7c0e6-107">LCS жобаңыздың Project Operations автоматтандырылған дайындық жүргізу ағынына қосу үшін келесі қадамдарды пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="7c0e6-108">[LCS](https://lcs.dynamics.com/v2) параметріне өтіп, **Мүмкіндіктерді басқаруды алдын-ала қарау** тақтасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="7c0e6-109">**Алдын ала қарау мүмкіндігі** тізімінде Project Operations жүйесін қосу үшін **Project Operations** және **Алдын ала қарау мүмкіндігі қосылды** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-109">In the **Preview feature** list, select **Project Operations** and the select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="7c0e6-110">Бұл қадам әрбір LCS жобасында тек бір рет орындалады.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="7c0e6-111">Project Operations ортасын дайындау</span><span class="sxs-lookup"><span data-stu-id="7c0e6-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="7c0e6-112">Жаңа Dynamics 365 Finance [демо-ортасын](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) немесе [сынақ ортасы/өндіріс ортасы](https://docs.microsoft.com/edynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) орналастыруын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/edynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="7c0e6-113">**Ортаны дайындау** шебері арқылы өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="7c0e6-114">Бағдарламаның таңдалған нұсқасының 10.0.13 немесе одан жоғары екендігіне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="7c0e6-115">Project Operations дайындау үшін **Кеңейтілген параметрлер** тармағында **Common Data Service** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="7c0e6-116">**Иә** опциясын таңдау арқылы **Common Data Service параметрін** қосып, содан соң қажетті өрістерде ақпарат енгізіңіз:</span><span class="sxs-lookup"><span data-stu-id="7c0e6-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="7c0e6-117">Атауы</span><span class="sxs-lookup"><span data-stu-id="7c0e6-117">Name</span></span>
  - <span data-ttu-id="7c0e6-118">Өңір</span><span class="sxs-lookup"><span data-stu-id="7c0e6-118">Region</span></span>
  - <span data-ttu-id="7c0e6-119">Тіл</span><span class="sxs-lookup"><span data-stu-id="7c0e6-119">Language</span></span>
  - <span data-ttu-id="7c0e6-120">Валюта</span><span class="sxs-lookup"><span data-stu-id="7c0e6-120">Currency</span></span>
 
5. <span data-ttu-id="7c0e6-121">**Common Data Service үлгісі** өрісінде **Project Operations** опциясын таңдаңыз</span><span class="sxs-lookup"><span data-stu-id="7c0e6-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="7c0e6-122">Орналастыру үшін орта түрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="7c0e6-123">Жазылымға негізделген сынақ CDS ортасын 30 күн ішінде пайдалануға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Орналастыру параметрлері](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="7c0e6-125">Қызмет көрсету шарттарын растау үшін **Келісу** опциясын таңдаңыз, содан кейін орналастыру параметрлеріне оралу үшін **Дайын** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Орналастыру келісімі](./media/2DeploymentConsent.png)

7. <span data-ttu-id="7c0e6-127">Шебердегі қалған қажетті өрістерді толтырыңыз және орналастыруды растаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="7c0e6-128">Ортаны дайындау уақыты ортаның түріне байланысты өзгеріп отырады.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="7c0e6-129">Дайындау алты сағатқа созылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="7c0e6-130">Орналастыру сәтті аяқталғаннан кейін, орта келесідей болады: **Орналастырылған**.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="7c0e6-131">Ортаның сәтті түрде орналастырылуын растау үшін **Жүйеге кіру** опциясын таңдап, растау үшін ортаға кіріңіз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![ ортасының мәліметтері](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="7c0e6-133">Project Operations Finance демо-деректерін қолдану (міндетті емес қадам)</span><span class="sxs-lookup"><span data-stu-id="7c0e6-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="7c0e6-134">Apply Project Operations Finance демо-деректерін [осы мақалада](resource-apply-finance-demo-data.md) сипатталғандай 10.0.13 қызмет шығарылымының бұлт қызметтеріне орналастырылған ортаға қолданыңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="7c0e6-135">Finance ортасына жаңартуларды қолдану</span><span class="sxs-lookup"><span data-stu-id="7c0e6-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="7c0e6-136">Project Operations жүйесі бағдарлама нұсқасының **10.0.13 (10.0.569.20009)** немесе одан жоғары нұсқасымен Finance ортасын қажет етеді.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="7c0e6-137">Бұл нұсқаны алу үшін Finance ортасына сапалық жаңартуларды қолдану қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="7c0e6-138">LCS қызметіндегі **Орта туралы мәліметтер** бетінде, **Қол жетімді жаңартулар** бөлімінде **Жаңартуды қарау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Жаңартуларды қарау](./media/5ViewUpdates.png)

2. <span data-ttu-id="7c0e6-140">**Екілік жаңартулар** бетінде **Буманы сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-140">On the **Binary updates** page, select **Save package.**</span></span>

![Буманы сақтау](./media/6SavePackage.png)

3. <span data-ttu-id="7c0e6-142">**Барлығын таңдау** түймешігін басып, содан соң **Буманы сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-142">Click **Select all** and then select **Save package**.</span></span>

![Жаңартуларды қарап шығу және сақтау](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="7c0e6-144">Буманың атауын және сипаттамасын енгізіп, содан кейін **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="7c0e6-145">Интернет қосылымына байланысты осы процесс ол біраз уақыт алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-145">Depending on the internet connection, this process might take some time.</span></span>

![Буманы активтер кітапханасына жүктеу](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="7c0e6-147">Бума сақталғаннан кейін **Дайын** опциясын таңдап, осы буманы LCS жобасындағы активтер кітапханасына сақтаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="7c0e6-148">Буманы сақтау және тексеру 15 минутты алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="7c0e6-149">Жаңартуды қолдану үшін LCS қызметіндегі **Орта туралы мәліметтер** бетіне өтіп, **Сақтау** > **Жаңартуларды қолдану** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Орталарды сақтау](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="7c0e6-151">Жаңартулар тізімінен жасалған буманы таңдап, **Қолдану** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Жаңартуларды қолдану](./media/10ApplyUpdates.png)

<span data-ttu-id="7c0e6-153">Ортаға қызмет көрсету біраз уақытты алады.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-153">Environment servicing will take some time.</span></span> <span data-ttu-id="7c0e6-154">Ол аяқталғаннан кейін орта орналастырылған күйге оралады.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-154">After it is complete, the environment will return to a deployed state.</span></span>

![Орта орналастырылды](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="7c0e6-156">Қос жазу байланысын орнату</span><span class="sxs-lookup"><span data-stu-id="7c0e6-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="7c0e6-157">LCS жобасында **Орта туралы мәліметтер** бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="7c0e6-158">**Common Data Service ортасы туралы ақпарат** тармағында **Бағдарламаларға арналған CDS сілтемесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="7c0e6-159">Сілтеме аяқталғаннан кейін **Бағдарламаларға арналған CDS сілтемесін** тағы да басыңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="7c0e6-160">Сіз Finance қызметіндегі қос жазуға қайта бағытталасыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-160">You will be redirected to Dual Write in Finance.</span></span>

![CDS сілтемесі](./media/12LinktoCDS.png)

4. <span data-ttu-id="7c0e6-162">Интеграция кезінде салыстырылатын нысандарға қол жеткізу үшін **Шешімді қолдану** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Шешімдерді қолдану](./media/13ApplySolutions.png)

5. <span data-ttu-id="7c0e6-164">Екі шешімді, **Dynamics 365 Finance and Operations қос жазу нысан картасын** және **Dynamics 365 Project Operations қос жазу нысан карталарын** таңдап, содан соң **Қолдану** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Шешімдерді растау](./media/14ConfirmSolutions.png)

<span data-ttu-id="7c0e6-166">Шешімдер қолданылғаннан кейін, Dual Write нысандары ортаға қолданылады.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Шешімдерді қолдану](./media/15ApplyingSolutions.png)

<span data-ttu-id="7c0e6-168">Нысандар қолданылғаннан кейін барлық қолжетімді салыстырулар ортада тізімделеді.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Қос жазу салыстырулары](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="7c0e6-170">Жаңартудан кейін деректер нысандарын жаңарту</span><span class="sxs-lookup"><span data-stu-id="7c0e6-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="7c0e6-171">Finance бөлімінде **Деректерді басқару** жұмыс кеңістігіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-171">In Finance, go to the **Data management** workspace.</span></span>

![Деректерді басқару орны](./media/16DataManagement.png)

2. <span data-ttu-id="7c0e6-173">**Framework параметрлері** тақтасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-173">Select the **Framework parameters** tile.</span></span>

![Framework параметрлері](./media/17FrameworkParameters.png)

3. <span data-ttu-id="7c0e6-175">**Нысан параметрлері** бетінде **Нысандар тізімін жаңарту** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Нысандар тізімін жаңарту](./media/18RefreshEntityList.png)

<span data-ttu-id="7c0e6-177">Жаңарту шамамен 20 минутты алады.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="7c0e6-178">Ол аяқталғаннан кейін ескерту аласыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-178">You will receive an alert when it is complete.</span></span>

![Растауды жаңарту](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="7c0e6-180">Project Operations қос жазу салыстыруларын орындау</span><span class="sxs-lookup"><span data-stu-id="7c0e6-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="7c0e6-181">LCS жобасында **Орта туралы мәліметтер** бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="7c0e6-182">**Common Data Service ортасы туралы ақпарат** тармағында **Бағдарламаларға арналған CDS сілтемесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-182">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="7c0e6-183">Сілтемені таңдағаннан кейін, сіз салыстырулардағы нысандар тізіміне қайта бағытталасыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="7c0e6-184">Келесі кестеде сипатталғандай салыстыруларды бастаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="7c0e6-185">Тізімде көрсетілгендей ретпен орындауды ұмытпаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="7c0e6-186">**Нысан картасы**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-186">**Entity Map**</span></span> | <span data-ttu-id="7c0e6-187">**Нысанды жаңарту**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-187">**Refresh entity**</span></span> | <span data-ttu-id="7c0e6-188">**Бастапқы синхрондау**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-188">**Initial sync**</span></span> | <span data-ttu-id="7c0e6-189">**Бастапқы синхрондау шебері**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-189">**Master for initial sync**</span></span> | <span data-ttu-id="7c0e6-190">**Алғышарттарды орындау**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-190">**Run prerequisites**</span></span> | <span data-ttu-id="7c0e6-191">**Алғышарттарды бастапқы синхрондау**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="7c0e6-192">**Барлық компанияларға арналған жобалық ресурстардың рөлі (тапсырыс беруге болатын ресурс санаттары)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="7c0e6-193">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-193">No</span></span> | <span data-ttu-id="7c0e6-194">Иә</span><span class="sxs-lookup"><span data-stu-id="7c0e6-194">Yes</span></span> | <span data-ttu-id="7c0e6-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="7c0e6-195">Common Data Service</span></span> | <span data-ttu-id="7c0e6-196">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-196">No</span></span> | <span data-ttu-id="7c0e6-197">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-197">N\A</span></span> |
| <span data-ttu-id="7c0e6-198">**Заңды нысандар (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="7c0e6-199">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-199">No</span></span> | <span data-ttu-id="7c0e6-200">Иә</span><span class="sxs-lookup"><span data-stu-id="7c0e6-200">Yes</span></span> | <span data-ttu-id="7c0e6-201">Finance and Operations бағдарламалары</span><span class="sxs-lookup"><span data-stu-id="7c0e6-201">Finance and Operations apps</span></span> | <span data-ttu-id="7c0e6-202">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-202">No</span></span> | <span data-ttu-id="7c0e6-203">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-203">N\A</span></span> |
| <span data-ttu-id="7c0e6-204">**Project Operations интеграциясының нақты мәндері (msdyn\_ нақты)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="7c0e6-205">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-205">No</span></span> | <span data-ttu-id="7c0e6-206">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-206">No</span></span> | <span data-ttu-id="7c0e6-207">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-207">N\A</span></span> | <span data-ttu-id="7c0e6-208">Иә</span><span class="sxs-lookup"><span data-stu-id="7c0e6-208">Yes</span></span> | <span data-ttu-id="7c0e6-209">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-209">No</span></span> |
| <span data-ttu-id="7c0e6-210">**Жобаға негізделген келісім-шарт жолдары (сатылым тапсырысы туралы деректер)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="7c0e6-211">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-211">No</span></span> | <span data-ttu-id="7c0e6-212">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-212">No</span></span> | <span data-ttu-id="7c0e6-213">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-213">N\A</span></span> | <span data-ttu-id="7c0e6-214">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-214">No</span></span> | <span data-ttu-id="7c0e6-215">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-215">No</span></span> |
| <span data-ttu-id="7c0e6-216">**Жобалық транзакция қатынастарына арналған интеграциялық нысан (msdyn\_ транзакциялар)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="7c0e6-217">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-217">No</span></span> | <span data-ttu-id="7c0e6-218">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-218">No</span></span> | <span data-ttu-id="7c0e6-219">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-219">N\A</span></span> | <span data-ttu-id="7c0e6-220">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-220">No</span></span> | <span data-ttu-id="7c0e6-221">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-221">N\A</span></span> |
| <span data-ttu-id="7c0e6-222">**Project Operations интеграциясы келісім-шарт жолының негізгі кезеңдері (msdyn\_келісімшарттар кестесінің мәндері)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="7c0e6-223">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-223">No</span></span> | <span data-ttu-id="7c0e6-224">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-224">No</span></span> | <span data-ttu-id="7c0e6-225">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-225">N\A</span></span> | <span data-ttu-id="7c0e6-226">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-226">No</span></span> | <span data-ttu-id="7c0e6-227">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-227">N\A</span></span> |
| <span data-ttu-id="7c0e6-228">**Шығындарды бағалау үшін Project Operations интеграциялық нысаны (msdyn\_бағалау жолдары)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="7c0e6-229">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-229">No</span></span> | <span data-ttu-id="7c0e6-230">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-230">No</span></span> | <span data-ttu-id="7c0e6-231">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-231">N\A</span></span> | <span data-ttu-id="7c0e6-232">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-232">No</span></span> | <span data-ttu-id="7c0e6-233">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-233">N\A</span></span> |
| <span data-ttu-id="7c0e6-234">**Сағаттық бағалау үшін Project Operations интеграциялық нысаны (msdyn\_ресурс тағайындаулары)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-234">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="7c0e6-235">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-235">No</span></span> | <span data-ttu-id="7c0e6-236">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-236">No</span></span> | <span data-ttu-id="7c0e6-237">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-237">N\A</span></span> | <span data-ttu-id="7c0e6-238">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-238">No</span></span> | <span data-ttu-id="7c0e6-239">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-239">N\A</span></span> |
| <span data-ttu-id="7c0e6-240">**Project Operations интеграциялау жобасының шығындарын экспорттау нысаны (msdyn\_шығындар)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="7c0e6-241">Иә</span><span class="sxs-lookup"><span data-stu-id="7c0e6-241">Yes</span></span> | <span data-ttu-id="7c0e6-242">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-242">No</span></span> | <span data-ttu-id="7c0e6-243">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-243">N\A</span></span> | <span data-ttu-id="7c0e6-244">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-244">No</span></span> | <span data-ttu-id="7c0e6-245">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-245">N\A</span></span> |
| <span data-ttu-id="7c0e6-246">**Сағаттық бағалау үшін Project Operations интеграциялық нысаны (msdyn\_ресурс тағайындаулары)**</span><span class="sxs-lookup"><span data-stu-id="7c0e6-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="7c0e6-247">Иә</span><span class="sxs-lookup"><span data-stu-id="7c0e6-247">Yes</span></span> | <span data-ttu-id="7c0e6-248">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-248">No</span></span> | <span data-ttu-id="7c0e6-249">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-249">N\A</span></span> | <span data-ttu-id="7c0e6-250">№</span><span class="sxs-lookup"><span data-stu-id="7c0e6-250">No</span></span> | <span data-ttu-id="7c0e6-251">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="7c0e6-251">N\A</span></span> |

4. <span data-ttu-id="7c0e6-252">Нысанды жаңарту үшін карта атауын таңдап, содан кейін **Нысандарды жаңарту** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 
5. <span data-ttu-id="7c0e6-253">Жаңарту аяқталғаннан кейін салыстыруды орындауды жалғастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-253">Proceed with running the map after the refresh is complete.</span></span>

![Салыстыруды жаңарту](./media/20RefreshMapping.png)

<span data-ttu-id="7c0e6-255">Келесі салыстыруды қоспас бұрын, кестедегі салыстырудың **Орындалу** күйінде екенін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="7c0e6-256">Көптеген алғышарттары бар салыстыруларды іске қосу біраз уақытты алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="7c0e6-257">Салыстыруды алғышарттармен іске қосу үшін **Байланысты нысан салыстыруларын көрсету** ауыстырып-қосқышын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="7c0e6-258">Егер кестеде **Алғышарттың бастапқы синхрондалуы** **Жоқ** күйінде екені көрсетілсе, оны іске қоспас бұрын балық алғышарт салыстыруларында **Бастапқы синхрондау** жалаушасының **Өшірулі** күйде екенін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-258">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Салыстыруды іске қосу](./media/21RunMap.png)

6. <span data-ttu-id="7c0e6-260">Жобаға қатысты барлық салыстырулардың орындалу күйінде екенін растаңыз.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-260">Validate all project related maps are in the running state.</span></span>

![Барлық салыстырулар орындалуда](./media/22AllMapsRunning.png)

<span data-ttu-id="7c0e6-262">Енді Project Operations ортасы дайындалған және конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="7c0e6-262">Your Project Operations environment is now provisioned and configured.</span></span>