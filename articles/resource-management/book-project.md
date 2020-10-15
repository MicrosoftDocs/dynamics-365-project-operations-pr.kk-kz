---
title: Жобаға тапсырыс беру
description: Бұл тақырыпта жобаға ресурсты резервтеу туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 19128264ed3db7efeeba948155f0ddbdc806c2a0
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908327"
---
# <a name="book-to-a-project"></a><span data-ttu-id="1ab2f-103">Жобаға тапсырыс беру</span><span class="sxs-lookup"><span data-stu-id="1ab2f-103">Book to a project</span></span>

<span data-ttu-id="1ab2f-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="1ab2f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1ab2f-105">Жоба менеджері немесе ресурс менеджері жалпы топ мүшесінен нақты талап анықталмай, жобаға ресурс бөлуі қажет болатын кездер болады.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-105">There are times where a Project manager or Resource manager will need to allocate a resource to project without a specific requirement being defined from a generic team member.</span></span> <span data-ttu-id="1ab2f-106">Бұған үш жолдың бірімен қол жеткізуге болады.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-106">This can be achieved in one of three ways.</span></span>

- <span data-ttu-id="1ab2f-107">Топ мүшесі торынан резервтеу</span><span class="sxs-lookup"><span data-stu-id="1ab2f-107">Book from the team member grid</span></span>
- <span data-ttu-id="1ab2f-108">Кесте тақтасынан тапсырыс беру</span><span class="sxs-lookup"><span data-stu-id="1ab2f-108">Book from the schedule board</span></span>
- <span data-ttu-id="1ab2f-109">**Жоба** пішінінен резервтеу</span><span class="sxs-lookup"><span data-stu-id="1ab2f-109">Book from the **Project** form</span></span>

## <a name="book-from-the-team-member-grid"></a><span data-ttu-id="1ab2f-110">Топ мүшесі торынан резервтеу</span><span class="sxs-lookup"><span data-stu-id="1ab2f-110">Book from the team member grid</span></span>

<span data-ttu-id="1ab2f-111">Егер ұйымыңыз Ресурстарды бөлудің гибридті режимінде жұмыс істейтін болса, жоба менеджері келесі қадамдарды орындау арқылы ресурстарды жобаға тікелей резервтей алады.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-111">If your organization is operating in hybrid Resource allocation mode, the Project manager can book a resource directly to the project by completing the following steps.</span></span>

1. <span data-ttu-id="1ab2f-112">Жобадан топ мүшелерінің торына өтіп, **Жаңа** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-112">From the project, go to the team member grid and select **New**.</span></span>
2. <span data-ttu-id="1ab2f-113">Ресурстың орын атауы мен рөлін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-113">Define the position name and the role of the resource.</span></span>
3. <span data-ttu-id="1ab2f-114">Қолжетімді іздеу ішінен брондауға болатын ресурстарды таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-114">Select the bookable resource from the available lookup.</span></span>
4. <span data-ttu-id="1ab2f-115">Ресурсты таңдағаннан кейін, ресурстарды брондау үшін өріс туралы келесі ақпаратты анықтаңыз:</span><span class="sxs-lookup"><span data-stu-id="1ab2f-115">After you select the resource, define the following field information to book the resource:</span></span>

    - <span data-ttu-id="1ab2f-116">Басталу күні</span><span class="sxs-lookup"><span data-stu-id="1ab2f-116">Start date</span></span>
    - <span data-ttu-id="1ab2f-117">Аяқталу күні</span><span class="sxs-lookup"><span data-stu-id="1ab2f-117">Finish date</span></span>
    - <span data-ttu-id="1ab2f-118">Тағайындау әдісі</span><span class="sxs-lookup"><span data-stu-id="1ab2f-118">Allocation method</span></span>
    - <span data-ttu-id="1ab2f-119">Қажет болса, сағаттар</span><span class="sxs-lookup"><span data-stu-id="1ab2f-119">Hours, if applicable</span></span>
    - <span data-ttu-id="1ab2f-120">Жоба бекітушісі</span><span class="sxs-lookup"><span data-stu-id="1ab2f-120">Project approver</span></span>

6. <span data-ttu-id="1ab2f-121">**Сақтау және жабу** опциясын таңдаңыз</span><span class="sxs-lookup"><span data-stu-id="1ab2f-121">Select **Save and Close**</span></span>

## <a name="book-from-the-schedule-board"></a><span data-ttu-id="1ab2f-122">Кесте тақтасынан тапсырыс беру</span><span class="sxs-lookup"><span data-stu-id="1ab2f-122">Book from the schedule board</span></span>

<span data-ttu-id="1ab2f-123">Ресурстар менеджері ресурстарды жобаға тікелей резервтеу қажет болғанда, олар кесте тақтасын және жоба талаптарын қолдана алады.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-123">When a Resource manager needs to book a resource directly to a project, they can use the schedule board and the project requirement.</span></span> <span data-ttu-id="1ab2f-124">Жоба талабы - бұл әрдайым тапсырыс беруге болатын ресурстарға деген талап.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-124">The project requirement is a resource requirement that is always available to be booked against.</span></span> <span data-ttu-id="1ab2f-125">Кесте тақтасынан жобаға тікелей резервтеу үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-125">To book directly to a project form the schedule board, complete the following steps.</span></span>

1. <span data-ttu-id="1ab2f-126">Кесте тақтасын және сол жақ бетті шарлаңыз, талап етілетін ресурстарды сүзіп алыңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-126">Navigate to the schedule board and on the left page, filter for the resources you are considering for the requirement.</span></span>
2. <span data-ttu-id="1ab2f-127">Төменгі тақтада, жоба талаптарының тізімін қарау үшін **Жоба** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-127">In the bottom pane, select the **Project** tab to view a list of project requirements.</span></span>
3. <span data-ttu-id="1ab2f-128">Талапты ресурсқа апарып, келесі ақпаратты анықтаңыз:</span><span class="sxs-lookup"><span data-stu-id="1ab2f-128">Drag the requirement onto a resource and define the following information:</span></span>

    - <span data-ttu-id="1ab2f-129">Басталу күні</span><span class="sxs-lookup"><span data-stu-id="1ab2f-129">Start date</span></span>
    - <span data-ttu-id="1ab2f-130">Аяқталу күні</span><span class="sxs-lookup"><span data-stu-id="1ab2f-130">Finish date</span></span>
    - <span data-ttu-id="1ab2f-131">Тапсырыс беру күйі</span><span class="sxs-lookup"><span data-stu-id="1ab2f-131">Booking status</span></span>
    - <span data-ttu-id="1ab2f-132">Тапсырыс беру әдісі</span><span class="sxs-lookup"><span data-stu-id="1ab2f-132">Booking method</span></span>
    - <span data-ttu-id="1ab2f-133">Ұзақтық</span><span class="sxs-lookup"><span data-stu-id="1ab2f-133">Duration</span></span>

## <a name="book-from-the-project-form"></a><span data-ttu-id="1ab2f-134">Жоба пішінінен резервтеу</span><span class="sxs-lookup"><span data-stu-id="1ab2f-134">Book from the Project form</span></span>

<span data-ttu-id="1ab2f-135">Жоба менеджері ретінде сізге жобаға ресурстарды брондау қажет болуы мүмкін, бірақ тек ресурстардың атауын емес, критерийлерді де білу қажет.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-135">As a Project manager, you might need to book a resource to a project, but only know the criteria rather than the name of the resource.</span></span> <span data-ttu-id="1ab2f-136">Ресурстың кез-келген қолжетімді төлсипаттарына негізделген ресурстарды табу мақсатында кесте көмекшісін пайдалану үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-136">Complete the following steps to use the schedule assistant to find a resource based on any available attributes of the resource.</span></span> 

1. <span data-ttu-id="1ab2f-137">Жобаға өтіп, кесте көмекшісін ашу үшін **Резервтеу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-137">Navigate to the project and select **Book** to open the Schedule Assistant.</span></span>
2. <span data-ttu-id="1ab2f-138">Кесте көмекшісінің сол жағындағы сүзгілерді пайдалану арқылы критерийлерді кішірейтіп, **Іздеу** параметрін ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-138">Using the filters on the left side of the Schedule Assistant, narrow the criteria and select **Search.**</span></span>
3. <span data-ttu-id="1ab2f-139">Нәтижесінде қайтарылған ресурстарға сүйене отырып, ресурстарды резервтей аласыз.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-139">Based on resources returned in the results, you can book a resource.</span></span>

> [!NOTE]
> <span data-ttu-id="1ab2f-140">Бұл әдіс ресурсқа ешқандай резерв жасамайды.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-140">This method doesn't create any bookings for the resource.</span></span> <span data-ttu-id="1ab2f-141">Орнына, ресурсты топқа қосады.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-141">Instead, it adds the resource to the team.</span></span> <span data-ttu-id="1ab2f-142">Топ мүшесі жобаға қосылғаннан кейін, жоба менеджері ресурстарға қажетті резервті қосу үшін резервтеуді қолдана алады немесе кеңейте алады.</span><span class="sxs-lookup"><span data-stu-id="1ab2f-142">After the team member has been added to the project, the project manager can use maintain bookings or extend bookings to add the required bookings to the resource.</span></span>
