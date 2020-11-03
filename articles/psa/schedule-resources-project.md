---
title: Жоба үшін ресурстарды жоспарлау
description: Project Service жобасы ресурстарын жоспарлау жолы
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: db69348aac96cbfaaa865228c9230cbda4b1e784
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079866"
---
# <a name="schedule-resources-for-a-project-project-service"></a><span data-ttu-id="9f007-103">Жобаға ресурстар жоспарлау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="9f007-103">Schedule resources for a project (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="9f007-104">Ресурстарды тіркеу әдісінің жалпы көрінісін алу үшін ресурс қолжетімділігін тексеруге болады немесе біліктіліктер, топ орны және басқа опциялар бойынша көріністі сүзгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="9f007-104">You can check resource availability to get an overall view of how booked your resources are, or you can filter the view by skills, team, location, and other options.</span></span>  
  
<span data-ttu-id="9f007-105">Кесте тақтасында ресурстар тізімі және олардың қолжетімділігі көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="9f007-105">The schedule board shows list of resources and their availability.</span></span> <span data-ttu-id="9f007-106">**Сағаттар** , **Күн** , **Апта** немесе **Ай** бойынша қолжетімділікті көрсету үшін қарау режимін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-106">Select a view mode to show availability by **Hours** , **Day** , **Week** , or **Month**.</span></span>  
  
<span data-ttu-id="9f007-107">Кесте тақтасын пайдаланбас бұрын оны орнатқан маңызды.</span><span class="sxs-lookup"><span data-stu-id="9f007-107">Before you use the schedule board, it’s important to set it up.</span></span> <span data-ttu-id="9f007-108">Толығырақ ақпарат алу үшін [Кесте тақтасын конфигурациялау (Field Service немесе Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-108">For more information, see [Configure the schedule board (Field Service or Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span></span>
  
<span data-ttu-id="9f007-109">Ескірек нұсқаны пайдаланып жатсаңыз, ресурстың қолжетімділігін [Ресурстың қолжетімділігін көру](../psa/view-resource-availability.md) бөлімінде қараңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-109">If you are using an older version, for resource availability, see [View resource availability](../psa/view-resource-availability.md).</span></span>  

> [!IMPORTANT]
>  <span data-ttu-id="9f007-110">Кесте тақтасының тапсырыс беру мүмкіндігін, геокодтауды және орын қызметтерін пайдалану үшін карталарды қосу қажет.</span><span class="sxs-lookup"><span data-stu-id="9f007-110">To use the schedule board booking functionality, geocoding, and location services, you need to turn on maps.</span></span>  
> 
> 1. <span data-ttu-id="9f007-111">Негізгі мәзірде **Ресурсты жоспарлау** > **Басқару** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-111">On the main menu, select **Resource Scheduling** > **Administration**.</span></span>  
> 2. <span data-ttu-id="9f007-112">**Жоспарлау параметрлері** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-112">Click **Scheduling parameters**.</span></span>  
> 3. <span data-ttu-id="9f007-113">Жазбаны ашып, **Resource Scheduling Optimization** бөлімін төмен айналдырыңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-113">Open record and scroll down to the **Resource Scheduling Optimization** section.</span></span>  
> 4. <span data-ttu-id="9f007-114">**Карталарға қосылу** өрісінде **Иә** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-114">On the **Connect to Maps** field, choose **Yes**.</span></span>  
> 5. <span data-ttu-id="9f007-115">Шарттарды қабылдаңыз және жазбаны сақтаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-115">Accept terms and save the record.</span></span>  
> 6. <span data-ttu-id="9f007-116">Негізгі мәзірде **Project Service** > **Кесте тақтасы** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-116">On the main menu, select **Project Service** > **Schedule board**.</span></span> <span data-ttu-id="9f007-117">Бұл жерде тапсырыс беру талабын қолмен жоспарлаудың бірнеше жолы бар.</span><span class="sxs-lookup"><span data-stu-id="9f007-117">From here, there are several ways to manually schedule a booking requirement.</span></span> <span data-ttu-id="9f007-118">Сіз үшін тиімді әдісін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-118">Choose the method that works for you.</span></span>
  
## <a name="find-available-resources"></a><span data-ttu-id="9f007-119">Қолжетімді ресурстарды табу</span><span class="sxs-lookup"><span data-stu-id="9f007-119">Find available resources</span></span>

1.  <span data-ttu-id="9f007-120">**Тапсырыс беру талабы** тізімінде жоспарланбаған тапсырысты тінтуірдің оң жағымен басыңыз және мыналардың біреуін таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="9f007-120">From the **Booking Requirement** list, right-click an unscheduled booking and choose one of the following:</span></span>  
  
- <span data-ttu-id="9f007-121">Кесте тақтасындағы тізімнен қолжетімді ресурсты табу үшін **Қолжетімділікті -Ағымдағы ресурстарды табу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-121">Choose **Find availability - Current Resources** to find an available resource from the list on the schedule board.</span></span>  
- <span data-ttu-id="9f007-122">Жүйедегі ресурстардан қолжетімді ресурсты табу үшін **Қолжетімділікті -Барлық ресурстарды табу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-122">Choose **Find availability - All Resources** , to find an available resource from resources in the system</span></span>  
   > [!NOTE]
   >  <span data-ttu-id="9f007-123">Бұны орындаған кезде сүзгілер таңдалған тапсырыс беру талабының параметрлерін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="9f007-123">When you do this, the filters will show options for the selected booking requirement.</span></span>  
  
2. <span data-ttu-id="9f007-124">Қолжетімді ұяшықты көрген кезде кесте тақтасындағы уақыт аралығын тінтуірдің оң жағымен басыңыз және **Осы жерде тапсырыс беру** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-124">When you see an available slot, right-click the time slot on the schedule board and choose **Book Here**.</span></span> <span data-ttu-id="9f007-125">Немесе тапсырыс беру талабын қолжетімді уақыт ұясына апарып тастаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-125">Or, drag and drop the booking requirement to the available time slot.</span></span>  
  

## <a name="book-a-resource-using-the-daily-view-and-find-whos-under-booked"></a><span data-ttu-id="9f007-126">Күнделікті көрініс арқылы ресурсты тіркеу және кімнің тіркелмегенін табу</span><span class="sxs-lookup"><span data-stu-id="9f007-126">Book a resource using the daily view and find who’s under-booked</span></span>
  
1.  <span data-ttu-id="9f007-127">Кесте тақтасында **Қарау режимі** параметрін таңдаңыз және **Күндер** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-127">On the schedule board, select **View Mode** and select **Days**.</span></span>  
  
    <span data-ttu-id="9f007-128">Бұл ресурстың күніне қанша сағат тіркелгенін және қанша күн бос екенін көрсететін тор көрінісін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="9f007-128">This shows a grid view of how many hours a resource is booked per day and which days they are free.</span></span>  
  
2.  <span data-ttu-id="9f007-129">Тіркеу қажет ресурс атын басып, **Тіркеу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-129">Click the name of the resource you want to book, and then select **Book**.</span></span>  
  
3.  <span data-ttu-id="9f007-130">**Ресурсты тіркеу (жасау)** диалогтық терезесінде тіркеу әдісімен және басталу мен аяқталу уақыттарымен ресурсты тіркеу қажет жобаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-130">On the **Resource booking (create)** dialog box, choose the project that you want to book the resource for along with booking method and start and end times.</span></span>  
  
4.  <span data-ttu-id="9f007-131">Әрекетті орындап болған соң, **Тапсырыс беру** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-131">When you’re done, select **Book**.</span></span>  
  
## <a name="view-to-the-schedule-board"></a><span data-ttu-id="9f007-132">Кесте тақтасын қарау</span><span class="sxs-lookup"><span data-stu-id="9f007-132">View to the schedule board</span></span>
  
1.  <span data-ttu-id="9f007-133">Төменгі тізімнен жоспарланбаған тапсырыс беру талабын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-133">Select an unscheduled booking requirement from the list at the bottom.</span></span>  
  
2.  <span data-ttu-id="9f007-134">Тапсырыс беру талабын кесте тақтасында қолжетімді ресурс/уақыт ұясына апарыңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-134">Drag the booking requirement to an available resource/time slot on the schedule board.</span></span>  
  
3.  <span data-ttu-id="9f007-135">Әрекетті орындап болған соң, **Тапсырыс беру** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f007-135">When you're done, select **Book**.</span></span>  
  
### <a name="additional-resources"></a><span data-ttu-id="9f007-136">Қосымша ресурстар</span><span class="sxs-lookup"><span data-stu-id="9f007-136">Additional resources</span></span>  
 [<span data-ttu-id="9f007-137">Ресурс менеджері нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="9f007-137">Resource manager guide</span></span>](../psa/resource-manager-guide.md)