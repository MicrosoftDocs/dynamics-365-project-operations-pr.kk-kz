---
title: Кесте көмекшісіне шолу
description: Бұл тақырып ресурстарға тапсырыс беру үшін кесте көмекшісімен жұмыс істеу туралы ақпарат береді.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: e14dbe5abb69a547e2d09ef9e6bcba48e1f89455
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279235"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="9e3b1-103">Кесте көмекшісіне шолу</span><span class="sxs-lookup"><span data-stu-id="9e3b1-103">Schedule assistant overview</span></span>

<span data-ttu-id="9e3b1-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="9e3b1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9e3b1-105">Кесте көмекшісі жоба менеджері анықтаған талаптарға негізделген ресурстарға тапсырыс беруге арналған.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="9e3b1-106">Кесте көмекшісі ресурстарды табуда ресурстарға деген қажеттілікте берілген параметрлерге сүйенеді.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="9e3b1-107">Кесте көмекшісі уақыт талабы немесе дағдылар сияқты сәйкес талаптарға сәйкес келетін ресурстарды ұсынады.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="9e3b1-108">Қолайлы ресурстар анықталғаннан кейін ресурс немесе жоба менеджері ресурстарды жұмысқа тапсырыс бере алады.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e3b1-109">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="9e3b1-109">Prerequisites</span></span>

<span data-ttu-id="9e3b1-110">Кесте көмекшісі - бұл Universal Resource Scheduling шешімінің бөлігі.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="9e3b1-111">Бұл шешім Dynamics 365 Project Operations, Dynamics 365 Field Service және Dynamics 365 Customer Service бағдарламаларының көмегімен қосылады және орнатылады.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="9e3b1-112">Сәйкес талаптар мен ресурстар</span><span class="sxs-lookup"><span data-stu-id="9e3b1-112">Matching requirements and resources</span></span>

<span data-ttu-id="9e3b1-113">Құрылған ресурстарға деген қажеттілік келесі мәліметтерге негізделген:</span><span class="sxs-lookup"><span data-stu-id="9e3b1-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="9e3b1-114">Сипаттамалар</span><span class="sxs-lookup"><span data-stu-id="9e3b1-114">Characteristics</span></span>
-   <span data-ttu-id="9e3b1-115">Рөлдер</span><span class="sxs-lookup"><span data-stu-id="9e3b1-115">Roles</span></span>
-   <span data-ttu-id="9e3b1-116">Бизнес бөлімшелер</span><span class="sxs-lookup"><span data-stu-id="9e3b1-116">Business units</span></span>
-   <span data-ttu-id="9e3b1-117">Ресурс параметрлері</span><span class="sxs-lookup"><span data-stu-id="9e3b1-117">Resource preferences</span></span>
-   <span data-ttu-id="9e3b1-118">Күш-жігер контуры</span><span class="sxs-lookup"><span data-stu-id="9e3b1-118">Effort contours</span></span>
-   <span data-ttu-id="9e3b1-119">Уақыт белдеуі</span><span class="sxs-lookup"><span data-stu-id="9e3b1-119">Time zone</span></span>

<span data-ttu-id="9e3b1-120">Кесте көмекшісі бұл мәліметтерді ресурстарды сүзу үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="9e3b1-121">Кесте көмекшісін іске қосу</span><span class="sxs-lookup"><span data-stu-id="9e3b1-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="9e3b1-122">Кесте көмекшісін іске қосудың екі жолы бар.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="9e3b1-123">Егер сіз гибридті режимді пайдаланатын болсаңыз, топ мүшелері торабында сіз ресурстарға орындалмаған талаптары бар кез-келген топ мүшелерін таңдап, содан кейін **Тапсырыс беру** опциясын таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="9e3b1-124">Егер сіз орталық режимді пайдалансаңыз, Ресурстар менеджері ресурстарды табады және таңдайды.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="9e3b1-125">Кесте көмекшісі сүзгілері</span><span class="sxs-lookup"><span data-stu-id="9e3b1-125">Schedule assistant filters</span></span>

<span data-ttu-id="9e3b1-126">Кесте көмекшісі іске қосылғаннан кейін ресурстарға деген қажеттілік туралы мәліметтер сол жақ тақтада сүзілген мәндер ретінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="9e3b1-127">Ресурстар менеджері немесе жоба менеджері жоспарлау қажеттіліктерін қанағаттандыру үшін сүзгілерді реттеу арқылы нәтижелерді дәл реттей алады.</span><span class="sxs-lookup"><span data-stu-id="9e3b1-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="9e3b1-128">Сүзгі тақтасы жұмысқа қатысты опцияларды көрсетеді, соның ішінде:</span><span class="sxs-lookup"><span data-stu-id="9e3b1-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="9e3b1-129">Жұмыстың басы мен соңы</span><span class="sxs-lookup"><span data-stu-id="9e3b1-129">Work start and end</span></span>
-   <span data-ttu-id="9e3b1-130">Сипаттамалар</span><span class="sxs-lookup"><span data-stu-id="9e3b1-130">Characteristics</span></span>
-   <span data-ttu-id="9e3b1-131">Рөлдер</span><span class="sxs-lookup"><span data-stu-id="9e3b1-131">Roles</span></span>
-   <span data-ttu-id="9e3b1-132">Ұйымдық бірліктер</span><span class="sxs-lookup"><span data-stu-id="9e3b1-132">Organizational units</span></span>
-   <span data-ttu-id="9e3b1-133">Ресурс компаниясы</span><span class="sxs-lookup"><span data-stu-id="9e3b1-133">Resourcing company</span></span>
-   <span data-ttu-id="9e3b1-134">Ресурс түрлері</span><span class="sxs-lookup"><span data-stu-id="9e3b1-134">Resource types</span></span>
-   <span data-ttu-id="9e3b1-135">Таңдаулы ресурстар</span><span class="sxs-lookup"><span data-stu-id="9e3b1-135">Preferred resources</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]