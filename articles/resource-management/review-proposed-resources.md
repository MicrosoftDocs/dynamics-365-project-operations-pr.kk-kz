---
title: Ұсынылған ресурстарды қарап шығу
description: Бұл тақырыпта жоба ресурстарын ұсыну жолы туралы ақпарат берілген.
author: ruhercul
manager: AnnBe
ms.date: 11/05/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 54a0924da17eac86e2fa400540e629f6d803aa35
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401180"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="d3fbf-103">Ұсынылған ресурстарды қарап шығу</span><span class="sxs-lookup"><span data-stu-id="d3fbf-103">Review proposed resources</span></span>

<span data-ttu-id="d3fbf-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="d3fbf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d3fbf-105">Ресурс менеджерлері ресурс сұрауын пайдалану арқылы жоба менеджеріне ресурстарды ұсына алады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="d3fbf-106">Сұрау торынан немесе сұраудың өзінен **Ресурстарды табу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="d3fbf-107">**Кесте көмекшісі** бетінде ресурсты таңдап, **Ресурсқа тапсырыс беруді жасау** тақтасындағы **Тапсырыс беру күйі** өрісінде **Тапсырыс беру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="d3fbf-108">Келесі күй жаңартулары пайда болады:</span><span class="sxs-lookup"><span data-stu-id="d3fbf-108">The following status updates occur:</span></span>

- <span data-ttu-id="d3fbf-109">**Кесте көмекшісі** бетінде тапсырыстың ұсынылғанын, бірақ қорытынды резервтелмегенін көрсету үшін күй индикаторлары жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="d3fbf-110">Ресурс сұрауында, күй **Қарап шығуды талап етеді** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="d3fbf-111">Жобаның **Топ** қойыншасында, жалпы топ мүшесінің **Сұрау күйі** мәні **Қарап шығуды талап етеді** мәніне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="d3fbf-112">Жоба менеджері ұсынысты қабылдай алады немесе одан бас тарта алады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="d3fbf-113">Ресурс менеджерлері ресурс сұрауларын өңдеген кезде келесі тәсілдердің кез келгенін пайдалана алады:</span><span class="sxs-lookup"><span data-stu-id="d3fbf-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="d3fbf-114">Егер қажетті сағаттарды орындау үшін бірде-бір ресурс болмаса, сұранысты қанағаттандыру үшін бірнеше ресурстарды ұсыну.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="d3fbf-115">Ұсынылған сағаттар қажетті сағаттарды қанағаттандыра алатын бірнеше ресурстар арасында бөлінеді.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="d3fbf-116">Бұл сценарийде сағаттар қабаттаспайды.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="d3fbf-117">Талап етілгеннен аз ресурстарды ұсыну.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="d3fbf-118">Бұл сценарийде ұсынылған ресурс сыйымдылығы сұрау салушы көрсеткен сағат санынан аз.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="d3fbf-119">Сондықтан сұрау салушы ұсынылған ресурстарды қабылдаған кезде, қалған сұранысты жинақтау үшін орындалмаған ресурс талабы жасалады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="d3fbf-120">Егер жұмысты орындау үшін бірде-бір ресурс болмаса, сұранысты қанағаттандыру үшін бірнеше ресурсты тіркеу.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="d3fbf-121">Талап етілгеннен аз ресурстарды тіркеу.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-121">Book fewer resources than are required.</span></span> <span data-ttu-id="d3fbf-122">Бұл сценарийде тіркелген сағат саны қажетті сағат санынан аз.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="d3fbf-123">Жүйе сізге тапсырыстардың орнына ресурстарды ұсынуға нұсқау береді, осылайша сұрау салушы қалған сұранысты тексеріп, оны бақылап отыра алады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="d3fbf-124">Ресурс қолжетімділігі</span><span class="sxs-lookup"><span data-stu-id="d3fbf-124">Resource availability</span></span>

<span data-ttu-id="d3fbf-125">Ресурс менеджерлерінің ресурстардың қолжетімділігін көре алатындығы және тапсырыстарды жаңарта алатындығы өте маңызды.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-125">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="d3fbf-126">Кейбір жағдайларда ресми сұраныс (ресурс сұрауы) жоқ, бірақ ресурс менеджері электрондық пошта, телефон қоңырауы немесе лездік хабар сияқты арналар арқылы келетін жоспарланбаған сұранысқа жауап беруі керек.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-126">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="d3fbf-127">Ресурс менеджерлері ресурстар мен тапсырыстарды жаңарту үшін кесте тақтасын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-127">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="d3fbf-128">Ресурстың қолжетімділігін есептеу үшін негіз ретінде ресурстың жұмыс сағаттары пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-128">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="d3fbf-129">Ресурс тапсырыстары ресурстардың мүмкіндіктерін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-129">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="d3fbf-130">Кесте тақтасы тапсырыстарды, мүмкіндікті және артық тапсырыстарды, сондай-ақ тапсырыстардың күйлерін көрсету үшін түстер мен көлеңкелеуді пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-130">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="d3fbf-131">Кесте тақтасы параметрлеріндегі параметр журналды көруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-131">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="d3fbf-132">Егер кесте тақтасындағы тапсырыс беруге болатын жеке ресурстың жанында оң жаққа бағыттаушы көрсеткі пайда болса, ресурс тіркелген жұмыс туралы мәліметтерді көрсету үшін ресурсты кеңейтуге болады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-132">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="d3fbf-133">Dynamics 365 Project Operations бағдарламасы Universal Resource Scheduling механизмін пайдаланғандықтан, сізде Dynamics 365 Field Service орнатылса, жобаларға, жұмыс тапсырыстарына және жоспарлауды кеңейткен басқа да нысандар үшін ресурс тапсырыстарының мәліметтерін көруге болады.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-133">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="d3fbf-134">Жеке ресурс туралы қосымша мәліметтерді көру үшін, ресурс картасын ашу үшін оны тінтуірдің оң жақ түймешігімен басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d3fbf-134">To view more details about an individual resource, right-click it to open the resource card.</span></span>

