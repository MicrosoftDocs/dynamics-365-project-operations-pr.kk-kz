---
title: Жоба параметрлері
description: Бұл тақырыпта жобаны басқару параметрлері туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: c9b8659f3b7ee81d2e21ef52743debd521fa9bb9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079823"
---
# <a name="project-settings"></a><span data-ttu-id="fe381-103">Жоба параметрлері</span><span class="sxs-lookup"><span data-stu-id="fe381-103">Project settings</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="fe381-104">Жобаны жоспарлау мүмкіндіктеріне қол жеткізу үшін, келесі параметрлерді пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-104">Use the following settings to access the project planning features.</span></span>

## <a name="work-template"></a><span data-ttu-id="fe381-105">Жұмыс үлгісі</span><span class="sxs-lookup"><span data-stu-id="fe381-105">Work template</span></span>

<span data-ttu-id="fe381-106">Жоба кестесін құру үшін, бір күндік жұмыс уақытының санын және қызмет етпейтін күндерді анықтайтын жобаның күнтізбелік үлгісін жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-106">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="fe381-107">Жобаның күнтізбелік үлгісін жасау үшін, жұмыс үлгісін жобаның **Күнтізбе үлгісі** өрісімен байланыстыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-107">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="fe381-108">Жұмыс үлгісін жасау үшін, осы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-108">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="fe381-109">PSA бағдарламасындағы сол жақ шарлау аумағында **Ресурстар** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-109">In PSA, in the left navigation pane, click **Resources**.</span></span> 
2. <span data-ttu-id="fe381-110">**Ресурстар** тізімінің бетінде пайдаланушы жазбасын ашып, **Жұмыс уақытын көрсету** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-110">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="fe381-111">Браузер бетінде қалқымалы терезелердің шығуына рұқсат бергеніңізге көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="fe381-111">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="fe381-112">Бұл ресурс үшін белгіленген жұмыс уақытын көруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="fe381-112">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="fe381-113">**Айлық көрініс** қойыншасында **Реттеу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-113">On the **Monthly View** tab, click **Set Up**.</span></span> <span data-ttu-id="fe381-114">Сонда үш параметр тізімі пайда болады:</span><span class="sxs-lookup"><span data-stu-id="fe381-114">A list of three options appears:</span></span> 

  - <span data-ttu-id="fe381-115">Жаңа апталық кесте</span><span class="sxs-lookup"><span data-stu-id="fe381-115">New Weekly Schedule</span></span>
  - <span data-ttu-id="fe381-116">Бір күнге жұмыс кестесі</span><span class="sxs-lookup"><span data-stu-id="fe381-116">Work Schedule for One Day</span></span>
  - <span data-ttu-id="fe381-117">Демалыс уақыты</span><span class="sxs-lookup"><span data-stu-id="fe381-117">Time Off</span></span>

> ![Реттеу параметрлері](media/project-13.png)

4. <span data-ttu-id="fe381-119">**Жаңа апталық кесте** параметрін таңдап, осы ресурс кестесінің параметрлерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-119">Select **New Weekly Schedule** , and then set the options for this resource schedule.</span></span> <span data-ttu-id="fe381-120">Апта сайын қайталанатын кестені, тәуліктік сағат параметрлерін, қызмет етпейтін күндерді және басқаларын орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-120">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="fe381-121">Күн ауқымын орнатып, **Сақтау** опциясын таңдаңыз да, **Жабу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-121">Set the date range, select **Save** , and then click **Close**.</span></span> 
6. <span data-ttu-id="fe381-122">**Ресурстар** тізім бетіне оралып, жұмыс уақытын орнатқан ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-122">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="fe381-123">Жұмыс үлгісін орнату үшін **Күнтізбені басқаша орнату** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-123">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="fe381-124">**Жұмыс үлгісі** диалогтық терезесінде жұмыс үлгісінің атауын енгізіп, **Қолдану** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-124">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="fe381-125">Енді жұмыс үлгісін жобаның күнтізбелік үлгісімен байланыстыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-125">You can now associate the work template with a project calendar template.</span></span>

## <a name="resource-roles"></a><span data-ttu-id="fe381-126">Ресурс рөлдері</span><span class="sxs-lookup"><span data-stu-id="fe381-126">Resource roles</span></span>

<span data-ttu-id="fe381-127">*Ресурс рөлі* термині жобада нақты тапсырмалар жиынын орындау үшін тұлғада болуы қажет біліктіліктер, құзыреттер және сертификаттар жиынына қатысты.</span><span class="sxs-lookup"><span data-stu-id="fe381-127">The term *resource role* refers to the set of skills, competencies, and certifications that a person must have to perform a specific set of tasks on a project.</span></span> <span data-ttu-id="fe381-128">PSA бағдарламасы ресурспен байланысты рөлге негізделген ресурстың уақыты бойынша құнын белгілеуге және есеп-шот ұсынуға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="fe381-128">PSA lets you cost and bill a resource's time based on the role that the resource is associated with.</span></span> <span data-ttu-id="fe381-129">Әр ұйым осы рөлдерді **Project Service** мәзіріндегі сол жақ шарлау аумағын қолдана отырып орнатуы керек.</span><span class="sxs-lookup"><span data-stu-id="fe381-129">Every organization must set up these roles by using the left navigation on the **Project Service** menu.</span></span>

<span data-ttu-id="fe381-130">Әрбір ұйым осы рөлдерді **Белсенді ресурс санаттары** бетінде орнатуы керек.</span><span class="sxs-lookup"><span data-stu-id="fe381-130">Every organization must set up these roles on the **Active Resource Categories** page.</span></span> <span data-ttu-id="fe381-131">Бұл бетті ашу үшін, сол жақ шарлау аумағында **Ресурс рөлдері** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="fe381-131">To open this page, in the left navigation pane, select **Resource Roles**.</span></span>

## <a name="price-lists"></a><span data-ttu-id="fe381-132">Бағатізбелер</span><span class="sxs-lookup"><span data-stu-id="fe381-132">Price lists</span></span>

<span data-ttu-id="fe381-133">Бағатізбелер ресурс рөлдерінің, шығын санаттарының, өнімдердің және ұйымдағы басқа элементтердің өзіндік құны мен сатылым бағаларын белгілеуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="fe381-133">Price lists let you set cost and sales prices for resource roles, expense categories, products, and other elements in an organization.</span></span> <span data-ttu-id="fe381-134">Жоба үшін жеткізілуі керек жұмысқа қаржылық болжамдар орнатпас бұрын, қосымша құн мен сатылым бағаларының тізімін жасау керек.</span><span class="sxs-lookup"><span data-stu-id="fe381-134">Before you set financial estimates for the work that must be delivered for a project, you should create a backing cost and sales price list.</span></span> <span data-ttu-id="fe381-135">Параметрлер бөлімінде ұйымда жасалған барлық жобаларға қолданылатын әдепкі құн мен сатылым бағаларының тізімін жасауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="fe381-135">In the parameters section, you should also set up a default cost and sales price list that applies to all projects that are created in the organization.</span></span> <span data-ttu-id="fe381-136">**Белсенді жоба параметрлері** бетінде әдепкі құн мен сатылым бағаларының тізімін жасағаныңызға көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="fe381-136">On the **Active Project Parameters** page, make sure that you set up a default cost and sales price list.</span></span>