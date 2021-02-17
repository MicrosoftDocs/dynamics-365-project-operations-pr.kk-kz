---
title: Әдістерді аяқтау құны
description: Бұл тақырыпта жобаны аяқтау үшін жұмсалатын шығындарды есептеу әдістері туралы ақпарат берілген.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 790b5c98182acdc0a37e3741a40baf7152f0bf66
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531478"
---
# <a name="cost-to-complete-methods"></a><span data-ttu-id="8fca7-103">Әдістерді аяқтау құны</span><span class="sxs-lookup"><span data-stu-id="8fca7-103">Cost to complete methods</span></span>

<span data-ttu-id="8fca7-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="8fca7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8fca7-105">Бұл тақырыпта жобаны аяқтау үшін жұмсалатын шығындарды есептеу әдістері туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="8fca7-105">This topic provides information about the methods used to calculate the cost to complete a project.</span></span> <span data-ttu-id="8fca7-106">Жобаны аяқтау үшін жұмсалатын шығындарды есептеудің бірнеше әдісін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="8fca7-106">There are multiple methods you can use to calculate the cost to complete a project.</span></span> 

<span data-ttu-id="8fca7-107">Жобаның болжамын құрған кезде, **Болжам жасау** бетіндегі, **Әдістерді аяқтау құны** өрісінде әдістерді аяқтау үшін келесі шығындардың бірін таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="8fca7-107">When you create an estimate for a project, on the **Create estimate** page, in the **Cost to complete method** field, you can select one of the following cost to complete methods.</span></span>

| <span data-ttu-id="8fca7-108">Әдісті аяқтау құны</span><span class="sxs-lookup"><span data-stu-id="8fca7-108">Cost to complete method</span></span>    | <span data-ttu-id="8fca7-109">Сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="8fca7-109">Description</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8fca7-110">Жалпы құны - нақты көрсеткіш</span><span class="sxs-lookup"><span data-stu-id="8fca7-110">Total cost-actual</span></span>            | <span data-ttu-id="8fca7-111">**Болжам беті** бетіндегі **Шығынды болжау** түймесінің көмегімен **Жалпы құн** немесе **Жалпы мөлшер** өрістерінде болжамды шығындарды қолмен енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="8fca7-111">Enter estimate costs manually in the **Total cost** or **Total quantity** fields using the **Cost estimate** button on the **Estimate page**.</span></span> <span data-ttu-id="8fca7-112">Жүйе енгізілген қорытындылардан нақты шығындарды алып тастайды.</span><span class="sxs-lookup"><span data-stu-id="8fca7-112">The system subtracts the actual costs from the totals you entered.</span></span> <span data-ttu-id="8fca7-113">Қорытынды – бұл жобаны аяқтауға арналған шығындар.</span><span class="sxs-lookup"><span data-stu-id="8fca7-113">The total is the cost to complete the project.</span></span> <span data-ttu-id="8fca7-114">Бұл әдіс Microsoft Dataverse шеңберінде Project Operations бағдарламасына енгізілген шығыс болжамдары мен ресурстар тағайындауларын пайдаланбайды.</span><span class="sxs-lookup"><span data-stu-id="8fca7-114">This method doesn't use the expense estimates and resources assignments entered in Project Operations built within Microsoft Dataverse.</span></span> <span data-ttu-id="8fca7-115">Жалпы құны немесе жалпы мөлшері қажетінше қолмен жаңартылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8fca7-115">The total cost or total quantity can be updated manually as needed.</span></span>  |
| <span data-ttu-id="8fca7-116">Жалпы болжам - нақты көрсеткіш</span><span class="sxs-lookup"><span data-stu-id="8fca7-116">Total forecast-actual</span></span>        | <span data-ttu-id="8fca7-117">Жобаның болжамды жалпы сомасын анықтау үшін ресурстарды тағайындау және шығыс болжамдарын пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="8fca7-117">Resource assignments and expense estimates are used to determine the total project forecast amount.</span></span> <span data-ttu-id="8fca7-118">Аяқтауға жұмсалатын шығынды есептеу үшін нақты шығындар осы болжаммен салыстырылады.</span><span class="sxs-lookup"><span data-stu-id="8fca7-118">Actual costs are compared against this forecast to calculate the cost to complete.</span></span>                                                                                                                                                                                                                                                                          |
| <span data-ttu-id="8fca7-119">Алдыңғы болжам бойынша</span><span class="sxs-lookup"><span data-stu-id="8fca7-119">As previous estimate</span></span>         | <span data-ttu-id="8fca7-120">Мұнда алдыңғы кезеңде пайдаланылған бағалау әдістері пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="8fca7-120">The same estimate methods that was used in the previous period is used here.</span></span> <span data-ttu-id="8fca7-121">Егер алдыңғы кезең болжау үлгісін қажет еткен болса, бұл әдіс болжау үлгісін қажет етеді.</span><span class="sxs-lookup"><span data-stu-id="8fca7-121">This method requires a forecast model if the previous period required a forecast model.</span></span>                                                                                                                                                                                                                                                                                                                           |
| <span data-ttu-id="8fca7-122">Аяқтауға кететін шығынды нөлге орнатыңыз</span><span class="sxs-lookup"><span data-stu-id="8fca7-122">Set cost to complete to zero</span></span> | <span data-ttu-id="8fca7-123">Әдетте, болжамды жоба жойылғанға дейін пайдаланылады, бұл әдіс жалпы болжамдарды кеңейтілген нақты транзакциялармен сәйкес келеді және **Аяқтау құны** бағанын жояды.</span><span class="sxs-lookup"><span data-stu-id="8fca7-123">Typically used before the estimate project is eliminated, this method matches total estimates with posted actual transactions and clears the **Cost to complete** column.</span></span> <span data-ttu-id="8fca7-124">Аяқталған кезде, нәтиже әрдайым 100 пайызды құрайды.</span><span class="sxs-lookup"><span data-stu-id="8fca7-124">When complete, the result is always 100 percent.</span></span> <span data-ttu-id="8fca7-125">Сіз жасаған әрбір шығын жолы үшін **Болжау** құсбелгісі алынып, жалпы болжам алдыңғы шығындар болжамына көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="8fca7-125">For each cost line that you create, the **Forecasting** check box is cleared and the total estimate is copied from the previous cost estimate.</span></span> <span data-ttu-id="8fca7-126">Болжалды кезеңдегі нақты тұтыну жобаны аяқтауға кететін шығыннан алынады.</span><span class="sxs-lookup"><span data-stu-id="8fca7-126">The actual consumption for the estimate period is deducted from the cost to complete the project.</span></span>              |
| <span data-ttu-id="8fca7-127">Шығын үлгісінен</span><span class="sxs-lookup"><span data-stu-id="8fca7-127">From cost template</span></span>           | <span data-ttu-id="8fca7-128">Таңдалған болжамды жобамен байланысты шығындар үлгісінде орнатылған аяқтау әдісінің құны.</span><span class="sxs-lookup"><span data-stu-id="8fca7-128">The cost to complete method that is set up in the cost template that's associated with the selected estimate project.</span></span>                                                                                                                                                                                                                                                                                                                                                                          |