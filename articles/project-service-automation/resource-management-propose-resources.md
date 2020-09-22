---
title: Жоба ресурстарын ұсыну
description: Бұл тақырыпта жоба ресурстарын ұсыну жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: bdb0dcb2-4421-4ee1-b97d-89a8cdefbd8d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 3a7f7c15c3c7a3c39f2b7b9eeb88b9cf0cfdc220
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753144"
---
# <a name="propose-project-resources"></a><span data-ttu-id="e374f-103">Жоба ресурстарын ұсыну</span><span class="sxs-lookup"><span data-stu-id="e374f-103">Propose project resources</span></span>

<span data-ttu-id="e374f-104">Ресурс менеджерлері ресурс сұрауын пайдалану арқылы жоба менеджеріне ресурстарды ұсына алады.</span><span class="sxs-lookup"><span data-stu-id="e374f-104">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="e374f-105">Сұрау торынан немесе сұраудың өзінен **Ресурстарды табу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e374f-105">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="e374f-106">**Кесте көмекшісі** бетінде ресурсты таңдап, **Ресурсқа тапсырыс беруді жасау** тақтасындағы **Тапсырыс беру күйі** өрісінде **Тапсырыс беру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e374f-106">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

    ![Ұсынылған ресурс таңдалды](media/Resource-Management-image62.png)

<span data-ttu-id="e374f-108">Келесі күй жаңартулары пайда болады:</span><span class="sxs-lookup"><span data-stu-id="e374f-108">The following status updates occur:</span></span>

- <span data-ttu-id="e374f-109">**Кесте көмекшісі** бетінде тапсырыстың ұсынылғанын, бірақ қорытынды резервтелмегенін көрсету үшін күй индикаторлары жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="e374f-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>

    !["Кесте көмекшісі" бетіндегі ұсынылған тапсырыстың күй көрсеткіштері](media/Resource-Management-image63.png)

- <span data-ttu-id="e374f-111">Ресурс сұрауында, күй **Қарап шығуды талап етеді** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="e374f-111">On the resource request, the status is changed to **Needs Review**.</span></span>

    !["Қарап шығуды талап етеді" күйіне өзгертілген ресурс сұрауының күйі](media/Resource-Management-image64.png)

- <span data-ttu-id="e374f-113">Жобаның **Топ** қойыншасында, жалпы топ мүшесінің **Сұрау күйі** мәні **Қарап шығуды талап етеді** мәніне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="e374f-113">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

    ![Жобаның "Топ" қойыншасында "Қарап шығуды талап етеді" күйіне өзгертілген жалпы топ мүшесінің күйі](media/Resource-Management-image48.png)

<span data-ttu-id="e374f-115">Жоба менеджері ұсынысты қабылдай алады немесе одан бас тарта алады.</span><span class="sxs-lookup"><span data-stu-id="e374f-115">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="e374f-116">Ресурс менеджерлері ресурс сұрауларын өңдеген кезде келесі тәсілдердің кез келгенін пайдалана алады:</span><span class="sxs-lookup"><span data-stu-id="e374f-116">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="e374f-117">Егер қажетті сағаттарды орындау үшін бірде-бір ресурс болмаса, сұранысты қанағаттандыру үшін бірнеше ресурстарды ұсыну.</span><span class="sxs-lookup"><span data-stu-id="e374f-117">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="e374f-118">Ұсынылған сағаттар қажетті сағаттарды қанағаттандыра алатын бірнеше ресурстар арасында бөлінеді.</span><span class="sxs-lookup"><span data-stu-id="e374f-118">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="e374f-119">Бұл сценарийде сағаттар қабаттаспайды.</span><span class="sxs-lookup"><span data-stu-id="e374f-119">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="e374f-120">Талап етілгеннен аз ресурстарды ұсыну.</span><span class="sxs-lookup"><span data-stu-id="e374f-120">Propose fewer resources than are required.</span></span> <span data-ttu-id="e374f-121">Бұл сценарийде ұсынылған ресурс сыйымдылығы сұрау салушы көрсеткен сағат санынан аз.</span><span class="sxs-lookup"><span data-stu-id="e374f-121">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="e374f-122">Сондықтан сұрау салушы ұсынылған ресурстарды қабылдаған кезде, қалған сұранысты жинақтау үшін орындалмаған ресурс талабы жасалады.</span><span class="sxs-lookup"><span data-stu-id="e374f-122">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="e374f-123">Егер жұмысты орындау үшін бірде-бір ресурс болмаса, сұранысты қанағаттандыру үшін бірнеше ресурсты тіркеу.</span><span class="sxs-lookup"><span data-stu-id="e374f-123">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="e374f-124">Талап етілгеннен аз ресурстарды тіркеу.</span><span class="sxs-lookup"><span data-stu-id="e374f-124">Book fewer resources than are required.</span></span> <span data-ttu-id="e374f-125">Бұл сценарийде тіркелген сағат саны қажетті сағат санынан аз.</span><span class="sxs-lookup"><span data-stu-id="e374f-125">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="e374f-126">Жүйе сізге тапсырыстардың орнына ресурстарды ұсынуға нұсқау береді, осылайша сұрау салушы қалған сұранысты тексеріп, оны бақылап отыра алады.</span><span class="sxs-lookup"><span data-stu-id="e374f-126">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="e374f-127">Шот ұсынылған қолданыс</span><span class="sxs-lookup"><span data-stu-id="e374f-127">Billable utilization</span></span>

<span data-ttu-id="e374f-128">Ресурстардың мақсатты шот ұсынылған қолданысы болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e374f-128">Resources can have a target billable utilization.</span></span> <span data-ttu-id="e374f-129">Осы мақсатты қолданыс ресурстың әдепкі рөліндегі атрибут ретінде анықталады немесе жеке тіркелетін ресурстың жазбасында орнатылады.</span><span class="sxs-lookup"><span data-stu-id="e374f-129">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="e374f-130">Пайдалану есептеулері ресурстар бекітілген уақыт жазбаларын пайдалану арқылы есеп берген нақты сағат санына негізделген.</span><span class="sxs-lookup"><span data-stu-id="e374f-130">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="e374f-131">Пайдалануды есептеу үшін келесі формулалар пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="e374f-131">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="e374f-132">Шот ұсынылған қолданыс = ақылы нақты сағаттар ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="e374f-132">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="e374f-133">Шот ұсынылмайтын қолданыс = шот ұсыну түрінің идентификаторы бар нақты уақыт = ақысыз, қосымша немесе қолжетімді емес ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="e374f-133">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="e374f-134">Ішкі = сатылым келісім-шарты жоқ нақты уақыт ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="e374f-134">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="e374f-135">Ресурс сыйымдылығы = ресурстың жұмыс сағаттары – кеңседен тыс – жұмыс істемейтін күндер</span><span class="sxs-lookup"><span data-stu-id="e374f-135">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="e374f-136">**Ресурсты пайдалану** көрінісін **Ресурстар** тақтасынан табуға болады.</span><span class="sxs-lookup"><span data-stu-id="e374f-136">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

![Ресурсты пайдалану көрінісі](media/Resource-Management-image65.png)

<span data-ttu-id="e374f-138">Тордағы әрбір ұяшық ресурстың күн, апта немесе ай сияқты кезеңдегі шот ұсынылған қолданысының пайыздық мөлшерін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="e374f-138">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="e374f-139">Ұяшықтарды бояу үшін келесі формулалар пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="e374f-139">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="e374f-140">**Жасыл:** Шот ұсынылған қолданыс \>= Ресурстың мақсатты қолданысы</span><span class="sxs-lookup"><span data-stu-id="e374f-140">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="e374f-141">**Сары:** Мақсатты қолданыс – 20 \<= Шот ұсынылған қолданыс \< Мақсатты қолданыс</span><span class="sxs-lookup"><span data-stu-id="e374f-141">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="e374f-142">**Қызыл:** Шот ұсынылған қолданыс \< Мақсатты қолданыс – 20</span><span class="sxs-lookup"><span data-stu-id="e374f-142">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="e374f-143">**Ресурсты пайдалану** көрінісі кесте тақтасына негізделгендіктен, нәтижелерді сүзгілеу үшін кесте тақтасының сүзгілеу мүмкіндіктерін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="e374f-143">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="e374f-144">Тор рөлге немесе жеке ресурсқа мақсатты қолданысты орнатуды талап етеді.</span><span class="sxs-lookup"><span data-stu-id="e374f-144">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="e374f-145">Бұл орнатуды орындау үшін, **Ресурстар** \> **Ресурс рөлдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="e374f-145">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="e374f-146">Сонымен қатар әрбір тіркелетін ресурсқа әдепкі рөлді тағайындау керек.</span><span class="sxs-lookup"><span data-stu-id="e374f-146">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="e374f-147">**Ресурстар** \> **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="e374f-147">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="e374f-148">**Project Service** қойыншасында, ресурс рөлінің анықталғанын және оның **Әдепкі** өрісі **Иә** параметріне орнатылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="e374f-148">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="e374f-149">**Әдепкі = жоқ** параметріне орнатылған қосымша рөлдерді қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="e374f-149">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="e374f-150">**Әдепкі = иә** параметріне орнатылған рөл ресурсты сол рөлдің мақсаты бойынша пайдалануды бағалау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e374f-150">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

![Орнатылған әдепкі рөл](media/Resource-Management-image67.png)

<span data-ttu-id="e374f-152">**Project Service** қойыншасында, ресурс үшін жеке мақсатты қолданысты орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="e374f-152">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="e374f-153">Сонда пайдалануды есептеу ресурстың әдепкі рөлінің орнына ресурстың мақсатын бағалау үшін мақсатты қолданысты пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e374f-153">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="e374f-154">Пайдалану ресурсқа егер оның торда көрсетілген уақыт кезеңінде бекітілген, ақылы уақыты болса ғана көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="e374f-154">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="e374f-155">Ресурс қолжетімділігі</span><span class="sxs-lookup"><span data-stu-id="e374f-155">Resource availability</span></span>

<span data-ttu-id="e374f-156">Ресурс менеджерлерінің ресурстардың қолжетімділігін көре алатындығы және тапсырыстарды жаңарта алатындығы өте маңызды.</span><span class="sxs-lookup"><span data-stu-id="e374f-156">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="e374f-157">Кейбір жағдайларда ресми сұраныс (ресурс сұрауы) жоқ, бірақ ресурс менеджері электрондық пошта, телефон қоңырауы немесе лездік хабар сияқты арналар арқылы келетін жоспарланбаған сұранысқа жауап беруі керек.</span><span class="sxs-lookup"><span data-stu-id="e374f-157">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="e374f-158">Ресурс менеджерлері ресурстар мен тапсырыстарды жаңарту үшін кесте тақтасын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e374f-158">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="e374f-159">Ресурстың қолжетімділігін есептеу үшін негіз ретінде ресурстың жұмыс сағаттары пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="e374f-159">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="e374f-160">Ресурс тапсырыстары ресурстардың мүмкіндіктерін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e374f-160">Resource bookings consume the capacity of the resources.</span></span>

![Кесте тақтасы](media/Resource-Management-image68.png)

<span data-ttu-id="e374f-162">Кесте тақтасы тапсырыстарды, мүмкіндікті және артық тапсырыстарды, сондай-ақ тапсырыстардың күйлерін көрсету үшін түстер мен көлеңкелеуді пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e374f-162">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="e374f-163">Кесте тақтасы параметрлеріндегі параметр журналды көруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="e374f-163">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="e374f-164">Егер кесте тақтасындағы тапсырыс беруге болатын жеке ресурстың жанында оң жаққа бағыттаушы көрсеткі пайда болса, ресурс тіркелген жұмыс туралы мәліметтерді көрсету үшін ресурсты кеңейтуге болады.</span><span class="sxs-lookup"><span data-stu-id="e374f-164">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

![Кесте тақтасында кеңейтілген тіркелетін ресурс](media/Resource-Management-image69.png)

<span data-ttu-id="e374f-166">Dynamics 365 Project Service Automation бағдарламасы Universal Resource Scheduling механизмін пайдаланатындықтан, Dynamics 365 Field Service орнатылған болса, жоба және жұмыс тапсырыстары үшін ресурсқа тапсырыс беру және жоспарлау ұзартылған басқа нысандар туралы мәліметтерді көруге болады.</span><span class="sxs-lookup"><span data-stu-id="e374f-166">Because Dynamics 365 Project Service Automation uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

![Жоба және жұмыс тапсырыстары үшін ресурсқа тапсырыс беру туралы мәліметтер](media/Resource-Management-image70.png)

<span data-ttu-id="e374f-168">Жеке ресурс туралы қосымша мәліметтерді көру үшін, ресурс картасын ашу үшін оны тінтуірдің оң жақ түймешігімен басыңыз.</span><span class="sxs-lookup"><span data-stu-id="e374f-168">To view more details about an individual resource, right-click it to open the resource card.</span></span>

![Ресурс картасы](media/Resource-Management-image71.png)
