---
title: Жоспарлау режимдері
description: Бұл тақырыпта жоспарлау режимдері туралы ақпарат берілген.
author: ruhercul
manager: AnnBe
ms.date: 05/04/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fe54944999617b248ff925148a78601dd4be7aca
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981442"
---
# <a name="scheduling-modes"></a><span data-ttu-id="e2661-103">Жоспарлау режимдері</span><span class="sxs-lookup"><span data-stu-id="e2661-103">Scheduling modes</span></span>

<span data-ttu-id="e2661-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="e2661-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="e2661-105">Dynamics 365 Project Operations ұйымдарға жұмыс декомпозициясының құрылымы аясындағы тапсырмалардағы негізгі айнымалыларға өзгерістерді басқару жолдарын анықтау мүмкіндігін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="e2661-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="e2661-106">Ұйымның нақты қажеттіліктері негізінде жоба менеджерлері жоба жасалған кезде жоспарлау режиміне өзгертулер енгізе алады.</span><span class="sxs-lookup"><span data-stu-id="e2661-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="e2661-107">Project Operations бағдарламасында үш жоспарлау режимі бар:</span><span class="sxs-lookup"><span data-stu-id="e2661-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="e2661-108">Бекітілген ұзақтық (бұл – әдепкі режим)</span><span class="sxs-lookup"><span data-stu-id="e2661-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="e2661-109">Бекітілген жұмыс</span><span class="sxs-lookup"><span data-stu-id="e2661-109">Fixed work</span></span>
  - <span data-ttu-id="e2661-110">Бекітілген бірліктер</span><span class="sxs-lookup"><span data-stu-id="e2661-110">Fixed units</span></span>

<span data-ttu-id="e2661-111">Жоспарлаудың нақты режимін анықтауға әсер ететін мәндер келесі формула бойынша анықталады:</span><span class="sxs-lookup"><span data-stu-id="e2661-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="e2661-112">Әрекет (*Жұмыс*) = Ұзақтығы x бірлік</span><span class="sxs-lookup"><span data-stu-id="e2661-112">Effort (*Work*) = Duration x Units</span></span>

<span data-ttu-id="e2661-113">Жобаның жоспарлау режимін анықтаған кезде кейін өзгерту мүмкін емес болатын осы мәндердің бірін орнатасыз.</span><span class="sxs-lookup"><span data-stu-id="e2661-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="e2661-114">Бұл мәнді тұрақты күйінде ұстау сол мәнге басымдық береді, бұл жүйеге басқа екі мән өзгерген кезде оны өзгертпеу туралы хабарлайды.</span><span class="sxs-lookup"><span data-stu-id="e2661-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="e2661-115">Келесі кестеде белгілі бір режимді таңдау әсерлері туралы ақпарат берілген.</span><span class="sxs-lookup"><span data-stu-id="e2661-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="e2661-116">**Осы тапсырмада**</span><span class="sxs-lookup"><span data-stu-id="e2661-116">**In this task**</span></span>             | <span data-ttu-id="e2661-117">**Егер бірліктерді қайта қарасаңыз**</span><span class="sxs-lookup"><span data-stu-id="e2661-117">**If you revise units**</span></span>   | <span data-ttu-id="e2661-118">**Егер ұзақтығын қайта қарасаңыз**</span><span class="sxs-lookup"><span data-stu-id="e2661-118">**If you revise duration**</span></span> | <span data-ttu-id="e2661-119">**Егер әрекетті қайта қарасаңыз**</span><span class="sxs-lookup"><span data-stu-id="e2661-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="e2661-120">Бекітілген бірліктер тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="e2661-120">Fixed units task</span></span>     | <span data-ttu-id="e2661-121">Ұзақтығы қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-121">Duration is recalculated.</span></span> | <span data-ttu-id="e2661-122">Әрекет қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-122">Effort is recalculated.</span></span>    | <span data-ttu-id="e2661-123">Ұзақтығы қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="e2661-124">Бекітілген әрекет тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="e2661-124">Fixed effort task</span></span>    | <span data-ttu-id="e2661-125">Ұзақтығы қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-125">Duration is recalculated.</span></span> | <span data-ttu-id="e2661-126">Бірліктер қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-126">Units are recalculated.</span></span>    | <span data-ttu-id="e2661-127">Ұзақтығы қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="e2661-128">Бекітілген ұзақтығы тапсырмасы</span><span class="sxs-lookup"><span data-stu-id="e2661-128">Fixed duration task</span></span>  | <span data-ttu-id="e2661-129">Әрекет қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-129">Effort is recalculated.</span></span>   | <span data-ttu-id="e2661-130">Әрекет қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-130">Effort is recalculated.</span></span>    | <span data-ttu-id="e2661-131">Бірліктер қайта есептеледі.</span><span class="sxs-lookup"><span data-stu-id="e2661-131">Units are recalculated.</span></span>   |

<span data-ttu-id="e2661-132">Берілген режимнің салдары туралы қосымша ақпаратты [Нақты жоспарлау үшін тапсырма түрін өзгерту](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="e2661-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="e2661-133">Тақырыпта **Жұмыс** термині **Әрекет** термині орнына пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e2661-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="e2661-134">Ұйымның жоспарлау режимін өзгерту</span><span class="sxs-lookup"><span data-stu-id="e2661-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="e2661-135">Ұйымның жоспарлау режимін анықтау үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="e2661-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="e2661-136">**Параметрлер** \> **Жалпы** \> **Параметрлер** тармағына өтіп, жоба параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e2661-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="e2661-137">**Жоба параметрлері** бетінде ұйымның әдепкі жоспарлау режимін таңдаңыз, содан кейін жоба менеджерінің жаңа жоба жасау кезінде параметрді алдын ала анықтау мүмкіндігін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="e2661-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="e2661-138">Жоба бойынша жоспарлау режимінің параметрін өзгерту</span><span class="sxs-lookup"><span data-stu-id="e2661-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="e2661-139">Егер ұйым жоба менеджеріне әдепкі жоспарлау режимін алдын ала анықтауға мүмкіндік берсе, жоба менеджері жаңа жоба жасаған кезде оны өзгерте алады.</span><span class="sxs-lookup"><span data-stu-id="e2661-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="e2661-140">Алайда жоба сақталғаннан кейін жоспарлау режимін өзгерту мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="e2661-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="e2661-141">Көшірілген жобалар</span><span class="sxs-lookup"><span data-stu-id="e2661-141">Copied projects</span></span>

<span data-ttu-id="e2661-142">Жоба жобаны көшіру әрекеті орындалған кезде жасалатындықтан, жоба менеджері жоспарлау режимін орната алмайды.</span><span class="sxs-lookup"><span data-stu-id="e2661-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="e2661-143">Тағайындалған жоба әрдайым ұйымдық деңгейде анықталған режимге сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="e2661-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="e2661-144">Көшірілген тапсырмалар</span><span class="sxs-lookup"><span data-stu-id="e2661-144">Copied tasks</span></span>

<span data-ttu-id="e2661-145">Тапсырма бір жобадан екіншісіне көшірілгенде, тапсырма тағайындалған жобаның жоспарлау режимін алады.</span><span class="sxs-lookup"><span data-stu-id="e2661-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
