---
title: Project Operations ресурстық/қосалқы емес сценарийлерге арналған Project Operations алдын ала қарау жазылымдарына кіру
description: Бұл тақырыпта ресурстық/қосалқы емес негіздегі сценарийлер үшін Project Operations жүйесіне жазылу және орналастыру туралы ақпарат берілген.
author: sigitac
ms.date: 10/07/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 1b8c8982ede83191ce346e76718322d47abf0dd8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000443"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="20d14-103">Project Operations ресурстық/қосалқы емес сценарийлерге арналған Project Operations алдын ала қарау жазылымдарына кіру</span><span class="sxs-lookup"><span data-stu-id="20d14-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="20d14-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="20d14-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="20d14-105">Бұл тақырып алдын ала қарау/серіктестік ұсынысқа жазылуды және ресурстық/қосалқы негіздегі сценарийлер үшін Project Operations ортасын орналастыру туралы ақпарат береді.</span><span class="sxs-lookup"><span data-stu-id="20d14-105">This topic explains how to subscribe to the preview/partner offer and deploy Project Operations environment for resource/ non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20d14-106">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="20d14-106">Prerequisites</span></span>

- <span data-ttu-id="20d14-107">Сізге алдын ала қарауға қатысуға шақыратын электрондық хат келеді.</span><span class="sxs-lookup"><span data-stu-id="20d14-107">You will receive an email inviting you to participate in the preview.</span></span> <span data-ttu-id="20d14-108">алдын ала қарауды [Project Operations веб-сайтынан](https://dynamics.microsoft.com/en-us/project-operations/overview/) сұратуға болады.</span><span class="sxs-lookup"><span data-stu-id="20d14-108">You can request a preview on the [Project Operations website](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span></span>
- <span data-ttu-id="20d14-109">Алдын ала қарауды орналастыратын пайдаланушының Azure қатысушысының басты әкімші құқықтары болуы керек.</span><span class="sxs-lookup"><span data-stu-id="20d14-109">The user who deploys the preview must have Azure tenant global administrator rights.</span></span>
- <span data-ttu-id="20d14-110">Finance ортасын орналастыру үшін әр ортаға ұсынылатын жарамды Azure жазылымы қажет.</span><span class="sxs-lookup"><span data-stu-id="20d14-110">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="20d14-111">Бастау үшін ұйымдарыңыздың бар жазылып немесе [Azure сынақ кезеңін](https://azure.microsoft.com/en-us/free/) пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="20d14-111">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="20d14-112">CDS ортасы шектеулі 30 күндік мерзімге тегін беріледі.</span><span class="sxs-lookup"><span data-stu-id="20d14-112">The CDS environment will be provided free for a limited 30 day period.</span></span>

## <a name="subscribe"></a><span data-ttu-id="20d14-113">Жазылу</span><span class="sxs-lookup"><span data-stu-id="20d14-113">Subscribe</span></span>

<span data-ttu-id="20d14-114">Сіздегі [алдын ала қарауды сұрау](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) расталған кезде, сізге Microsoft корпорациясынан электрондық пошта арқылы үш ұсыныс жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="20d14-114">When your [preview request](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) is approved, you will receive three offers from Microsoft by email.</span></span> <span data-ttu-id="20d14-115">Бұл ұсыныстар Project Operations алдын ала қарауын орналастыруға мүмкіндік береді:</span><span class="sxs-lookup"><span data-stu-id="20d14-115">These offers allow you to deploy the Project Operations Preview:</span></span>

- <span data-ttu-id="20d14-116">Dynamics 365 Project Operations (CRM) - алдын ала қарау сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="20d14-116">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span>
- <span data-ttu-id="20d14-117">Office 365 Project Operations - алдын ала қарау сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="20d14-117">Office 365 Project Operations - Preview Trial</span></span>
- <span data-ttu-id="20d14-118">Dynamics 365 Finance - алдын ала қарау сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="20d14-118">Dynamics 365 Finance - Preview Trial</span></span>

> [!IMPORTANT]
> <span data-ttu-id="20d14-119">Бұл тапсырманы ұйымда тек бір адам, яғни қатысушы әкімші орындауы қажет.</span><span class="sxs-lookup"><span data-stu-id="20d14-119">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="20d14-120">Егер сіз осы шығарылымның жазылушысы болмасаңыз, ұйымның тіркеліп, пайдаланушы тіркелгі деректерін алғанға дейін күтіңіз.</span><span class="sxs-lookup"><span data-stu-id="20d14-120">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>

### <a name="dynamics-365-project-operations-crm---preview-trial"></a><span data-ttu-id="20d14-121">Dynamics 365 Project Operations (CRM) - алдын ала қарау сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="20d14-121">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span> 

<span data-ttu-id="20d14-122">Бастамас бұрын, браузерге Project Operations алдын ала қарауды қалайтын пайдаланушының жұмыс тіркелгісімен кіргеніңізге көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="20d14-122">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="20d14-123">**Dynamics 365 Project Operations (CRM) - алдын ала қарау сынақ нұсқасы** бірінші ұсыныс кодын шолғыш URL мекенжайына қою арқылы оны белсендіріңіз.</span><span class="sxs-lookup"><span data-stu-id="20d14-123">Redeem the first offer code, **Dynamics 365 Project Operations (CRM) - Preview Trial** by pasting it into the browser URL.</span></span>

![Ұсынысты белсендіру](./media/16RedeemFirstOfferNew.png)

2. <span data-ttu-id="20d14-125">Тапсырысыңызды растаңыз.</span><span class="sxs-lookup"><span data-stu-id="20d14-125">Confirm your order.</span></span>

![Тапсырысты растау](./media/17ConfirmOrderNew.png)

<span data-ttu-id="20d14-127">Растау ұсынысы сәтті өтелгенін көресіз.</span><span class="sxs-lookup"><span data-stu-id="20d14-127">You will see confirmation offer was successfully redeemed.</span></span>

![Расталым](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a><span data-ttu-id="20d14-129">Office 365 Project Operations - алдын ала қарау сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="20d14-129">Office 365 Project Operations - Preview Trial</span></span>

<span data-ttu-id="20d14-130">Бірінші ұсыныс кодындағыдай қадамдарды қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="20d14-130">Repeat the same steps as with the first offer code.</span></span> <span data-ttu-id="20d14-131">Екінші ұсыныс кодын бірінші ұсыныс кодымен пайдаланылған пайдаланушы тіркелгісі арқылы қосқаныңызға көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="20d14-131">Make sure to add the second offer code using the same user account that was used with the first offer code.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="20d14-132">Dynamics 365 Finance алдын ала қарау сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="20d14-132">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="20d14-133">Дәл осы әрекеттерді сәлемдесу электрондық пошта хабарынан соңғы ұсынысымен қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="20d14-133">Repeat the same steps with the last offer from the Welcome email.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="20d14-134">Лицензияларды тағайындау</span><span class="sxs-lookup"><span data-stu-id="20d14-134">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="20d14-135">Келесі қадамдарды орындау үшін ұйымыңыздың Microsoft 365 порталына арналған әкімшілік қатынас қажет.</span><span class="sxs-lookup"><span data-stu-id="20d14-135">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="20d14-136">Пайдаланушыларыңызға лицензияларды тағайындау үшін [Microsoft 365 басқару орталығына](https://portal.office.com/) өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="20d14-136">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

![Басқару орталығының басты беті](./media/14AdminPortal.png)

2. <span data-ttu-id="20d14-138">**Белсенді пайдаланушылар** бетінен лицензияны тағайындағыңыз келетін пайдаланушыларды таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="20d14-138">On the **Active users** page, select the users that you want to assign a license to.</span></span>

![Лицензияларды тағайындау](./media/15AssignLicenses.png)

3. <span data-ttu-id="20d14-140">**Dynamics 365 Project Operations (CRM) алдын ала қарау** және **Office 365 Project Operations - алдын ала қарау** лицензиясының таңдалғанын тексеріп, **Өзгерістерді сақтау** түймесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="20d14-140">Verify that the **Dynamics 365 Project Operations (CRM) Preview** and **Office 365 Project Operations - Preview** license have been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="20d14-141">Finance сынақ ұсынысын пайдаланушыға тағайындаудың қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="20d14-141">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="20d14-142">LCS параметрінде жаңа жобаны бастау</span><span class="sxs-lookup"><span data-stu-id="20d14-142">Start a new project in LCS</span></span>

<span data-ttu-id="20d14-143">Тақырыпта сипатталғандай жаңа LCS жобасын жасаңыз,[ LCS қызметінде жаңа жобаны бастаңыз](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="20d14-143">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="20d14-144">LCS жобасына Azure жазылымын қосу</span><span class="sxs-lookup"><span data-stu-id="20d14-144">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="20d14-145">Бұл тапсырманы орындау үшін тақырыптағы қадамдарды орындаңыз, [LCS жобасына Azure жазылымын қосыңыз](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="20d14-145">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="20d14-146">Ресурстық/қосалқы емес сценарийлерге арналған Project Operations жүйесі үшін Finance демо-ортасын орналастыру</span><span class="sxs-lookup"><span data-stu-id="20d14-146">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="20d14-147">Орналастыруды аяқтау үшін тақырыптағы нұсқауларды орындаңыз, [Жаңа ортаны дайындаңыз](resource-provision-new-environment.md).</span><span class="sxs-lookup"><span data-stu-id="20d14-147">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="20d14-148">Алдын ала қарау үшін [демо-орта](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) орналастыру түрін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="20d14-148">Use the [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="20d14-149">CDS параметрі және конфигурация деректерін орнату</span><span class="sxs-lookup"><span data-stu-id="20d14-149">Install CDS setup and configuration data</span></span>

<span data-ttu-id="20d14-150">CDS баптау және конфигурация туралы деректерді тақырыпта сипатталғандай орнатыңыз, [Common Data Service қызметіндегі конфигурация деректерін орнатыңыз және қолданыңыз](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="20d14-150">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="20d14-151">Бұл қадамды Finance демо ортасы орнатылғаннан және құрылымдық жұмыс тапсырысы демо деректері дайын болғаннан кейін ғана орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="20d14-151">Complete this step only after Finance demo environment is deployed and demo data in FO is ready.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]