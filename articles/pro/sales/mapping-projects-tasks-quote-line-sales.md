---
title: Жобалар мен тапсырмаларды жобаға негізделген баға ұсыну жолымен салыстыру
description: Бұл тақырып жобалар мен тапсырмаларды жобаға негізделген тапсырмалар жолымен салыстыру туралы ақпарат береді.
author: rumant
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 871d323136cd982bd48ed9aa2b9c34017951d2d8
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130720"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a><span data-ttu-id="88743-103">Жобалар мен тапсырмаларды жобаға негізделген баға ұсыну жолымен салыстыру</span><span class="sxs-lookup"><span data-stu-id="88743-103">Map projects and tasks to a project-based quote line</span></span>

<span data-ttu-id="88743-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="88743-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="88743-105">Жобаға негізделген баға ұсыну жолдарында әлдеқашан баға ұсыну жолына байланысты жобаның нақты тапсырмаларын салыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="88743-105">On project-based quote lines, you can map the specific tasks of a project that is already associated to a quote line.</span></span>

<span data-ttu-id="88743-106">Тапсырмаларды баға ұсыну жолымен салыстырған кезде, баға ұсыну жолында анықтаған келесі элементтер тек осы тапсырмаларға қатысты болады:</span><span class="sxs-lookup"><span data-stu-id="88743-106">When you map tasks to a quote line, the following items you defined on the quote line will only apply to those tasks:</span></span>

- <span data-ttu-id="88743-107">Төлем әдісі</span><span class="sxs-lookup"><span data-stu-id="88743-107">Billing method</span></span>
- <span data-ttu-id="88743-108">Төлем қабілеттілігі параметрлері</span><span class="sxs-lookup"><span data-stu-id="88743-108">Chargeability options</span></span>
- <span data-ttu-id="88743-109">Асырмау шектері</span><span class="sxs-lookup"><span data-stu-id="88743-109">Not-to-exceed limits</span></span>
- <span data-ttu-id="88743-110">Тұтынушылар</span><span class="sxs-lookup"><span data-stu-id="88743-110">Customers</span></span>

<span data-ttu-id="88743-111">Мысалы, бір кезеңі белгіленген баға, ал қалған барлық кезеңдері уақыт пен материал болатын жоба болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="88743-111">For example, you might have a project where one phase is fixed price and all the other phases are time and materials.</span></span> <span data-ttu-id="88743-112">Бұл жағдайда бірінші кезеңді және оның барлық еншілес тапсырмаларын осы кезеңнің бекітілген бағаның төлем әдісімен баға ұсыну жолына байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="88743-112">In this case, you can associate the first phase, and all of its child tasks, to the quote line for that phase with a fixed price billing method.</span></span> <span data-ttu-id="88743-113">Содан кейін барлық басқа кезеңдерді уақыт пен материалдарға негізделген баға ұсыну жолына байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="88743-113">You can then associate all the other phases to the time and materials-based quote line.</span></span>

## <a name="associate-tasks-to-project-based-quote-lines"></a><span data-ttu-id="88743-114">Тапсырмаларды жобаға негізделген баға ұсыну жолдарымен байланыстыру</span><span class="sxs-lookup"><span data-stu-id="88743-114">Associate tasks to project-based quote lines</span></span>

<span data-ttu-id="88743-115">Тапсырмаларды келесі орындардан баға ұсыну жолдарымен байланыстыруға болады:</span><span class="sxs-lookup"><span data-stu-id="88743-115">You can associate tasks with quote lines from the following locations:</span></span>

- <span data-ttu-id="88743-116">**Жоба** беті > **Тапсырма шоты** қойыншасы (оңтайлы)</span><span class="sxs-lookup"><span data-stu-id="88743-116">**Project** page > **Task billing** tab (optimal)</span></span>
- <span data-ttu-id="88743-117">**Баға ұсыну жолы** беті > **Ақылы тапсырмалар** қойыншасы</span><span class="sxs-lookup"><span data-stu-id="88743-117">**Quote Line** page > **Chargeable tasks** tab</span></span> 

### <a name="from-the-project-page"></a><span data-ttu-id="88743-118">Жоба бетінен:</span><span class="sxs-lookup"><span data-stu-id="88743-118">From the Project page</span></span>

<span data-ttu-id="88743-119">**Жоба** беті тапсырмаларды баға ұсыну жолдарымен байланыстырудың оңтайлы тәжірибесін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="88743-119">The **Project** page provides the optimal experience for associating tasks to quote lines.</span></span> <span data-ttu-id="88743-120">Бұл бетті бірнеше тапсырмаларды таңдау үшін және олардың барлығын, сонымен қатар олардың еншілес тапсырмаларын, таңдалған баға ұсыну жолымен байланыстыру үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="88743-120">You can use this page to select multiple tasks and associate all of them, plus their child tasks, to the selected quote line.</span></span>

1. <span data-ttu-id="88743-121">Жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасында **Жоба** өрісінің толтырылғанына көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="88743-121">On the **General** tab of a project–based quote line, verify the **Project** field is filled out.</span></span>
2. <span data-ttu-id="88743-122">**Қосылған тапсырмалар** өрісінде **Тек таңдалған тапсырмалар** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-122">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="88743-123">Жобаға негізделген баға ұсыну жолын сақтаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-123">Save the project-based quote line.</span></span> <span data-ttu-id="88743-124">Пішін жаңарған кезде **Ақылы тапсырмалар** қойыншасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="88743-124">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="88743-125">**Жалпы** қойыншасында **Жоба** өрісінен жобаның сілтемесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-125">On the **General** tab, select the link for the project from the **Project** field.</span></span>
5. <span data-ttu-id="88743-126">**Жоба** бетінде **Тапсырма шоты** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-126">On the **Project** page, select the **Task billing** tab.</span></span>
6. <span data-ttu-id="88743-127">Тапсырмаға сәйкес шот ұсынысын орнатуға қолданылатын екінші торда бір немесе бірнеше тапсырмаларды таңдап, содан кейін **Баға ұсыну жолдарын байланыстыру** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-127">In the second grid, which applies to task-specific billing setup, select one or more tasks and then select **Associate quote lines**.</span></span>
7. <span data-ttu-id="88743-128">Пайда болған диалогтік бетте баға ұсынысында жобаға негізделген баға ұсыну жолдарын көрсететін баға ұсыну жолын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-128">In the dialog page that appears, select a quote line that displays project-based quote lines on the quote.</span></span>
8. <span data-ttu-id="88743-129">**Есеп-шот ұсыну түрі** өрісінде осы тапсырмалардың ақылы немесе ақысыз екендігін көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="88743-129">In the **Billing type** field, indicate if these tasks are chargeable or non-chargeable.</span></span>
9. <span data-ttu-id="88743-130">Байланысқа таңдалған тапсырмалардың еншілес тапсырмаларын қосу керектігін көрсету үшін құсбелгіні қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-130">Select the check box to indicate if the association should include child tasks of the selected tasks.</span></span> <span data-ttu-id="88743-131">Құсбелгіні қою таңдалған тапсырмалардың еншілес тапсырмаларын баға ұсыну жолымен байланыстырады.</span><span class="sxs-lookup"><span data-stu-id="88743-131">Checking the box will associate the child tasks of the selected tasks to the quote line.</span></span>
10. <span data-ttu-id="88743-132">Диалогтік терезені жабу үшін **OK** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-132">Select **OK** to close the dialog.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="88743-133">Баға ұсыну жолы бетінен</span><span class="sxs-lookup"><span data-stu-id="88743-133">From the Quote line page</span></span>

<span data-ttu-id="88743-134">Жоба тапсырмаларын баға ұсыну жолдарына **Баға ұсыну жолы** бетіндегі **Ақылы тапсырмалар** қойыншасынан байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="88743-134">You can associate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

>[!NOTE]
><span data-ttu-id="88743-135">Жоба тапсырмаларын баға ұсыну жолдарына байланыстырудың оңтайлы орны - **Жоба** бетіндегі **Тапсырма шоты** қойыншасы.</span><span class="sxs-lookup"><span data-stu-id="88743-135">The optimal place to associate project tasks to quote lines is on the **Task billing** tab on the **Project** page.</span></span> <span data-ttu-id="88743-136">Тапсырмаларды **Баға ұсыну жолы** бетіндегі **Ақылы тапсырмалар** қойыншасынан байланыстырсаңыз, әр жобаны қолмен байланыстыру қажет.</span><span class="sxs-lookup"><span data-stu-id="88743-136">If you associate tasks from the **Chargeable tasks** tab on **Quote line** page, you must manually associate each project.</span></span>

1. <span data-ttu-id="88743-137">Жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасында **Жоба** өрісінде жобаның таңдалғанына көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="88743-137">On the **General** tab of a project–based quote line, verify that there is a project selected in the **Project** field.</span></span>
2. <span data-ttu-id="88743-138">**Қосылған тапсырмалар** өрісінде **Тек таңдалған тапсырмалар** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-138">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="88743-139">Жобаға негізделген баға ұсыну жолын сақтаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-139">Save the project-based quote line.</span></span> <span data-ttu-id="88743-140">Пішін жаңарған кезде **Ақылы тапсырмалар** қойыншасы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="88743-140">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="88743-141">**Ақылы тапсырмалар** қойыншасында **Баға ұсыну жолының тапсырмасын қосу** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-141">On the **Chargeable tasks** tab, select **Add a quote line task**.</span></span>
5. <span data-ttu-id="88743-142">**Баға ұсыну жолының тапсырмасы** бетіндегі **Тапсырмалар** өрісінде тапсырманы таңдаңыз және **Есеп-шот ұсыну түрі** өрісінде **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-142">On the **Quote line task** page, in the **Tasks** field, select the task and in the **Billing type** field, select **Save**.</span></span> 
6. <span data-ttu-id="88743-143">Бетті жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-143">Close the page.</span></span> <span data-ttu-id="88743-144">Таңдалған тапсырма енді баға ұсыну жолымен байланысты.</span><span class="sxs-lookup"><span data-stu-id="88743-144">The selected task is now associated to the quote line.</span></span>

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a><span data-ttu-id="88743-145">Тапсырмалардың жобаға негізделген баға ұсыну жолдарымен байланысын жою</span><span class="sxs-lookup"><span data-stu-id="88743-145">Disassociate tasks from project–based quote lines</span></span>

### <a name="from-the-project-page"></a><span data-ttu-id="88743-146">Жоба бетінен:</span><span class="sxs-lookup"><span data-stu-id="88743-146">From the Project page</span></span>

<span data-ttu-id="88743-147">Бұл әдіс тапсырмалардың баға ұсыну жолдарымен байланыстын жоюдың ең оңтайлы тәжірибесін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="88743-147">This method provides the most optimal experience for disassociating tasks from quote lines.</span></span> <span data-ttu-id="88743-148">Бірнеше тапсырмаларды таңдап, олардың барлығының, сонымен қатар олардың еншілес тапсырмаларының, таңдалған баға ұсыну жолымен байланысын жоюға болады.</span><span class="sxs-lookup"><span data-stu-id="88743-148">You can select multiple tasks and disassociate all of the them, plus their child tasks, from the selected quote line.</span></span>

1. <span data-ttu-id="88743-149">Жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасында **Жоба** өрісінде жоба сілтемесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-149">On the **General** tab of a project–based quote line, in the **Project** field, select the project link.</span></span>
2. <span data-ttu-id="88743-150">**Жоба** бетінде **Тапсырма шоты** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-150">On the **Project** page, select the **Task billing** tab.</span></span>
3. <span data-ttu-id="88743-151">Тапсырмаға сәйкес шот ұсынысын орнатуға қолданылатын екінші торда бір немесе бірнеше тапсырмаларды таңдап, содан кейін **Баға ұсыну жолдарымен байланысты жою** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-151">In the second grid, which applies to task-specific billing setup, select one or more tasks, and then select **Disassociate quote lines**.</span></span>
4. <span data-ttu-id="88743-152">Пайда болған диалогтік бетте баға ұсыну жолын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-152">In the dialog page that appears, select a quote line.</span></span>
5. <span data-ttu-id="88743-153">Байланысқа таңдалған тапсырмалардың еншілес тапсырмаларынан жою керектігін де көрсету үшін құсбелгіні қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-153">Select the check box to indicate whether the association should also be removed from child tasks of the selected tasks.</span></span> <span data-ttu-id="88743-154">Құсбелгіні қою сондай-ақ таңдалған тапсырмалардың еншілес тапсырмаларының баға ұсыну жолымен байланысын жояды.</span><span class="sxs-lookup"><span data-stu-id="88743-154">Checking the box will also disassociate the child tasks of the selected tasks to the quote line.</span></span>
6. <span data-ttu-id="88743-155">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-155">Select **OK**.</span></span> <span data-ttu-id="88743-156">Ескерту хабары осы байланысты жойсаңыз, тапсырмада бұрын жазылған кез келген нақты көрсеткішті қалпына келтіруге болатынын хабарлайды.</span><span class="sxs-lookup"><span data-stu-id="88743-156">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
7. <span data-ttu-id="88743-157">Жалғастыру үшін **OK** түймешігін таңдап, тапсырма мен жобаға негізделген баға ұсыну жолы арасындағы байланысты жойыңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-157">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="88743-158">Баға ұсыну жолы бетінен</span><span class="sxs-lookup"><span data-stu-id="88743-158">From the Quote line page</span></span>

<span data-ttu-id="88743-159">Сондай-ақ жоба тапсырмаларының баға ұсыну жолдарымен байланысын **Баға ұсыну жолы** бетіндегі **Ақылы тапсырмалар** қойыншасынан жоюға болады.</span><span class="sxs-lookup"><span data-stu-id="88743-159">You can also disassociate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

1. <span data-ttu-id="88743-160">**Ақылы тапсырмалар** қойыншасында **Баға ұсыну жолының тапсырмасын жою** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-160">On the **Chargeable tasks** tab, select **Delete a quote line task**.</span></span>
2. <span data-ttu-id="88743-161">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-161">Select **OK**.</span></span> <span data-ttu-id="88743-162">Ескерту хабары осы байланысты жойсаңыз, тапсырмада бұрын жазылған кез келген нақты көрсеткішті қалпына келтіруге болатынын хабарлайды.</span><span class="sxs-lookup"><span data-stu-id="88743-162">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
3. <span data-ttu-id="88743-163">Жалғастыру үшін **OK** түймешігін таңдап, тапсырма мен жобаға негізделген баға ұсыну жолы арасындағы байланысты жойыңыз.</span><span class="sxs-lookup"><span data-stu-id="88743-163">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

>[!NOTE]
> <span data-ttu-id="88743-164">Бұл процедура тапсырманы жобадан жоймайды.</span><span class="sxs-lookup"><span data-stu-id="88743-164">This procedure doesn't delete the task from the project.</span></span> <span data-ttu-id="88743-165">Ол тек тапсырмалардың жобаға негізделген баға ұсыну жолымен байланысын жояды.</span><span class="sxs-lookup"><span data-stu-id="88743-165">It only removes the task association from the project-based quote line.</span></span>
