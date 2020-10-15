---
title: Шығыс туралы есеп бойынша тарату
description: Шығыстар туралы есепте шығыстарды енгізген кезде, оларды бірнеше жобалар, заңды нысандар немесе ұйымдағы шоттар бойынша бөлуге болады.
author: suvaidya
manager: AnnBe
ms.date: 10/10/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: a1fa7383e7715fe57380de0a006ccc4e020bb5a5
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908308"
---
# <a name="distributions-on-an-expense-report"></a><span data-ttu-id="098f1-103">Шығыс туралы есеп бойынша тарату</span><span class="sxs-lookup"><span data-stu-id="098f1-103">Distributions on an expense report</span></span>

<span data-ttu-id="098f1-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="098f1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="098f1-105">Шығыстар туралы есепте шығыстарды енгізген кезде, оларды бірнеше жобалар, қаржылық өлшемдер немесе ұйымдағы шоттар бойынша бөлуге болады.</span><span class="sxs-lookup"><span data-stu-id="098f1-105">When you enter expenses on an expense report, you can distribute them across multiple projects, financial dimensions, or accounts in your organization.</span></span>

<span data-ttu-id="098f1-106">Мысалы, Фабрикамның сату өкілі Нэнси Копенгагеннен Франкфуртке дейін барды.</span><span class="sxs-lookup"><span data-stu-id="098f1-106">For example, Nancy, a Fabrikam sales representative, traveled from Copenhagen to Frankfurt.</span></span> <span data-ttu-id="098f1-107">Франкфуртта Нэнси екі ұйыммен кездесті, әр ұйым үшін бөлек жобаларды талқылады.</span><span class="sxs-lookup"><span data-stu-id="098f1-107">In Frankfurt, Nancy met with two organizations to discuss separate projects for each organization.</span></span> <span data-ttu-id="098f1-108">Нэнси А жобасы бойынша А ұйымымен жеті жұмыс күнін, В жобасы бойынша В ұйымымен үш жұмыс күнін өткізді.</span><span class="sxs-lookup"><span data-stu-id="098f1-108">Nancy spent seven business days working with organization A on project A, and three business days working with organization B on project B.</span></span>

<span data-ttu-id="098f1-109">Франкфуртта болған кезде Нэнси екі бөлек жобада жұмыс істегендіктен, шығыстар туралы есеп берген кезде, Нэнси шығындарды әр жобаға сәйкес бөледі.</span><span class="sxs-lookup"><span data-stu-id="098f1-109">Because Nancy worked on two separate projects while was in Frankfurt, when she enters the expense report, Nancy distributes the expenses as appropriate for each project.</span></span> <span data-ttu-id="098f1-110">Келесі кестеде Нэнсидің шығыстарды қалай бөлгендігі көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="098f1-110">The following table shows how Nancy distributed the expenses.</span></span>

| <span data-ttu-id="098f1-111">Шығыс түрі</span><span class="sxs-lookup"><span data-stu-id="098f1-111">Expense type</span></span> | <span data-ttu-id="098f1-112">Жалпы шығыс мөлшері</span><span class="sxs-lookup"><span data-stu-id="098f1-112">Total expense amount</span></span> | <span data-ttu-id="098f1-113">А жобасына бөлінген сома</span><span class="sxs-lookup"><span data-stu-id="098f1-113">Amount distributed to project A</span></span> | <span data-ttu-id="098f1-114">В жобасына бөлінген сома</span><span class="sxs-lookup"><span data-stu-id="098f1-114">Amount distributed to project B</span></span> |
|--------------|----------------------|---------------------------------|---------------------------------|
| <span data-ttu-id="098f1-115">Пойыз ақысы</span><span class="sxs-lookup"><span data-stu-id="098f1-115">Train fare</span></span>   | <span data-ttu-id="098f1-116">DKK 578</span><span class="sxs-lookup"><span data-stu-id="098f1-116">DKK 578</span></span>              | <span data-ttu-id="098f1-117">DKK 405</span><span class="sxs-lookup"><span data-stu-id="098f1-117">DKK 405</span></span>                         | <span data-ttu-id="098f1-118">DKK 173</span><span class="sxs-lookup"><span data-stu-id="098f1-118">DKK 173</span></span>                         |
| <span data-ttu-id="098f1-119">Қонақүй</span><span class="sxs-lookup"><span data-stu-id="098f1-119">Hotel</span></span>        | <span data-ttu-id="098f1-120">EUR 725</span><span class="sxs-lookup"><span data-stu-id="098f1-120">EUR 725</span></span>              | <span data-ttu-id="098f1-121">EUR 557</span><span class="sxs-lookup"><span data-stu-id="098f1-121">EUR 557</span></span>                         | <span data-ttu-id="098f1-122">EUR 168</span><span class="sxs-lookup"><span data-stu-id="098f1-122">EUR 168</span></span>                         |
| <span data-ttu-id="098f1-123">Тамақтану</span><span class="sxs-lookup"><span data-stu-id="098f1-123">Meals</span></span>        | <span data-ttu-id="098f1-124">EUR 346</span><span class="sxs-lookup"><span data-stu-id="098f1-124">EUR 346</span></span>              | <span data-ttu-id="098f1-125">EUR 284</span><span class="sxs-lookup"><span data-stu-id="098f1-125">EUR 284</span></span>                         | <span data-ttu-id="098f1-126">EUR 62</span><span class="sxs-lookup"><span data-stu-id="098f1-126">EUR 62</span></span>                          |
