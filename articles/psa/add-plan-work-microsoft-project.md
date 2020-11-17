---
title: Microsoft Project бағдарламасында жұмысты жоспарлау үшін Project Service қондырмасын пайдалану | MicrosoftDocs
description: Бұл тақырыпта Microsoft Project Service үшін Microsoft Project қондырмасын қосу, конфигурациялау және пайдалану жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
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
ms.openlocfilehash: 6bc74442866caccc02e53afc913a55aab81f9629
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129685"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a><span data-ttu-id="bffdc-103">Microsoft Project бағдарламасында жұмысты жоспарлау үшін Project Service Automation қосылатын модулін пайдалану</span><span class="sxs-lookup"><span data-stu-id="bffdc-103">Use the Project Service Automation Add-in to plan your work in Microsoft Project</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="bffdc-104">жүйесі болжамдарды қоса жоба жоспарлауын орындауды жеңілдетеді.</span><span class="sxs-lookup"><span data-stu-id="bffdc-104">makes it easier for you to do your project planning, including estimates.</span></span> <span data-ttu-id="bffdc-105">Соңғы ұсыныс жіберілген кезде құн, әрекет және сатылым мәндерінің анық болуы үшін жұмысты анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-105">You can define the work so that costs, effort, and sales value are clear as the final proposal is submitted.</span></span>  

 <span data-ttu-id="bffdc-106">Енді [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] жүйесін орнатуға және жоспарлау жұмысын [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасының таныс ортасында орындауға болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-106">Now you can install the [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] and do your planning work in the familiar environment of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span> <span data-ttu-id="bffdc-107">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасының күшті жоспарлау мен басқару мүмкіндіктерін пайдаланып, жоба жоспарын Project Service Automation қызметінде жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-107">Use the robust planning and management capabilities of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and then update your project plan in Project Service Automation.</span></span>  

> [!IMPORTANT]
> - <span data-ttu-id="bffdc-108">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобалары үшін [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлдарын сақтау мақсатында SharePoint құжаттарды басқару мүмкіндігін пайдалану үшін, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] әкімшісі құжаттарды басқару мүмкіндігін іске қосуы керек.</span><span class="sxs-lookup"><span data-stu-id="bffdc-108">To use SharePoint document management to store your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] files for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] projects, your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] admin will need to turn on document management.</span></span> 
> - <span data-ttu-id="bffdc-109">[!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] тек [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="bffdc-109">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] is only compatible with [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span></span>  

## <a name="download-and-install-the-add-in"></a><span data-ttu-id="bffdc-110">Қосылатын модульді жүктеп алу және орнату</span><span class="sxs-lookup"><span data-stu-id="bffdc-110">Download and install the add-in</span></span>  
 <span data-ttu-id="bffdc-111">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне кіру ақпаратын дайындап қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-111">Have your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sign-in information ready.</span></span> <span data-ttu-id="bffdc-112">Осы ақпарат [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасынан [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне қосылу үшін қажет.</span><span class="sxs-lookup"><span data-stu-id="bffdc-112">You will need this information to connect from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

1.  <span data-ttu-id="bffdc-113">Жүктеп алу орталығынан Project Service бағдарламасының [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) немесе [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956) қолдау көрсетілетін нұсқасы үшін қондырманы жүктеп алыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-113">From the Download Center, download the add-in for your supported version of Project Service, either [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) or [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span></span>  

2.  <span data-ttu-id="bffdc-114">Жүктеп алу сілтемесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-114">Click the download link.</span></span>  

3.  <span data-ttu-id="bffdc-115">Жүктеп алу аяқталған кезде қондырманы орнату үшін **Иә** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-115">When the download is complete, click **Yes** to install the add-in.</span></span>  

## <a name="configure-the-add-in"></a><span data-ttu-id="bffdc-116">Қосылатын модульді конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="bffdc-116">Configure the add-in</span></span>  

1. <span data-ttu-id="bffdc-117">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын ашыңыз және **Project Service** қойыншасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-117">Open [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and click the **Project Service** tab.</span></span>  

2. <span data-ttu-id="bffdc-118">**Қосылу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-118">Click **Connect**.</span></span>  

3. <span data-ttu-id="bffdc-119">Жүйеге кіру ақпаратын енгізіп, **Кіру** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-119">Enter your sign-in information and then click **Sign in**.</span></span>  

   <span data-ttu-id="bffdc-120">Енді қосылатын модуль пайдалануын бастауға болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-120">Now you can start using the add-in.</span></span>  

## <a name="read-from-a-template"></a><span data-ttu-id="bffdc-121">Үлгіден оқу</span><span class="sxs-lookup"><span data-stu-id="bffdc-121">Read from a template</span></span>  
 <span data-ttu-id="bffdc-122">Жобаны жоспарлауды бастау үшін [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішінде жасалған және [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасына көшірілген үлгіден оқыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-122">Read from a template that you created in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] and copied into [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to start your project planning.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="bffdc-123">[Жоба үлгісін жасау (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="bffdc-123">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1.  <span data-ttu-id="bffdc-124">**Project Service** қойыншасынан **Оқу** > **Project Service Automation жоба үлгісі** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-124">From the **Project Service** tab, click **Read** > **Project Service Automation Project Template**.</span></span>  

2.  <span data-ttu-id="bffdc-125">Тізімнен жоба үлгісін таңдап, **Ашу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-125">Choose a project template from the list and then click **Open**.</span></span>  

    > [!NOTE]
    >  <span data-ttu-id="bffdc-126">Әдепкі бойынша, үлгіден Project бағдарламасына көшірілген тапсырмалар қолмен жоспарланған ретінде орнатылады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-126">By default, the tasks that are copied from the template into Project are set as manually scheduled.</span></span>  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a><span data-ttu-id="bffdc-127">Жоба ресурстарына [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] рөлдерін белгілеу</span><span class="sxs-lookup"><span data-stu-id="bffdc-127">Assign [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] roles to project resources</span></span>  

1.  <span data-ttu-id="bffdc-128">Жобаны ашыңыз және **Тапсырма** таспасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-128">Open a project and click the **Task** ribbon.</span></span>  

2.  <span data-ttu-id="bffdc-129">**Гант диаграммасы** мәзірін басып, **Ресурс парағы** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-129">Click the **Gantt Chart** menu and then choose **Resource Sheet**.</span></span>  

3.  <span data-ttu-id="bffdc-130">Ресурс парағында **Project Service ресурс рөлі** ашылмалы мәзірін басыңыз және Project Service Automation рөлін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-130">On the Resource Sheet, click the **Project Service Resource Role** drop-down menu and choose a Project Service Automation role.</span></span>  

## <a name="staff-your-project-with-resources"></a><span data-ttu-id="bffdc-131">Жобаны ресурстармен жабдықтау</span><span class="sxs-lookup"><span data-stu-id="bffdc-131">Staff your project with resources</span></span>  

1.  <span data-ttu-id="bffdc-132">Project Service қойыншасынан жолды таңдаңыз және **Ресурстар табу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-132">From the Project Service tab, select a row and click **Find Resources**.</span></span>  

2.  <span data-ttu-id="bffdc-133">**Ресурсты тіркеу** экранында жобаға пайдалану қажет ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-133">On the **Book Resource** screen, select the resource that you want to use for the project.</span></span>  

3.  <span data-ttu-id="bffdc-134">**Тіркеу** пәрменін таңдап, **OK** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-134">Click **Book** and then click **OK**.</span></span>  

## <a name="publish-your-project"></a><span data-ttu-id="bffdc-135">Жобаны жариялау</span><span class="sxs-lookup"><span data-stu-id="bffdc-135">Publish your project</span></span>  
<span data-ttu-id="bffdc-136">Жоба жоспарлауы аяқталған кезде келесі қадам жобаны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне импорттау және жариялау болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-136">When your project planning is complete, the next step is to import and publish the project in to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

<span data-ttu-id="bffdc-137">Жоба [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне импортталады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-137">The project will import into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="bffdc-138">Бағалар және топ жасау процесі қолданылады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-138">The pricing and team generation process are applied.</span></span> <span data-ttu-id="bffdc-139">Топтың, жоба болжамдарының және жұмыс декомпозициясы құрылымының жасалғанын көру үшін жобаны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесінде ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-139">Open the project in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to see that the team, project estimates, and work breakdown structure has been generated.</span></span> <span data-ttu-id="bffdc-140">Төмендегі кестеде нәтижелерді табатын жер көрсетілген:</span><span class="sxs-lookup"><span data-stu-id="bffdc-140">The following table shows where to find the results:</span></span>


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="bffdc-141">**Гант диаграммасы**</span><span class="sxs-lookup"><span data-stu-id="bffdc-141">**Gantt Chart**</span></span>   | <span data-ttu-id="bffdc-142">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жұмыс декомпозициясының құрылымы** экранына импорттайды.</span><span class="sxs-lookup"><span data-stu-id="bffdc-142">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Work Breakdown Structure** screen.</span></span> |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="bffdc-143">**Ресурс парағы**</span><span class="sxs-lookup"><span data-stu-id="bffdc-143">**Resource Sheet**</span></span> |   <span data-ttu-id="bffdc-144">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жоба тобы мүшелері** экранына импорттайды.</span><span class="sxs-lookup"><span data-stu-id="bffdc-144">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Team Members** screen.</span></span>   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="bffdc-145">**Пайдалану пайдалану**</span><span class="sxs-lookup"><span data-stu-id="bffdc-145">**Use Usage**</span></span>    |    <span data-ttu-id="bffdc-146">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жоба болжамдары** экранына импорттайды.</span><span class="sxs-lookup"><span data-stu-id="bffdc-146">Omports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Estimates** screen.</span></span>     |

<span data-ttu-id="bffdc-147">**Жобаны импорттау және жариялау үшін**</span><span class="sxs-lookup"><span data-stu-id="bffdc-147">**To import and publish your project**</span></span>  
1. <span data-ttu-id="bffdc-148">**Project Service** қойыншасынан **Жариялау** > **Жаңа Project Service Automation жобасы** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-148">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project**.</span></span>  

2. <span data-ttu-id="bffdc-149">**Project Service қызметіндегі жаңа жобаға жариялау** диалогтық терезесінде **Жоба атауы** мәнін енгізіңіз және **Тұтынушы** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-149">On **Publish to a new project in Project Service** dialog box, enter the **Project Name** and select the **Customer**.</span></span>  

3. <span data-ttu-id="bffdc-150">Сонымен қатар, жоспардың Project файлын Project Service Automation қызметіне байланыстыру үшін **Жоба жоспарын Project Service Automation қызметіне байланыстыру** пәрменін белгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-150">Optionally check the **Link project plan to Project Service Automation** to link the plan Project file to Project Service Automation.</span></span>  

4. <span data-ttu-id="bffdc-151">**Жариялау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-151">Click **Publish**.</span></span>  

   <span data-ttu-id="bffdc-152">Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне байланыстыру Project файлын басты етеді және [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіндегі жұмыс декомпозициясының құрылымын тек оқуға арналған етіп орнатады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-152">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to read-only.</span></span>  <span data-ttu-id="bffdc-153">Жоба жоспарына өзгерістер енгізу үшін оларды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасау және жаңартулар ретінде [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіне жариялау қажет.</span><span class="sxs-lookup"><span data-stu-id="bffdc-153">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

## <a name="edit-a-project-thats-been-imported"></a><span data-ttu-id="bffdc-154">Импортталған жобаны өңдеу</span><span class="sxs-lookup"><span data-stu-id="bffdc-154">Edit a project that’s been imported</span></span>  
 <span data-ttu-id="bffdc-155">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметіне импортталған жоба жоспарына өзгерістер енгізу үшін екі таңдау бар:</span><span class="sxs-lookup"><span data-stu-id="bffdc-155">To make changes to a project plan that's been imported into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you have two options:</span></span>  

- <span data-ttu-id="bffdc-156">Басты файлды ашып, оны [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында өңдеңіз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-156">Open the master file and edit it in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

- <span data-ttu-id="bffdc-157">Файлды ажыратыңыз және оны тікелей Project Service қызметінде өңдеңіз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-157">Unlink the file and edit it directly in Project Service.</span></span> <span data-ttu-id="bffdc-158">Әдепкі бойынша, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ішінен жүктеп салынған жоба құлыпталады және оны тек Project бағдарламасында өңдеуге болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-158">By default, a project that’s been uploaded from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] is locked and can only be edited in Project.</span></span> <span data-ttu-id="bffdc-159">Файлды [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішінде өңдеу үшін файл ажыратылу болуы керек.</span><span class="sxs-lookup"><span data-stu-id="bffdc-159">To edit the file in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], the file has to be unlinked.</span></span>  

### <a name="edit-in-pn_microsoft_project"></a><span data-ttu-id="bffdc-160">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында өңдеу</span><span class="sxs-lookup"><span data-stu-id="bffdc-160">Edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span></span>  

1. <span data-ttu-id="bffdc-161">Негізгі мәзірден **Project Service** > **Жобалар** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-161">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="bffdc-162">Жобалар тізімінен [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасалған жобаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-162">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="bffdc-163">Таспадан **MS Project бағдарламасында ашу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-163">Click **Open in MS Project** from the ribbon.</span></span> <span data-ttu-id="bffdc-164">Бұл байланысқан басты файлды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-164">This will open the linked master file in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a><span data-ttu-id="bffdc-165">Файлды ажырату және [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] қызметінде өңдеу</span><span class="sxs-lookup"><span data-stu-id="bffdc-165">Unlink a file and edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span></span>  

1. <span data-ttu-id="bffdc-166">Негізгі мәзірден **Project Service** > **Жобалар** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-166">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="bffdc-167">Жобалар тізімінен [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасалған жобаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-167">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="bffdc-168">Таспадан **MS Project бағдарламасынан ажырату** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-168">Click **Unlink from MS Project** from the ribbon.</span></span>  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a><span data-ttu-id="bffdc-169">SharePoint немесе Office топтарына жоба файлын жүктеп салу</span><span class="sxs-lookup"><span data-stu-id="bffdc-169">Upload a Project file to SharePoint or Office Groups</span></span>  
 <span data-ttu-id="bffdc-170">Жоба файлын SharePoint бағдарламасына жүктеп салып, оны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасына арналған "Қатысты құжаттар" аймағынан табуға болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-170">You can upload your Project file to SharePoint and find it under the Associated Documents for your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  <span data-ttu-id="bffdc-171">Әкімші SharePoint құжаттарды басқару мүмкіндігін конфигурациялауы және оны жоба нысаны үшін қосуы қажет.</span><span class="sxs-lookup"><span data-stu-id="bffdc-171">You need to have your administrator configure SharePoint document management and turn it on for the Project entity.</span></span> 

 <span data-ttu-id="bffdc-172">Әрі Office Groups орнатылған болса, Project файлын [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] ішіне жүктеп салуға болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-172">You can also upload your Project file to [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] if you have Office Groups set up.</span></span>

### <a name="upload-a-file-for-sharepoint"></a><span data-ttu-id="bffdc-173">SharePoint бағдарламасы үшін файлды жүктеп салу</span><span class="sxs-lookup"><span data-stu-id="bffdc-173">Upload a file for SharePoint</span></span>  

1. <span data-ttu-id="bffdc-174">Негізгі мәзірден **Project Service** > **Жүктеп салу** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-174">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="bffdc-175">**Project Service Automation жоба құжаттарына** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-175">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="bffdc-176">**[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашуды қосу** диалогтық терезесінде **Иә** немесе **Жоқ** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-176">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="bffdc-177">**Иә** параметрін таңдасаңыз, Project Service Automation қызметінде **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** түймешігін басып, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын іске қосып, SharePoint құжаттар кітапханасынан жоба файлын жүктеуге болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-177">If you click **Yes**, you'll be able select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="bffdc-178">**Жоқ** параметрін таңдасаңыз, **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** түймешігінің сілтемесі істемейді.</span><span class="sxs-lookup"><span data-stu-id="bffdc-178">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="bffdc-179">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметінде **Құжаттар** астында нақты [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасы үшін табуға болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-179">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

### <a name="upload-a-file-for-office-groups"></a><span data-ttu-id="bffdc-180">Файлды Office Groups үшін жүктеп салу</span><span class="sxs-lookup"><span data-stu-id="bffdc-180">Upload a file for Office Groups</span></span>  

1. <span data-ttu-id="bffdc-181">Негізгі мәзірден **Project Service** > **Жүктеп салу** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-181">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="bffdc-182">**Project Service Automation жоба құжаттарына** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-182">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="bffdc-183">**[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашуды қосу** диалогтық терезесінде **Иә** немесе **Жоқ** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-183">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="bffdc-184">**Иә** параметрін таңдасаңыз, Project Service Automation қызметінде **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** түймешігін басып, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын іске қосып, SharePoint құжаттар кітапханасынан жоба файлын жүктеуге болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-184">If you click **Yes**, you'll be able to select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="bffdc-185">**Жоқ** параметрін таңдасаңыз, **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** түймешігінің сілтемесі істемейді.</span><span class="sxs-lookup"><span data-stu-id="bffdc-185">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="bffdc-186">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметінде **Құжаттар** астында нақты [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасы үшін табуға болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-186">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

## <a name="publish--your-project-as-a-template"></a><span data-ttu-id="bffdc-187">Жобаны үлгі ретінде жариялау</span><span class="sxs-lookup"><span data-stu-id="bffdc-187">Publish  your project as a template</span></span>  
 <span data-ttu-id="bffdc-188">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіндегі жоба үлгісі ретінде сақтап, жобаны сақтауға және қайта пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-188">You can save your project and reuse it by saving it as a project template in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  <span data-ttu-id="bffdc-189">Жоба үлгілері [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіндегі қайта пайдаланылатын жоба жоспарлары болып табылады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-189">Project templates are reusable project plans in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="bffdc-190">[Жоба үлгісін жасау (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="bffdc-190">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1. <span data-ttu-id="bffdc-191">**Project Service** қойыншасынан **Жариялау** > **Жаңа Project Service Automation жоба үлгісі** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-191">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project Template**.</span></span>  

2. <span data-ttu-id="bffdc-192">**Project Service үлгісінде жаңа жобаны жариялау** диалогтық терезесінде **Жоба үлгісінің атауы** параметрін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-192">On the **Publish to a new project in Project Service template** dialog box, enter the **Project template name**.</span></span>  

3. <span data-ttu-id="bffdc-193">Сонымен қатар, Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметіне байланыстыру үшін **Жоба жоспарын Project Service Automation қызметіне байланыстыру** пәрменін белгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-193">Optionally, check the **Link project plan to Project Service Automation** to link the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

4. <span data-ttu-id="bffdc-194">**Жариялау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="bffdc-194">Click **Publish**.</span></span>  

<span data-ttu-id="bffdc-195">Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне байланыстыру Project файлын басты етеді және [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] үлгісіндегі жұмыс декомпозициясының құрылымын тек оқуға арналған етіп орнатады.</span><span class="sxs-lookup"><span data-stu-id="bffdc-195">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] template to read-only.</span></span>  <span data-ttu-id="bffdc-196">Жоба жоспарына өзгерістер енгізу үшін оларды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасау және жаңартулар ретінде [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіне жариялау қажет.</span><span class="sxs-lookup"><span data-stu-id="bffdc-196">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>

### <a name="see-also"></a><span data-ttu-id="bffdc-197">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="bffdc-197">See Also</span></span>  
 [<span data-ttu-id="bffdc-198">Жоба менеджерінің нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="bffdc-198">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
