---
title: Уақыт жазбаларын жасау
description: Бұл тақырыпта уақыт жазбаларын жасау жолы туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 878413a24baa340b745a045a6991a63a00851c8b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079751"
---
# <a name="create-time-entries"></a><span data-ttu-id="9871f-103">Уақыт жазбаларын жасау</span><span class="sxs-lookup"><span data-stu-id="9871f-103">Create time entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="9871f-104">Dynamics 365 Project Service Automation алдыңғы нұсқаларында уақыт жазбалары апта сайын енгізілді.</span><span class="sxs-lookup"><span data-stu-id="9871f-104">In previous versions of Dynamics 365 Project Service Automation, time entries were entered on a weekly basis.</span></span> <span data-ttu-id="9871f-105">Project Service Automation 3-нұсқасында уақыт жазбалары күнделікті енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="9871f-105">In version 3 of Project Service Automation, time entries are entered on a daily basis.</span></span> <span data-ttu-id="9871f-106">Алайда бірнеше уақыт жазбалары жасалған соң, оларды жаппай жасауға немесе көшіруге болады.</span><span class="sxs-lookup"><span data-stu-id="9871f-106">However, after a few time entries have been created, you can bulk create or copy them.</span></span>

## <a name="create-a-time-entry"></a><span data-ttu-id="9871f-107">Уақыт жазбасын жасау</span><span class="sxs-lookup"><span data-stu-id="9871f-107">Create a time entry</span></span>

<span data-ttu-id="9871f-108">Уақыт жазбасын жасау үшін осы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-108">Follow these steps to create a time entry.</span></span>

1. <span data-ttu-id="9871f-109">**Уақыт жазбалары** бетінде **Жаңа** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-109">On the **Time Entries** page, select **New**.</span></span>
2. <span data-ttu-id="9871f-110">**Жылдам жасау: Уақыт жазбасы** диалогтық терезесінде уақыт жазбасының ұзақтығын минуттармен, сағатпен немесе күнмен енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="9871f-110">In the **Quick Create: Time Entry** dialog box, enter the duration of the time entry in minutes, hours, or days.</span></span> <span data-ttu-id="9871f-111">Ұзақтық келесі пішімде енгізілуі тиіс: *x* минут, *x* сағат немесе *x* күн.</span><span class="sxs-lookup"><span data-stu-id="9871f-111">The duration must be entered in the following format: *x* minutes, *x* hours, or *x* days.</span></span> <span data-ttu-id="9871f-112">Сағаттар мен күндерді ондық сандармен енгізуге болады, мысалы, *x.x* сағат немесе *x.x* күн.</span><span class="sxs-lookup"><span data-stu-id="9871f-112">Hours and days can also be entered as decimal values, such as *x.x* hours or *x.x* days.</span></span>
3. <span data-ttu-id="9871f-113">Уақыт жазбасының түрін және уақыт жазбасын енгізетін жобаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-113">Select the type of time entry and the project that you're entering the time entry for.</span></span>
4. <span data-ttu-id="9871f-114">**Жоба тапсырмасы** өрісінде осы уақыт жазбасына арналған тапсырманы табыңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-114">In the **Project Task** field, find the task for this time entry.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9871f-115">Егер пайдаланушыға тағайындалмаған тапсырма үшін уақыт жазбасын жасасаңыз, **Жоба тапсырмасы** өрісінде **Іздеу** түймесін басып, **Көріністі өзгерту** түймешігін таңдаңыз, содан кейін барлық тапсырмаларды тізімдеу үшін **Барлық белсенді жоба тапсырмалары** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-115">If you're creating a time entry for a task that isn't assigned to a user, in the **Project Task** field, select the **Search** button, select **Change View** , and then select **All Active Project Tasks** to list all tasks.</span></span>

5. <span data-ttu-id="9871f-116">Егер сипаттама қажет болса, сипаттаманы енгізіп, **Сақтау және жабу** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-116">Enter a description, if a description is required, and then select **Save and Close**.</span></span>

<span data-ttu-id="9871f-117">Уақыт жазбасы жасалып, сақталғаннан кейін, оны уақыт жазбасы торында өңдеуге болады.</span><span class="sxs-lookup"><span data-stu-id="9871f-117">After the time entry is created and saved, you can edit it in the time entry grid.</span></span> <span data-ttu-id="9871f-118">Уақыт жазбасы торында екі пішімге қолдау көрсетіледі:</span><span class="sxs-lookup"><span data-stu-id="9871f-118">The time entry grid supports two formats:</span></span>

- <span data-ttu-id="9871f-119">Уақыт жазбаларын **сағ: мм** пішімінде енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="9871f-119">You can enter time entries in **hh:mm** format.</span></span> <span data-ttu-id="9871f-120">Содан кейін бұл пішім сағаттар мен бөлшектерге айналады.</span><span class="sxs-lookup"><span data-stu-id="9871f-120">This format is then converted to hours and fractions.</span></span>
- <span data-ttu-id="9871f-121">Сағаттар мен бөлшектерді тікелей енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="9871f-121">You can enter hours and fractions directly.</span></span>

<span data-ttu-id="9871f-122">Бір сағаттың бөлшектері минуттар емес екенін ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9871f-122">Note that the fractions of an hour aren't minutes.</span></span> <span data-ttu-id="9871f-123">Демек, 1,5 сағат 1 сағат 30 минутты құрайды.</span><span class="sxs-lookup"><span data-stu-id="9871f-123">Therefore, 1.5 hours represents 1 hour and 30 minutes.</span></span> <span data-ttu-id="9871f-124">Дәл осындай ереже күннің бөлшектеріне қолданылады.</span><span class="sxs-lookup"><span data-stu-id="9871f-124">The same rule applies to fractions of a day.</span></span> <span data-ttu-id="9871f-125">Бір күн 24 сағатты, ал 0,5 күн 12 сағатты білдіреді.</span><span class="sxs-lookup"><span data-stu-id="9871f-125">One day is 24 hours, and 0.5 days represents 12 hours.</span></span>

## <a name="bulk-create-time-entries"></a><span data-ttu-id="9871f-126">Уақыт жазбаларын жаппай жасау</span><span class="sxs-lookup"><span data-stu-id="9871f-126">Bulk create time entries</span></span>

<span data-ttu-id="9871f-127">Бірнеше уақыт жазбалары жасалған соң, қосымша уақыт жазбаларын жаппай жасау үшін оларды көшіруге болады.</span><span class="sxs-lookup"><span data-stu-id="9871f-127">After a few time entries have been created, you can copy them to create additional time entries in bulk.</span></span>

1. <span data-ttu-id="9871f-128">**Уақыт жазбалары** бетінде **Аптаны көшіру** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-128">On the **Time Entries** page, select **Copy Week**.</span></span>
2. <span data-ttu-id="9871f-129">**Басталу мерзімі** өріс тобындағы **Басталу күні** және **Аяқталу күні** өрістерінде уақыт жазбаларын көшіру үшін күндер ауқымын анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-129">In the **From Period** field group, in the **Start Date** and **End Date** fields, define the date range to copy time entries from.</span></span>
3. <span data-ttu-id="9871f-130">**Аяқталу мерзімі** өріс тобында **Басталу күні** өрісінде уақыт жазбаларын жасау күнін көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="9871f-130">In the **To Period** field group, in the **Start Date** field, specify the date to create time entries for.</span></span>
4. <span data-ttu-id="9871f-131">**Аяқталу мерзімі** өріс тобында көрсетілген апта күніне сәйкес келетін уақыт жазбаларының көшірмесін жасау үшін **Көшіру** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-131">Select **Copy** to create a copy of the time entries that correspond to the day of the week that is specified in the **To Period** field group.</span></span> <span data-ttu-id="9871f-132">Мысалы, өткен аптаның дүйсенбі күніндегі уақыт жазбасы **Аяқталу мерзімі** өріс тобында көрсетілген аптаның дүйсенбі күніне көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="9871f-132">For example, the time entry for Monday of last week is copied to Monday of the week that is specified in the **To Period** field group.</span></span>

## <a name="import-data-for-time-entries"></a><span data-ttu-id="9871f-133">Уақыт жазбаларына арналған деректерді импорттау</span><span class="sxs-lookup"><span data-stu-id="9871f-133">Import data for time entries</span></span>

<span data-ttu-id="9871f-134">Жоба тапсырыстары мен тапсырмаларынан деректерді импорттай аласыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-134">You can import data from project bookings and assignments.</span></span> <span data-ttu-id="9871f-135">Деректерді импорттаған кезде, импортталатын тапсырыстардың күндер ауқымын көрсетіп, содан кейін **Жоба** ретінде құруға болатын тапсырыстарды нақты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-135">When you import data, you can specify the date range of the bookings to import and then explicitly select the bookings that should be created as **Draft** time entries.</span></span>

## <a name="group-by-sort-search-and-filter-capabilities"></a><span data-ttu-id="9871f-136">Топтау әдісі, сұрыптау, іздеу және сүзу мүмкіндіктері</span><span class="sxs-lookup"><span data-stu-id="9871f-136">Group by, sort, search, and filter capabilities</span></span>

<span data-ttu-id="9871f-137">Уақыт жазбаларын бағандарда көрсетілген өлшемдер бойынша топтауға және сүзуге болады.</span><span class="sxs-lookup"><span data-stu-id="9871f-137">You can group and filter time entries by the dimensions that are specified in the columns.</span></span> <span data-ttu-id="9871f-138">**Топтау әдісі** өрісінде уақыт жазбаларын сүзу үшін пайдаланылатын өлшемді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-138">In the **Group by** field, select the dimension to use to filter time entries.</span></span> <span data-ttu-id="9871f-139">Сіз сонымен қатар баған тақырыптарындағы сұрыптау көрсеткісін пайдаланып уақыт жазбаларын өсу немесе кему ретімен сұрыптай аласыз.</span><span class="sxs-lookup"><span data-stu-id="9871f-139">You can also sort the time entry records in ascending or descending order by using the sort arrow on the column headings.</span></span> <span data-ttu-id="9871f-140">Сонымен қатар баған тақырыптарындағы **Сүзгі** түймешігін таңдау арқылы, содан кейін **Іздеу** терезесінде уақыт жазбаларын жоба атауы, жоба тапсырмасы немесе ресурс бойынша іздеу үшін пайдалану керек мәтінді енгізу арқылы көрсетуге немесе жасыруға болады.</span><span class="sxs-lookup"><span data-stu-id="9871f-140">Additionally, you can show or hide entries by selecting the **Filter** button on the column headings, and then, in the **Search** box, entering the text that should be used to search for time entries by project name, project task, time entry, or resource.</span></span>
