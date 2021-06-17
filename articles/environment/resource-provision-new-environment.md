---
title: Жаңа ортаны дайындау
description: Бұл тақырып жаңа Project Operations ортасын дайындау туралы ақпарат береді.
author: sigitac
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d0712d9d5dfc6c35ccd07142ff5948f50e6a254c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995493"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="883e3-103">Жаңа ортаны дайындау</span><span class="sxs-lookup"><span data-stu-id="883e3-103">Provision a new environment</span></span>

<span data-ttu-id="883e3-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="883e3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="883e3-105">Бұл тақырыпта ресурс/биржадан тыс негіздегі сценарийлерге арналған жаңа Dynamics 365 Project Operations ортасын дайындау жолдары туралы ақпарат беріледі.</span><span class="sxs-lookup"><span data-stu-id="883e3-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="883e3-106">LCS жобасында Project Operations автоматтандырылған дайындық жүргізу процесін қосу</span><span class="sxs-lookup"><span data-stu-id="883e3-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="883e3-107">LCS жобаңыздың Project Operations автоматтандырылған дайындық жүргізу ағынына қосу үшін келесі қадамдарды пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="883e3-108">[LCS](https://lcs.dynamics.com/v2) параметріне өтіп, **Мүмкіндіктерді басқаруды алдын ала қарау** тақтасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="883e3-109">**Алдын ала қарау мүмкіндігі** тізімінде Project Operations жүйесін қосу үшін **Project Operations мүмкіндігі** және **Алдын ала қарау мүмкіндігі қосылды** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="883e3-110">Бұл қадам әрбір LCS жобасында тек бір рет орындалады.</span><span class="sxs-lookup"><span data-stu-id="883e3-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="883e3-111">Project Operations ортасын дайындау</span><span class="sxs-lookup"><span data-stu-id="883e3-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="883e3-112">Жаңа Dynamics 365 Finance [демо-ортасын](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) немесе [сынақ ортасы/өндіріс ортасы](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) орналастыруын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-112">Open a new Dynamics 365 Finance [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="883e3-113">**Ортаны дайындау** шебері арқылы өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="883e3-114">Бағдарламаның таңдалған нұсқасының 10.0.13 немесе одан жоғары екендігіне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="883e3-115">Project Operations дайындау үшін **Кеңейтілген параметрлер** тармағында **Common Data Service** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="883e3-116">**Иә** опциясын таңдау арқылы **Common Data Service параметрін** қосып, содан соң қажетті өрістерде ақпарат енгізіңіз:</span><span class="sxs-lookup"><span data-stu-id="883e3-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="883e3-117">Атауы</span><span class="sxs-lookup"><span data-stu-id="883e3-117">Name</span></span>
  - <span data-ttu-id="883e3-118">Өңір</span><span class="sxs-lookup"><span data-stu-id="883e3-118">Region</span></span>
  - <span data-ttu-id="883e3-119">Тіл</span><span class="sxs-lookup"><span data-stu-id="883e3-119">Language</span></span>
  - <span data-ttu-id="883e3-120">Валюта</span><span class="sxs-lookup"><span data-stu-id="883e3-120">Currency</span></span>
 
5. <span data-ttu-id="883e3-121">**Common Data Service үлгісі** өрісінде **Project Operations** опциясын таңдаңыз</span><span class="sxs-lookup"><span data-stu-id="883e3-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="883e3-122">Орналастыру үшін орта түрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="883e3-123">Жазылымға негізделген сынақ CDS ортасын 30 күн ішінде пайдалануға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="883e3-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Орналастыру параметрлері](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="883e3-125">Қызмет көрсету шарттарын растау үшін **Келісу** опциясын таңдаңыз, содан кейін орналастыру параметрлеріне оралу үшін **Дайын** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Орналастыру келісімі](./media/2DeploymentConsent.png)

7. <span data-ttu-id="883e3-127">Қосымша - демо нұсқадағы деректерді ортаға қолдану.</span><span class="sxs-lookup"><span data-stu-id="883e3-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="883e3-128">**Кеңейтілген параметрлер** тармағына өтіңіз, **SQL дерекқорының конфигурациясын реттеу** параметрін таңдап, **Бағдарлама дерекқоры үшін деректер жиынын көрсету** параметрін **Демо** нұсқасына орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="883e3-129">Шебердегі қалған қажетті өрістерді толтырыңыз және орналастыруды растаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="883e3-130">Ортаны дайындау уақыты орта түріне байланысты өзгереді.</span><span class="sxs-lookup"><span data-stu-id="883e3-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="883e3-131">Дайындау алты сағатқа созылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="883e3-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="883e3-132">Орналастыру сәтті аяқталғаннан кейін, орта келесідей болады: **Орналастырылған**.</span><span class="sxs-lookup"><span data-stu-id="883e3-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="883e3-133">Ортаның сәтті орналастырылғанын растау үшін **Жүйеге кіру** параметрін таңдап, растау үшін ортаға кіріңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![ ортасының мәліметтері](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="883e3-135">Finance ортасына жаңартуларды қолдану</span><span class="sxs-lookup"><span data-stu-id="883e3-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="883e3-136">Project Operations жүйесі бағдарлама нұсқасының **10.0.13 (10.0.569.20009)** немесе одан жоғары нұсқасымен Finance ортасын қажет етеді.</span><span class="sxs-lookup"><span data-stu-id="883e3-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="883e3-137">Бұл нұсқаны алу үшін Finance ортасына сапалық жаңартуларды қолдану қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="883e3-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="883e3-138">LCS қызметіндегі **Орта туралы мәліметтер** бетінде, **Қол жетімді жаңартулар** бөлімінде **Жаңартуды қарау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Жаңартуларды қарау](./media/5ViewUpdates.png)

2. <span data-ttu-id="883e3-140">**Екілік жаңартулар** бетінде **Буманы сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-140">On the **Binary updates** page, select **Save package.**</span></span>

![Буманы сақтау](./media/6SavePackage.png)

3. <span data-ttu-id="883e3-142">**Барлығын таңдау** түймешігін басып, содан соң **Буманы сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-142">Click **Select all** and then select **Save package**.</span></span>

![Жаңартуларды қарап шығу және сақтау](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="883e3-144">Буманың атауын және сипаттамасын енгізіп, содан кейін **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="883e3-145">Интернет қосылымына байланысты осы процесс ол біраз уақыт алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="883e3-145">Depending on the internet connection, this process might take some time.</span></span>

![Буманы активтер кітапханасына жүктеу](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="883e3-147">Бума сақталғаннан кейін **Дайын** опциясын таңдап, осы буманы LCS жобасындағы активтер кітапханасына сақтаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="883e3-148">Буманы сақтау және тексеру 15 минутты алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="883e3-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="883e3-149">Жаңартуды қолдану үшін LCS қызметіндегі **Орта туралы мәліметтер** бетіне өтіп, **Сақтау** > **Жаңартуларды қолдану** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Орталарды сақтау](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="883e3-151">Жаңартулар тізімінен жасалған буманы таңдап, **Қолдану** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Жаңартуларды қолдану](./media/10ApplyUpdates.png)

<span data-ttu-id="883e3-153">Ортаға қызмет көрсету біраз уақытты алады.</span><span class="sxs-lookup"><span data-stu-id="883e3-153">Environment servicing will take some time.</span></span> <span data-ttu-id="883e3-154">Ол аяқталғаннан кейін орта орналастырылған күйге оралады.</span><span class="sxs-lookup"><span data-stu-id="883e3-154">After it is complete, the environment will return to a deployed state.</span></span>

![Орта орналастырылды](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="883e3-156">Қос жазу байланысын орнату</span><span class="sxs-lookup"><span data-stu-id="883e3-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="883e3-157">LCS жобасында **Орта туралы мәліметтер** бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="883e3-158">**Common Data Service ортасы туралы ақпарат** тармағында **Бағдарламаларға арналған CDS сілтемесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="883e3-159">Сілтеме аяқталғаннан кейін **Бағдарламаларға арналған CDS сілтемесін** тағы да басыңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="883e3-160">Сіз Finance қызметіндегі қос жазуға қайта бағытталасыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-160">You will be redirected to Dual Write in Finance.</span></span>

![CDS сілтемесі](./media/12LinktoCDS.png)

4. <span data-ttu-id="883e3-162">Интеграция кезінде салыстырылатын нысандарға қол жеткізу үшін **Шешімді қолдану** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Шешімдерді қолдану](./media/13ApplySolutions.png)

5. <span data-ttu-id="883e3-164">**Dynamics 365 Finance and Operations қос жазу нысан картасы** және **Dynamics 365 Project Operations қос жазу нысан карталары** шешімдерінің екеуін де таңдап, содан соң **Қолдану** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Шешімдерді растау](./media/14ConfirmSolutions.png)

<span data-ttu-id="883e3-166">Шешімдер қолданылғаннан кейін, Dual Write нысандары ортаға қолданылады.</span><span class="sxs-lookup"><span data-stu-id="883e3-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Шешімдерді қолдану](./media/15ApplyingSolutions.png)

<span data-ttu-id="883e3-168">Нысандар қолданылғаннан кейін барлық қолжетімді салыстырулар ортада тізімделеді.</span><span class="sxs-lookup"><span data-stu-id="883e3-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Қос жазу салыстырулары](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="883e3-170">Жаңартудан кейін деректер нысандарын жаңарту</span><span class="sxs-lookup"><span data-stu-id="883e3-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="883e3-171">Finance бөлімінде **Деректерді басқару** жұмыс кеңістігіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-171">In Finance, go to the **Data management** workspace.</span></span>

![Деректерді басқару орны](./media/16DataManagement.png)

2. <span data-ttu-id="883e3-173">**Framework параметрлері** тақтасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-173">Select the **Framework parameters** tile.</span></span>

![Framework параметрлері](./media/17FrameworkParameters.png)

3. <span data-ttu-id="883e3-175">**Нысан параметрлері** бетінде **Нысандар тізімін жаңарту** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Нысандар тізімін жаңарту](./media/18RefreshEntityList.png)

<span data-ttu-id="883e3-177">Жаңарту шамамен 20 минутты алады.</span><span class="sxs-lookup"><span data-stu-id="883e3-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="883e3-178">Ол аяқталғаннан кейін ескерту аласыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-178">You will receive an alert when it is complete.</span></span>

![Растауды жаңарту](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="883e3-180">Dataverse ортасындағы Project Operations бағдарламасының қауіпсіздік параметрлерін жаңарту</span><span class="sxs-lookup"><span data-stu-id="883e3-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="883e3-181">Dataverse ортасындағы Project Operations бағдарламасына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="883e3-182">**Параметрлер** > **Қауіпсіздік** > **Қауіпсіздік рөлдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="883e3-183">**Қауіпсіздік рөлдері** бетінде, рөлдер тізімінен **қос жазу бағдарламасының пайдаланушысы** параметрін таңдап, **Реттелетін нысандар** қойыншасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="883e3-184">Рөлдің келесілер үшін **Оқу** және **Қосу** рұқсаттары бар екенін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="883e3-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="883e3-185">**Валюта айырбастау бағамының түрі**</span><span class="sxs-lookup"><span data-stu-id="883e3-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="883e3-186">**Тіркелгілер диаграммасы**</span><span class="sxs-lookup"><span data-stu-id="883e3-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="883e3-187">**Қаржылық күнтізбе**</span><span class="sxs-lookup"><span data-stu-id="883e3-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="883e3-188">**Кітап**</span><span class="sxs-lookup"><span data-stu-id="883e3-188">**Ledger**</span></span>

5. <span data-ttu-id="883e3-189">Қауіпсіздік рөлі жаңартылғаннан кейін **Параметрлер** > **Қауіпсіздік** > **Топтар** тармағына өтіп, **Жергілікті іскери иеленуші** тобының көрінісіндегі әдепкі топты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="883e3-190">**Рөлдерді басқару** параметрін таңдап, **қос жазу бағдарламасының пайдаланушысы** қауіпсіздік артықшылығының топқа қолданылуын қадағалаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="883e3-191">Project Operations қос жазу салыстыруларын орындау</span><span class="sxs-lookup"><span data-stu-id="883e3-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="883e3-192">LCS жобасында **Орта туралы мәліметтер** бетіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="883e3-193">**Common Data Service ортасы туралы ақпарат** тармағында **Бағдарламаларға арналған CDS сілтемесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="883e3-194">Сілтемені таңдағаннан кейін, сіз салыстырулардағы нысандар тізіміне қайта бағытталасыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="883e3-195">Келесі кестеде сипатталғандай салыстыруларды бастаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="883e3-196">Тізімде көрсетілгендей ретпен орындауды ұмытпаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="883e3-197">**Нысан картасы**</span><span class="sxs-lookup"><span data-stu-id="883e3-197">**Entity Map**</span></span> | <span data-ttu-id="883e3-198">**Нысанды жаңарту**</span><span class="sxs-lookup"><span data-stu-id="883e3-198">**Refresh entity**</span></span> | <span data-ttu-id="883e3-199">**Бастапқы синхрондау**</span><span class="sxs-lookup"><span data-stu-id="883e3-199">**Initial sync**</span></span> | <span data-ttu-id="883e3-200">**Бастапқы синхрондау шебері**</span><span class="sxs-lookup"><span data-stu-id="883e3-200">**Master for initial sync**</span></span> | <span data-ttu-id="883e3-201">**Алғышарттарды орындау**</span><span class="sxs-lookup"><span data-stu-id="883e3-201">**Run prerequisites**</span></span> | <span data-ttu-id="883e3-202">**Алғышарттарды бастапқы синхрондау**</span><span class="sxs-lookup"><span data-stu-id="883e3-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="883e3-203">**Барлық компанияларға арналған жобалық ресурстардың рөлі (тапсырыс беруге болатын ресурс санаттары)**</span><span class="sxs-lookup"><span data-stu-id="883e3-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="883e3-204">No</span><span class="sxs-lookup"><span data-stu-id="883e3-204">No</span></span> | <span data-ttu-id="883e3-205">Иә</span><span class="sxs-lookup"><span data-stu-id="883e3-205">Yes</span></span> | <span data-ttu-id="883e3-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="883e3-206">Common Data Service</span></span> | <span data-ttu-id="883e3-207">No</span><span class="sxs-lookup"><span data-stu-id="883e3-207">No</span></span> | <span data-ttu-id="883e3-208">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-208">N\A</span></span> |
| <span data-ttu-id="883e3-209">**Заңды нысандар (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="883e3-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="883e3-210">No</span><span class="sxs-lookup"><span data-stu-id="883e3-210">No</span></span> | <span data-ttu-id="883e3-211">Иә</span><span class="sxs-lookup"><span data-stu-id="883e3-211">Yes</span></span> | <span data-ttu-id="883e3-212">Finance and Operations бағдарламалары</span><span class="sxs-lookup"><span data-stu-id="883e3-212">Finance and Operations apps</span></span> | <span data-ttu-id="883e3-213">No</span><span class="sxs-lookup"><span data-stu-id="883e3-213">No</span></span> | <span data-ttu-id="883e3-214">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-214">N\A</span></span> |
| <span data-ttu-id="883e3-215">**Кітап (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="883e3-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="883e3-216">No</span><span class="sxs-lookup"><span data-stu-id="883e3-216">No</span></span> | <span data-ttu-id="883e3-217">Иә</span><span class="sxs-lookup"><span data-stu-id="883e3-217">Yes</span></span> | <span data-ttu-id="883e3-218">Finance and Operations бағдарламалары</span><span class="sxs-lookup"><span data-stu-id="883e3-218">Finance and Operations apps</span></span> | <span data-ttu-id="883e3-219">Иә</span><span class="sxs-lookup"><span data-stu-id="883e3-219">Yes</span></span> | <span data-ttu-id="883e3-220">Иә, Finance and Operations бағдарламалары</span><span class="sxs-lookup"><span data-stu-id="883e3-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="883e3-221">**Project Operations біріктіруінің нақты мәндері (msdyn\_ нақты)**</span><span class="sxs-lookup"><span data-stu-id="883e3-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="883e3-222">No</span><span class="sxs-lookup"><span data-stu-id="883e3-222">No</span></span> | <span data-ttu-id="883e3-223">№</span><span class="sxs-lookup"><span data-stu-id="883e3-223">No</span></span> | <span data-ttu-id="883e3-224">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-224">N\A</span></span> | <span data-ttu-id="883e3-225">Иә</span><span class="sxs-lookup"><span data-stu-id="883e3-225">Yes</span></span> | <span data-ttu-id="883e3-226">№</span><span class="sxs-lookup"><span data-stu-id="883e3-226">No</span></span> |
| <span data-ttu-id="883e3-227">**Жобаға негізделген келісім-шарт жолдары (сатылым тапсырысы туралы деректер)**</span><span class="sxs-lookup"><span data-stu-id="883e3-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="883e3-228">№</span><span class="sxs-lookup"><span data-stu-id="883e3-228">No</span></span> | <span data-ttu-id="883e3-229">№</span><span class="sxs-lookup"><span data-stu-id="883e3-229">No</span></span> | <span data-ttu-id="883e3-230">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-230">N\A</span></span> | <span data-ttu-id="883e3-231">№</span><span class="sxs-lookup"><span data-stu-id="883e3-231">No</span></span> | <span data-ttu-id="883e3-232">№</span><span class="sxs-lookup"><span data-stu-id="883e3-232">No</span></span> |
| <span data-ttu-id="883e3-233">**Жобалық транзакция қатынастарына арналған интеграциялық нысан (msdyn\_ транзакциялар)**</span><span class="sxs-lookup"><span data-stu-id="883e3-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="883e3-234">№</span><span class="sxs-lookup"><span data-stu-id="883e3-234">No</span></span> | <span data-ttu-id="883e3-235">№</span><span class="sxs-lookup"><span data-stu-id="883e3-235">No</span></span> | <span data-ttu-id="883e3-236">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-236">N\A</span></span> | <span data-ttu-id="883e3-237">№</span><span class="sxs-lookup"><span data-stu-id="883e3-237">No</span></span> | <span data-ttu-id="883e3-238">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-238">N\A</span></span> |
| <span data-ttu-id="883e3-239">**Project Operations біріктіруі келісім-шарт жолының негізгі кезеңдері (msdyn\_келісімшарттар кестесінің мәндері)**</span><span class="sxs-lookup"><span data-stu-id="883e3-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="883e3-240">№</span><span class="sxs-lookup"><span data-stu-id="883e3-240">No</span></span> | <span data-ttu-id="883e3-241">№</span><span class="sxs-lookup"><span data-stu-id="883e3-241">No</span></span> | <span data-ttu-id="883e3-242">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-242">N\A</span></span> | <span data-ttu-id="883e3-243">№</span><span class="sxs-lookup"><span data-stu-id="883e3-243">No</span></span> | <span data-ttu-id="883e3-244">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-244">N\A</span></span> |
| <span data-ttu-id="883e3-245">**Шығындарды бағалау үшін Project Operations интеграциялық нысаны (msdyn\_бағалау жолдары)**</span><span class="sxs-lookup"><span data-stu-id="883e3-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="883e3-246">№</span><span class="sxs-lookup"><span data-stu-id="883e3-246">No</span></span> | <span data-ttu-id="883e3-247">№</span><span class="sxs-lookup"><span data-stu-id="883e3-247">No</span></span> | <span data-ttu-id="883e3-248">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-248">N\A</span></span> | <span data-ttu-id="883e3-249">№</span><span class="sxs-lookup"><span data-stu-id="883e3-249">No</span></span> | <span data-ttu-id="883e3-250">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-250">N\A</span></span> |
| <span data-ttu-id="883e3-251">**Project Operations интеграциялау жобасының шығыс санаттарын экспорттау нысаны (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="883e3-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="883e3-252">№</span><span class="sxs-lookup"><span data-stu-id="883e3-252">No</span></span> | <span data-ttu-id="883e3-253">№</span><span class="sxs-lookup"><span data-stu-id="883e3-253">No</span></span> | <span data-ttu-id="883e3-254">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-254">N\A</span></span> | <span data-ttu-id="883e3-255">№</span><span class="sxs-lookup"><span data-stu-id="883e3-255">No</span></span> | <span data-ttu-id="883e3-256">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-256">N\A</span></span> |
| <span data-ttu-id="883e3-257">**Project Operations интеграциялау жобасының шығындарын экспорттау нысаны (msdyn\_шығындар)**</span><span class="sxs-lookup"><span data-stu-id="883e3-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="883e3-258">Иә</span><span class="sxs-lookup"><span data-stu-id="883e3-258">Yes</span></span> | <span data-ttu-id="883e3-259">№</span><span class="sxs-lookup"><span data-stu-id="883e3-259">No</span></span> | <span data-ttu-id="883e3-260">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-260">N\A</span></span> | <span data-ttu-id="883e3-261">№</span><span class="sxs-lookup"><span data-stu-id="883e3-261">No</span></span> | <span data-ttu-id="883e3-262">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-262">N\A</span></span> |
| <span data-ttu-id="883e3-263">**Сағаттық бағалау үшін Project Operations интеграциялық нысаны (msdyn\_ресурс тағайындаулары)**</span><span class="sxs-lookup"><span data-stu-id="883e3-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="883e3-264">Иә</span><span class="sxs-lookup"><span data-stu-id="883e3-264">Yes</span></span> | <span data-ttu-id="883e3-265">№</span><span class="sxs-lookup"><span data-stu-id="883e3-265">No</span></span> | <span data-ttu-id="883e3-266">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-266">N\A</span></span> | <span data-ttu-id="883e3-267">№</span><span class="sxs-lookup"><span data-stu-id="883e3-267">No</span></span> | <span data-ttu-id="883e3-268">Қолданылмайды</span><span class="sxs-lookup"><span data-stu-id="883e3-268">N\A</span></span> |


4. <span data-ttu-id="883e3-269">Нысанды жаңарту үшін карта атауын таңдап, содан кейін **Нысандарды жаңарту** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Салыстыруды жаңарту](./media/20RefreshMapping.png)

5. <span data-ttu-id="883e3-271">Жаңарту аяқталғаннан кейін, салыстыруды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="883e3-272">Келесі салыстыруды қоспас бұрын, кестедегі салыстырудың **Орындалу** күйінде екенін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="883e3-273">Көптеген алғышарттары бар салыстыруларды іске қосу біраз уақытты алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="883e3-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="883e3-274">Салыстыруды алғышарттармен іске қосу үшін **Байланысты нысан салыстыруларын көрсету** ауыстырып-қосқышын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="883e3-275">Егер кестеде **Алғышарттың бастапқы синхрондалуы** **Жоқ** күйінде екені көрсетілсе, оны іске қоспас бұрын балық алғышарт салыстыруларында **Бастапқы синхрондау** жалаушасының **Өшірулі** күйде екенін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="883e3-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Салыстыруды іске қосу](./media/21RunMap.png)

6. <span data-ttu-id="883e3-277">Жобаға қатысты барлық салыстырулардың орындалу күйінде екенін растаңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-277">Validate all project related maps are in the running state.</span></span>

![Барлық салыстырулар орындалуда](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="883e3-279">Project Operations жүйесіне арналған CDS бағдарламасында конфигурация деректерін қолдану (міндетті емес)</span><span class="sxs-lookup"><span data-stu-id="883e3-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="883e3-280">Егер сіз демо-деректерді Finance ортасына қолданған болсаңыз, демо-деректерді CDS ортасына қолдану үшін [Project Operations жүйесіне арналған Common Data Service қызметінде конфигурация деректерін орнату және қолдану](resource-apply-pro-setup-config-data.md) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="883e3-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="883e3-281">Енді Project Operations ортасы дайындалған және конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="883e3-281">Your Project Operations environment is now provisioned and configured.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]