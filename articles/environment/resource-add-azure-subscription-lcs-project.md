---
title: LCS жобасына Azure жазылымын қосу
description: Бұл тақырып Azure жазылымын LCS жобасына қалай қосуға болатындығы туралы ақпарат береді.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6daa86d453ec5022cdd75dff0394c8818292406c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000623"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="8ecbd-103">LCS жобасына Azure жазылымын қосу</span><span class="sxs-lookup"><span data-stu-id="8ecbd-103">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="8ecbd-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="8ecbd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8ecbd-105">Бұлт қызметтеріне орналастырылған орталар бұрыннан бар Azure жазылымын қолдану арқылы орналастырылуы керек.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="8ecbd-106">Бұл тақырып бұрыннан бар Azure жазылымын LCS жобасына қалай қосуға болатындығын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="8ecbd-107">Әкімшінің келісімін беріңіз</span><span class="sxs-lookup"><span data-stu-id="8ecbd-107">Grant admin consent</span></span>

1. <span data-ttu-id="8ecbd-108">Сіздің LCS жобаңызда **Қоршаған орта** бөлімінде **Microsoft Azure параметрлері** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![Microsoft Azure параметрлері](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="8ecbd-110">**Жоба параметрлері** бетінде, **Azure коннекторлары** қойыншасынан **Рұқсат ету** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="8ecbd-111">Бұл қоршаған ортаны осы жобаға орналастыруға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-111">This allows environments to be deployed to this project.</span></span>

![Azure коннекторлары](./media/2AzureConnectors.png)

3. <span data-ttu-id="8ecbd-113">Әкімшінің келісімін беру үшін **Рұқсат ету** опциясын қайта таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-113">Select **Authorize** again to provide admin consent.</span></span>

![Әкімшінің келісімін беріңіз](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="8ecbd-115">Рұқсаттар туралы сұранысты қабылдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-115">Accept the permissions request.</span></span>

![Рұқсаттар сұранысын қабылдаңыз](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="8ecbd-117">Авторизация енді аяқталды.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-117">The authorization is now complete.</span></span> 

![Авторизация сәтті өтті](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="8ecbd-119">Azure жазылымыңызға Dynamics Deployment Services қолжетімдігін қамтамасыз етіңіз</span><span class="sxs-lookup"><span data-stu-id="8ecbd-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="8ecbd-120">[Microsoft Azure шот фактурасын жазу](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) тармағына өтіңіз және жазылымыңызды таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="8ecbd-121">Dynamics Deploy Services орталарды орналастыра алу үшін осы жазылымға қол жеткізуі керек.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![Azure жазылым мәліметтері](./media/6AzureSubscription.png)

2. <span data-ttu-id="8ecbd-123">Шарлау тақтасында **Қатынауды басқару (IAM)** опциясын таңдаңыз, содан кейін **Рөл тағайындауды қосу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="8ecbd-124">Оң жақтағы жүгірткіден **Салымшы рөлі** опциясын таңдаңыз және берілген тізімнен **Dynamics Deployment Services** қызметтерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="8ecbd-125">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-125">Select **Save**.</span></span>

![Жазылымға кіру](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="8ecbd-127">LCS жобасына Azure жазылым коннекторын қосу</span><span class="sxs-lookup"><span data-stu-id="8ecbd-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="8ecbd-128">Сіздің LCS жобаңызда **Microsoft Azure параметрлері** бетінде жаңа коннекторды қосу үшін **Қосу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="8ecbd-129">Azure жазылым идентификатор нөмірін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="8ecbd-130">Сіз Azure жазылым идентификаторын [Azure порталы](https://ms.portal.azure.com/), **Параметрлер** астында, экранның төменгі сол жағынан таба аласыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="8ecbd-131">**Azure Resource Manager мүмкіндігін пайдалану үшін конфигурациялау** өрісінде **Иә** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="8ecbd-132">Azure жазылымы AAD қатысушы домені сіз қолданып отырған домен иеленуші Azure жазылымымен сәйкес келетініне көз жеткізіп, **Келесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="8ecbd-133">Растау үшін **Microsoft Azure орнату** экранында **Келесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="8ecbd-134">Осы экранда қате пайда болса, осы тақырыптағы [Azure жазылымына Dynamics Deployment Services қолжетімдігін қамтамасыз ету](#provide) бөліміне оралыңыз және барлық қадамдарды орындағаныңызға көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="8ecbd-135">Azure басқару куәлігін компьютердегі жергілікті қалтаға жүктеңіз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-135">Download the Azure Management Certificate to a local folder on your computer.</span></span> <span data-ttu-id="8ecbd-136">Azure жазылым әкімшісінен жазылымды таңдап, **Параметрлер** > **Басқару куәліктері** терезесіне өту арқылы сертификатты Azure басқару порталына жүктеп салуын сұраңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-136">Ask your Azure subscription administrator to upload the certificate to Azure Management Portal by selecting the subscription and going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="8ecbd-137">Бұл сертификат LCS қызметіне Azure жүйесімен өз атыңыздан байланысуға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-137">This certificate enables LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="8ecbd-138">Пайдаланушының жазылымға қолжетімділігі бар болса, бұл қадамды өткізіп жіберуге болады.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-138">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="8ecbd-139">**Келесі** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-139">Select  **Next**.</span></span>
8. <span data-ttu-id="8ecbd-140">Орнатылатын Azure аймағын таңдап, осы жүйені пайдаланғыңыз келетін жақын жерден деректер орталығын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-140">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="8ecbd-141">**Қосылу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-141">Select  **Connect**.</span></span>

<span data-ttu-id="8ecbd-142">Сіз Azure жазылымына сәтті қосылдыңыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-142">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="8ecbd-143">Сіз енді Dynamics 365 Finance қызметін бұлт қызметтеріне орналастырылған орталарға орналастыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="8ecbd-143">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
