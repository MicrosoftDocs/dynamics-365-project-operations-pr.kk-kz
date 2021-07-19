---
title: Қос жазу мүмкіндігіне ие Project Operations Dataverse бағдарламасын қолмен орналастыру
description: Бұл тақырып қос жазу мүмкіндігіне қолдау көрсетуі үшін Project Operations Dataverse бағдарламасын қолмен орналастыру жолын түсіндіреді.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2ad147da542fc9e7a2705da7a834d1a6512907e5
ms.sourcegitcommit: 205a94ab4168de25b102f31d00a691c8205ba63e
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/18/2021
ms.locfileid: "6274015"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a><span data-ttu-id="a32b8-103">Қос жазу мүмкіндігіне ие Project Operations Dataverse бағдарламасын қолмен орналастыру</span><span class="sxs-lookup"><span data-stu-id="a32b8-103">Manually deploy the Project Operations Dataverse app with dual-write support</span></span>

<span data-ttu-id="a32b8-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="a32b8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a32b8-105">Бұл тақырып қос жазу мүмкіндігіне қолдау көрсетуі үшін Microsoft Dynamics 365 Project Operations бағдарламасын Microsoft Dataverse жүйесіне қолмен орналастыру жолын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="a32b8-105">This topic explains how to manually deploy Microsoft Dynamics 365 Project Operations in Microsoft Dataverse so that it supports dual-write.</span></span> <span data-ttu-id="a32b8-106">Project Operations бағдарламасы ортаның конфигурациясын анықтайды және алғышарттар орындалған жағдайда қос жазу мүмкіндігіне қосымша қолдау көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="a32b8-106">Project Operations detects the environment's configuration and adds additional support for dual-write if the prerequisites are met.</span></span>

<span data-ttu-id="a32b8-107">Microsoft Dynamics Lifecycle Services (LCS) арқылы орналастыру кезінде егер сіз осы тақырыптағы нұсқауларды орындаған болсаңыз, Microsoft Power Platform біріктіруін (бұрын Common Data Service ортасы деп аталған) орналастыруды өткізіп жіберсеңіз болады.</span><span class="sxs-lookup"><span data-stu-id="a32b8-107">During deployment through Microsoft Dynamics Lifecycle Services (LCS), if you've followed the instructions in this topic, you can skip the deployment of the Microsoft Power Platform integration (previously known as the Common Data Service environment).</span></span>

<span data-ttu-id="a32b8-108">Қос жазу мүмкіндігіне қолдау көрсетуі үшін Project Operations бағдарламасын Dataverse жүйесіне орналастырудың төрт негізгі қадамы бар:</span><span class="sxs-lookup"><span data-stu-id="a32b8-108">The process of deploying Project Operations in Dataverse so that it supports dual-write has four main steps:</span></span>

1. <span data-ttu-id="a32b8-109">[Dataverse жүйесінде қос жазу мүмкіндігіне қолдау көрсететін жаңа орта жасау](#create).</span><span class="sxs-lookup"><span data-stu-id="a32b8-109">[Create a new environment in Dataverse that supports dual-write](#create).</span></span>
2. <span data-ttu-id="a32b8-110">[Ортаға қос жазу алғышарттарын қосу](#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="a32b8-110">[Add dual-write prerequisites to the environment](#prerequisites).</span></span>
3. <span data-ttu-id="a32b8-111">[Project Operations Dataverse бағдарламасын қосу](#dataverse).</span><span class="sxs-lookup"><span data-stu-id="a32b8-111">[Add the Project Operations Dataverse app](#dataverse).</span></span>
4. <span data-ttu-id="a32b8-112">[Орталарды байланыстыру](#link).</span><span class="sxs-lookup"><span data-stu-id="a32b8-112">[Link your environments](#link).</span></span>

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a><span data-ttu-id="a32b8-113">Dataverse жүйесінде қос жазу мүмкіндігіне қолдау көрсететін жаңа орта жасау</span><span class="sxs-lookup"><span data-stu-id="a32b8-113">Create a new environment in Dataverse that supports dual-write</span></span>

<span data-ttu-id="a32b8-114">Бұл процедураны орындау үшін әкімші ретінде кіру керек.</span><span class="sxs-lookup"><span data-stu-id="a32b8-114">To complete this procedure, you must sign in as an administrator.</span></span>

1. <span data-ttu-id="a32b8-115">[Power Platform басқару орталығын](https://admin.powerplatform.com) ашыңыз және әкімші ретінде кіріңіз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-115">Open the [Power Platform admin center](https://admin.powerplatform.com), and sign in as an administrator.</span></span>
2. <span data-ttu-id="a32b8-116">Жаңа орта жасаңыз және оған атау беріңіз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-116">Create a new environment, and name it.</span></span>
3. <span data-ttu-id="a32b8-117">Орта түрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-117">Select the environment type.</span></span> <span data-ttu-id="a32b8-118">Егер сіз сынақ нұсқасы ұсынысына жазылсаңыз, **Сынақ нұсқасы (жазылымға негізделген)** түрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-118">If you signed up for the trial offer, select **Trial (subscription-based)**.</span></span>
4. <span data-ttu-id="a32b8-119">Орналастыру аймағын растаңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-119">Confirm the deployment region.</span></span>
5. <span data-ttu-id="a32b8-120">**Осы орта үшін дерекқор жасау** опциясын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-120">Enable the **Create a database for this environment** option.</span></span> 
6. <span data-ttu-id="a32b8-121">Тілді растаңыз және содан кейін валютаның Finance and Operations бағдарламаларының валютасына сәйкес келетінін растаңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-121">Confirm the language, and then confirm that the currency matches the currency for your Finance and Operations apps.</span></span>
7. <span data-ttu-id="a32b8-122">**Dynamics 365 бағдарламалары** опциясын қосыңыз және **Осы бағдарламаларды автоматты түрде орналастыру** өрісінің **Жоқ** мәніне орнатылғанын растаңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-122">Enable the **Dynamics 365 apps** option, and confirm that the **Automatically deploy these apps** field is set to **None**.</span></span>
8. <span data-ttu-id="a32b8-123">Қауіпсіздік тобы қажет болса, қауіпсіздік тобын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-123">Add a security group, if a security group is required.</span></span>
9. <span data-ttu-id="a32b8-124">Орта жасау үшін **Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-124">Select **Save** to create the environment.</span></span>
10. <span data-ttu-id="a32b8-125">Орналастыру аяқталғанын және ортаның **Дайын** күйіне жетуін күтіңіз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-125">Wait until the deployment is completed and the environment reaches the **Ready** state.</span></span>

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a><span data-ttu-id="a32b8-126">Ортаға қос жазу алғышарттарын қосу</span><span class="sxs-lookup"><span data-stu-id="a32b8-126">Add dual-write prerequisites to the environment</span></span>

<span data-ttu-id="a32b8-127">Қос жазу қолдауы **Компания** нысаны сияқты негізгі нысандарға қосылатын қосымша өрістерді қамтиды.</span><span class="sxs-lookup"><span data-stu-id="a32b8-127">Dual-write support includes additional fields that are added to key entities, such as the **Company** entity.</span></span> <span data-ttu-id="a32b8-128">Егер сіз бұрыннан бар ортаға қос жазу қолдауын қоссаңыз, қолдауды қосу үшін деректерді жаңартуыңыз керек болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="a32b8-128">If you're adding dual-write support to an existing environment, you might have to update the data to enable the support.</span></span> <span data-ttu-id="a32b8-129">Деректерді бастапқы жүктеу әдісі туралы ақпарат алу үшін [Компания деректерін бастапқы жүктеу](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-129">For information about how to bootstrap the data, see [Bootstrap company data](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span></span> <span data-ttu-id="a32b8-130">Қос жазу мүмкіндігін туралы қосымша ақпарат алу үшін [Қос жазу жүйесінің талаптары](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-130">For more information about dual-write, see [Dual-write system requirements](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span></span>

<span data-ttu-id="a32b8-131">Ортаға қос жазу алғышарттарын қосу үшін осы процедураны аяқтаңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-131">Complete this procedure to add the dual-write prerequisites to your environment.</span></span>

1. <span data-ttu-id="a32b8-132">Жаңа ғана жасаған ортаны ашыңыз және содан кейін **Ресурс** \> **Dynamics 365 бағдарламалары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-132">Open the environment that you just created, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="a32b8-133">Бағдарлама тізімінде **Қос жазу негізгі шешімі** параметрін таңдаңыз және оны орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-133">Select **Dual-write core solution** in the app list, and install it.</span></span>
3. <span data-ttu-id="a32b8-134">Орнату аяқталғанша күтіңіз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-134">Wait until the installation is completed.</span></span> <span data-ttu-id="a32b8-135">Содан кейін бағдарлама тізімінде **Қос жазу бағдарламасы өзара қатынасының шешімі** параметрін таңдаңыз және оны орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-135">Then select **Dual-write application orchestration solution** in the app list, and install it.</span></span>

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a><span data-ttu-id="a32b8-136">Project Operations Dataverse бағдарламасын қосу</span><span class="sxs-lookup"><span data-stu-id="a32b8-136">Add the Project Operations Dataverse app</span></span>

<span data-ttu-id="a32b8-137">Сіз бұл процедураны тек Project Operations бағдарламасын орнатпас бұрын алдыңғы процедураларды орындаған жағдайда ғана орындай аласыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-137">You can complete this procedure only if you completed the previous procedures before you installed Project Operations.</span></span> <span data-ttu-id="a32b8-138">Орнату кезінде жүйе орта конфигурациясын талдайды және қажет болған жағдайда қос жазу мүмкіндігіне қолдау қосады.</span><span class="sxs-lookup"><span data-stu-id="a32b8-138">During installation, the system analyzes the environment configuration and adds support for dual-write if it's required.</span></span>

1. <span data-ttu-id="a32b8-139">Бұрын жасаған ортаны ашыңыз және содан кейін **Ресурс** \> **Dynamics 365 бағдарламалары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-139">Open the environment that you created earlier, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="a32b8-140">Бағдарлама тізімінен **Microsoft Dynamics 365 Project Operations** бағдарламасын таңдаңыз және оны орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-140">Select **Microsoft Dynamics 365 Project Operations** in the app list, and install it.</span></span>

## <a name="link-your-environments"></a><a name="link"></a><span data-ttu-id="a32b8-141">Орталарды байланыстыру</span><span class="sxs-lookup"><span data-stu-id="a32b8-141">Link your environments</span></span>

<span data-ttu-id="a32b8-142">Dataverse ортасы орналастырылғаннан кейін, Finance and Operations бағдарламаларындағы сілтемені реттеуге болады.</span><span class="sxs-lookup"><span data-stu-id="a32b8-142">After the Dataverse environment is deployed, you can set up the link in your Finance and Operations apps.</span></span> <span data-ttu-id="a32b8-143">[Орталарды байланыстыру үшін қос жазу шеберін пайдалану](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment) бөліміндегі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="a32b8-143">Follow the steps in [Use the dual-write wizard to link your environments](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span></span>
