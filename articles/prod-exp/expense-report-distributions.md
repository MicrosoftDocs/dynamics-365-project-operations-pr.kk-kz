---
title: Шығыс туралы есеп бойынша тарату
description: Шығыстар туралы есепте шығыстарды енгізген кезде, шығысты бірнеше жобалар, заңды нысандар немесе ұйымдағы шоттар бойынша таратуға болады.
author: ShylaThompson
manager: AnnBe
ms.date: 09/19/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a43de30d916d2775f28f59f404c34b60a43fff9c
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960749"
---
# <a name="expense-report-distributions"></a><span data-ttu-id="e3681-103">Шығыс туралы есеп бойынша тарату</span><span class="sxs-lookup"><span data-stu-id="e3681-103">Expense report distributions</span></span>

<span data-ttu-id="e3681-104">Шығыстар туралы есепте шығыстарды енгізген кезде, шығысты бірнеше жобалар, қаржылық өлшемдер немесе ұйымдағы шоттар бойынша таратуға болады.</span><span class="sxs-lookup"><span data-stu-id="e3681-104">When you enter expenses on an expense report, you can distribute the expense across multiple projects, financial dimensions, or accounts in your organization.</span></span>

<span data-ttu-id="e3681-105">Мысалы, Фабрикамның сату өкілі Нэнси Копенгагеннен Франкфуртке дейін барды.</span><span class="sxs-lookup"><span data-stu-id="e3681-105">For example, Nancy, a Fabrikam sales representative, traveled from Copenhagen to Frankfurt.</span></span> <span data-ttu-id="e3681-106">Франкфуртта ол екі ұйыммен кездесті, әр ұйым үшін бөлек жобаларды талқылады.</span><span class="sxs-lookup"><span data-stu-id="e3681-106">In Frankfurt, she met with two organizations to discuss separate projects for each organization.</span></span> <span data-ttu-id="e3681-107">Нэнси А жобасы бойынша А ұйымымен жеті жұмыс күнін, В жобасы бойынша В ұйымымен үш жұмыс күнін өткізді.</span><span class="sxs-lookup"><span data-stu-id="e3681-107">Nancy spent seven business days working with organization A on project A, and three business days working with organization B on project B.</span></span>

<span data-ttu-id="e3681-108">Франкфуртта болған кезде Нэнси екі бөлек жобада жұмыс істегендіктен, шығыстар туралы есебін берген кезде, ол шығындарды әр жобаға сәйкес бөледі.</span><span class="sxs-lookup"><span data-stu-id="e3681-108">Because Nancy worked on two separate projects when she was in Frankfurt, when she enters her expense report, she distributes her expenses as appropriate for each project.</span></span> <span data-ttu-id="e3681-109">Келесі кестеде Нэнсидің шығыстарды қалай бөлгендігі көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="e3681-109">The following table shows how Nancy distributed her expenses.</span></span>


| <span data-ttu-id="e3681-110">Шығыс түрі</span><span class="sxs-lookup"><span data-stu-id="e3681-110">Expense type</span></span> | <span data-ttu-id="e3681-111">Жалпы шығыс мөлшері</span><span class="sxs-lookup"><span data-stu-id="e3681-111">Total expense amount</span></span>|<span data-ttu-id="e3681-112">А жобасына бөлінген сома</span><span class="sxs-lookup"><span data-stu-id="e3681-112">Amount distributed to project A</span></span>| <span data-ttu-id="e3681-113">В жобасына бөлінген сома</span><span class="sxs-lookup"><span data-stu-id="e3681-113">Amount distributed to project B</span></span> |
|--------------|---------------------|-------------------------------|---------------------------------|
|<span data-ttu-id="e3681-114">Пойыз ақысы</span><span class="sxs-lookup"><span data-stu-id="e3681-114">Train fare</span></span>   |<span data-ttu-id="e3681-115">DKK 578</span><span class="sxs-lookup"><span data-stu-id="e3681-115">DKK 578</span></span>              |<span data-ttu-id="e3681-116">DKK 405</span><span class="sxs-lookup"><span data-stu-id="e3681-116">DKK 405</span></span>                        |<span data-ttu-id="e3681-117">DKK 173</span><span class="sxs-lookup"><span data-stu-id="e3681-117">DKK 173</span></span>                          |
|<span data-ttu-id="e3681-118">Қонақүй</span><span class="sxs-lookup"><span data-stu-id="e3681-118">Hotel</span></span>         |<span data-ttu-id="e3681-119">EUR 725</span><span class="sxs-lookup"><span data-stu-id="e3681-119">EUR 725</span></span>              |<span data-ttu-id="e3681-120">EUR 557</span><span class="sxs-lookup"><span data-stu-id="e3681-120">EUR 557</span></span>                        |<span data-ttu-id="e3681-121">EUR 168</span><span class="sxs-lookup"><span data-stu-id="e3681-121">EUR 168</span></span>                          |
|<span data-ttu-id="e3681-122">Тамақтану</span><span class="sxs-lookup"><span data-stu-id="e3681-122">Meals</span></span>         |<span data-ttu-id="e3681-123">EUR 346</span><span class="sxs-lookup"><span data-stu-id="e3681-123">EUR 346</span></span>              |<span data-ttu-id="e3681-124">EUR 284</span><span class="sxs-lookup"><span data-stu-id="e3681-124">EUR 284</span></span>                        |<span data-ttu-id="e3681-125">EUR 62</span><span class="sxs-lookup"><span data-stu-id="e3681-125">EUR 62</span></span>                           |

