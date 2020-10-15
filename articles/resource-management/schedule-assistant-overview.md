---
title: Кесте көмекшісіне шолу
description: Бұл тақырып ресурстарға тапсырыс беру үшін кесте көмекшісімен жұмыс істеу туралы ақпарат береді.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: da551e805f395e466952df1dbb7d193bdddba358
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908310"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="03e88-103">Кесте көмекшісіне шолу</span><span class="sxs-lookup"><span data-stu-id="03e88-103">Schedule assistant overview</span></span>

<span data-ttu-id="03e88-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="03e88-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="03e88-105">Кесте көмекшісі жоба менеджері анықтаған талаптарға негізделген ресурстарға тапсырыс беруге арналған.</span><span class="sxs-lookup"><span data-stu-id="03e88-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="03e88-106">Кесте көмекшісі ресурстарды табуда ресурстарға деген қажеттілікте берілген параметрлерге сүйенеді.</span><span class="sxs-lookup"><span data-stu-id="03e88-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="03e88-107">Кесте көмекшісі уақыт талабы немесе дағдылар сияқты сәйкес талаптарға сәйкес келетін ресурстарды ұсынады.</span><span class="sxs-lookup"><span data-stu-id="03e88-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="03e88-108">Қолайлы ресурстар анықталғаннан кейін ресурс немесе жоба менеджері ресурстарды жұмысқа тапсырыс бере алады.</span><span class="sxs-lookup"><span data-stu-id="03e88-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03e88-109">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="03e88-109">Prerequisites</span></span>

<span data-ttu-id="03e88-110">Кесте көмекшісі - бұл Universal Resource Scheduling шешімінің бөлігі.</span><span class="sxs-lookup"><span data-stu-id="03e88-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="03e88-111">Бұл шешім Dynamics 365 Project Operations, Dynamics 365 Field Service және Dynamics 365 Customer Service бағдарламалар құрамына енгізілген және орнатылған.</span><span class="sxs-lookup"><span data-stu-id="03e88-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="03e88-112">Сәйкес талаптар мен ресурстар</span><span class="sxs-lookup"><span data-stu-id="03e88-112">Matching requirements and resources</span></span>

<span data-ttu-id="03e88-113">Құрылған ресурстарға деген қажеттілік келесі мәліметтерге негізделген:</span><span class="sxs-lookup"><span data-stu-id="03e88-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="03e88-114">Сипаттамалар</span><span class="sxs-lookup"><span data-stu-id="03e88-114">Characteristics</span></span>
-   <span data-ttu-id="03e88-115">Рөлдер</span><span class="sxs-lookup"><span data-stu-id="03e88-115">Roles</span></span>
-   <span data-ttu-id="03e88-116">Бизнес бөлімшелер</span><span class="sxs-lookup"><span data-stu-id="03e88-116">Business units</span></span>
-   <span data-ttu-id="03e88-117">Ресурс параметрлері</span><span class="sxs-lookup"><span data-stu-id="03e88-117">Resource preferences</span></span>
-   <span data-ttu-id="03e88-118">Күш-жігер контуры</span><span class="sxs-lookup"><span data-stu-id="03e88-118">Effort contours</span></span>
-   <span data-ttu-id="03e88-119">Уақыт белдеуі</span><span class="sxs-lookup"><span data-stu-id="03e88-119">Time zone</span></span>

<span data-ttu-id="03e88-120">Кесте көмекшісі бұл мәліметтерді ресурстарды сүзу үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="03e88-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="03e88-121">Кесте көмекшісін іске қосу</span><span class="sxs-lookup"><span data-stu-id="03e88-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="03e88-122">Кесте көмекшісін іске қосудың екі жолы бар.</span><span class="sxs-lookup"><span data-stu-id="03e88-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="03e88-123">Егер сіз гибридті режимді пайдаланатын болсаңыз, топ мүшелері торабында сіз ресурстарға орындалмаған талаптары бар кез-келген топ мүшелерін таңдап, содан кейін **Тапсырыс беру** опциясын таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="03e88-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="03e88-124">Егер сіз орталық режимді пайдалансаңыз, Ресурстар менеджері ресурстарды табады және таңдайды.</span><span class="sxs-lookup"><span data-stu-id="03e88-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="03e88-125">Кесте көмекшісі сүзгілері</span><span class="sxs-lookup"><span data-stu-id="03e88-125">Schedule assistant filters</span></span>

<span data-ttu-id="03e88-126">Кесте көмекшісі іске қосылғаннан кейін ресурстарға деген қажеттілік туралы мәліметтер сол жақ тақтада сүзілген мәндер ретінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="03e88-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="03e88-127">Ресурстар менеджері немесе жоба менеджері жоспарлау қажеттіліктерін қанағаттандыру үшін сүзгілерді реттеу арқылы нәтижелерді дәл реттей алады.</span><span class="sxs-lookup"><span data-stu-id="03e88-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="03e88-128">Сүзгі тақтасы жұмысқа қатысты опцияларды көрсетеді, соның ішінде:</span><span class="sxs-lookup"><span data-stu-id="03e88-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="03e88-129">Жұмыстың басы мен соңы</span><span class="sxs-lookup"><span data-stu-id="03e88-129">Work start and end</span></span>
-   <span data-ttu-id="03e88-130">Сипаттамалар</span><span class="sxs-lookup"><span data-stu-id="03e88-130">Characteristics</span></span>
-   <span data-ttu-id="03e88-131">Рөлдер</span><span class="sxs-lookup"><span data-stu-id="03e88-131">Roles</span></span>
-   <span data-ttu-id="03e88-132">Ұйымдық бірліктер</span><span class="sxs-lookup"><span data-stu-id="03e88-132">Organizational units</span></span>
-   <span data-ttu-id="03e88-133">Ресурс компаниясы</span><span class="sxs-lookup"><span data-stu-id="03e88-133">Resourcing company</span></span>
-   <span data-ttu-id="03e88-134">Ресурс түрлері</span><span class="sxs-lookup"><span data-stu-id="03e88-134">Resource types</span></span>
-   <span data-ttu-id="03e88-135">Таңдаулы ресурстар</span><span class="sxs-lookup"><span data-stu-id="03e88-135">Preferred resources</span></span>