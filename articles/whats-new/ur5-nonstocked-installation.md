---
title: Finance ортасында Project Operations бағдарламасын жаңарту
description: Бұл тақырыпта Project Operations бағдарламасын Dynamics 365 Finance ортасында жаңарту жолы туралы ақпарат берілген.
author: ruhercul
manager: tfehr
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d68296ec59f0bd58f848154c90e02c58f275ab12
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291986"
---
# <a name="update-project-operations-in-your-finance-environment"></a><span data-ttu-id="f4565-103">Finance ортасында Project Operations бағдарламасын жаңарту</span><span class="sxs-lookup"><span data-stu-id="f4565-103">Update Project Operations in your Finance environment</span></span>

<span data-ttu-id="f4565-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="f4565-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="f4565-105">Бұл тақырыпта Dynamics 365 Project Operations бағдарламасын Dynamics 365 Finance ортасында жаңарту жолы туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="f4565-105">This topic provides information about how to update Dynamics 365 Project Operations in your Dynamics 365 Finance environment.</span></span> <span data-ttu-id="f4565-106">Project Operations бағдарламасын 5-жаңартуға (UR5) дейін жаңарту үшін қажет үш процедура бар:</span><span class="sxs-lookup"><span data-stu-id="f4565-106">There are three procedures that are required to update Project Operations to Update 5 (UR5):</span></span>

- [<span data-ttu-id="f4565-107">Буманы алдын ала қарау нұсқасындағы жобаға импорттау</span><span class="sxs-lookup"><span data-stu-id="f4565-107">Import the package into your preview project</span></span>](#import)
- [<span data-ttu-id="f4565-108">Жаңартуды қолдану</span><span class="sxs-lookup"><span data-stu-id="f4565-108">Apply the update</span></span>](#apply)
- [<span data-ttu-id="f4565-109">Dataverse ортасын жаңарту</span><span class="sxs-lookup"><span data-stu-id="f4565-109">Update your Dataverse environment</span></span>](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a><span data-ttu-id="f4565-110">Буманы LCS жобасына импорттау</span><span class="sxs-lookup"><span data-stu-id="f4565-110">Import the package into your LCS project</span></span>

1. <span data-ttu-id="f4565-111">[Lifecycle Services (LCS)](https://lcs.dynamics.com/) порталына жоба иесі немесе орта менеджері ретінде кіріңіз.</span><span class="sxs-lookup"><span data-stu-id="f4565-111">Sign in to [Lifecycle Services (LCS)](https://lcs.dynamics.com/) as a Project Owner or Environment manager.</span></span>
2. <span data-ttu-id="f4565-112">Жобалар тізімінен LCS жобасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-112">From the list of projects, select your LCS project.</span></span>
3. <span data-ttu-id="f4565-113">**Жоба** бетіндегі **Орталар** тобынан жаңарту керек ортаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-113">On the **Project** page, in the **Environments** group, open the environment that you want to update.</span></span>
4. <span data-ttu-id="f4565-114">Ортаның жұмыс істеп тұрғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="f4565-114">Verify that the environment is running.</span></span> <span data-ttu-id="f4565-115">Егер ол қосылмаса, ортада жұмыс істеуді бастаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-115">If it isn't started, start the environment.</span></span>
5. <span data-ttu-id="f4565-116">**Қолжетімді жаңартулар** астындағы **Жаңа шығарылым** бөлімінен 10.0.15 нұсқасы үшін **Жаңартуды қарау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-116">In the **New release** section under **Available updates**, select **View update** for 10.0.15.</span></span>

!["Жаңартуды қарау" түймешігі](media/view-update.png)

6. <span data-ttu-id="f4565-118">**Екілік жаңартулар** бетінде **Буманы сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-118">On the **Binary updates** page, select **Save package**.</span></span>
7. <span data-ttu-id="f4565-119">**Жаңартуларды қарап шығу және сақтау** бетінде **Буманы сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-119">On the **Review and save updates** page, select **Save package**.</span></span>
8. <span data-ttu-id="f4565-120">Ашылатын **Буманы активтер кітапханасына сақтау** бөлігіне буманың атауын енгізіп, содан кейін **Буманы сақтау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-120">On the **Save package to asset library** pane that opens, enter the package name and then select **Save package**.</span></span>
9. <span data-ttu-id="f4565-121">LCS буманы сақтауды аяқтағаннан кейін, **Дайын** түймешігі қосылды.</span><span class="sxs-lookup"><span data-stu-id="f4565-121">When LCS has finished saving the package, the **Done** button is enabled.</span></span> <span data-ttu-id="f4565-122">**Дайын** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-122">Select **Done**.</span></span> <span data-ttu-id="f4565-123">LCS буманы тексереді.</span><span class="sxs-lookup"><span data-stu-id="f4565-123">LCS will verify the package.</span></span> <span data-ttu-id="f4565-124">Тексеру бірнеше минутқа немесе бір сағатқа дейін созылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f4565-124">Verification can take a few minutes or up to one hour.</span></span>


## <a name="apply-the-package-update"></a><a name="apply"></a><span data-ttu-id="f4565-125">Бума жаңартуын қолдану</span><span class="sxs-lookup"><span data-stu-id="f4565-125">Apply the package update</span></span>

1. <span data-ttu-id="f4565-126">LCS порталындағы **Орта туралы мәліметтер** бетінен **Сақтау** > **Жаңартуларды қолдану** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-126">In LCS, on the **Environment details** page, select **Maintain** > **Apply Updates**.</span></span>
2. <span data-ttu-id="f4565-127">Тізімнен бұрын сақтаған буманы таңдап, содан кейін **Қолдану** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-127">From the list, select the package that you saved earlier, and then select **Apply**.</span></span>
3. <span data-ttu-id="f4565-128">Буманы орналастыру керектігін растау үшін **Иә** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-128">Select **Yes** to confirm that you want to deploy the package.</span></span>

![Буманы орналастыру диалогтік терезесін растау](media/confirm-package-deployment.png)

4. <span data-ttu-id="f4565-130">Бағдарламаны жаңарту керектігін растау үшін **Иә** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-130">Select **Yes** to confirm that you want to update the application.</span></span>

![Бағдарламаны жаңарту диалогтік терезесін растау](media/confirm-application-update.png)

<span data-ttu-id="f4565-132">Орналастыру және бағдарламаны жаңарту басталады.</span><span class="sxs-lookup"><span data-stu-id="f4565-132">The deployment and application update will start.</span></span> 

<span data-ttu-id="f4565-133">**Орта туралы мәліметтер** бетінде, жоғарғы оң жақ бұрышта орта күйі **Қызмет көрсету** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="f4565-133">On the **Environment details** page, in the top-right corner, the environment status will update to **Servicing**.</span></span> <span data-ttu-id="f4565-134">Шамамен екі сағат ішінде жаңарту аяқталады.</span><span class="sxs-lookup"><span data-stu-id="f4565-134">In approximately two hours, the update will be complete.</span></span> <span data-ttu-id="f4565-135">Бағдарлама шығарылымы туралы ақпарат **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** параметріне, орта күйі **Орналастырылған** күйіне жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="f4565-135">The application release information will update to **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** and the environment status will update to **Deployed**.</span></span>


## <a name="update-your-dataverse-environment"></a><a name="update"></a><span data-ttu-id="f4565-136">Dataverse ортасын жаңарту</span><span class="sxs-lookup"><span data-stu-id="f4565-136">Update your Dataverse environment</span></span>

1. <span data-ttu-id="f4565-137">[Power Platform басқару орталығына](https://admin.powerplatform.com/)кіріңіз.</span><span class="sxs-lookup"><span data-stu-id="f4565-137">Sign in to the [Power Platform admin center](https://admin.powerplatform.com/).</span></span>
2. <span data-ttu-id="f4565-138">Тізімнен Project Operations бағдарламасын орнату үшін пайдаланылған ортаны тауып ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-138">In the list, find and open the environment that you used to install Project Operations.</span></span>
3. <span data-ttu-id="f4565-139">**Орталар** бетінен **Ресурс** > **Dynamics 365 бағдарламалары** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-139">On the **Environments** page, select **Resource** > **Dynamics 365 apps**.</span></span>
4. <span data-ttu-id="f4565-140">Тізімнен **Microsoft Dynamics 365 Project Operations** бағдарламасын тауып, **Күй** бағанынан **Қолжетімді жаңарту** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-140">In the list, locate **Microsoft Dynamics 365 Project Operations**, and in the **Status** column, select **Update Available**.</span></span>
5. <span data-ttu-id="f4565-141">**Мен қызмет көрсету шарттарымен келісемін** құсбелгісін қойып, содан кейін **Жаңарту** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-141">Select the **I agree to the terms of service** check box, and then select **Update**.</span></span> <span data-ttu-id="f4565-142">Шешімнің соңғы нұсқасы орнатылады.</span><span class="sxs-lookup"><span data-stu-id="f4565-142">The latest version of the solution will be installed.</span></span>

<span data-ttu-id="f4565-143">Орнату аяқталғаннан кейін, сізде 4.5.0.134 нұсқасы орнатылады.</span><span class="sxs-lookup"><span data-stu-id="f4565-143">After the installation is complete, you'll have version 4.5.0.134 installed.</span></span>

## <a name="configure-new-features"></a><span data-ttu-id="f4565-144">Жаңа функцияларды конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="f4565-144">Configure new features</span></span>

### <a name="enable-dual-write-mapping"></a><span data-ttu-id="f4565-145">Қос жазу салыстыруын қосу</span><span class="sxs-lookup"><span data-stu-id="f4565-145">Enable dual-write mapping</span></span>

<span data-ttu-id="f4565-146">Finance және Dataverse орталарында жаңартуды аяқтағаннан кейін, қажет қос жазу салыстыруларын қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="f4565-146">After you complete the update on the Finance and Dataverse environments, you can enable the required dual-write mappings.</span></span> <span data-ttu-id="f4565-147">Қос жазу салыстыруларын қосу үшін келесі процедураларды аяқтаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-147">Complete the following procedures to enable dual-write mappings.</span></span>

- [<span data-ttu-id="f4565-148">Customer Engagement ортасында қауіпсіздік параметрлерін жаңарту</span><span class="sxs-lookup"><span data-stu-id="f4565-148">Update security settings on Customer Engagement environment</span></span>](#security)
- [<span data-ttu-id="f4565-149">Деректер нысандарын жаңарту</span><span class="sxs-lookup"><span data-stu-id="f4565-149">Refresh data entities</span></span>](#refresh)
- [<span data-ttu-id="f4565-150">Қос жазу салыстыруларын жаңарту және іске қосу</span><span class="sxs-lookup"><span data-stu-id="f4565-150">Update and run the dual-write mappings</span></span>](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a><span data-ttu-id="f4565-151">Dataverse ортасында қауіпсіздік параметрлерін жаңарту</span><span class="sxs-lookup"><span data-stu-id="f4565-151">Update security settings on the Dataverse environment</span></span>

<span data-ttu-id="f4565-152">UR5 жаңарту орамасына жаңарту бөлігі ретінде нысандарға арналған қауіпсіздік артықшылықтарына келесі жаңартулар қажет.</span><span class="sxs-lookup"><span data-stu-id="f4565-152">The following updates to the security privileges for entities are required as part of the update to UR5.</span></span>

1. <span data-ttu-id="f4565-153">Dataverse ортасында **Параметрлер** тармағына өтіп, **Жүйе** тобында **Қауіпсіздік** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-153">In your Dataverse environment, go to **Settings**, and in the **System** group, select **Security**.</span></span>

![Dataverse ортасының параметрлері](media/Picture21.png)

2. <span data-ttu-id="f4565-155">**Қауіпсіздік рөлдері** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-155">Select **Security Roles**.</span></span>
3. <span data-ttu-id="f4565-156">Рөлдер тізімінен **қос жазу бағдарламасының пайдаланушысы** параметрін таңдап, **Реттелетін нысандар** қойыншасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-156">From the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span> 
4. <span data-ttu-id="f4565-157">Рөлдің келесілер үшін **Оқу** және **Қосу** рұқсаттары бар екенін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="f4565-157">Verify that the role has **Read** and **Append To** permissions for:</span></span>

      - <span data-ttu-id="f4565-158">**Валюта айырбастау бағамының түрі**</span><span class="sxs-lookup"><span data-stu-id="f4565-158">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="f4565-159">**Тіркелгілер диаграммасы**</span><span class="sxs-lookup"><span data-stu-id="f4565-159">**Chart Of Accounts**</span></span> 
      - <span data-ttu-id="f4565-160">**Қаржылық күнтізбе**</span><span class="sxs-lookup"><span data-stu-id="f4565-160">**Fiscal Calendar**</span></span> 
      - <span data-ttu-id="f4565-161">**Кітап**</span><span class="sxs-lookup"><span data-stu-id="f4565-161">**Ledger**</span></span>

5. <span data-ttu-id="f4565-162">Қауіпсіздік рөлі жаңартылғаннан кейін, **Параметрлер** > **Қауіпсіздік** > **Топтар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f4565-162">After the security role is updated, go to **Settings** > **Security** > **Teams**.</span></span> <span data-ttu-id="f4565-163">**Қос жазу бағдарламасының пайдаланушысы** рөлі топқа қолданылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="f4565-163">Verify that the **dual-write app user** role has been applied to the team.</span></span> 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a><span data-ttu-id="f4565-164">Деректер нысандарын жаңартулар тізімінен жаңарту</span><span class="sxs-lookup"><span data-stu-id="f4565-164">Refresh data entities from the update</span></span>

1. <span data-ttu-id="f4565-165">Finance ортасынан **Деректерді басқару** жұмыс кеңістігін ашып, содан кейін **Құрылым параметрлері** бетін ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-165">In your Finance environment, open the **Data management** workspace, and then open the **Framework parameters** page.</span></span>
2. <span data-ttu-id="f4565-166">**Нысан параметрлері** қойыншасында **Нысандар тізімін жаңарту** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-166">On the **Entity settings** tab, select **Refresh entity list**.</span></span>
3. <span data-ttu-id="f4565-167">Нысанды жаңартуды растау үшін **Жабу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-167">Select **Close** to confirm the entity refresh.</span></span>

 > [!NOTE]
 > <span data-ttu-id="f4565-168">Бұл процесті аяқтау шамамен 20 минутқа созылады.</span><span class="sxs-lookup"><span data-stu-id="f4565-168">This process will take approximately 20 minutes to complete.</span></span> <span data-ttu-id="f4565-169">Жаңартудың аяқталғаны туралы сізге хабарлайды.</span><span class="sxs-lookup"><span data-stu-id="f4565-169">You will be notified when the refresh is complete.</span></span>

### <a name="update-dual-write-mappings"></a><a name="run"></a><span data-ttu-id="f4565-170">Қос жазу салыстыруларын жаңарту</span><span class="sxs-lookup"><span data-stu-id="f4565-170">Update dual-write mappings</span></span>

1. <span data-ttu-id="f4565-171">**Деректерді басқару** жұмыс кеңістігінен **Қос жазу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-171">In the **Data management** workspace, select **Dual-write**.</span></span>
2. <span data-ttu-id="f4565-172">**Шешімдерді қолдану** пәрменін таңдаңыз, тізімнен екі шешімді де таңдап, содан **Қолдану** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-172">Select **Apply solutions**, select both solutions in the list, and then select **Apply**.</span></span>
3. <span data-ttu-id="f4565-173">**Қос жазу** бетінде келесі кесте карталарын таңдап, содан кейін **Тоқтату** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-173">On the **Dual-write** page, select the following table maps, and then select **Stop**.</span></span>

    - <span data-ttu-id="f4565-174">**Project Operations біріктіруінің нақты мәндері (msdyn_actuals)**</span><span class="sxs-lookup"><span data-stu-id="f4565-174">**Project Operations integration actuals (msdyn_actuals)**</span></span>
    - <span data-ttu-id="f4565-175">**Project Operations біріктіруі жобасының шығыс санаттары (msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="f4565-175">**Project Operations integration project expense categories (msdyn_expensecategories)**</span></span>
    - <span data-ttu-id="f4565-176">**Project Operations біріктіруінің нақты мәндері жобасының шығыстарын экспорттау нысаны (msdyn_expenses)**</span><span class="sxs-lookup"><span data-stu-id="f4565-176">**Project Operations integration actuals project expenses export entity (msdyn_expenses)**</span></span>

4. <span data-ttu-id="f4565-177">**Кесте картасының нұсқасы** бетінде үш нұсқаның әрқайсысына картаның жаңа нұсқасын қолданыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-177">On the **Table map version** page, apply a new version of the map to each of the three entities.</span></span>
5. <span data-ttu-id="f4565-178">**Қос жазу** бетінде карталарды қайта іске қосу үшін "іске қосу" түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-178">On the **Dual-write** page, select run to restart the maps.</span></span>
6. <span data-ttu-id="f4565-179">Карталар тізімінен барлық артықшылықтарымен бірге **Кітап (msdyn_ledgers)** картасын таңдап, **Бастапқы синхрондау** ұяшығына құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-179">From the list of maps, select the **Ledger (msdyn_ledgers)** map with all prerequisites and select the **Initial sync** check box.</span></span> 
7. <span data-ttu-id="f4565-180">**Бастапқы синхрондау шебері** өрісінен **Finance and Operations бағдарламалары** тармағын таңдап, **Іске қосу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="f4565-180">In the **Master for initial sync** field, select **Finance and Operations apps** and then select **Run**.</span></span>
 
 ![Кітап картасын синхрондау](media/DW6.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]