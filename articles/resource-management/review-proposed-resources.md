---
title: Ұсынылған ресурстарды қарап шығу
description: Бұл тақырыпта жоба ресурстарын ұсыну жолы туралы ақпарат берілген.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: ad5cbdeb5fe05e6115eb024833a8d58b626ea4c9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079627"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="055f0-103">Ұсынылған ресурстарды қарап шығу</span><span class="sxs-lookup"><span data-stu-id="055f0-103">Review proposed resources</span></span>

<span data-ttu-id="055f0-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="055f0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="055f0-105">Ресурс менеджерлері ресурс сұрауын пайдалану арқылы жоба менеджеріне ресурстарды ұсына алады.</span><span class="sxs-lookup"><span data-stu-id="055f0-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="055f0-106">Сұрау торынан немесе сұраудың өзінен **Ресурстарды табу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="055f0-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="055f0-107">**Кесте көмекшісі** бетінде ресурсты таңдап, **Ресурсқа тапсырыс беруді жасау** тақтасындағы **Тапсырыс беру күйі** өрісінде **Тапсырыс беру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="055f0-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="055f0-108">Келесі күй жаңартулары пайда болады:</span><span class="sxs-lookup"><span data-stu-id="055f0-108">The following status updates occur:</span></span>

- <span data-ttu-id="055f0-109">**Кесте көмекшісі** бетінде тапсырыстың ұсынылғанын, бірақ қорытынды резервтелмегенін көрсету үшін күй индикаторлары жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="055f0-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="055f0-110">Ресурс сұрауында, күй **Қарап шығуды талап етеді** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="055f0-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="055f0-111">Жобаның **Топ** қойыншасында, жалпы топ мүшесінің **Сұрау күйі** мәні **Қарап шығуды талап етеді** мәніне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="055f0-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="055f0-112">Жоба менеджері ұсынысты қабылдай алады немесе одан бас тарта алады.</span><span class="sxs-lookup"><span data-stu-id="055f0-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="055f0-113">Ресурс менеджерлері ресурс сұрауларын өңдеген кезде келесі тәсілдердің кез келгенін пайдалана алады:</span><span class="sxs-lookup"><span data-stu-id="055f0-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="055f0-114">Егер қажетті сағаттарды орындау үшін бірде-бір ресурс болмаса, сұранысты қанағаттандыру үшін бірнеше ресурстарды ұсыну.</span><span class="sxs-lookup"><span data-stu-id="055f0-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="055f0-115">Ұсынылған сағаттар қажетті сағаттарды қанағаттандыра алатын бірнеше ресурстар арасында бөлінеді.</span><span class="sxs-lookup"><span data-stu-id="055f0-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="055f0-116">Бұл сценарийде сағаттар қабаттаспайды.</span><span class="sxs-lookup"><span data-stu-id="055f0-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="055f0-117">Талап етілгеннен аз ресурстарды ұсыну.</span><span class="sxs-lookup"><span data-stu-id="055f0-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="055f0-118">Бұл сценарийде ұсынылған ресурс сыйымдылығы сұрау салушы көрсеткен сағат санынан аз.</span><span class="sxs-lookup"><span data-stu-id="055f0-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="055f0-119">Сондықтан сұрау салушы ұсынылған ресурстарды қабылдаған кезде, қалған сұранысты жинақтау үшін орындалмаған ресурс талабы жасалады.</span><span class="sxs-lookup"><span data-stu-id="055f0-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="055f0-120">Егер жұмысты орындау үшін бірде-бір ресурс болмаса, сұранысты қанағаттандыру үшін бірнеше ресурсты тіркеу.</span><span class="sxs-lookup"><span data-stu-id="055f0-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="055f0-121">Талап етілгеннен аз ресурстарды тіркеу.</span><span class="sxs-lookup"><span data-stu-id="055f0-121">Book fewer resources than are required.</span></span> <span data-ttu-id="055f0-122">Бұл сценарийде тіркелген сағат саны қажетті сағат санынан аз.</span><span class="sxs-lookup"><span data-stu-id="055f0-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="055f0-123">Жүйе сізге тапсырыстардың орнына ресурстарды ұсынуға нұсқау береді, осылайша сұрау салушы қалған сұранысты тексеріп, оны бақылап отыра алады.</span><span class="sxs-lookup"><span data-stu-id="055f0-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="055f0-124">Шот ұсынылған қолданыс</span><span class="sxs-lookup"><span data-stu-id="055f0-124">Billable utilization</span></span>

<span data-ttu-id="055f0-125">Ресурстардың мақсатты шот ұсынылған қолданысы болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="055f0-125">Resources can have a target billable utilization.</span></span> <span data-ttu-id="055f0-126">Осы мақсатты қолданыс ресурстың әдепкі рөліндегі атрибут ретінде анықталады немесе жеке тіркелетін ресурстың жазбасында орнатылады.</span><span class="sxs-lookup"><span data-stu-id="055f0-126">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="055f0-127">Пайдалану есептеулері ресурстар бекітілген уақыт жазбаларын пайдалану арқылы есеп берген нақты сағат санына негізделген.</span><span class="sxs-lookup"><span data-stu-id="055f0-127">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="055f0-128">Пайдалануды есептеу үшін келесі формулалар пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="055f0-128">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="055f0-129">Шот ұсынылған қолданыс = ақылы нақты сағаттар ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="055f0-129">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="055f0-130">Шот ұсынылмайтын қолданыс = шот ұсыну түрінің идентификаторы бар нақты уақыт = ақысыз, қосымша немесе қолжетімді емес ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="055f0-130">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="055f0-131">Ішкі = сатылым келісім-шарты жоқ нақты уақыт ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="055f0-131">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="055f0-132">Ресурс сыйымдылығы = ресурстың жұмыс сағаттары – кеңседен тыс – жұмыс істемейтін күндер</span><span class="sxs-lookup"><span data-stu-id="055f0-132">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="055f0-133">**Ресурсты пайдалану** көрінісін **Ресурстар** тақтасынан табуға болады.</span><span class="sxs-lookup"><span data-stu-id="055f0-133">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="055f0-134">Тордағы әрбір ұяшық ресурстың күн, апта немесе ай сияқты кезеңдегі шот ұсынылған қолданысының пайыздық мөлшерін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="055f0-134">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="055f0-135">Ұяшықтарды бояу үшін келесі формулалар пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="055f0-135">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="055f0-136">**Жасыл:** Шот ұсынылған қолданыс \>= Ресурстың мақсатты қолданысы</span><span class="sxs-lookup"><span data-stu-id="055f0-136">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="055f0-137">**Сары:** Мақсатты қолданыс – 20 \<= Шот ұсынылған қолданыс \< Мақсатты қолданыс</span><span class="sxs-lookup"><span data-stu-id="055f0-137">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="055f0-138">**Қызыл:** Шот ұсынылған қолданыс \< Мақсатты қолданыс – 20</span><span class="sxs-lookup"><span data-stu-id="055f0-138">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="055f0-139">**Ресурсты пайдалану** көрінісі кесте тақтасына негізделгендіктен, нәтижелерді сүзгілеу үшін кесте тақтасының сүзгілеу мүмкіндіктерін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="055f0-139">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="055f0-140">Тор рөлге немесе жеке ресурсқа мақсатты қолданысты орнатуды талап етеді.</span><span class="sxs-lookup"><span data-stu-id="055f0-140">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="055f0-141">Бұл орнатуды орындау үшін, **Ресурстар** \> **Ресурс рөлдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="055f0-141">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="055f0-142">Сонымен қатар әрбір тіркелетін ресурсқа әдепкі рөлді тағайындау керек.</span><span class="sxs-lookup"><span data-stu-id="055f0-142">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="055f0-143">**Ресурстар** \> **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="055f0-143">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="055f0-144">**Project Service** қойыншасында, ресурс рөлінің анықталғанын және оның **Әдепкі** өрісі **Иә** параметріне орнатылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="055f0-144">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="055f0-145">**Әдепкі = жоқ** параметріне орнатылған қосымша рөлдерді қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="055f0-145">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="055f0-146">**Әдепкі = иә** параметріне орнатылған рөл ресурсты сол рөлдің мақсаты бойынша пайдалануды бағалау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="055f0-146">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="055f0-147">**Project Service** қойыншасында, ресурс үшін жеке мақсатты қолданысты орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="055f0-147">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="055f0-148">Сонда пайдалануды есептеу ресурстың әдепкі рөлінің орнына ресурстың мақсатын бағалау үшін мақсатты қолданысты пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="055f0-148">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="055f0-149">Пайдалану ресурсқа егер оның торда көрсетілген уақыт кезеңінде бекітілген, ақылы уақыты болса ғана көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="055f0-149">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="055f0-150">Ресурс қолжетімділігі</span><span class="sxs-lookup"><span data-stu-id="055f0-150">Resource availability</span></span>

<span data-ttu-id="055f0-151">Ресурс менеджерлерінің ресурстардың қолжетімділігін көре алатындығы және тапсырыстарды жаңарта алатындығы өте маңызды.</span><span class="sxs-lookup"><span data-stu-id="055f0-151">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="055f0-152">Кейбір жағдайларда ресми сұраныс (ресурс сұрауы) жоқ, бірақ ресурс менеджері электрондық пошта, телефон қоңырауы немесе лездік хабар сияқты арналар арқылы келетін жоспарланбаған сұранысқа жауап беруі керек.</span><span class="sxs-lookup"><span data-stu-id="055f0-152">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="055f0-153">Ресурс менеджерлері ресурстар мен тапсырыстарды жаңарту үшін кесте тақтасын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="055f0-153">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="055f0-154">Ресурстың қолжетімділігін есептеу үшін негіз ретінде ресурстың жұмыс сағаттары пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="055f0-154">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="055f0-155">Ресурс тапсырыстары ресурстардың мүмкіндіктерін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="055f0-155">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="055f0-156">Кесте тақтасы тапсырыстарды, мүмкіндікті және артық тапсырыстарды, сондай-ақ тапсырыстардың күйлерін көрсету үшін түстер мен көлеңкелеуді пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="055f0-156">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="055f0-157">Кесте тақтасы параметрлеріндегі параметр журналды көруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="055f0-157">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="055f0-158">Егер кесте тақтасындағы тапсырыс беруге болатын жеке ресурстың жанында оң жаққа бағыттаушы көрсеткі пайда болса, ресурс тіркелген жұмыс туралы мәліметтерді көрсету үшін ресурсты кеңейтуге болады.</span><span class="sxs-lookup"><span data-stu-id="055f0-158">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="055f0-159">Dynamics 365 Project Operations бағдарламасы Universal Resource Scheduling механизмін пайдаланғандықтан, сізде Dynamics 365 Field Service орнатылса, жобаларға, жұмыс тапсырыстарына және жоспарлауды кеңейткен басқа да нысандар үшін ресурс тапсырыстарының мәліметтерін көруге болады.</span><span class="sxs-lookup"><span data-stu-id="055f0-159">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="055f0-160">Жеке ресурс туралы қосымша мәліметтерді көру үшін, ресурс картасын ашу үшін оны тінтуірдің оң жақ түймешігімен басыңыз.</span><span class="sxs-lookup"><span data-stu-id="055f0-160">To view more details about an individual resource, right-click it to open the resource card.</span></span>

