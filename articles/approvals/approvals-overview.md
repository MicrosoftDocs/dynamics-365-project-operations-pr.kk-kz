---
title: Бекітулерге шолу
description: Бұл тақырыпта Project Operations бағдарламасындағы растаулармен жұмыс істеу туралы ақпарат берілген.
author: stsporen
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 37994422e9146765076fdbb77f5c763b4f1d0802
ms.sourcegitcommit: 2cf93d8bf0be5b61a739195a41334c34d910e9ba
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961173"
---
# <a name="approvals-overview"></a><span data-ttu-id="fa465-103">Бекітулерге шолу</span><span class="sxs-lookup"><span data-stu-id="fa465-103">Approvals overview</span></span>

<span data-ttu-id="fa465-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="fa465-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="fa465-105">Уақыт пен шығыстарды жіберу мақұлдаудың жұмыс ағыны арқылы өтеді.</span><span class="sxs-lookup"><span data-stu-id="fa465-105">Time and Expense submissions move through an approval workflow.</span></span> <span data-ttu-id="fa465-106">Жазбалар мақұлданғаннан кейін, транзакциялар нақты көрсеткіштерге жазылады немесе уақыт кестеге жазылады.</span><span class="sxs-lookup"><span data-stu-id="fa465-106">After the entries are approved, transactions are recorded in actuals or time is booked in the schedule.</span></span>

## <a name="approvals-workflow"></a><span data-ttu-id="fa465-107">Мақұлдаудың жұмыс ағыны</span><span class="sxs-lookup"><span data-stu-id="fa465-107">Approvals workflow</span></span>
<span data-ttu-id="fa465-108">Уақыт немесе шығыс жазбасын жасап, жіберген кезде, мақұлдау жазбасы жасалады.</span><span class="sxs-lookup"><span data-stu-id="fa465-108">When you create and submit a time or expense entry, an approval entry is created.</span></span> <span data-ttu-id="fa465-109">Жоба бекітушісі немесе менеджер сіздің жазбаңызды қарап, мақұлдайды.</span><span class="sxs-lookup"><span data-stu-id="fa465-109">The Project approver or your manager reviews and approves your entry.</span></span> <span data-ttu-id="fa465-110">Егер жазба жобамен қатысты болса, ол мақұлданған кезде нақты көрсеткіштер жасалады.</span><span class="sxs-lookup"><span data-stu-id="fa465-110">If the entry is related to a project, when it's approved, the actuals will be created.</span></span> <span data-ttu-id="fa465-111">Бұл құн мен төлемдерді бақылауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="fa465-111">This allows the cost and billing to be tracked.</span></span> 

## <a name="approve-an-entry"></a><span data-ttu-id="fa465-112">Жазбаны мақұлдау</span><span class="sxs-lookup"><span data-stu-id="fa465-112">Approve an entry</span></span>
<span data-ttu-id="fa465-113">**Мақұлдаулар** пішіні әртүрлі мақұлдауларды көре алу үшін түрлі көріністерді ауыстыруға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="fa465-113">The **Approvals** form allows you to switch between different views so that you can view the different types of approvals.</span></span>
  
1. <span data-ttu-id="fa465-114">**Мақұлдаулар** пішініне өтіп, **Шығыстар**, **Уақыт** немесе **Қайта шақырулар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-114">Go to the **Approvals** form and select **Expenses**, **Time**, or **Recalls**.</span></span>
2. <span data-ttu-id="fa465-115">Әр мақұлдауды қарап шығып, мақұлдау керек біреуін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-115">Review each approval, and select the ones you want to approve.</span></span>
3. <span data-ttu-id="fa465-116">Таңдалған жазбаларды мақұлдау үшін **Мақұлдау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-116">Select **Approve** to approve the selected entries.</span></span>
<span data-ttu-id="fa465-117">Жүйе бұл жазбаларды өңдейді және нақты көрсеткіштер немесе тапсырма жасайды.</span><span class="sxs-lookup"><span data-stu-id="fa465-117">The system will process these entries and create actuals or a booking.</span></span>

## <a name="reject-an-entry"></a><span data-ttu-id="fa465-118">Жазбаны қабылдамаңыз</span><span class="sxs-lookup"><span data-stu-id="fa465-118">Reject an entry</span></span>
<span data-ttu-id="fa465-119">Жобаны бекітуші ретінде пайдаланушыға түзету үшін жазбаны кері жіберуіңіз керек болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="fa465-119">As the Project approver, you may have to send an entry back to a user for correction.</span></span>
  
1. <span data-ttu-id="fa465-120">**Мақұлдаулар** пішініне өтіп, қабылдамау үшін жазбаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-120">Go to the **Approvals** form and select the entry to reject.</span></span> 
2. <span data-ttu-id="fa465-121">**Қабылдамау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-121">Select **Reject**.</span></span>
3. <span data-ttu-id="fa465-122">Қосымша - пайдаланушыға жазбаның не себепті қабылданбайтынын хабарлау үшін **Түсіндірмелерді қабылдамау** диалогтік терезесінде түсіндірме қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-122">Optional - Add a comment in the **Rejection Comments** dialog to inform the user why the entry is being rejected.</span></span>
4. <span data-ttu-id="fa465-123">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-123">Select **OK**.</span></span> <span data-ttu-id="fa465-124">Жазба пайдаланушыға қайтарылады.</span><span class="sxs-lookup"><span data-stu-id="fa465-124">The entry will be returned to the user.</span></span>
  
## <a name="recall-entries"></a><span data-ttu-id="fa465-125">Жазбаларды қайта шақыру</span><span class="sxs-lookup"><span data-stu-id="fa465-125">Recall entries</span></span>
<span data-ttu-id="fa465-126">Бір сәтте сізге жіберілген жазбаны қайта шақыру қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="fa465-126">At some point, you might need to recall a submitted entry.</span></span> <span data-ttu-id="fa465-127">Егер жазба мақұлданбаған болса, ол бірден қайтарылады.</span><span class="sxs-lookup"><span data-stu-id="fa465-127">If the entry has not been approved, it will be returned immediately.</span></span> <span data-ttu-id="fa465-128">Алайда мақұлданған жазба елеулі әсер етуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="fa465-128">An approved entry however, may have a material impact.</span></span> <span data-ttu-id="fa465-129">Жобаны бекітуші нақты көрсеткіштердегі транзакцияны қалпына келтіру үшін қайта шақыруды мақұлдауы керек.</span><span class="sxs-lookup"><span data-stu-id="fa465-129">The Project approver is required to approve the recall in order to reverse the transaction in Actuals.</span></span>

## <a name="specify-project-approvers"></a><span data-ttu-id="fa465-130">Жоба бекітушілерін көрсетіңіз</span><span class="sxs-lookup"><span data-stu-id="fa465-130">Specify Project approvers</span></span>
<span data-ttu-id="fa465-131">Әр жобада бірнеше жоба тобының мүшелері бар.</span><span class="sxs-lookup"><span data-stu-id="fa465-131">Each project has a number of project team members.</span></span> <span data-ttu-id="fa465-132">Сіз жобаның бекітушілері болып табылатын топ мүшелерін көрсете аласыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-132">You can specify which team members are also Project approvers.</span></span>

1. <span data-ttu-id="fa465-133">**Жобалар** пішініне өтіп, тізімнен жобаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-133">Go to the **Projects** form and open the project from the list.</span></span>
2. <span data-ttu-id="fa465-134">**Топ** қойыншасында, жоба бекітушісі болатын топ мүшесін таңдап, содан кейін **Өңдеу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-134">On the **Team** tab, select the team member who will be a Project approver and then select **Edit**.</span></span>
3. <span data-ttu-id="fa465-135">**Жоба бекітушісі** өрісін **Иә** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-135">Set the **Project Approver** field to **Yes**.</span></span>
4. <span data-ttu-id="fa465-136">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-136">Select **Save**.</span></span>
5. <span data-ttu-id="fa465-137">Қосымша жоба бекітушілерін қосу үшін 2-4 қадамдарын қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-137">Repeat steps 2-4 to add additional Project approvers.</span></span>

## <a name="configure-the-users-manager"></a><span data-ttu-id="fa465-138">Пайдаланушының менеджерін конфигурациялаңыз</span><span class="sxs-lookup"><span data-stu-id="fa465-138">Configure the user's manager</span></span>

1. <span data-ttu-id="fa465-139">**Параметрлер** > **Қауіпсіздік** > **Пайдаланушылар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="fa465-139">Go to **Settings** > **Security** > **Users**.</span></span>
2. <span data-ttu-id="fa465-140">Менеджер тағайындайтын пайдаланушыны таңдаңыз және **Ұйым туралы ақпарат** аймағында, тізімнен менеджерді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-140">Select the user to whom you are assigning a manager and in the **Organization Information** area, select the manager from the list.</span></span> 
3. <span data-ttu-id="fa465-141">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fa465-141">Select **Save**.</span></span>

