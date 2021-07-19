---
title: Алдын ала қарау жазылымына тіркелу - жеңілдетілген
description: Бұл тақырыпта Project Operations жеңілдетілген орналастыру бағдарламасына жазылу және оны орналастыру амалы туралы ақпарат берілген - проформа-шотын ұсыну мәмілесі.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2b5a65f5e29915c349d40400ebbf3e4923b36a67
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334789"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a><span data-ttu-id="f93f2-103">Алдын ала қарау жазылымына тіркелу - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="f93f2-103">Sign up for a preview subscription - lite</span></span> 

<span data-ttu-id="f93f2-104">Бұл тақырып сынақ ұсынысына жазылу және Dynamics 365 Project Operations жеңілдетілген орналастыруын орналастыру әдісін түсіндіреді - проформа есеп‑‑шоты бойынша.</span><span class="sxs-lookup"><span data-stu-id="f93f2-104">This topic explains how to subscribe to the trial offer and deploy Dynamics 365 Project Operations lite deployment - deal to proforma invoicing.</span></span>

> [!NOTE]
> <span data-ttu-id="f93f2-105">Бұл процесс Project Operations алдағы шығарылымдарында өзгереді.</span><span class="sxs-lookup"><span data-stu-id="f93f2-105">This process will change in upcoming releases of Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f93f2-106">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="f93f2-106">Prerequisites</span></span>
- <span data-ttu-id="f93f2-107">Алдын ала қарауды орналастыратын пайдаланушының Azure қатысушысының басты әкімші құқықтары болуы керек.</span><span class="sxs-lookup"><span data-stu-id="f93f2-107">The user who deploys the preview must have Azure tenant global administrator rights.</span></span> <span data-ttu-id="f93f2-108">Бірінші ұсыныс өтелімі кезінде қатысушыны жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="f93f2-108">You can create a tenant during the first offer redemption.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f93f2-109">Бұл тапсырманы ұйымда тек бір адам, яғни қатысушы әкімші орындауы қажет.</span><span class="sxs-lookup"><span data-stu-id="f93f2-109">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="f93f2-110">Егер сіз осы шығарылымның жазылушысы болмасаңыз, ұйымның тіркеліп, пайдаланушы тіркелгі деректерін алғанға дейін күтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-110">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>
> 
> <span data-ttu-id="f93f2-111">Сынақ нұсқалары қатысушыда бір рет қолданылады.</span><span class="sxs-lookup"><span data-stu-id="f93f2-111">Trials are single use in the tenant.</span></span> <span data-ttu-id="f93f2-112">Сынақ нұсқасын тек бір рет ғана іске қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="f93f2-112">You can only run a trial one time.</span></span> <span data-ttu-id="f93f2-113">Сынақ нұсқасы үшін жаңа қатысушы жасауға кеңес береміз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-113">We recommend that you create a new tenant for the purpose of the trial.</span></span>

### <a name="dynamics-365-project-operations-trial"></a><span data-ttu-id="f93f2-114">Dynamics 365 Project Operations сынақ нұсқасы</span><span class="sxs-lookup"><span data-stu-id="f93f2-114">Dynamics 365 Project Operations trial</span></span> 

<span data-ttu-id="f93f2-115">Бастамас бұрын, браузерге Project Operations алдын ала қарауды қалайтын пайдаланушының жұмыс тіркелгісімен кіргеніңізге көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-115">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="f93f2-116">**Dynamics 365 Project Operations** алғашқы ұсыныс қодын белсендіру үшін [Project Operations сынақ нұсқасына](https://aka.ms/try-po) өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-116">Go to [Project Operations Trial](https://aka.ms/try-po) to redeem the first offer code, **Dynamics 365 Project Operations**.</span></span>
2. <span data-ttu-id="f93f2-117">Тапсырысыңызды растаңыз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-117">Confirm your order.</span></span>

  <span data-ttu-id="f93f2-118">Растау ұсынысы сәтті іске қосылғанын көресіз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-118">You'll see the confirmation offer was successfully redeemed.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="f93f2-119">Лицензияларды тағайындау</span><span class="sxs-lookup"><span data-stu-id="f93f2-119">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f93f2-120">Келесі қадамдарды орындау үшін ұйымыңыздың Microsoft 365 порталына арналған әкімшілік қатынас қажет.</span><span class="sxs-lookup"><span data-stu-id="f93f2-120">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>


1. <span data-ttu-id="f93f2-121">Пайдаланушыларыңызға лицензияларды тағайындау үшін [Microsoft 365 басқару орталығына](https://portal.office.com/) өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-121">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>
2. <span data-ttu-id="f93f2-122">**Белсенді пайдаланушылар** бетінен лицензияны тағайындағыңыз келетін пайдаланушыларды таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-122">On the **Active users** page, select the users that you want to assign a license to.</span></span>
3. <span data-ttu-id="f93f2-123">**Dynamics 365 Project Operations** лицензиясының таңдалғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-123">Verify that the **Dynamics 365 Project Operations** license is selected.</span></span> 
4. <span data-ttu-id="f93f2-124">**Өзгерістерді сақтау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-124">Select **Save changes**.</span></span>

## <a name="create-a-new-dataverse-environment"></a><span data-ttu-id="f93f2-125">Жаңа Dataverse ортасын жасау</span><span class="sxs-lookup"><span data-stu-id="f93f2-125">Create a new Dataverse environment</span></span>

1. <span data-ttu-id="f93f2-126">[Dataverse орналастыру үлгісі](lite-deployment.md) бөліміндегі нұсқауларды орындау арқылы жаңа Project Operations Dataverse орналастыру ортасын дайындаңыз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-126">Provision a new Project Operations Dataverse deployment environment by following instructions in the topic, [Dataverse deployment model](lite-deployment.md).</span></span> <span data-ttu-id="f93f2-127">Орта түрін таңдағанда, міндетті түрде **Сынақ (жазылымға негізделген)** пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-127">When you select the environment type, make sure to use **Trial (Subscription based)**.</span></span>

  ![Жаңа орта](./media/19CreateEnvironment.png)

2. <span data-ttu-id="f93f2-129">**Dynamics 365 бағдарламаларын қосу** параметрін таңдап, **Бағдарламаларды автоматты түрде орналастыру** өрісін бос қалдырыңыз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-129">Select the **Enable Dynamics 365 apps** setting, and leave **Automatically deploy these apps** blank.</span></span>  
3. <span data-ttu-id="f93f2-130">Орта жасау үшін **Сақтау** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-130">Select **Save** to create the environment.</span></span>

  ![Дерекқорды қосу](./media/20CreateEnvironment1.png)

4. <span data-ttu-id="f93f2-132">Орта жасалғаннан кейін, **Microsoft Dynamics 365 Project Operations** шешімін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-132">After the environment is created, install **Microsoft Dynamics 365 Project Operations** solution.</span></span> 

![Шешім орнату](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a><span data-ttu-id="f93f2-134">CDS конфигурациясын орнатып, демо деректерді реттеңіз</span><span class="sxs-lookup"><span data-stu-id="f93f2-134">Install a CDS configuration and setup demo data</span></span>

<span data-ttu-id="f93f2-135">[Демо нұсқа параметрлері мен конфигурация деректерін қолдану](lite-apply-demo-setup-config-data.md) бөліміндегі нұсқауларды орындау арқылы CDS конфигурациясын орнатып, демо деректерді реттеңіз.</span><span class="sxs-lookup"><span data-stu-id="f93f2-135">Install the CDS configuration and set up demo data by following instructions in the topic, [Apply demo setup and configuration data](lite-apply-demo-setup-config-data.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
