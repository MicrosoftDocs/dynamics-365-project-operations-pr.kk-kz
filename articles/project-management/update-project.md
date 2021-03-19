---
title: Жобаны жаңарту
description: Бұл тақырыпта Project Operations бағдарламасындағы жобаларды жаңарту туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 27444b072bdf7de55d6b38c30c1ea5fe66ed46ac
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286390"
---
# <a name="update-a-project"></a><span data-ttu-id="53f97-103">Жобаны жаңарту</span><span class="sxs-lookup"><span data-stu-id="53f97-103">Update a project</span></span>

<span data-ttu-id="53f97-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="53f97-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="53f97-105">Төменде жоба жасалғаннан кейін оны жаңартуға болатын өрістердің қорытындысы және жаңартулардың кез келген қолданылатын салдары келтірілген.</span><span class="sxs-lookup"><span data-stu-id="53f97-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="53f97-106">Жобаның мәлімет өрістері</span><span class="sxs-lookup"><span data-stu-id="53f97-106">Project detail fields</span></span>

- <span data-ttu-id="53f97-107">**Атауы**: жоба атауы.</span><span class="sxs-lookup"><span data-stu-id="53f97-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="53f97-108">**Сипаттамасы**: жобаның шолуы.</span><span class="sxs-lookup"><span data-stu-id="53f97-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="53f97-109">**Тұтынушы**: жоба жеткізілетін компания.</span><span class="sxs-lookup"><span data-stu-id="53f97-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="53f97-110">**Күнтізбе үлгісі**: жобаның жұмыс уақыты.</span><span class="sxs-lookup"><span data-stu-id="53f97-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="53f97-111">Өріс өзгерген кезде, бүкіл кесте қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="53f97-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="53f97-112">**Валюта**: жоба валютасы.</span><span class="sxs-lookup"><span data-stu-id="53f97-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="53f97-113">Бұл өріс келісім-шарт бірлігінде анықталған валютаға негізделген.</span><span class="sxs-lookup"><span data-stu-id="53f97-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="53f97-114">Келісім-шарт бірлігі жаңартылған кезде өріс те жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="53f97-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="53f97-115">**Келісім-шарт бірлігі**: негізінен сатылымды ұтуға және жұмыс пен тұтынушыға қызмет көрсетуді жеткізуге жауапты компанияның тобын немесе бөлімін көрсететін ұйымдық бөлімше.</span><span class="sxs-lookup"><span data-stu-id="53f97-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="53f97-116">**Жоба менеджері**: уақыт жазбалары мен шығыстарды тексеруге және бекітуге құқығы бар жоба тобы мүшесі.</span><span class="sxs-lookup"><span data-stu-id="53f97-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="53f97-117">Өрістерді бағалау</span><span class="sxs-lookup"><span data-stu-id="53f97-117">Estimate fields</span></span>

- <span data-ttu-id="53f97-118">**Болжалды басталу күні**: жоба басталатын күн.</span><span class="sxs-lookup"><span data-stu-id="53f97-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="53f97-119">Бұл өріс жаңартылған кезде, жобадағы кез келген тапсырмалар жаңа басталу күнімен пропорционалды түрде ауысады.</span><span class="sxs-lookup"><span data-stu-id="53f97-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="53f97-120">**Аяқталу күні**: жоба аяқталатын күн.</span><span class="sxs-lookup"><span data-stu-id="53f97-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="53f97-121">**Талпыныс**: жобаның болжамды талпынысы.</span><span class="sxs-lookup"><span data-stu-id="53f97-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="53f97-122">Жобаға тапсырмалар қосылған кезде, бұл өрісті өңдеу мүмкін болмайды.</span><span class="sxs-lookup"><span data-stu-id="53f97-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="53f97-123">**Болжалды еңбек құны**: жобаның болжалды еңбек құны.</span><span class="sxs-lookup"><span data-stu-id="53f97-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="53f97-124">Жобаға еңбек құны қосылған кезде, бұл өрісті өңдеу мүмкін болмайды.</span><span class="sxs-lookup"><span data-stu-id="53f97-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="53f97-125">**Болжалды шығыстар**: жобаның болжалды шығыстары.</span><span class="sxs-lookup"><span data-stu-id="53f97-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="53f97-126">Жобаға шығыстар қосылған кезде, бұл өрісті өңдеу мүмкін болмайды.</span><span class="sxs-lookup"><span data-stu-id="53f97-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="53f97-127">Жобаның нақты өрістері</span><span class="sxs-lookup"><span data-stu-id="53f97-127">Project actual fields</span></span>
- <span data-ttu-id="53f97-128">**Нақты басталуы**: жоба басталған күн.</span><span class="sxs-lookup"><span data-stu-id="53f97-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="53f97-129">**Нақты аяқталуы**: жоба аяқталған кезде жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="53f97-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="53f97-130">Жоба күйі өрістері</span><span class="sxs-lookup"><span data-stu-id="53f97-130">Project status fields</span></span>

- <span data-ttu-id="53f97-131">**Жалпы жоба күйі**: жоба менеджері ұсынатын жалпы жоба күйі.</span><span class="sxs-lookup"><span data-stu-id="53f97-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="53f97-132">**Комментарийлер**: жоба менеджері ұсынған жобаның қазіргі күйіне қатысты мәлімдеме.</span><span class="sxs-lookup"><span data-stu-id="53f97-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]