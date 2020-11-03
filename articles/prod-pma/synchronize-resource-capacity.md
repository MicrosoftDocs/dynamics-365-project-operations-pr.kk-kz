---
title: Ресурс мүмкіндігін синхрондау
description: Бұл тақырыпта күнтізбелер мен жобалар бойынша ресурстардың мүмкіндігін синхрондау жолы туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 006ebbfea42572f17663fab324a20a10321b78f0
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079638"
---
# <a name="synchronize-resource-capacity"></a><span data-ttu-id="42914-103">Ресурс мүмкіндігін синхрондау</span><span class="sxs-lookup"><span data-stu-id="42914-103">Synchronize resource capacity</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="42914-104">Ресурстарды синхрондау процестері күнтізбе мен негізгі күнтізбеге арналған ақпараттың жобалық ресурстарды жоспарлауға енуіне көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="42914-104">The processes for resource synchronization help guarantee that information for the calendar and base calendar trickles down into project resource scheduling.</span></span> <span data-ttu-id="42914-105">Егер күнтізбе өзгертілсе, процестер жоба ресурстарын жоспарлауға қажетті жаңартуларды енгізеді.</span><span class="sxs-lookup"><span data-stu-id="42914-105">If the calendar is changed, the processes make the required updates to the scheduling of project resources.</span></span> <span data-ttu-id="42914-106">Бұл процестер өнімділікті жақсартуға көмектеседі, өйткені күнтізбелік ресурстар туралы ақпарат алдын ала синхрондалады.</span><span class="sxs-lookup"><span data-stu-id="42914-106">The processes also help improve performance, because the calendar's resource information is synchronized in advance.</span></span> <span data-ttu-id="42914-107">Сондықтан ресурстарды жоспарлау туралы ақпаратты жаңарту тезірек болады.</span><span class="sxs-lookup"><span data-stu-id="42914-107">Therefore, updates to resource scheduling information occur more quickly.</span></span> <span data-ttu-id="42914-108">Процестерді бір-бірден емес, топтама ретінде жоспарлауға кеңес береміз.</span><span class="sxs-lookup"><span data-stu-id="42914-108">We recommend that you schedule the processes as a batch instead of one at a time.</span></span> <span data-ttu-id="42914-109">Әйтпесе, біреу ақпарат соңғы синхрондалғанда инклюзивті күндерін ұмытып кету қаупі бар.</span><span class="sxs-lookup"><span data-stu-id="42914-109">Otherwise, there is a risk that someone will forget the inclusive dates when the information was last synchronized.</span></span> <span data-ttu-id="42914-110">Егер инклюзивті күндер пайдаланылмаса, күнді синхрондау кезінде бос орындар пайда болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="42914-110">If inclusive dates aren't used, gaps can occur during date synchronization.</span></span>

![Күнтізбені синхрондау](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a><span data-ttu-id="42914-112">Ресурстық сыйымдылықтың жиынтығын синхрондау</span><span class="sxs-lookup"><span data-stu-id="42914-112">Synchronize resource capacity roll-ups</span></span>

<span data-ttu-id="42914-113">Синхрондау процесі барлық ресурстардың күнтізбелік ақпаратын синхрондауға арналған.</span><span class="sxs-lookup"><span data-stu-id="42914-113">The synchronization process is designed to synchronize all resource calendar information.</span></span> <span data-ttu-id="42914-114">Бұл ақпарат жобаның күнтізбелік мүмкіндіктер кестесінің барлық өзгерістері туралы негізгі күнтізбелік ақпаратты қамтиды.</span><span class="sxs-lookup"><span data-stu-id="42914-114">This information includes base calendar information about any changes to the project's Resource calendar capacity table.</span></span> <span data-ttu-id="42914-115">Егер жобаға жаңа ресурстар қосылса, синхрондау күнтізбелік ақпараттың қолжетімділігін қамтамасыз етуге көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="42914-115">If new resources are added in the project, synchronization helps guarantee that the updated calendar information is available.</span></span> <span data-ttu-id="42914-116">Бұл синхрондауды кез келген уақытта жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="42914-116">This synchronization can be done at any time.</span></span>

<span data-ttu-id="42914-117">Топтаманы қолдануды ұсынамыз.</span><span class="sxs-lookup"><span data-stu-id="42914-117">We recommend that you use a batch.</span></span> <span data-ttu-id="42914-118">Параметрлер резервтелген сыйымдылықты синхрондау кезінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="42914-118">The options are available during synchronization of capacity reservations.</span></span>

1. <span data-ttu-id="42914-119">**Жобаны басқару және есеп** &gt; **Жүйелі** &gt; **Сыйымдылықты синхрондау** &gt; **Ресурстық сыйымдылықтың жиынтығын синхрондау** тармақтарын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="42914-119">Select **Project management and accounting** &gt; **Periodic** &gt; **Capacity synchronization** &gt; **Synchronize resources capacity roll-ups**.</span></span>
2. <span data-ttu-id="42914-120">Параметрлерді келесі кестеге орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="42914-120">Set the options in the following table.</span></span>

    | <span data-ttu-id="42914-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="42914-121">Option</span></span>      | <span data-ttu-id="42914-122">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="42914-122">Description</span></span> |
    |-------------|-------------|
    | <span data-ttu-id="42914-123">Мерзім коды</span><span class="sxs-lookup"><span data-stu-id="42914-123">Period code</span></span> | <span data-ttu-id="42914-124">Қажет болса, ресурстық сыйымдылықтың жиынтығына арналған синхрондау процесінің басталу және аяқталу күндерін орнату үшін бас кітаптың күндер аралығы кодын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="42914-124">Optionally select the General ledger date interval code to set the start and end dates for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="42914-125">Басталу күні</span><span class="sxs-lookup"><span data-stu-id="42914-125">Start date</span></span>  | <span data-ttu-id="42914-126">Ресурстық сыйымдылықтың жиынтығын синхрондау процесінің басталу күнін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="42914-126">Enter the start date for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="42914-127">Аяқталған күні</span><span class="sxs-lookup"><span data-stu-id="42914-127">End date</span></span>    | <span data-ttu-id="42914-128">Ресурстық сыйымдылықтың жиынтығын синхрондау процесінің аяқталу күнін енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="42914-128">Enter the end date for the synchronization process for resource capacity roll-ups.</span></span> |

<span data-ttu-id="42914-129">[![Синхрондау процесі](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span><span class="sxs-lookup"><span data-stu-id="42914-129">[![Synchronization process](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span></span>