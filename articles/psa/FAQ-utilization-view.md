---
title: Ресурстарға арналған ақылы қолданыс түрін көру
description: Бұл тақырыпта ресурсты қолдану көрінісі туралы ақпарат беріледі.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: a1d1db532c65b2a13f3cf4e1281a5987490b96df
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122170"
---
# <a name="view-chargeable-utilization-for-resources"></a><span data-ttu-id="534e4-103">Ресурстарға арналған ақылы қолданыс түрін көру</span><span class="sxs-lookup"><span data-stu-id="534e4-103">View chargeable utilization for resources</span></span>
 
<span data-ttu-id="534e4-104">**Project Service ресурстарын қолдану** бетіндегі **Қолданыс көрінісінде** резервтелетін әр ресурсқа арналған ақылы қолданыс түрі көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="534e4-104">The **Utilization View** on the **Project Service Resource Utilization** page shows the chargeable utilization for each bookable resource.</span></span> <span data-ttu-id="534e4-105">Көрініс кесте тақтасына негізделетіндіктен, көптеген бірдей функцияларды таба аласыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-105">Because the view is based on the schedule board, you’ll find many of the same functions.</span></span>

> ![Қолданыс көрінісі скриншоты](media/FAQ-utilization-1.png)
 

<span data-ttu-id="534e4-107">Ақылы қолданыс есептеуі келесідей жұмыс істейді:</span><span class="sxs-lookup"><span data-stu-id="534e4-107">The chargeable utilization calculation works as follows:</span></span>

   <span data-ttu-id="534e4-108">Ақылы қолданыс = (Ақылы нақты сағаттар) / (ресурс сыйымдылығы).</span><span class="sxs-lookup"><span data-stu-id="534e4-108">Chargeable utilization = (Chargeable actual hours) / (resource capacity)</span></span>

<span data-ttu-id="534e4-109">Ұяшықтарда таңдалған кезең бойынша есептелген ақылы қолданыс түрі көрсетілген (күндер, апталар немесе айлар).</span><span class="sxs-lookup"><span data-stu-id="534e4-109">The cells represent the calculated chargeable utilization for the selected period (days, weeks, or months).</span></span>

<span data-ttu-id="534e4-110">Әрбір ұяшықтағы түстерде мақсатты ақылы қолданыспен салыстырғанда ресурстың ақылы қолданысы көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="534e4-110">The colors in each cell show the chargeable utilization for a resource as compared to their target chargeable utilization.</span></span> 

<span data-ttu-id="534e4-111">Мақсатты қолданысты ресурстың әдепкі рөліне немесе жеке ресурсқа орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-111">The target utilization can be set on the resource’s default role or on the individual resource itself.</span></span> <span data-ttu-id="534e4-112">Есептеу кезінде алдымен мақсаттың жеке мәні, одан кейін ресурстың әдепкі рөлі тексеріледі.</span><span class="sxs-lookup"><span data-stu-id="534e4-112">The calculation looks at the individual for the target first, and then to the resource’s default role.</span></span>

## <a name="set-target-on-a-resource"></a><span data-ttu-id="534e4-113">Мақсатты ресурсқа орнату</span><span class="sxs-lookup"><span data-stu-id="534e4-113">Set target on a resource</span></span>

1. <span data-ttu-id="534e4-114">**Ресурстар** \> **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="534e4-114">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="534e4-115">Жазбаны ашу үшін ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-115">Select a resource to open the record.</span></span> 
3. <span data-ttu-id="534e4-116">**Project Service** қойыншасында, ресурстың мақсатты қолданысын орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="534e4-116">On the **Project Service** tab, you can set the resource’s target utilization.</span></span>

> ![Мақсатты қолданысты орнату үшін Жоба қызметі қойыншасын пайдалану скриншоты](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a><span data-ttu-id="534e4-118">Рөлге мақсатты қолданысты орнату</span><span class="sxs-lookup"><span data-stu-id="534e4-118">Set target utilization on a role</span></span>

1. <span data-ttu-id="534e4-119">**Ресурстар** \> **Ресурс рөлдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="534e4-119">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="534e4-120">Рөлді таңдап, жазбаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-120">Select a role and open the record.</span></span> 
3. <span data-ttu-id="534e4-121">Рөлдің мақсатты қолданысын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-121">Set the target utilization for the role.</span></span>

> ![Мақсатты қолданысты орнату үшін Ресурс рөлдерін пайдалану скриншоты](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a><span data-ttu-id="534e4-123">Ресурстың ақылы қолданысын есептеу</span><span class="sxs-lookup"><span data-stu-id="534e4-123">Calculate chargeable utilization for a resource</span></span>

<span data-ttu-id="534e4-124">Ресурстың ақылы қолданысын есептеу үшін, біраз алғышарттарды орындауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="534e4-124">To calculate chargeable utilization for a resource, you will need to complete some pre-requisites.</span></span> 

### <a name="set-default-role-for-individual-resource"></a><span data-ttu-id="534e4-125">Жеке ресурс үшін әдепкі рөлді орнату</span><span class="sxs-lookup"><span data-stu-id="534e4-125">Set default role for individual resource</span></span>

<span data-ttu-id="534e4-126">Алдымен, мақсатты қолданыс жеке ресурсқа немесе ресурс рөлдеріне орнатылуы керек.</span><span class="sxs-lookup"><span data-stu-id="534e4-126">First, the target utilization must be set on either the individual resource or on resource roles.</span></span> <span data-ttu-id="534e4-127">Мақсаттар үшін ресурс рөлдері пайдаланылса, әрбір жеке ресурстың әдепкі рөлі болуы қажет.</span><span class="sxs-lookup"><span data-stu-id="534e4-127">If you are using resource roles for targets, each individual resource must have a default role.</span></span> 

1. <span data-ttu-id="534e4-128">Оны орнату үшін, **Ресурстар** \> **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="534e4-128">To set this, go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="534e4-129">Ресурсты таңдап, жазбаны ашыңыз да, **Project Service** қойыншасы таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-129">Select a resource, open the record, and then select the **Project Service** tab.</span></span> 
3. <span data-ttu-id="534e4-130">**Ресурс рөлі** торында ресурс үшін бір рөл бар екеніне және **Әдепкі бойынша** күйі **Иә** күйіне орнатылғанына көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="534e4-130">In the **Resource Role** grid, make sure there’s one role for the resource and **Is Default** is set to **Yes**.</span></span>
 
### <a name="change-billing-type-for-resource-role"></a><span data-ttu-id="534e4-131">Ресурс рөлінің шот ұсыну түрін өзгерту</span><span class="sxs-lookup"><span data-stu-id="534e4-131">Change billing type for resource role</span></span>

<span data-ttu-id="534e4-132">Ресурс рөлдері **Ақылы** шот ұсыну түріне орнатылуы керек.</span><span class="sxs-lookup"><span data-stu-id="534e4-132">The resource roles must be set to have a billing type of **Chargeable**.</span></span> 

1. <span data-ttu-id="534e4-133">**Ресурстар** \> **Ресурс рөлдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="534e4-133">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="534e4-134">Жаңарту қажет жазбаны ашып, әдепкі шот ұсыну түрін **Ақылы** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-134">Open the record you want to update, and then set the billing type default to **Chargeable**.</span></span>

### <a name="set-working-hours-for-resource-role"></a><span data-ttu-id="534e4-135">Ресурс рөлінің жұмыс уақытын орнату</span><span class="sxs-lookup"><span data-stu-id="534e4-135">Set working hours for resource role</span></span>
 
<span data-ttu-id="534e4-136">Ресурста мүмкіндікті есептеуге арналған жұмыс уақыты болуы керек.</span><span class="sxs-lookup"><span data-stu-id="534e4-136">The resource must have working hours for the capacity calculation.</span></span> 

1. <span data-ttu-id="534e4-137">**Ресурстар** \> **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="534e4-137">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="534e4-138">Жазбаны ашу үшін ресурсты таңдап, **Жұмыс уақытын көрсету** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-138">Select a resource to open the record, and then select **Show Work Hours**.</span></span> 
3. <span data-ttu-id="534e4-139">**Ресурстар тізімі** көрінісінен **Жұмыс уақыты үлгісін** қолдану арқылы ресурстар тізімін жаппай жаңарта аласыз.</span><span class="sxs-lookup"><span data-stu-id="534e4-139">You can bulk-update the list of resources by applying a **Work Hour Template** from the **Resource List** view.</span></span>

## <a name="troubleshooting-chargeable-actual-hours"></a><span data-ttu-id="534e4-140">Ақылы нақты сағаттар бойынша ақауларды жою</span><span class="sxs-lookup"><span data-stu-id="534e4-140">Troubleshooting chargeable actual hours</span></span>

<span data-ttu-id="534e4-141">Ақылы нақты сағаттар саны **Нақты мәндер** нысанынан алынады.</span><span class="sxs-lookup"><span data-stu-id="534e4-141">The chargeable actual hours are sourced from the **Actuals** entity.</span></span> <span data-ttu-id="534e4-142">**Ақылы** шот ұсыну түріндегі нақты мәндер есептеуге қосылады және осыған байланысты нақты мәндері ақылы болып есептелетін жобаларға ие болуыңыз қажет.</span><span class="sxs-lookup"><span data-stu-id="534e4-142">Actuals with a billing type of **Chargeable** are included in the calculation and, for this reason, you must have projects where the actuals that are chargeable.</span></span>

<span data-ttu-id="534e4-143">Ақылы қолданысты көрмесеңіз, мұнда тексеруге болатын кейбір заттар болады:</span><span class="sxs-lookup"><span data-stu-id="534e4-143">If you are not seeing chargeable utilization, here are some things you can check:</span></span>

- <span data-ttu-id="534e4-144">Ресурста мүмкіндікке анықталған жұмыс уақыты бар.</span><span class="sxs-lookup"><span data-stu-id="534e4-144">The resource has working hours defined for capacity.</span></span>
- <span data-ttu-id="534e4-145">Ресурстың жеке анықталған қолданыс мақсаты немесе әдепкі белгіленген рөлі бар.</span><span class="sxs-lookup"><span data-stu-id="534e4-145">The resource has either an individually defined utilization target or has a default role assigned to it.</span></span> <span data-ttu-id="534e4-146">Рөлде анықталған қолданыс мақсаты бар.</span><span class="sxs-lookup"><span data-stu-id="534e4-146">The role has a utilization target defined for it.</span></span>
- <span data-ttu-id="534e4-147">Нақты мәндердің қолданыс есептеуіне болжанған мерзімге арналған **Ақылы** шот ұсыну түрі бар.</span><span class="sxs-lookup"><span data-stu-id="534e4-147">Actuals have a billing type of **Chargeable** for the period you are expecting a utilization calculation for.</span></span> <span data-ttu-id="534e4-148">Ақылыдан басқа шот ұсыну түрі бар нақты мәндерді көрсеңіз, келесілерді тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="534e4-148">Check the following if you are seeing actuals with billing types other than chargeable:</span></span>

  - <span data-ttu-id="534e4-149">Нақты мәнде пайдаланылатын рөлде ақылыдан басқа әдепкі шот ұсыну түрі бар.</span><span class="sxs-lookup"><span data-stu-id="534e4-149">The role used on the actual has a default billing type of something other than chargeable.</span></span>
  - <span data-ttu-id="534e4-150">Жобаның келісім-шарт жолы ақылы емес күйге орнатылған.</span><span class="sxs-lookup"><span data-stu-id="534e4-150">The role on the project contract line backing the project has been set to non-chargeable.</span></span>
  - <span data-ttu-id="534e4-151">Жобада байланысты келісім-шарт жолы жоқ.</span><span class="sxs-lookup"><span data-stu-id="534e4-151">The project does not have an associated contract line.</span></span>

