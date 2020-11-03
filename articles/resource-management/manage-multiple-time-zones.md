---
title: Уақыт белдеулерін басқару
description: Жоба жасалған кезде оның уақыт белдеуі қолданылатын жұмыс уақытының үлгісінде белгіленген уақыт белдеуіне негізделеді.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 27f58f0dacc3404119a719547ad374629c740740
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079598"
---
# <a name="manage-time-zones"></a><span data-ttu-id="fb4df-103">Уақыт белдеулерін басқару</span><span class="sxs-lookup"><span data-stu-id="fb4df-103">Manage time zones</span></span>

<span data-ttu-id="fb4df-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="fb4df-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


## <a name="projects"></a><span data-ttu-id="fb4df-105">Жобалар</span><span class="sxs-lookup"><span data-stu-id="fb4df-105">Projects</span></span>

<span data-ttu-id="fb4df-106">Жоба жасалған кезде, уақыт белдеуі қолданылатын жұмыс уақытының үлгісінде белгіленген уақыт белдеуіне негізделеді.</span><span class="sxs-lookup"><span data-stu-id="fb4df-106">When a project is created, the time zone is based on the time zone defined in the applied work hour template.</span></span> <span data-ttu-id="fb4df-107">**Жоба** өрісінде, күндер әрдайым пайдаланушының тіркелген әр қойыншасының уақыт белдеуіне қатысты болады, **Тапсырма** қойыншасынан басқа. Жұмыс декомпозициясының құрылымын көрген кезде, күндер әрдайым жобаның уақыт белдеуінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fb4df-107">On the **Project** for, the dates are always relative to the time zone of the user that is logged in on each tab, except the **Task** tab. When you view the work breakdown structure, the dates will always be displayed in the project’s time zone.</span></span>

## <a name="tasks"></a><span data-ttu-id="fb4df-108">Тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="fb4df-108">Tasks</span></span>

<span data-ttu-id="fb4df-109">Тапсырма жасалған кезде, басталу уақыты, аяқталу уақыты және сағат/күн жобаның жұмыс сағатымен бақыланады.</span><span class="sxs-lookup"><span data-stu-id="fb4df-109">When a task is created, the start time, end time, and hours/day is controlled by the working hours of the project.</span></span> <span data-ttu-id="fb4df-110">Мысалы, егер тапсырма уақыт белдеуі -8 PST болатын жобамен жасалса және келесі жұмыс сағаты дүйсенбіден жұмаға дейін 9:00-ден 17:00-ге дейін болса, тағайындаусыз жасалған кез-келген тапсырма жоба күнтізбесінің басталу және аяқталу уақытына байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="fb4df-110">For example, if a task is created with a project whose time zone is -8 PST and has the following working hours: 9:00 AM to 5:00 PM Monday to Friday, any task created without an assignment will respect the start time and end time of the project calendar.</span></span>

## <a name="manage-resources-with-time-zones"></a><span data-ttu-id="fb4df-111">Ресурстарды уақыт белдеулерімен басқарыңыз</span><span class="sxs-lookup"><span data-stu-id="fb4df-111">Manage resources with time zones</span></span>

<span data-ttu-id="fb4df-112">**Брондауды ұзарту** параметрін пайдалану кезінде нақты және болжамды нәтижелерге ие болу үшін, орындалуы керек екі негізгі алғышарт бар:</span><span class="sxs-lookup"><span data-stu-id="fb4df-112">For accurate and predictable results when using **Extend Booking** , there are two key prerequisites that must be met:</span></span>  

- <span data-ttu-id="fb4df-113">Пайдаланушы құрылғының уақыт белдеуін жүйенің **Даралау параметрлерінде** анықталған уақыт белдеуіне сәйкес етіп теңшеуі керек.</span><span class="sxs-lookup"><span data-stu-id="fb4df-113">The user must configure their device's time zone to match the time zone defined in the system's **Personalization Settings**.</span></span>
 
  ![Windows 10 жүйесіндегі уақыт белдеуінің параметрлері](media/reconcile-assignments-03.png)

  ![Жекелендіру параметрлеріндегі уақыт белдеуінің параметрлері](media/reconcile-assignments-04.png)
 
- <span data-ttu-id="fb4df-116">Тапсырыс беруге болатын ресурста сұралған кеңейтімді анықтау үшін қолданылатын контурмен сәйкес келетін жұмыс уақытының кемінде бір минуты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="fb4df-116">The bookable resource must have at least one minute of working time that overlaps with the contours that are used to define the requested extension.</span></span> <span data-ttu-id="fb4df-117">Мысалы, жұмыс сағаты 9:00 мен 19:00 аралығында болатын келесі ресурстар.</span><span class="sxs-lookup"><span data-stu-id="fb4df-117">For example, the following resources with working hours that fall between 9:00 AM and 7:00 PM.</span></span> 

  ![Ресурс контурларын салыстыру](media/reconcile-assignments-05.png)

<span data-ttu-id="fb4df-119">Төмендегі кестеде келесілер көрсетілген:</span><span class="sxs-lookup"><span data-stu-id="fb4df-119">The following table shows:</span></span>

- <span data-ttu-id="fb4df-120">Жоба күнтізбесінің үлгісі</span><span class="sxs-lookup"><span data-stu-id="fb4df-120">A project calendar template</span></span>
- <span data-ttu-id="fb4df-121">А ресурсы: бұл ресурстың күнтізбесі бірдей және жобамен бірдей уақыт белдеуінде орналасқан.</span><span class="sxs-lookup"><span data-stu-id="fb4df-121">Resource A: This resource has the same calendar and is in the same time zone as the project.</span></span> <span data-ttu-id="fb4df-122">Тапсырыстардың басталу уақыты - 9:00.</span><span class="sxs-lookup"><span data-stu-id="fb4df-122">The start time of the bookings will be 9:00 AM.</span></span>
- <span data-ttu-id="fb4df-123">Б ресурсы: Бұл ресурс жобадан басқа уақыт белдеуінде орналасқан және олардың уақыт белдеуінде таңғы сағат 7: 00-де басталады.</span><span class="sxs-lookup"><span data-stu-id="fb4df-123">Resource B: This resource is located in a different time zone than the project and starts at 7:00 AM in their time zone.</span></span> <span data-ttu-id="fb4df-124">Алайда, тапсырыстар 9:00-де басталады, себебі бұл тапсырма контурының ең ерте басталу уақыты.</span><span class="sxs-lookup"><span data-stu-id="fb4df-124">However, the bookings will begin at 9:00 AM as that is the earliest start time of the assignment contour.</span></span>
- <span data-ttu-id="fb4df-125">C және D ресурстары: ресурстар әртүрлі уақыт белдеулерінде орналасқан, олар бір-бірінен де, жобадан да өзгеше, ал олардың броньдаулары сәйкес басталу уақытынан ерте басталады.</span><span class="sxs-lookup"><span data-stu-id="fb4df-125">Resources C and D: The resources are located in different time zones, both different from each other and the project, and their bookings start no earlier than their respective available start times.</span></span>

|<span data-ttu-id="fb4df-126">Нысан</span><span class="sxs-lookup"><span data-stu-id="fb4df-126">Entity</span></span>  |<span data-ttu-id="fb4df-127">Күнтізбе</span><span class="sxs-lookup"><span data-stu-id="fb4df-127">Calendar</span></span>  |
|-|-|
|<span data-ttu-id="fb4df-128">Жоба күнтізбесінің үлгісі</span><span class="sxs-lookup"><span data-stu-id="fb4df-128">Project calendar template</span></span>   | ![жоба күнтізбесі](media/reconcile-assignments-06.png) |
|<span data-ttu-id="fb4df-130">A ресурсы</span><span class="sxs-lookup"><span data-stu-id="fb4df-130">Resource A</span></span>  | ![A ресурсының күнтізбесі](media/reconcile-assignments-06.png) |
|<span data-ttu-id="fb4df-132">B ресурсы</span><span class="sxs-lookup"><span data-stu-id="fb4df-132">Resource B</span></span>  |  ![B ресурсының күнтізбесі](media/reconcile-assignments-07.png) |
|<span data-ttu-id="fb4df-134">C ресурсы</span><span class="sxs-lookup"><span data-stu-id="fb4df-134">Resource C</span></span>  |  ![C ресурсының күнтізбесі](media/reconcile-assignments-08.png) |
|<span data-ttu-id="fb4df-136">D ресурсы</span><span class="sxs-lookup"><span data-stu-id="fb4df-136">Resource D</span></span>  | ![D ресурсының күнтізбесі](media/reconcile-assignments-09.png)  |
 
<span data-ttu-id="fb4df-138">**Біріктіру** көрінісіне өткен кезде, ресурстарды тағайындаулар және онымен байланысты тапсырыс тапшылығы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="fb4df-138">When you navigate to the **Reconciliation** view, the resource assignments and the associated booking shortages are displayed.</span></span>

![Кеңейту алдындағы салыстыру көрінісі](media/reconcile-assignments-10.png)

<span data-ttu-id="fb4df-140">Кеңейту функциясы әр ресурс үшін қолданылғаннан кейін, әр ресурс үшін тапсырыстар сәтті ұзартылады, себебі әр ресурстардың жұмыс сағаты тапшылық контурымен қабаттасады.</span><span class="sxs-lookup"><span data-stu-id="fb4df-140">After the extend booking functionality has been used for each resource, bookings are successfully extended for each resource because each resource’s working hours overlapped with the contours of the shortage.</span></span>

![Тапсырыстың мерзімін ұзартқаннан кейінгі салыстыру көрінісі](media/reconcile-assignments-11.png) 

<span data-ttu-id="fb4df-142">Брондаудың басталу уақытындағы айырмашылықтарды көрсететін тапсырыстар мәліметтерін қарауды ұмытпаңыз.</span><span class="sxs-lookup"><span data-stu-id="fb4df-142">Notice that a closer look at the details of the bookings shows differences in the start time of the bookings.</span></span> <span data-ttu-id="fb4df-143">Брондау тапсырма контурының басталу уақытынан ерте және ресурстардың қолжетімді басталу уақытынан ерте басталады.</span><span class="sxs-lookup"><span data-stu-id="fb4df-143">The bookings start no earlier than the start time of the assignment contour and no earlier than the available start time of the resource.</span></span>

![Кесте тақтасындағы ресурстардың тапсырыстары](media/reconcile-assignments-12.png)
