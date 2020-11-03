---
title: Кесте тақтасынан жоба тапсырысын жасау
description: Бұл тақырыпта кесте тақтасынан жоба тапсырысын жасау жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 57fbc71681015fca73cdda4bc7d392f6be4289f3
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079677"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a><span data-ttu-id="29b88-103">Кесте тақтасынан жоба тапсырысын жасау</span><span class="sxs-lookup"><span data-stu-id="29b88-103">Create a project booking from the Schedule board</span></span>

<span data-ttu-id="29b88-104">Ресурсты жобаға тікелей жобаның **Топ** қойыншасынан немесе жалпы топ мүшесі тағайындауынан ресурс талабын жасап, жасалған талапты жоба тобы мүшесімен орындау арқылы тіркеуге болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-104">You can book a resource onto a project directly from the **Team** tab of the project or by generating a resource requirement from a generic team member assignment and then fulfilling the generated requirement with a project team member.</span></span>

<span data-ttu-id="29b88-105">Сондай-ақ ресурсты кесте тақтасынан жобаға тікелей тіркеуге болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-105">You can also book a resource onto a project directly from the Schedule board.</span></span> <span data-ttu-id="29b88-106">Бұны шешудің үш жолы бар:</span><span class="sxs-lookup"><span data-stu-id="29b88-106">There are three ways to do this:</span></span>

- <span data-ttu-id="29b88-107">**Құрылған ресурс талабынан тіркеу:** жалпы ресурсты жасап, жоба ішінде тапсырмаларды тағайындағаннан кейін, ресурс талабын жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-107">**Book from a generated resource requirement:** You can generate a resource requirement after you create a generic resource and assign tasks within a project.</span></span>

- <span data-ttu-id="29b88-108">**Негізгі талаптан тіркеу:** негізгі талаптар **Жоба** қойыншасындағы кесте тақтасында көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="29b88-108">**Book from the primary requirement:** The primary requirements show up on the Schedule board on the **Project** tab.</span></span> 

- <span data-ttu-id="29b88-109">**Жаңа ресурс талабынан тіркеу:** ресурс талабын жаңадан жасап, оны жобамен байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-109">**Book from a new resource requirement:** You can create a resource requirement from scratch and associate it with a project.</span></span> <span data-ttu-id="29b88-110">Кесте тақтасында ресурс талабы **Ашық талаптар** қойыншасында көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="29b88-110">On the Schedule board, the resource requirement shows up on the **Open Requirements** tab.</span></span>

## <a name="book-from-a-generated-resource-requirement"></a><span data-ttu-id="29b88-111">Құрылған ресурс талабынан тіркеу</span><span class="sxs-lookup"><span data-stu-id="29b88-111">Book from a generated resource requirement</span></span>

<span data-ttu-id="29b88-112">Жалпы ресурсты жасап, оны жобадағы бір немесе бірнеше тапсырмаға тағайындауға болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-112">You can create a generic resource and assign it one or more tasks within a project.</span></span> <span data-ttu-id="29b88-113">Содан кейін жалпы топ мүшесінен ресурс талабын құруға болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-113">Then you can generate a resource requirement from the generic team member.</span></span> 

1.  <span data-ttu-id="29b88-114">Кесте тақтасында бұл ресурс **Ашық талаптар** қойыншасында көрсетіледі. Көптеген ашық талаптарыңыз болса, торда баған сүзгілерін пайдалану керек болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29b88-114">On the Schedule board, this resource will show up on the **Open Requirements** tab. You might need to use column filters on the grid if you have many open requirements.</span></span> 

    <span data-ttu-id="29b88-115">![Кесте тақтасында "Талаптар" қойыншасын ашу](media/FAQ-Project-Booking-Schedule-Board-1.png "Тапсырыстар мен тағайындаулар кестесі скриншоты")</span><span class="sxs-lookup"><span data-stu-id="29b88-115">![Open Requirements tab on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-1.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="29b88-116">Талапты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29b88-116">Select the requirement.</span></span> <span data-ttu-id="29b88-117">Осы кезде таңдалған жолдың жоғарғы жағында **Қолжетімділікті табу** қойыншасы пайда болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-117">The **Find Availability** tab will appear at the top of the selected row.</span></span>
 
3. <span data-ttu-id="29b88-118">Қойыншаны таңдаған кезде, кесте тақтасы "Кесте көмекшісі" режимінде ашылып, ресурс талабына сәйкес келетін қолжетімді ресурстарды сүзгілейді.</span><span class="sxs-lookup"><span data-stu-id="29b88-118">When you select the tab, the Schedule Assistant mode of the Schedule board opens and then filters the available resources that meet the resource requirement.</span></span> <span data-ttu-id="29b88-119">Содан кейін ресурсты тіркеуге болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-119">After that, you can book a resource.</span></span>

4. <span data-ttu-id="29b88-120">Сонымен қатар, таңдалған қатарды кесте тақтасының астынан жоғарыдағы тордағы ресурс ұяшығына сүйреп апаруға болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-120">You can also drag and drop the selected row from the bottom of the Schedule board to a resource cell in the grid above.</span></span> <span data-ttu-id="29b88-121">Оны апарған кезде оң жақта **Ресурс тапсырысын жасау** тақтасы ашылады.</span><span class="sxs-lookup"><span data-stu-id="29b88-121">When you drop it, it opens the **Create Resource Booking** panel on the right.</span></span>

    <span data-ttu-id="29b88-122">**Тіркеу** параметрін таңдау ресурсты жоба тобына тіркейді.</span><span class="sxs-lookup"><span data-stu-id="29b88-122">Selecting **Book** books the resource onto the project team.</span></span>

![Ресурсқа тапсырыс беру тақтасын жасау](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a><span data-ttu-id="29b88-124">Негізгі талаптан тіркеу</span><span class="sxs-lookup"><span data-stu-id="29b88-124">Book from the Primary Requirement</span></span>

<span data-ttu-id="29b88-125">Жоба қызметінде жоба жасау Негізгі талап деп аталатын ресурс талабын автоматты түрде жасайды.</span><span class="sxs-lookup"><span data-stu-id="29b88-125">Creating a project in Project Service automatically creates a resource requirement called the Primary Requirement.</span></span> <span data-ttu-id="29b88-126">Бұл - талап жасамай немесе біреуін жаңадан жасамай кесте тақтасының көмегімен ресурсты жылдам тіркеу үшін пайдаланылатын бос талап.</span><span class="sxs-lookup"><span data-stu-id="29b88-126">This is an empty requirement that is used to quickly book a resource with the Schedule board without generating a requirement or creating one from scratch.</span></span> <span data-ttu-id="29b88-127">Талап бос болғандықтан, егер қолданылатын болса, тағайындау әдісі мен сағат санымен қоса, күндерді де көрсетуіңіз қажет.</span><span class="sxs-lookup"><span data-stu-id="29b88-127">Because the requirement is empty, you’ll need to specify dates as well as the allocation method and hours, if applicable.</span></span> 

1. <span data-ttu-id="29b88-128">Ресурсты негізгі талаппен бірге тіркеу үшін, кесте тақтасынан **Жоба** қойыншасын таңдаңыз. Көптеген жобалар болса, **Жоба** бағанында баған сүзгісін пайдалану қажет болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="29b88-128">To book a resource with the Primary Requirement, on the Schedule board, select the **Project** tab. You might need to use the column filter on the **Project** column if you have many projects.</span></span>

   <span data-ttu-id="29b88-129">![Кесте тақтасындағы "Баған" сүзгілері](media/FAQ-Project-Booking-Schedule-Board-2.png "Тапсырыстар мен тағайындаулар кестесі скриншоты")</span><span class="sxs-lookup"><span data-stu-id="29b88-129">![Column filters on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-2.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="29b88-130">Атауы жоба атауы болып табылатын және ұзақтығы нөлге (0) тең талапты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29b88-130">Select the requirement that only has the project name as its name and has a duration of zero (0).</span></span>

3. <span data-ttu-id="29b88-131">Қатарда пайда болатын **Қолжетімділігін табу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29b88-131">Select the **Find Availability** tab that appears on the row.</span></span> <span data-ttu-id="29b88-132">Бұл кесте тақтасын "Кесте көмекшісі" режиміне қойып, жобаға тіркеуге болатын қолжетімді ресурстарды көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="29b88-132">This puts the Schedule board in Schedule Assistant mode and shows the available resources that can be booked onto the project.</span></span>

4. <span data-ttu-id="29b88-133">**Негізгі талап** ұзақтығы 0 мәніне тең бос талап болғандықтан, ресурсты таңдау және тіркеу кезінде **Ресурс тапсырысын жасау** тақтасында ұзақтықты орнату қажет болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-133">Because a **Primary Requirement** is an empty requirement with zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when selecting and booking a resource.</span></span>

5. <span data-ttu-id="29b88-134">Сондай-ақ кесте тақтасының астынғы жағында **Жобаның негізгі талабы** параметрін таңдап, оны тіркелетін ресурсқа сүйреп апаруға болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-134">You can also select the **Project Primary Requirement** at the bottom of the Schedule board and drag and drop it on a resource to book it.</span></span>
 
    <span data-ttu-id="29b88-135">**Негізгі талап** ұзақтығы 0 мәніне тең бос талап болғандықтан, ресурсты таңдау және тіркеу кезінде **Ресурс тапсырысын жасау** тақтасында ұзақтықты орнату қажет болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-135">Because the **Primary Requirement** is an empty requirement that has zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when you select and book a resource.</span></span>
 
    <span data-ttu-id="29b88-136">Кесте тақтасындағы **Негізгі талап** арқылы ресурсты тіркеу кезінде, оны жоба тобына ешбір тағайындауларсыз қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="29b88-136">When you book a resource through the **Primary Requirement** on the Schedule board, you add it to the project team without any assignments.</span></span>
 
## <a name="book-from-a-new-resource-requirement"></a><span data-ttu-id="29b88-137">Жаңа ресурс талабынан тіркеу</span><span class="sxs-lookup"><span data-stu-id="29b88-137">Book from a new resource requirement</span></span>
<span data-ttu-id="29b88-138">Жаңа ресурс талабынан тапсырыс беру үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="29b88-138">Complete the following steps to book from a new resource requirement.</span></span> 

1. <span data-ttu-id="29b88-139">Жаңа ресурс талабын жасау үшін **Ресурс талаптары** параметріне өтіп, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29b88-139">Go to **Resource Requirements** , and then select **New** to create a new resource requirement.</span></span>

2. <span data-ttu-id="29b88-140">**Жоба** қойыншасында жоба талабын байланыстыру қажет жобаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="29b88-140">On the **Project** tab, select a project to associate the requirement to the project.</span></span>
 
    <span data-ttu-id="29b88-141">Осы жаңа талап кесте тақтасында орындауға болатын **Ашық талап** параметрі ретінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="29b88-141">On the Schedule board, this new requirement shows as an **Open Requirement** that you can fulfill.</span></span>

3. <span data-ttu-id="29b88-142">Жоба тобына қосу қажет ресурсты тіркеңіз.</span><span class="sxs-lookup"><span data-stu-id="29b88-142">Book the resource to add it to the project team.</span></span>

4. <span data-ttu-id="29b88-143">Енді ресурс тіркеліп, тапсырмаларды қолмен белгілеу қажет.</span><span class="sxs-lookup"><span data-stu-id="29b88-143">Now that the resource is booked, you must assign tasks manually.</span></span>
