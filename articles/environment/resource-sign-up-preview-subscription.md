---
title: Project Operations ресурстық/қосалқы емес сценарийлерге арналған Project Operations алдын ала қарау жазылымдарына кіру
description: Бұл тақырыпта ресурстық/қосалқы емес негіздегі сценарийлер үшін Project Operations жүйесіне жазылу және орналастыру туралы ақпарат берілген.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: da93fcf23ee3f255812842e31cb22b5d39daa963
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334834"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="1b7e7-103">Project Operations ресурстық/қосалқы емес сценарийлерге арналған Project Operations алдын ала қарау жазылымдарына кіру</span><span class="sxs-lookup"><span data-stu-id="1b7e7-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="1b7e7-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="1b7e7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="1b7e7-105">Бұл тақырып сынақ нұсқасы ұсынысына жазылу және ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations бағдарламасын орналастыру жолын түсіндіреді.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-105">This topic explains how to subscribe to the trial offer and deploy Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b7e7-106">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="1b7e7-106">Prerequisites</span></span>
- <span data-ttu-id="1b7e7-107">Алдын ала қарауды орналастыратын пайдаланушының Azure қатысушысының басты әкімші құқықтары болуы керек.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-107">The user who deploys the preview must have Azure tenant global administrator rights.</span></span> <span data-ttu-id="1b7e7-108">Бірінші ұсыныс өтелімі кезінде қатысушыны жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-108">You can create a tenant during the first offer redemption.</span></span> 
- <span data-ttu-id="1b7e7-109">Finance ортасын орналастыру үшін әр ортаға ұсынылатын жарамды Azure жазылымы қажет.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-109">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="1b7e7-110">Бастау үшін ұйымдарыңыздың бар жазылып немесе [Azure сынақ кезеңін](https://azure.microsoft.com/en-us/free/) пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-110">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="1b7e7-111">CDS ортасы шектеулі 30 күндік мерзімге тегін беріледі.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-111">The CDS environment will be provided free for a limited 30 day period.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1b7e7-112">Бұл тапсырманы ұйымда тек бір адам, яғни қатысушы әкімші орындауы қажет.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-112">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="1b7e7-113">Егер сіз осы шығарылымның жазылушысы болмасаңыз, ұйымның тіркеліп, пайдаланушы тіркелгі деректерін алғанға дейін күтіңіз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-113">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>
> 
> <span data-ttu-id="1b7e7-114">Сынақ нұсқалары қатысушыда бір рет қолданылады.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-114">Trials are single use in the tenant.</span></span> <span data-ttu-id="1b7e7-115">Сынақ нұсқасын тек бір рет ғана іске қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-115">You can only run a trial one time.</span></span> <span data-ttu-id="1b7e7-116">Сынақ нұсқасы үшін жаңа қатысушы жасауға кеңес береміз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-116">We recommend that you create a new tenant for the purpose of the trial.</span></span>


### <a name="dynamics-365-project-operations-ce---preview-trial"></a><span data-ttu-id="1b7e7-117">Dynamics 365 Project Operations (CE) - алдын ала қарау сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="1b7e7-117">Dynamics 365 Project Operations (CE) - Preview Trial</span></span> 

<span data-ttu-id="1b7e7-118">Бастамас бұрын, браузерге Project Operations алдын ала қарауды қалайтын пайдаланушының жұмыс тіркелгісімен кіргеніңізге көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-118">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="1b7e7-119">**Dynamics 365 Project Operations** алғашқы ұсыныс кодын осы жерде [Project Operations сынақ нұсқасында](https://aka.ms/try-po) белсендіріңіз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-119">Redeem the first offer code, **Dynamics 365 Project Operations** here [Project Operations Trial](https://aka.ms/try-po).</span></span>
2. <span data-ttu-id="1b7e7-120">Тапсырысыңызды растаңыз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-120">Confirm your order.</span></span>

  <span data-ttu-id="1b7e7-121">Растау ұсынысы сәтті өтелгенін көресіз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-121">You will see confirmation offer was successfully redeemed.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="1b7e7-122">Dynamics 365 Finance алдын ала қарау сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="1b7e7-122">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="1b7e7-123">[Dynamics 365 for Finance алдын-ала қарау сынақ нұсқасы](https://aka.ms/trypoche) бетіне өтіңіз және алдыңғы бөлімдегі қадамдарды ұсыныспен қайталаңыз, бұлт орналастырылған хостингті ортаға тіркеліңіз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-123">Go to [Dynamics 365 for Finance Preview Trial](https://aka.ms/trypoche) and repeat the steps from the previous section with the offer, Sign up for the Cloud Hosted Environment.</span></span>  

## <a name="assign-licenses"></a><span data-ttu-id="1b7e7-124">Лицензияларды тағайындау</span><span class="sxs-lookup"><span data-stu-id="1b7e7-124">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1b7e7-125">Келесі қадамдарды орындау үшін ұйымыңыздың Microsoft 365 порталына арналған әкімшілік қатынас қажет.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-125">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="1b7e7-126">Пайдаланушыларыңызға лицензияларды тағайындау үшін [Microsoft 365 басқару орталығына](https://portal.office.com/) өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-126">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

2. <span data-ttu-id="1b7e7-127">**Белсенді пайдаланушылар** бетінен лицензияны тағайындағыңыз келетін пайдаланушыларды таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-127">On the **Active users** page, select the users that you want to assign a license to.</span></span>

3. <span data-ttu-id="1b7e7-128">**Dynamics 365 Project Operations** лицензиясының таңдалғанын тексеріңіз және **Өзгерістерді сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-128">Verify that the **Dynamics 365 Project Operations** license has been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="1b7e7-129">Finance сынақ ұсынысын пайдаланушыға тағайындаудың қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-129">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="1b7e7-130">LCS параметрінде жаңа жобаны бастау</span><span class="sxs-lookup"><span data-stu-id="1b7e7-130">Start a new project in LCS</span></span>

<span data-ttu-id="1b7e7-131">Тақырыпта сипатталғандай жаңа LCS жобасын жасаңыз,[ LCS қызметінде жаңа жобаны бастаңыз](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="1b7e7-131">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="1b7e7-132">LCS жобасына Azure жазылымын қосу</span><span class="sxs-lookup"><span data-stu-id="1b7e7-132">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="1b7e7-133">Бұл тапсырманы орындау үшін тақырыптағы қадамдарды орындаңыз, [LCS жобасына Azure жазылымын қосыңыз](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="1b7e7-133">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="1b7e7-134">Ресурстық/қосалқы емес сценарийлерге арналған Project Operations жүйесі үшін Finance демо-ортасын орналастыру</span><span class="sxs-lookup"><span data-stu-id="1b7e7-134">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="1b7e7-135">Орналастыруды аяқтау үшін тақырыптағы нұсқауларды орындаңыз, [Жаңа ортаны дайындаңыз](resource-provision-new-environment.md).</span><span class="sxs-lookup"><span data-stu-id="1b7e7-135">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="1b7e7-136">Алдын ала қарау үшін [демо-орта](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) орналастыру түрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-136">Use the [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="1b7e7-137">CDS параметрі және конфигурация деректерін орнату</span><span class="sxs-lookup"><span data-stu-id="1b7e7-137">Install CDS setup and configuration data</span></span>

<span data-ttu-id="1b7e7-138">CDS баптау және конфигурация туралы деректерді тақырыпта сипатталғандай орнатыңыз, [Common Data Service қызметіндегі конфигурация деректерін орнатыңыз және қолданыңыз](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="1b7e7-138">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="1b7e7-139">Бұл қадамды қаржы демо ортасы орналастырылғаннан кейін және демо деректер дайын болғаннан кейін ғана орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="1b7e7-139">Complete this step only after Finance demo environment is deployed and demo data is ready.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
