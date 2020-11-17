---
title: Ресурсты басқару режимдеріне шолу
description: Бұл тақырыпта Dynamics 365 Project Operations бағдарламасындағы "Ресурсты басқару" функционалдығы туралы ақпарат беріледі.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 73ba6190e2e366f22372102d14d26f6d71ba0bc1
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4118525"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="89131-103">Ресурсты басқару режимдеріне шолу</span><span class="sxs-lookup"><span data-stu-id="89131-103">Resource management modes overview</span></span>

<span data-ttu-id="89131-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="89131-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="89131-105">Жалпы тапсырыс беру ағынының орындалуы үшін Dynamics 365 Project Operations екі режимді қолдайды.</span><span class="sxs-lookup"><span data-stu-id="89131-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="89131-106">Басқару режимі жоба параметрі ретінде анықталады және егер сіздің бизнесіңіз өзгерісті қажет етсе, оны өзгертуге болады.</span><span class="sxs-lookup"><span data-stu-id="89131-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="89131-107">Орталық режим</span><span class="sxs-lookup"><span data-stu-id="89131-107">Central mode</span></span>
<span data-ttu-id="89131-108">Жобаларға ресурстарды бөлуді орталықтандыратын ұйымдар үшін орталық режим жоба менеджерлерінің жоба деңгейінде ресурстарға қажеттіліктерді анықтай алуына кепілдік береді.</span><span class="sxs-lookup"><span data-stu-id="89131-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="89131-109">Ресурс талаптарын орындау ресурс менеджеріне беріледі.</span><span class="sxs-lookup"><span data-stu-id="89131-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="89131-110">Жоба менеджерлері ресурс менеджері ұсынған ресурстарды қабылдай алады немесе бас тарта алады.</span><span class="sxs-lookup"><span data-stu-id="89131-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Орталық режим](./media/resource-management-central.png)

<span data-ttu-id="89131-112">Ресурстарды орталық режиммен басқару үшін мына сілтемені қараңыз:</span><span class="sxs-lookup"><span data-stu-id="89131-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="89131-113">Жалпы тапсырыс беруге болатын ресурстарды тапсырмаға тағайындау және ресурс талаптарын құру</span><span class="sxs-lookup"><span data-stu-id="89131-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="89131-114">Ресурс талаптарынан атаулы ресустарға тапсырыс беру</span><span class="sxs-lookup"><span data-stu-id="89131-114">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="89131-115">Ресурс сұрауын жіберу</span><span class="sxs-lookup"><span data-stu-id="89131-115">Submit a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="89131-116">Ресурс сұрауын орындау</span><span class="sxs-lookup"><span data-stu-id="89131-116">Fulfill a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="89131-117">Ресурс сұрауынан ұсынылған жоба ресурсын қабылдау немесе қабылдамау</span><span class="sxs-lookup"><span data-stu-id="89131-117">Accept or reject a proposed project resource from a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="89131-118">Гибридтік режим</span><span class="sxs-lookup"><span data-stu-id="89131-118">Hybrid mode</span></span>
<span data-ttu-id="89131-119">Ресурстарды бөлу кезінде икемділікті талап ететін ұйымдар үшін гибридті режим жоба менеджерлеріне де, ресурстар менеджерлеріне де ресурстарға тапсырыс беруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="89131-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Гибридтік режим](./media/resource-management-hybrid.png)

<span data-ttu-id="89131-121">Қолдау көрсетілетін орталық режим процесінен басқа, гибридтік режимде барлық қолдау көрсетілетін тапсырыс беру ағындарын басқару үшін келесі тақырыптарды қараңыз:</span><span class="sxs-lookup"><span data-stu-id="89131-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="89131-122">Ресурсты тікелей жобаға тапсырыс беру:</span><span class="sxs-lookup"><span data-stu-id="89131-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="89131-123">Жоба тобы үшін аталған тапсырыс беруге болатын ресурстарға тапсырыс беру және тапсырмаларды тағайындау</span><span class="sxs-lookup"><span data-stu-id="89131-123">Book named bookable resources to a project team and assign tasks</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="89131-124">Ресурс талабынан ресурсқа тапсырыс беру:</span><span class="sxs-lookup"><span data-stu-id="89131-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="89131-125">Жалпы тапсырыс беруге болатын ресурстарды тапсырмаға тағайындау және ресурс талаптарын құру</span><span class="sxs-lookup"><span data-stu-id="89131-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="89131-126">Ресурс талаптарынан атаулы ресустарға тапсырыс беру</span><span class="sxs-lookup"><span data-stu-id="89131-126">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
