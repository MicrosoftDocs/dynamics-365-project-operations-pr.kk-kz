---
title: 2.x қолданба нұсқасында ресурстарды қалай "жұмсақ тіркеуге" болады?
description: Бұл мақалада Жоба қызметі көмегімен жоба тобы мүшелерін "жұмсақ тіркеу" жолы сипатталған.
author: JohnPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.prod: Applies to Project Service version 2.x
ms.technology: ''
ms.assetid: 27063de4-cb0c-436f-970e-c87ebcab92db
ms.author: john.burrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: aad119c0907cdd31220a0d73e6e7d99ee63e2e13
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753076"
---
# <a name="how-do-i-soft-book-resources-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="8fb86-103">Веб-бағдарламаға (Project Service v2.x бағдарламасы) ресурстарды қалай "жұмсақ тіркеуге" болады?</span><span class="sxs-lookup"><span data-stu-id="8fb86-103">How do I "soft book" resources in the web app (Project Service app v2.x)?</span></span>

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="8fb86-104">Ресурсты жобаға белгілеу жоспарланғанын көрсету үшін ресурсты жоба тобына болжалды жоспарлауға немесе "жұмсақ тіркеуге" болады.</span><span class="sxs-lookup"><span data-stu-id="8fb86-104">You can tentatively schedule or "soft book" a resource onto a project team to show you plan to assign the resource to a project.</span></span> <span data-ttu-id="8fb86-105">Жұмсақ тіркеу пәрмені ресурстың қолжетімді мүмкіндігін пайдаланбайды.</span><span class="sxs-lookup"><span data-stu-id="8fb86-105">Soft bookings don’t consume a resource’s available capacity.</span></span> <span data-ttu-id="8fb86-106">Жұмсақ тіркелген топ мүшелері жоба тапсырмаларға белгіленбейді.</span><span class="sxs-lookup"><span data-stu-id="8fb86-106">Soft-booked team members can’t be assigned to project tasks.</span></span> <span data-ttu-id="8fb86-107">Тек Қатты тіркелген күйдегі және Орындалған түрдегі ресурстарды тапсырмаларға белгілеуге болады (оларда тағайындау талпынысын қамтуға тіркеу уақыты жеткілікті деп болжанады).</span><span class="sxs-lookup"><span data-stu-id="8fb86-107">Only resources with the Status Hard Booked and Commit Type Committed can be assigned to tasks (assuming they have enough hard booking hours to cover the assignment effort).</span></span>

<span data-ttu-id="8fb86-108">Жұмсақ тіркелген жоба тобы мүшелері Жұмсақ тіркеу бағанында көрсетілген жұмсақ тіркелген сағаттары бар Топ мүшесі торында көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8fb86-108">Soft-booked project team members show up in the Team Member grid with their soft-booked hours shown in the Soft Book column.</span></span> <span data-ttu-id="8fb86-109">Сонымен қатар, олар кесте тақтасында көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8fb86-109">They also show up on the schedule board.</span></span> <span data-ttu-id="8fb86-110">Оған қоса, олар жұмсақ тіркеу ретінде мүмкіндікті қолдану ресурс мүмкіндігін қолданбайтынын көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="8fb86-110">Again, they don’t indicate any consumption of capacity as soft-booking doesn’t consume capacity of a resource.</span></span>

<span data-ttu-id="8fb86-111">Project Service 2.x жобасына топ мүшесін жұмсақ тіркеудің үш жолы бар.</span><span class="sxs-lookup"><span data-stu-id="8fb86-111">There are three ways to soft-book a team member onto a project with Project Service version 2.x.</span></span> <span data-ttu-id="8fb86-112">Кесте тақтасымен жұмсақ тіркеуге, Тапсырыстарды жүргізу мүмкіндігін пайдалануға немесе жалпы ресурсты жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="8fb86-112">You can soft-book with the schedule board, use the Maintain Bookings feature, or by creating a generic resource.</span></span> <span data-ttu-id="8fb86-113">Бұл әдістер төменде сипатталған.</span><span class="sxs-lookup"><span data-stu-id="8fb86-113">These methods are described below.</span></span>

## <a name="soft-book-with-the-schedule-board"></a><span data-ttu-id="8fb86-114">Кесте тақтасымен жұмсақ тіркеу</span><span class="sxs-lookup"><span data-stu-id="8fb86-114">Soft-book with the schedule board</span></span>

<span data-ttu-id="8fb86-115">Кесте тақтасымен жұмсақ тіркеу үшін, осы процедураны орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="8fb86-115">To soft-book with the schedule board, follow this procedure:</span></span> 
1. <span data-ttu-id="8fb86-116">Кесте тақтасын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-116">Open the schedule board.</span></span>
2. <span data-ttu-id="8fb86-117">Кесте тақтасының Тапсырыс талаптары тақтасы астынан Жоба қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-117">Select the Project tab on the bottom Booking Requirements panel of the schedule board.</span></span>
3. <span data-ttu-id="8fb86-118">Ресурсты жұмсақ тіркеу керек жобаны табыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-118">Find the project you wish to soft-book a resource on.</span></span> <span data-ttu-id="8fb86-119">Көптеген жобалар болса, Жоба бағаны тақырыбын басып, жобаны табу үшін сүзгіні пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-119">If you have many projects, click on the Project column header and then use the filter to find your project.</span></span>
4. <span data-ttu-id="8fb86-120">Жобаны басып, ресурс уақыты торына сүйреп апарыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-120">Click on the project, then drag and drop it on the resource’s time grid.</span></span>
5. <span data-ttu-id="8fb86-121">Бұл оң жақта Ресурс тапсырысын жасау тақтасын ашады.</span><span class="sxs-lookup"><span data-stu-id="8fb86-121">This opens the Create Resource Booking panel on the right.</span></span> <span data-ttu-id="8fb86-122">Басталу және аяқталу күнін реттеп, Тапсырыс күйін жұмсақ ретінде таңдап, сағат санын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-122">Adjust the start and end date, select the Booking Status as Soft and set the hours.</span></span> 
6. <span data-ttu-id="8fb86-123">Тапсырыс беру түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-123">Click Book.</span></span>
7. <span data-ttu-id="8fb86-124">Жобаға оралсаңыз, ресурс енді Жұмсақ тіркеу бағанындағы жұмсақ тіркелген сағат саны бар топ мүшесі ретінде көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="8fb86-124">Back on the project, the resource will now show as a team member with the soft booked hours in the Soft Book column.</span></span>

<span data-ttu-id="8fb86-125">Оларды жұмыс декомпозициясының құрылымындағы (WBS) тапсырмаларға белгілей алмайтыныңызды ескеріңіз, себебі ресурстар белгіленетін топқа қатты тіркелуі керек.</span><span class="sxs-lookup"><span data-stu-id="8fb86-125">Note that you can’t assign them to tasks on the work breakdown structure (WBS) as resources must be hard booked on the team to be assigned.</span></span>

## <a name="soft-book-using-the-maintain-bookings-feature"></a><span data-ttu-id="8fb86-126">Тапсырыстарды жүргізу мүмкіндігімен жұмсақ тіркеу</span><span class="sxs-lookup"><span data-stu-id="8fb86-126">Soft-book using the Maintain Bookings feature</span></span>

<span data-ttu-id="8fb86-127">Тапсырыстарды жүргізу пәрменімен жұмсақ тіркеу үшін, осы процедураны орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="8fb86-127">To soft-book with Maintain Bookings follow this procedure:</span></span>
1. <span data-ttu-id="8fb86-128">Топ мүшесі торынан Жаңа түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-128">From the team member grid, Click New.</span></span>
2. <span data-ttu-id="8fb86-129">Тіркелетін ресурсты, рөлді, басталу/аяқталу күндерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-129">Select the bookable resource, role, from/to.</span></span>
3. <span data-ttu-id="8fb86-130">Ешқандай күйінен басқа тағайындау әдісін таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="8fb86-130">Select an allocation method other than None:</span></span>
- <span data-ttu-id="8fb86-131">Толық мүмкіндік</span><span class="sxs-lookup"><span data-stu-id="8fb86-131">Full Capacity</span></span>
- <span data-ttu-id="8fb86-132">Пайыздық мүмкіндік</span><span class="sxs-lookup"><span data-stu-id="8fb86-132">Percentage Capacity</span></span>
- <span data-ttu-id="8fb86-133">Сағаттарды бірқалыпты тарату бойынша</span><span class="sxs-lookup"><span data-stu-id="8fb86-133">By Hours Distribute Evenly</span></span>
- <span data-ttu-id="8fb86-134">Сағаттарды алдын ала жүктеу бойынша</span><span class="sxs-lookup"><span data-stu-id="8fb86-134">By Hours Front Load</span></span>
4. <span data-ttu-id="8fb86-135">Сақтау түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-135">Click Save.</span></span> <span data-ttu-id="8fb86-136">Ресурсты топ торынан көресіз және сағаттары Қатты болып көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="8fb86-136">You’ll see the resource on the team grid and their hours indicated as Hard.</span></span>
5. <span data-ttu-id="8fb86-137">Тапсырыстарды жүргізу түймесін басу арқылы ресурс тапсырыстарын жүргізіңіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-137">Maintain the resource’s bookings by clicking Maintain Bookings.</span></span>
6. <span data-ttu-id="8fb86-138">Кесте тақтасы ашылса, тапсырыстарды көрсету үшін ресурсты кеңейтіңіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-138">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="8fb86-139">Қатты ретінде көрсетілген тапсырысты көресіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-139">You will see the booking indicated as Hard.</span></span>
7. <span data-ttu-id="8fb86-140">Күйді өзгерту параметрі астынан тапсырысты тінтуірдің оң жағымен басып, Жұмсақ тіркеу параметрін, одан кейін Жұмсақ параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-140">Right-click the booking, under Change Status, select Soft Book and then Soft.</span></span> <span data-ttu-id="8fb86-141">Енді тапсырыс күйі Жұмсақ болады.</span><span class="sxs-lookup"><span data-stu-id="8fb86-141">The booking status is now Soft.</span></span>
8. <span data-ttu-id="8fb86-142">Кесте тақтасын жапқаннан кейін топ мүшесі торында ресурс сағаттары Қатты күйден Жұмсақ күйге өзгертілгенін көресіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-142">After closing the schedule board, you’ll see that the hours for the resource have changed from Hard to Soft on the team member grid.</span></span>
<span data-ttu-id="8fb86-143">Топқа ресурсты қатты тіркеп, тапсырмаларын WBS жүйесіне белгілеген болсаңыз, Қатты күйінен Жұмсақ күйіне өзгерту үшін тапсырыстар жүргізу параметрі пайдаланылған кезде ол осы ресурс тапсырмалар тағайындауларын жояды, тапсырмаларға тек қатты тіркелген ресурстарды белгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="8fb86-143">Note that if you hard book a resource onto the team and then assign them tasks in the WBS, when you use maintain bookings to change the status of Hard to Soft, it will remove the assignments from the tasks for that resource, as only hard booked resources can be assigned to tasks.</span></span>

## <a name="soft-book-by-creating-a-generic-resource"></a><span data-ttu-id="8fb86-144">Жалпы ресурсты жасау арқылы жұмсақ тіркеу</span><span class="sxs-lookup"><span data-stu-id="8fb86-144">Soft-book by creating a generic resource</span></span>

<span data-ttu-id="8fb86-145">Жалпы ресурс тобы мүшесін құру, кесте тақтасын немесе ресурс сұрауын орындау және тіркеу барысында түрін өзгерту арқылы жұмсақ тіркеуді жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-145">You can create a soft-booking by generating a generic resource team member, fulfilling with schedule board or Resource Request and changing the type during the booking.</span></span>
<span data-ttu-id="8fb86-146">Осыны істеу үшін, келесі процедураны пайдаланыңыз:</span><span class="sxs-lookup"><span data-stu-id="8fb86-146">To do this, use the following procedure:</span></span>

1. <span data-ttu-id="8fb86-147">Жобаның WBS жүйесінде жалпы топ мүшелерін құру керек тапсырмаларға рөлдерді белгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-147">On the project WBS, assign roles to the tasks you wish to generate generic team members for.</span></span>
2. <span data-ttu-id="8fb86-148">Жоба тобын құру түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-148">Click Generate Project Team.</span></span>
3. <span data-ttu-id="8fb86-149">Жоба тобы мүшесі торынан жалпы ресурсты таңдап, Тіркеу түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-149">On the project team member grid, select the generic resource and click Book.</span></span>
4. <span data-ttu-id="8fb86-150">Кесте тақтасынан тіркеу керек ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-150">On the schedule board, select the resource that you wish to book.</span></span>
5. <span data-ttu-id="8fb86-151">Кесте тақтасының Ресурс тапсырысын жасау тақтасында Тапсырыс күйіне Жұмсақ күйіне өзгертіңіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-151">On the schedule board’s Create Resource Booking panel, change the Booking Status to Soft.</span></span>
6. <span data-ttu-id="8fb86-152">Тіркеу немесе Тіркеп шығу түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-152">Click Book or Book and Exit.</span></span>

<span data-ttu-id="8fb86-153">Кесте тақтасын жапқаннан кейін Жұмсақ тіркелген сағат саны мен белгіленген сағат саны көмегімен топқа қосылған, таңдалған ресурсты көресіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-153">After closing the schedule board, you’ll see the selected resource added to the team with Soft booked hours as well as assigned hours.</span></span> <span data-ttu-id="8fb86-154">Сонымен қатар, жұмсақ тіркелген топ мүшесіне белгіленген тапсырмалар индикаторы ретінде топ қалған жалпы ресурсты көресіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-154">You’ll also see that the generic resource remains on the team as an indicator that the tasks are assigned to a soft-booked team member.</span></span>

<span data-ttu-id="8fb86-155">Жұмсақ тіркелген топ мүшесі ресурсын қатты тіркелген топ мүшесіне өзгертуге дайын болғанда оларды тапсырмаларға белгілей белгілей алу үшін, келесі әрекетті орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="8fb86-155">When you’re ready to change a soft-booked team member resource to a hard-booked team member so that you can assign them to tasks, do the following:</span></span>

1. <span data-ttu-id="8fb86-156">Ресурсты таңдап, Тапсырыстарды жүргізу түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-156">Select that resource and click Maintain Bookings.</span></span>
2. <span data-ttu-id="8fb86-157">Кесте тақтасы ашылса, тапсырыстарды көрсету үшін ресурсты кеңейтіңіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-157">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="8fb86-158">Жұмсақ ретінде белгіленген тапсырысты көресіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-158">You’ll see the booking marked as Soft.</span></span>
3. <span data-ttu-id="8fb86-159">Күйді өзгерту параметрі астынан тапсырысты тінтуірдің оң жағымен басып, Қатты тіркеу параметрін, одан кейін Қатты параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-159">Right-click the booking, under Change Status, select Hard Book and then Hard.</span></span> <span data-ttu-id="8fb86-160">Енді тапсырыс күйі Қатты болады.</span><span class="sxs-lookup"><span data-stu-id="8fb86-160">The booking status is now Hard.</span></span>
4. <span data-ttu-id="8fb86-161">Кесте тақтасын жапқаннан кейін топ мүшесі торында ресурс сағаттары Жұмсақ күйден Қатты күйге өзгертілгенін көресіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-161">After closing the schedule board, you’ll see that the hours for the resource have changed from Soft to Hard on the team member grid.</span></span> <span data-ttu-id="8fb86-162">Енді ресурсты тапсырмаларға белгілей аласыз (осында қатты тіркелген сағаттар саны мен тағайындау тапсырмасының талпыныс сағаттары саны арасында туралау берілген).</span><span class="sxs-lookup"><span data-stu-id="8fb86-162">You may now assign the resource to tasks (provided there is alignment between the hard-booked hours and the effort hours of the task for assignment).</span></span> <span data-ttu-id="8fb86-163">Жоғарыдағы 3-элементте жалпы ресурсты орындау қадамдары орындалса, жұмсақ тіркелген ресурс күйін қатты күйіне өзгерткен кезде жалпы топ мүшесі топтан жойылатынын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="8fb86-163">Note that if you followed the generic resource fulfilment steps in item #3 above, when you change the status of the soft-booked bookable resource to hard, the generic team member is removed from the team.</span></span>
