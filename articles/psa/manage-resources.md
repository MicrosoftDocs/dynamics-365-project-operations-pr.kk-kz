---
title: Ресурстарды басқару
description: Бұл бөлімде ресурстарды басқару жолы туралы ақпарат берілген.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 05/13/2019
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
ms.openlocfilehash: b067f900fa49bba04536b49600dbe80a2167f707
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997833"
---
# <a name="manage-resources"></a><span data-ttu-id="44b0f-103">Ресурстарды басқару</span><span class="sxs-lookup"><span data-stu-id="44b0f-103">Manage resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="44b0f-104">Dynamics 365 Project Service Automation бүкіл ұйым бойынша ресурс сұрауы және пайдалану жолының визуалды шолуын қамтамасыз ететін ресурс менеджерінің бақылау тақтасын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-104">Dynamics 365 Project Service Automation includes a resource manager dashboard that provides a visual overview of resource demand and utilization throughout the organization.</span></span> <span data-ttu-id="44b0f-105">Осы бақылау тақтасындағы диаграммаларды келесі ақпаратты визуализациялау үшін пайдалануға болады:</span><span class="sxs-lookup"><span data-stu-id="44b0f-105">You can use the charts on this dashboard to visualize the following information:</span></span>

- <span data-ttu-id="44b0f-106">**Ресурс сұрауы** - **Белсенді ресурс сұрауы** диаграммасында жіберілген ресурстар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-106">**Resource demand** – The **Active Resource Request** chart shows resources that have been submitted.</span></span> <span data-ttu-id="44b0f-107">Ресурстар рөл немесе жоба бойынша біріктіріледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-107">The resources are aggregated by either role or project.</span></span>
- <span data-ttu-id="44b0f-108">**Жіберілмеген ресурс сұрауы** - **Тағайындалмаған ресурс сұрауы** диаграммасында жіберілмеген барлық ресурстар талаптары көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-108">**Unsubmitted resource demand** – The **Unassigned Resource Demand** chart shows all the resource requirements that haven't been submitted.</span></span> <span data-ttu-id="44b0f-109">Бұл ресурс менеджерлеріне берік емес және ресурс сұрауы арқылы жіберілуі мүмкін сұрауды көруге көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-109">It helps resource managers view demand that isn't firm and might be submitted through a resource request.</span></span>
- <span data-ttu-id="44b0f-110">**Өткен аптада шот ұсынылған қолданыс** - **Рөл бойынша қолданыс** диаграммасында рөл арқылы ұйымның мақсатты шот ұсынылған қолданысы бойынша рөл арқылы нақты шот ұсынылған қолданыстың пайыздық көрсеткіші көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-110">**Billable utilization for the past week** – The **Utilization by Role** chart shows the percentage of the organization's actual billable utilization by role against its target billable utilization by role.</span></span>

    > [!NOTE]
    > <span data-ttu-id="44b0f-111">**Рөл бойынша қолданыс** диаграммасын қолжетімді ету үшін, UpdateRoleUtilization жұмыс ағынын іске қосатын тапсырманы жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-111">To make the **Utilization by Role** chart available, create a job that runs the UpdateRoleUtilization workflow.</span></span> <span data-ttu-id="44b0f-112">Бұл қайталанатын тапсырма әр жеті күн сайын алдыңғы жеті күн бойынша шот ұсынылған қолданысты есептеу үшін орындалады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-112">This recurring job runs every seven days to calculate billable utilization for the previous seven days.</span></span> <span data-ttu-id="44b0f-113">Нәтижелер рөл бойынша біріктіріледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-113">The results are aggregated by role.</span></span>

## <a name="manage-project-team-members"></a><span data-ttu-id="44b0f-114">Жоба тобының мүшелерін басқару</span><span class="sxs-lookup"><span data-stu-id="44b0f-114">Manage project team members</span></span>

<span data-ttu-id="44b0f-115">Жоба менеджерлері жобалардағы ресурстарды басқару үшін, ресурс менеджерінің бақылау тақтасын қолдана алады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-115">Project managers can use the resource manager dashboard to manage the resources on projects.</span></span> <span data-ttu-id="44b0f-116">Мысалы, олар топ мүшесін жобаға тікелей қосып, жалпы ресурс арқылы алынған ресурстарға қойылатын талаптарды орындау үшін топ мүшелерін резервтей алады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-116">For example, they can add a team member directly to a project and book a team member to fulfill the resource requirements that were captured by a generic resource.</span></span>

### <a name="add-a-team-member-directly-to-a-project"></a><span data-ttu-id="44b0f-117">Топ мүшесін жобаға тікелей қосу</span><span class="sxs-lookup"><span data-stu-id="44b0f-117">Add a team member directly to a project</span></span>

<span data-ttu-id="44b0f-118">Топ мүшесін жобаға тікелей қосу үшін, **Жобалар** бетіндегі **Топ** қойыншасында **Жаңа** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-118">To add a team member directly to a project, on the **Projects** page, on the **Team** tab, select **New**.</span></span> <span data-ttu-id="44b0f-119">Сонда **Жылдам құру: жоба тобының мүшесі** диалогтық терезесі пайда болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-119">The **Quick Create:Project Team Member** dialog box appears.</span></span> <span data-ttu-id="44b0f-120">Осы диалогтық терезеде келесі тапсырмаларды орындауға болады:</span><span class="sxs-lookup"><span data-stu-id="44b0f-120">In this dialog box, you can perform these tasks:</span></span>

- <span data-ttu-id="44b0f-121">**Аталған ресурсты резервтеу** – **Резервтеу үшін қолжетімді ресурс** өрісінде ресурс атауын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-121">**Book a named resource** – In the **Bookable Resource** field, select the name of the resource.</span></span> <span data-ttu-id="44b0f-122">Содан кейін рөлді таңдап, кезеңді белгілеңіз де бөлу әдісін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-122">Then select the role, set the period, and select an allocation method.</span></span> <span data-ttu-id="44b0f-123">Таңдалған атаулы ресурс жобаға таңдалған бөлу әдісі мен ресурстар күнтізбесін қолдану арқылы қосылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-123">The named resource that you selected is added to the project by using the selected allocation method and the resources calendar.</span></span>
- <span data-ttu-id="44b0f-124">**Жалпы ресурс қосу** – **Резервтеу үшін қолжетімді ресурс** өрісін бос қалдырып, рөлді таңдаңыз да, кезеңді белгілеңіз және бөлу әдісін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-124">**Add a generic resource** – Leave the **Bookable resource** field blank, and then select the role, set the period, and select the preferred allocation method.</span></span> <span data-ttu-id="44b0f-125">Жалпы ресурс топта аталған ресурстарды резервтеу үшін пайдаланылатын сұрау үлгісін сақтайтын толтырғыш ретінде қосылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-125">A generic resource is added to the team as a placeholder to hold the demand pattern that is used to book named resources on the team.</span></span> <span data-ttu-id="44b0f-126">Талап жоба күнтізбесі бойынша жасалады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-126">The requirement is made according to the project calendar.</span></span>
- <span data-ttu-id="44b0f-127">**Аталған ресурсты ресурс сыйымдылығын пайдаланбай топқа қосу** – **Резервтеу үшін қолжетімді ресурс** өрісінде ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-127">**Add a named resource to the team without consuming resource capacity** – In the **Bookable Resource** field, select a resource.</span></span> <span data-ttu-id="44b0f-128">Содан кейін кезеңді таңдап, бөлу әдісі ретінде **Жоқ** мәнін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-128">Then select the period, and select **None** as the allocation method.</span></span> <span data-ttu-id="44b0f-129">Сонда ресурс топқа қосылады, бірақ ресурс сыйымдылығы резервтеу арқылы пайдаланылмайды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-129">The resource is added to the team, but the resource's capacity isn't consumed through a booking.</span></span>

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a><span data-ttu-id="44b0f-130">Жалпы ресурсқа арналған ресурс талаптарын орындау үшін топ мүшелерін резервтеу</span><span class="sxs-lookup"><span data-stu-id="44b0f-130">Book a team member to fulfill resource requirements for a generic resource</span></span>

<span data-ttu-id="44b0f-131">PSA бағдарламасында жоба тобы бойынша жалпы ресурсты резервтеуге, рөлді, қажетті сыйымдылықты және сыйымдылықты бөлу жолын көрсетуге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-131">In PSA, you can book a generic resource on a project team, and can specify the role, the required capacity, and how that capacity is distributed.</span></span> <span data-ttu-id="44b0f-132">Ресурсқа қойылатын талапта жалпы ресурстармен байланысты атрибуттарды көрсете аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-132">On the resource requirement, you can specify attributes that are associated with the generic resource.</span></span> <span data-ttu-id="44b0f-133">Бұл атрибуттарға қажетті дағдылар, таңдаулы ұйымдық бөлімше және таңдаулы ресурстар кіреді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-133">These attributes include required skills, the preferred organizational unit, and preferred resources.</span></span>

<span data-ttu-id="44b0f-134">Әзірлеушіге арналған жалпы ресурс бойынша қажетті дағдыларды анықтау үшін, келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-134">Follow these steps to specify required skills on a generic resource for a developer.</span></span>

1. <span data-ttu-id="44b0f-135">**Жобалар** бетіндегі **Топ** қойыншасында жалпы ресурсты резервтеу үшін **Жаңа** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-135">On the **Projects** page, on the **Team** tab, select **New** to book a generic resource.</span></span>

    ![Топта резервтелген жалпы ресурс](media/Resource-Management-image9.png)

2. <span data-ttu-id="44b0f-137">**Барлық топ мүшелері** көрінісіндегі **Ресурс талабы** бағанында жалпы ресурсқа қажетті дағдыларды қосу үшін сілтемені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-137">In the **All Team Members** view, in the **Resource Requirement** column, select the link to add required skills for the generic resource.</span></span>

    ![Талап сілтемесі](media/Resource-Management-image10.png)

3. <span data-ttu-id="44b0f-139">Пайда болатын **Ресурс талабы** бетіндегі **Дағдылар** торында эллипсті (**...**) таңдап, әзірлеушіге қажетті дағдыларды қосу үшін **Жаңа талап сипаттамасын қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-139">On the **Resource Requirement** page that appears, in the **Skills** grid, select the ellipsis (**...**) and then select **Add New Requirement Characteristic** to add the required skills for your developer.</span></span>

    ![Жаңа талап сипаттамасының пәрменін қосу](media/Resource-Management-image11.png)

4. <span data-ttu-id="44b0f-141">Пайда болатын **Жылдам жасау: талап сипаттамасы** диалогтық терезесіндегі **Сипаттама** өрісінде қажетті дағдыны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-141">In the **Quick Create: Requirement Characteristic** dialog box that appears, in the **Characteristic** field, select the required skill.</span></span> <span data-ttu-id="44b0f-142">Содан кейін **Бағалау мәні** өрісінде сол дағдының кәсіби деңгейін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-142">Then, in the **Rating value** field, select the proficiency level for that skill.</span></span> <span data-ttu-id="44b0f-143">Соңында **Ресурс талабы** өрісінде ұйымдық бөлімшелерден немесе тіпті аталған ресурстардан алынған бастапқы ресурстарға қойылатын талапты орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-143">Finally, in the **Resource Requirement** field, set the requirement to source resources from organizational units or even named resources.</span></span> <span data-ttu-id="44b0f-144">Аяқтағаннан кейін, **Сақтау** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-144">When you've finished, select **Save**.</span></span>

    ![Жылдам жасау: талап сипаттамасы диалогтық терезесі](media/Resource-Management-image12.png)

5. <span data-ttu-id="44b0f-146">**Ресурс талабы** бетінде ресурсқа қойылатын талапты орындау үшін, **Резервтеу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-146">On the **Resource Requirement** page, select **Book** to fulfill the resource requirement.</span></span>

    ![Ресурс талабы бетіндегі "Резервтеу" түймешігі](media/Resource-Management-image13.png)

    <span data-ttu-id="44b0f-148">Сондай-ақ жалпы ресурсты **Барлық топ мүшелері** торынан таңдап, **Резервтеу** параметрін таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-148">You can also select the generic resource in the **All Team Members** grid and then select **Book**.</span></span>

    ![Барлық топ мүшелері торының үстіндегі "Резервтеу" түймешігі](media/Resource-Management-image14.png)

    > [!NOTE]
    > <span data-ttu-id="44b0f-150">Бұл мысалда талап етілетін 40 сағат бар, бірақ нақты резервтелген сағаттар жоқ, себебі жалпы ресурстарда резервтеу мүмкіндігі жоқ.</span><span class="sxs-lookup"><span data-stu-id="44b0f-150">In this example, there are 40 required hours but no actual booked hours, because generic resources don't have bookings.</span></span> <span data-ttu-id="44b0f-151">Сонымен қатар тағайындалған сағаттар жоқ, себебі жалпы ресурс топқа тікелей қосылған.</span><span class="sxs-lookup"><span data-stu-id="44b0f-151">Additionally, there are no assigned hours, because the generic resource was added directly to the team.</span></span> <span data-ttu-id="44b0f-152">Бұл тапсырма тағайындауы арқылы қосылмаған.</span><span class="sxs-lookup"><span data-stu-id="44b0f-152">It wasn't added by using task assignment.</span></span>

    <span data-ttu-id="44b0f-153">**Жоспарлау бойынша көмекші** бетінде қолжетімді ресурстарды ресурсқа қойылатын талапта көрсетілген талаптар бойынша сүзгілеуге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-153">On the **Scheduling Assistant** page, you can filter available resources by the requirements that are specified on the resource requirement.</span></span> <span data-ttu-id="44b0f-154">Ресурстар кесте тақтасында көрсетілген сұрыптау параметрлері бойынша сұрыпталады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-154">Resources are sorted according to the sorting parameters that are specified on the Schedule Board.</span></span>

    ![Жоспарлау көмекшісі беті](media/Resource-Management-image15.png)

    <span data-ttu-id="44b0f-156">Жиі қолданылатын сүзгілер келесідей:</span><span class="sxs-lookup"><span data-stu-id="44b0f-156">Here are some filters that are often used:</span></span>

    - <span data-ttu-id="44b0f-157">**Бағалау бойынша сипаттама** – біліктілік бағалауына қосымша ретінде, дағдылары, сертификаттары және басқа ресурстық қасиеттері бойынша сүзгілеу.</span><span class="sxs-lookup"><span data-stu-id="44b0f-157">**Characteristics along with a rating** – Filter by skills, certifications, and other resource qualities, in addition to ratings of proficiency.</span></span>
    - <span data-ttu-id="44b0f-158">**Рөлдер** – резервтеу үшін қолжетімді ресурстарға тағайындалған әдепкі рөлдер бойынша сүзгілеу.</span><span class="sxs-lookup"><span data-stu-id="44b0f-158">**Roles** – Filter by the default roles that are assigned to bookable resources.</span></span>
    - <span data-ttu-id="44b0f-159">**Ұйымдық бөлімшелер** – резервтеу үшін қолжетімді ресурстарды тағайындалған ұйымдық бөлімшелер бойынша сүзгілеу.</span><span class="sxs-lookup"><span data-stu-id="44b0f-159">**Organizational units** – Filter bookable resources by the organizational units that they are assigned to.</span></span>

6. <span data-ttu-id="44b0f-160">Егер алғашқы талаптарды іздеудің нәтижелеріне қанағаттанбасаңыз, сүзгілеу шарттарын өзгерте аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-160">If you aren't satisfied with the results of the initial requirement search, you can change the filter criteria.</span></span> <span data-ttu-id="44b0f-161">Сол жақтағы **Сүзгі көрінісі** тақтасын кеңейтіп, қосымша ресурстар табу үшін **Іздеу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-161">Expand the **Filter View** pane on the left, and then select **Search** to find additional resources.</span></span>

    ![Сүзгі көрінісі тақтасы](media/Resource-Management-image16.png)

7. <span data-ttu-id="44b0f-163">Нәтижелерді сұрыптау әдісін өзгерту үшін, **Сұрыптау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-163">To change how the results are sorted, select **Sort**.</span></span>

    ![Сұрыптау пәрмені](media/Resource-Management-image17.png)

8. <span data-ttu-id="44b0f-165">Тордың жоғарғы жағында көрсетілгендей, ресурстарды талапта көрсетілген сұрауға сәйкес таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-165">Select resources according to the demand that is specified on the requirement, as indicated at the top of the grid.</span></span> <span data-ttu-id="44b0f-166">Тордағы ұяшықтардың таңдау белгісін алып тастап, ресурс сыйымдылығын ашық қалдыруға болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-166">You can clear the selection of cells in the grid and leave that resource capacity open.</span></span> <span data-ttu-id="44b0f-167">Бір уақытта резервтелген ретінде тек бір ресурсты таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-167">Only one resource at a time can be selected as booked.</span></span>

9. <span data-ttu-id="44b0f-168">Таңдалған ресурсты резервтеу үшін **Резервтеу** параметрін таңдап, кестелер тақтасын ашық қалдырыңыз, осылайша қосымша ресурстарды таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-168">Select **Book** to book the selected resource and leave the Schedule Board open, so that you can select additional resources.</span></span> <span data-ttu-id="44b0f-169">Не болмаса, таңдалған ресурсты резервтеу және кесте тақтасын жабу үшін **Резервтеу және шығу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-169">Alternatively, select **Book & Exit** to book the selected resource and close the Schedule Board.</span></span>

    ![Резервтелетін ресурс](media/Resource-Management-image19.png)

    <span data-ttu-id="44b0f-171">Резервтелген сағаттар туралы хабарлама келеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-171">You receive a notification about booked hours.</span></span> <span data-ttu-id="44b0f-172">Сұрау индикаторлары резервтеу талабының қаншалықты қанағаттандырылатындығын және қаншалықты қалғандығын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-172">The demand indicators show how much the booking requirement is satisfied and how much remains.</span></span> <span data-ttu-id="44b0f-173">Сондай-ақ таңдалған ресурс сыйымдылығы қандай мөлшерде тұтынылатындығын көруге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-173">You can also see how much of the selected resource's capacity is consumed.</span></span> <span data-ttu-id="44b0f-174">Ресурстарды резервтеу туралы қосымша ақпаратты көру үшін **Кеңейту** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-174">Select **Expand** to view more details about resource bookings.</span></span>

9. <span data-ttu-id="44b0f-175">**Барлық топ мүшелері** көрінісіне оралыңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-175">Return to the **All Team Members** view.</span></span> <span data-ttu-id="44b0f-176">Торда жалпы ресурстың аталған ресурсқа ауыстырылғанын және 40 сағаттың сол ресурс үшін резервтелгенін ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-176">In the grid, notice that the generic resource has been replaced by the named resource, and 40 hours are listed as booked for that resource.</span></span>

    ![Жаңартылған барлық топ мүшелері торы](media/Resource-Management-image20.png)

    > [!NOTE]
    > <span data-ttu-id="44b0f-178">Тағайындалған сағаттар көрсетілмейді, себебі олар тікелей топта резервтелген.</span><span class="sxs-lookup"><span data-stu-id="44b0f-178">No assigned hours are shown, because they were booked directly on the team.</span></span> <span data-ttu-id="44b0f-179">Олар тапсырма тағайындауын қолдану арқылы резервтелмеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-179">They weren't booked by using task assignment.</span></span>

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a><span data-ttu-id="44b0f-180">Жалпы ресурстарды тапсырмаларға тағайындау және ресурс талаптарын жасау</span><span class="sxs-lookup"><span data-stu-id="44b0f-180">Assign generic resources to tasks and generate resource requirements</span></span>

<span data-ttu-id="44b0f-181">PSA бағдарламасында тапсырмалар жасап, оларға жалпы ресурстар тағайындауға болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-181">In PSA, you can create tasks and then assign generic resources to them.</span></span> <span data-ttu-id="44b0f-182">Осылайша, кестеңізді және қаржылық нөмірлеріңізді бағалау кезінде, ресурс сұрауын толтырғыштар арқылы ұсынуға болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-182">In this way, resource demand can be represented by placeholders while you estimate your schedule and financial numbers.</span></span> <span data-ttu-id="44b0f-183">Содан кейін жалпы ресурстарға қойылатын талаптарды құрып, оларды орындай аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-183">You can then generate resource requirements for the generic resources and fulfill them.</span></span>

1. <span data-ttu-id="44b0f-184">**Жобалар** бетіндегі **Кесте** қойыншасында тапсырма құру үшін **Қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-184">On the **Projects** page, on the **Schedule** tab, select **Add** to create a task.</span></span>

    ![Жаңа тапсырма жасалды](media/Resource-Management-image21.png)

2. <span data-ttu-id="44b0f-186">**Ресурстар** өрісінде **Ресурс таңдау құралы** белгісін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-186">In the **Resources** field, select the **Resource Picker** symbol.</span></span> <span data-ttu-id="44b0f-187">Сонда ресурс таңдау құралы пайда болып, жоба бойынша топ мүшелерін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-187">The Resource Picker appears and shows existing team members for the project.</span></span>

    ![Ресурс таңдау құралы](media/Resource-Management-image22.png)

3. <span data-ttu-id="44b0f-189">Жаңа жалпы ресурстың атауын енгізіп, **Жасау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-189">Enter the name of the new generic resource, and then select **Create**.</span></span>

    ![Жаңа жалпы ресурстың атауы енгізілді](media/Resource-Management-image23.png)

4. <span data-ttu-id="44b0f-191">Пайда болатын **Жылдам жасау: жоба тобының мүшесі** диалогтық терезесіндегі **Рөл** өрісінде жалпы ресурс рөлін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-191">In the **Quick Create: Project Team Member** dialog box that appears, in the **Role** field, select the role for the generic resource.</span></span> <span data-ttu-id="44b0f-192">**Ресурс бірлігі** өрісінде жалпы ресурс үшін ұйымдық бөлімшені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-192">In the **Resourcing Unit** field, select the organizational unit for the generic resource.</span></span> <span data-ttu-id="44b0f-193">Содан кейін **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-193">Then select **Save**.</span></span>

    ![Жылдам құру: жоба тобының мүшесі диалогтық терезесі](media/Resource-Management-image24.png)

    <span data-ttu-id="44b0f-195">Жалпы топ мүшесі енді тапсырмаға тағайындалды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-195">The generic team member is now assigned to the task.</span></span>

    ![Жалпы топ мүшесі тапсырмаға тағайындалды](media/Resource-Management-image25.png)

    <span data-ttu-id="44b0f-197">**Топ** қойыншасында жалпы топтың жаңа мүшесін көресіз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-197">On the **Team** tab, you will see the new generic team member.</span></span> <span data-ttu-id="44b0f-198">Оның тағайындалған сағаттарды ғана қамтитынын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-198">Notice that it has only assigned hours.</span></span> <span data-ttu-id="44b0f-199">Бұл сағаттар жалпы топ мүшесіне тағайындалған барлық тапсырмалардың қосындысы болып табылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-199">These hours are the sum of all tasks that are assigned to the generic team member.</span></span> <span data-ttu-id="44b0f-200">Жалпы топ мүшесінің әлі қажетті сағаттары немесе ресурс талабы жоқ.</span><span class="sxs-lookup"><span data-stu-id="44b0f-200">The generic team member doesn't yet have required hours or a resource requirement.</span></span>

    ![Топ қойыншасындағы жалпы топ мүшесі](media/Resource-Management-image26.png)

5. <span data-ttu-id="44b0f-202">Енді ресурс таңдау құралы арқылы жалпы топ мүшесін басқа тапсырмаларға тағайындауға болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-202">You can now assign the generic team member to other tasks by using the Resource Picker.</span></span>

    ![Ресурсты таңдау құралындағы жалпы топ мүшесі](media/Resource-Management-image27.png)

    <span data-ttu-id="44b0f-204">Тапсырмаларға жалпы ресурсты тағайындауды аяқтағаннан кейін, жалпы ресурс үшін ресурс талабын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-204">When you've finished assigning the generic resource to tasks, you can generate a resource requirement for the generic resource.</span></span>

5. <span data-ttu-id="44b0f-205">**Топ** қойыншасында жалпы ресурсты, содан кейін **Талапты жасау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-205">On the **Team** tab, select the generic resource, and then select **Generate Requirement**.</span></span>

    ![Талапты жасау пәрмені](media/Resource-Management-image28.png)

    <span data-ttu-id="44b0f-207">Талап жасалған кезде, жалпы топ мүшесінде қажетті сағаттар мен ресурс талабына сілтеме бар болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-207">When the requirement is generated, the generic team member will have required hours and a link for the resource requirement.</span></span>

    ![Ресурс талабына сілтеме](media/Resource-Management-image29.png)

    <span data-ttu-id="44b0f-209">Аталған ресурсты резервтегеннен кейін, жалпы ресурс топтан жойылады да аталған ресурспен алмастырылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-209">After you book a named resource, the generic resource is removed from the team and replaced by the named resource.</span></span>

    ![Жалпы ресурс аталған ресурспен алмастырылады](media/Resource-Management-image30.png)

    <span data-ttu-id="44b0f-211">**Кесте** қойыншасындағы жалпы ресурс тағайындаулары жойылып, аталған ресурспен алмастырылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-211">On the **Schedule** tab, the generic resource assignments are removed and replaced by the named resource.</span></span>

    ![Жалпы ресурс тағайындаулары "Кесте" қойыншасындағы аталған ресурспен алмастырылады](media/Resource-Management-image31.png)

    > [!NOTE]
    > <span data-ttu-id="44b0f-213">Бұл әрекет аталған ресурс жалпы ресурс талабы үшін толығымен резервтелгенде ғана пайда болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-213">This behavior occurs only when a named resource is fully booked for the generic resource requirement.</span></span> <span data-ttu-id="44b0f-214">Аталған ресурс жалпы ресурс талабын ішінара алмастырғанда немесе аталған бірнеше ресурс жалпы ресурс талабын алмастырғанда, жалпы ресурс тапсырмаға тағайындалған күйінде қалады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-214">When either a named resource partially replaces the generic resource requirement or multiple named resources replace the generic resource requirement, the generic resource remains assigned to the task.</span></span>

    <span data-ttu-id="44b0f-215">Келесі суретте 80 сағаттық тапсырма бес күндік кезеңге жоспарланған (бес күн ішінде күніне 16 сағат) және **Функционалды** деп аталатын жалпы ресурсқа тағайындалған.</span><span class="sxs-lookup"><span data-stu-id="44b0f-215">In the following illustration, an 80-hour task has been planned for a five-day duration (16 hours per day over five days) and assigned to the generic resource that is named **Functional**.</span></span>

    ![Сексен сағаттық, бес күндік тапсырма функционалды жалпы ресурсқа тағайындалған](media/Resource-Management-image32.png)

    <span data-ttu-id="44b0f-217">Талапты жасаған кезде, ол бес күннің ішінде 80 сағатқа созылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-217">When you generate the requirement, it's for 80 hours over five days.</span></span>

    ![Бес күн ішінде 80 сағат бойы жасалған талап](media/Resource-Management-image33.png)

    <span data-ttu-id="44b0f-219">Қолжетімді ресурстар күніне сегіз сағат қана жұмыс істейтіндіктен, талапты орындау үшін екі ресурс қажет.</span><span class="sxs-lookup"><span data-stu-id="44b0f-219">Because available resources work only eight hours per day, two resources are needed to fulfill the requirement.</span></span>

    ![Екінші ресурс](media/Resource-Management-image35.png)

    <span data-ttu-id="44b0f-221">**Топ** қойыншасында енді жалпы ресурста қажетті сағаттардың жоқ екенін көре аласыз, бірақ тағайындалған сағаттар орындалу әрекетін құрайтын екі аталған ресурспен бірге көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-221">On the **Team** tab, you can now see that the generic resource has no required hours, but the assigned hours still appear together with the two named resources that make up the fulfillment.</span></span>

    ![Топ қойыншасындағы екі аталған ресурс](media/Resource-Management-image36.png)

    <span data-ttu-id="44b0f-223">**Кесте** қойыншасында жалпы ресурс тапсырмаға тағайындалған күйінде қалады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-223">On the **Schedule** tab, the generic resource remains assigned to the task.</span></span>

    ![Кесте қойыншасындағы жалпы ресурстар](media/Resource-Management-image37.png)

<span data-ttu-id="44b0f-225">PSA бағдарламасы ресурстың екеуін де тапсырмаға тағайындамайды, себебі бұл әрекеттен болжамдылығы төмен кесте жасалады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-225">PSA doesn't assign both resources to the task, because that behavior would produce a less predictable schedule.</span></span> <span data-ttu-id="44b0f-226">Бұл қарапайым мысалда сағаттарды екі ресурсқа тең бөлген оңай.</span><span class="sxs-lookup"><span data-stu-id="44b0f-226">In this simple example, it's easy to divide the hours equally between two resources.</span></span> <span data-ttu-id="44b0f-227">Алайда, бірнеше тапсырманы және бірнеше ресурсты қамтитын әлдеқайда күрделі сценарийлерде PSA бағдарламасы бірнеше тапсырма бойынша бірнеше ресурстан алынған тапсырыстарды бөлу жолы туралы болжам жасауы керек.</span><span class="sxs-lookup"><span data-stu-id="44b0f-227">However, in more complex scenarios that involve multiple tasks and multiple resources, PSA would have to make assumptions about how it should allocate the bookings that are received for multiple resources across multiple tasks.</span></span>

<span data-ttu-id="44b0f-228">Сондықтан, осы сценарийлерде жоба менеджері бірнеше тапсырысты талдауға және қажет болған жағдайда оларды тағайындауға жауап береді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-228">Therefore, in these scenarios, the project manager is responsible for parsing the multiple bookings and assigning them as needed.</span></span> <span data-ttu-id="44b0f-229">Тапсырыстарды бөлектеу үшін, жоба менеджері жалпы ресурстардың тапсырмаларын аталған ресурстарға тағайындайды, содан кейін **Салыстырып тексеру** көрінісін бөлектеу әрекетінің тапсырыспен бірге жұмыс істейтініне көз жеткізу үшін қолданады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-229">To allocate the bookings, the project manager assigns the tasks from the generic resources to the named resources and then uses the **Reconciliation** view to make sure that the allocation works with the bookings.</span></span>

### <a name="edit-a-resource-requirement"></a><span data-ttu-id="44b0f-230">Ресурс талабын өңдеу</span><span class="sxs-lookup"><span data-stu-id="44b0f-230">Edit a resource requirement</span></span>

<span data-ttu-id="44b0f-231">Ресурс талабы жасалғаннан кейін, жоба менеджері немесе ресурс менеджері кесте тақтасы қолданылған кезде, іздеу шарттарын нақтылау үшін мәліметтерді өңдеуді қалауы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="44b0f-231">After a resource requirement has been created, a project manager or resource manager might want to edit the details to refine the search criteria when the Schedule Board is used.</span></span> <span data-ttu-id="44b0f-232">Ресурс талабын өңдеу үшін, келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-232">To edit the resource requirement, follow these steps.</span></span>

1. <span data-ttu-id="44b0f-233">**Жобалар** бетіндегі **Топ** қойыншасында жалпы ресурс бойынша кез келген талап сілтемесін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-233">On the **Projects** page, on the **Team** tab, select the link to any requirement on a generic resource.</span></span>
2. <span data-ttu-id="44b0f-234">Пайда болатын **Ресурс талабы** бетінде бірнеше атрибутты жаңартуға болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-234">On the **Resource Requirement** page that appears, you can update several attributes.</span></span> <span data-ttu-id="44b0f-235">Мысалы:</span><span class="sxs-lookup"><span data-stu-id="44b0f-235">Here are some examples:</span></span>

    - <span data-ttu-id="44b0f-236">Атауы</span><span class="sxs-lookup"><span data-stu-id="44b0f-236">Name</span></span>
    - <span data-ttu-id="44b0f-237">Бастапқы күні</span><span class="sxs-lookup"><span data-stu-id="44b0f-237">From Date</span></span>
    - <span data-ttu-id="44b0f-238">Соңғы күні</span><span class="sxs-lookup"><span data-stu-id="44b0f-238">To Date</span></span>
    - <span data-ttu-id="44b0f-239">Ұзақтық</span><span class="sxs-lookup"><span data-stu-id="44b0f-239">Duration</span></span>
    - <span data-ttu-id="44b0f-240">Ресурс түрі</span><span class="sxs-lookup"><span data-stu-id="44b0f-240">Resource Type</span></span>

<span data-ttu-id="44b0f-241">**Ресурс талабы** бетінде жоба менеджері немесе ресурс менеджері келесі ақпаратты да анықтай алады:</span><span class="sxs-lookup"><span data-stu-id="44b0f-241">On the **Resource Requirement** page, the project manager or resource manager can also define the following information:</span></span>

- <span data-ttu-id="44b0f-242">Дағдылар</span><span class="sxs-lookup"><span data-stu-id="44b0f-242">Skills</span></span>
- <span data-ttu-id="44b0f-243">Рөлдер</span><span class="sxs-lookup"><span data-stu-id="44b0f-243">Roles</span></span>
- <span data-ttu-id="44b0f-244">Ресурс параметрлері</span><span class="sxs-lookup"><span data-stu-id="44b0f-244">Resource preferences</span></span>
- <span data-ttu-id="44b0f-245">Таңдаулы ұйымдық бөлімшелер</span><span class="sxs-lookup"><span data-stu-id="44b0f-245">Preferred organizational unit</span></span>

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a><span data-ttu-id="44b0f-246">Ресурс тапсырыстарын жобада резервтелгеннен кейін жаңарту</span><span class="sxs-lookup"><span data-stu-id="44b0f-246">Update resource bookings after they are booked on a project</span></span>

<span data-ttu-id="44b0f-247">Жоба тобына жалпы немесе аталған ресурсты қосқаннан кейін, ресурс тапсырыстарын өзгертуге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-247">After you've added a generic or named resource to a project team, you can change the resource's bookings.</span></span>

1. <span data-ttu-id="44b0f-248">**Жобалар** бетіндегі **Топ** қойыншасында топ мүшесін, содан кейін **Тапсырыстарды жүргізу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-248">On the **Projects** page, on the **Team** tab, select a team member, and then select **Maintain Bookings**.</span></span>

    ![Таңдалған топ мүшесі үшін кесте тақтасы ашылды](media/Resource-Management-image40.png)

    <span data-ttu-id="44b0f-250">Кесте тақтасы пайда болады және жоба тобы мүшесінің тапсырыстарын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-250">The Schedule Board appears and shows the project team member's bookings.</span></span> <span data-ttu-id="44b0f-251">Осы жоба және топ мүшесінің мүмкіндігін пайдаланатын басқа жобалар бойынша резервтелген сағаттарды көру үшін, топ мүшесінің жазбасын кеңейтіңіз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-251">Expand the team member's record to view the hours that have been booked against this project and other projects that are consuming the team member's capacity.</span></span>

2. <span data-ttu-id="44b0f-252">Тапсырысты кеңейту немесе қысқарту үшін, оны таңдап сүйреңіз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-252">Select and drag the booking to extend or shorten it.</span></span> <span data-ttu-id="44b0f-253">Сонда тапсырысты реттеуге мүмкіндік беретін **Ресурс тапсырысын жасау** диалогтық терезесі пайда болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-253">A **Create Resource Booking** dialog box appears that lets you adjust the booking.</span></span>

    ![Ресурс тапсырысын жасау диалогтық терезесі](media/Resource-Management-image41.png)

3. <span data-ttu-id="44b0f-255">Тапсырысты тінтуірдің оң жақ түймешігімен басыңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-255">Right-click the booking.</span></span> <span data-ttu-id="44b0f-256">Келесі әрекеттерді орындау үшін, контекстік мәзірді пайдалануға болады:</span><span class="sxs-lookup"><span data-stu-id="44b0f-256">You can then use the shortcut menu to complete the following actions:</span></span>

    - <span data-ttu-id="44b0f-257">Тапсырыс күйін өзгертіңіз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-257">Change the booking status.</span></span>
    - <span data-ttu-id="44b0f-258">Тапсырысты өңдеңіз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-258">Edit the booking.</span></span>
    - <span data-ttu-id="44b0f-259">Жоба тобындағы ресурсты алмастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-259">Substitute a resource on the project team.</span></span>

### <a name="change-the-booking-status"></a><span data-ttu-id="44b0f-260">Тапсырыс күйін өзгерту</span><span class="sxs-lookup"><span data-stu-id="44b0f-260">Change the booking status</span></span>

<span data-ttu-id="44b0f-261">Кез келген әдепкі немесе реттелмелі тапсырыс күйін өзгертуге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-261">You can change any default or custom booking status.</span></span>

![Күйді өзгерту пәрмені](media/Resource-Management-image42.png)

<span data-ttu-id="44b0f-263">Келесі күйлер PSA бағдарламасында қамтылған:</span><span class="sxs-lookup"><span data-stu-id="44b0f-263">The following statuses are included in PSA:</span></span>

- <span data-ttu-id="44b0f-264">**Бас тартылды** – бұл күй ресурстың тапсырысын болдырмайды және ресурс сыйымдылығын босатады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-264">**Canceled** – This status cancels a resource's booking and frees up the resource's capacity.</span></span>
- <span data-ttu-id="44b0f-265">**Қорытынды резервтеу** – бұл күй ресурстың сыйымдылығын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-265">**Hard Book** – This status consumes a resource's capacity.</span></span> <span data-ttu-id="44b0f-266">Әдетте **Жобалар** бетіндегі **Барлық топ мүшелері** торынан **Тапсырыстарды жүргізу** параметрін ашқан кезде, тапсырыс осы күйге ие болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-266">A booking typically has this status when you open **Maintain Bookings** from the **All Team Members** grid on the **Projects** page.</span></span>
- <span data-ttu-id="44b0f-267">**Алдын ала резервтеу** – бұл күй топқа ресурсты қосады, бірақ ресурстың сыйымдылығын пайдаланбайды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-267">**Soft Book** – This status adds a resource to a team but doesn't consume the resource's capacity.</span></span> <span data-ttu-id="44b0f-268">Бұл ресурстың ықтимал тапсырма үшін сақталғанын, бірақ басқа тапсырмалар үшін қажет болса, сыйымдылығы бар екенін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-268">It indicates that the resource has been reserved for potential work but still has capacity if it's needed on other jobs.</span></span> <span data-ttu-id="44b0f-269">Ресурстың жалпы қолжетімділігі тұрғысынан, алдын ала резервтеулер қорытынды резервтеулерге қарағанда басқа күйге ие.</span><span class="sxs-lookup"><span data-stu-id="44b0f-269">In the view of overall resource availability, soft bookings have a different status than hard bookings.</span></span>
- <span data-ttu-id="44b0f-270">**Ұсынылған** – бұл күй ресурс менеджері немесе жоба менеджерінің ресурс туралы ұсынысын білдіреді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-270">**Proposed** – This status represents a resource manager's or project manager's proposal for a resource.</span></span> <span data-ttu-id="44b0f-271">Ұсыныстар ресурстың сыйымдылығын пайдаланбайды және ресурс жоба тобына қосылмайды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-271">Proposals don't consume the capacity of a resource, and the resource isn't added to the project team.</span></span> <span data-ttu-id="44b0f-272">Топтағы ресурсты түпкілікті резервтеу үшін, жоба менеджері ұсынысты қабылдауы керек.</span><span class="sxs-lookup"><span data-stu-id="44b0f-272">To hard-book the resource on the team, the project manager must accept the proposal.</span></span>

### <a name="submit-resource-requests"></a><span data-ttu-id="44b0f-273">Ресурс сұрауларын жіберу</span><span class="sxs-lookup"><span data-stu-id="44b0f-273">Submit resource requests</span></span>

<span data-ttu-id="44b0f-274">Ресурс сұраулары ресурс менеджері орындауы керек сұранысты (ресурс талабы) орындау үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-274">Resource requests are used to carry the demand (resource requirement) that must be fulfilled by a resource manager.</span></span> <span data-ttu-id="44b0f-275">Топта әлдеқашан бар жалпы ресурс үшін ресурс сұрауын тікелей жіберуге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-275">For a generic resource that is already on the team, you can submit a resource request directly.</span></span> <span data-ttu-id="44b0f-276">Ресурс сұрауы екі жолмен орындалуы мүмкін:</span><span class="sxs-lookup"><span data-stu-id="44b0f-276">A resource request can be fulfilled in two ways:</span></span>

- <span data-ttu-id="44b0f-277">Ресурс менеджері сұрауды тікелей орындайды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-277">The resource manager directly fulfills the request.</span></span> <span data-ttu-id="44b0f-278">Бұл жағдайда, жалпы ресурс аталған ресурсы бар қорытынды резервтеумен ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-278">In this case, the generic resource is replaced by a hard booking that has a named resource.</span></span>
- <span data-ttu-id="44b0f-279">Ресурс менеджері жоба менеджеріне ресурсты ұсынады, ал жоба менеджері ұсынылған ресурсты мақұлдайды немесе қабылдамайды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-279">The resource manager proposes a resource to the project manager, and the project manager approves or rejects the proposed resource.</span></span>

#### <a name="direct-fulfillment-of-resource-requests"></a><span data-ttu-id="44b0f-280">Ресурс сұрауларын тікелей орындау</span><span class="sxs-lookup"><span data-stu-id="44b0f-280">Direct fulfillment of resource requests</span></span>

<span data-ttu-id="44b0f-281">Ресурс талабы жасалған кезде, жоба менеджері ресурсты таңдап, **Сұрау жіберу** пәрменін таңдау арқылы жалпы ресурсқа сұрау жібере алады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-281">When a resource requirement is generated, a project manager can submit a resource request for a generic resource by selecting the resource and then selecting **Submit Request**.</span></span>

![Сұрау жіберу түймешігі](media/Resource-Management-image45.png)

<span data-ttu-id="44b0f-283">Ресурс туралы пікірлер сұрауды орындайтын ресурс менеджеріне берілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="44b0f-283">Comments about the resource can be provided to the resource manager who is fulfilling the request.</span></span> <span data-ttu-id="44b0f-284">Сұрау жіберілгеннен кейін, топ мүшесінің **Күй** өрісі **Жіберілді** күйіне өзгертіледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-284">After the request is submitted, the **Status** field for the team member is changed to **Submitted**.</span></span>

![Міндетті емес пікірлерді енгізу](media/Resource-Management-image46.png)

<span data-ttu-id="44b0f-286">Ресурс менеджері сұрауды орындаған кезде, жалпы топ мүшесі **Барлық топ мүшелері** торындағы аталған ресурспен алмастырылады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-286">When the resource manager fulfills the request, the generic team member is replaced by the named resource in the **All Team Members** grid.</span></span>

![Жалпы топ мүшесі "Барлық топ мүшелері" торындағы аталған ресурспен алмастырылады](media/Resource-Management-image47.png)

#### <a name="use-a-resource-proposal-for-resource-requests"></a><span data-ttu-id="44b0f-288">Ресурс сұраулары үшін ресурс ұсынысын пайдалану</span><span class="sxs-lookup"><span data-stu-id="44b0f-288">Use a resource proposal for resource requests</span></span>

<span data-ttu-id="44b0f-289">Ресурс сұрауы бойынша тікелей резервтеудің орнына, ресурс менеджері жоба менеджеріне ресурсты ұсына алады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-289">Instead of directly booking a resource on a resource request, a resource manager can propose a resource to the project manager.</span></span> <span data-ttu-id="44b0f-290">Ресурс менеджері талаптарға дәл сәйкестік болмаған кезде осы опцияны қолдана алады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-290">A resource manager might use this option when an exact match for the requirements isn't available.</span></span> <span data-ttu-id="44b0f-291">Ресурс менеджері ресурсты ұсынған кезде, жоба менеджері жалпы топ мүшесінің **Күй** өрісі **Қарап шығуды талап етеді** күйіне өзгертілгенін көреді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-291">When a resource manager proposes a resource, the project manager sees that the **Status** field for the generic team member is changed to **Needs Review**.</span></span>

![Жалпы топ мүшесінің күйі "Қарап шығуды талап етеді" күйіне өзгереді](media/Resource-Management-image48.png)

<span data-ttu-id="44b0f-293">Ұсынылған ресурсты ұсынысты резервтеу әсерінің визуализациясымен бірге көру үшін, **Қарап шығуды талап етеді** күйі бар топ мүшесін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-293">To view the proposed resource together with a visualization of the effect of the proposal's booking, double-click the team member that has a status of **Needs Review**.</span></span> <span data-ttu-id="44b0f-294">Содан кейін **Ұсынылатын ресурстар** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-294">Then select the **Proposed Resources** tab.</span></span>

![Ұсынылған ресурстар қойыншасы](media/Resource-Management-image49.png)

<span data-ttu-id="44b0f-296">Барлық ұсынылған ресурстарды қабылдау **Барлық ұсыныстарды қабылдау** параметрін немесе оларды қабылдамау үшін **Барлық ұсыныстарды қабылдамау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-296">Select **Accept All Proposals** to accept all proposed resources or **Reject All Proposals** to reject them.</span></span> <span data-ttu-id="44b0f-297">Егер ұсынылған ресурстарды қабылдасаңыз, онда олар жобада топ мүшелері ретінде түпкілікті резервтеледі және жалпы ресурстарды алмастырады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-297">If you accept the proposed resources, they are hard-booked on the project as team members and replace the generic resources.</span></span>

> [!NOTE]
> <span data-ttu-id="44b0f-298">Барлық ұсынылған ресурстарды қабылдауыңыз немесе қабылдамауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="44b0f-298">You must either accept or reject all proposed resources.</span></span> <span data-ttu-id="44b0f-299">Оларды ішінара қабылдасаңыз немесе қабылдамасаңыз болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-299">You can't partially accept or reject them.</span></span>

### <a name="substitute-a-resource-on-the-project-team"></a><span data-ttu-id="44b0f-300">Жоба тобындағы ресурсты алмастыру</span><span class="sxs-lookup"><span data-stu-id="44b0f-300">Substitute a resource on the project team</span></span>

<span data-ttu-id="44b0f-301">Кейде жоба менеджері резервтелген топ мүшесін жоба бойынша алмастыруы керек.</span><span class="sxs-lookup"><span data-stu-id="44b0f-301">Sometimes, a project manager must substitute a booked team member on a project.</span></span>

1. <span data-ttu-id="44b0f-302">**Жобалар** бетіндегі **Топ** қойыншасында алмастыру керек ресурсты, содан кейін **Тапсырыстарды жүргізу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-302">On the **Projects** page, on the **Team** tab, select the resource that needs a substitute, and then select **Maintain Bookings**.</span></span>
2. <span data-ttu-id="44b0f-303">Тағайындалған жобаларын көру үшін ресурсты кеңейтіңіз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-303">Expand the resource to view the projects that it's assigned to.</span></span>

    ![Ресурс тағайындалған жобаларын көрсету үшін кеңейтіледі](media/Resource-Management-image50.png)

3. <span data-ttu-id="44b0f-305">Жобаны тінтуірдің оң жақ түймешігімен басып, **Орын басушы ресурс** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-305">Right-click the project, and then select **Substitute Resource**.</span></span>
4. <span data-ttu-id="44b0f-306">Егер ағымдағы ресурсты алмастырғыңыз келетін ресурсты білсеңіз, атауын таңдаңыз немесе теріңіз де, **Қайта тағайындау** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-306">If you know the resource that you want to substitute for the current resource, select or type the name, and then select **Re-assign**.</span></span>

    ![Орын басушы ресурсты көрсету](media/Resource-Management-image51.png)

    <span data-ttu-id="44b0f-308">Не болмаса, ресурсты іздеу үшін келесі қадамдарды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="44b0f-308">Alternatively, follow these steps to search for a resource:</span></span>

    1. <span data-ttu-id="44b0f-309">**Ауыстырылатын элементті табу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-309">Select **Find Substitution**.</span></span>

        ![Орын басушы ресурсты іздеу](media/Resource-Management-image52.png)

        <span data-ttu-id="44b0f-311">Кесте көмекшісі қолжетімді орын басушылар тізімін қайтарады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-311">The Schedule Assistant returns a list of available substitutes.</span></span> <span data-ttu-id="44b0f-312">Кесте көмекшісінде қолайлы орын басушыны табу үшін қолжетімді ресурстарды одан әрі сүзгілей аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-312">In the Schedule Assistant, you can further filter the available resources to find a suitable substitute.</span></span>

        ![Қолжетімді орын басушылар тізімі](media/Resource-Management-image53.png)

    2. <span data-ttu-id="44b0f-314">Ресурсты ауыстыру үшін, қажетті ресурсты басып, **Ауыстыру** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-314">To substitute the resource, select the resource that you want, and then select **Substitute**.</span></span>

        ![Орын басушы ресурс таңдалған](media/Resource-Management-image54.png)

    <span data-ttu-id="44b0f-316">Тапсырыстар мен тағайындаулар жаңа ресурспен алмастырылды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-316">The bookings and assignments are substituted with the new resource.</span></span>

    ![Жаңа ресурспен алмастырылған тапсырыстар мен тағайындаулар](media/Resource-Management-image55.png)

## <a name="reconcile-team-member-bookings-and-assignments"></a><span data-ttu-id="44b0f-318">Топ мүшесінің тапсырыстары мен тағайындауларын салыстырып тексеру</span><span class="sxs-lookup"><span data-stu-id="44b0f-318">Reconcile team member bookings and assignments</span></span>

<span data-ttu-id="44b0f-319">Топ мүшелері үшін тапсырыстар мен тағайындаулар бір-бірімен тығыз байланысқан.</span><span class="sxs-lookup"><span data-stu-id="44b0f-319">For team members, bookings and assignments are loosely coupled.</span></span> <span data-ttu-id="44b0f-320">Басқаша айтқанда, ресурстарда тағайындаулар бар болуы, бірақ тапсырыстар жоқ болуы немесе тапсырыстар бар болуы, бірақ тағайындаулар жоқ болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="44b0f-320">In other words, resources can have assignments but no bookings, or they can have bookings but no assignments.</span></span> <span data-ttu-id="44b0f-321">Ең дұрысы, тапсырыстар мен тағайындаулар ресурстар тапсырма тағайындауларын орындауға қабілетті болатындай туралануы керек.</span><span class="sxs-lookup"><span data-stu-id="44b0f-321">Ideally, bookings and assignments should be aligned, so that resources have committed capacity to perform the task assignments.</span></span> <span data-ttu-id="44b0f-322">Алайда, тапсырыстар қолжетімділікке негізделуі мүмкін және жоба жалғасқан кезде тапсырма мерзімі өзгеруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="44b0f-322">However, the bookings might be based on availability, and task timings might change as the project continues.</span></span> <span data-ttu-id="44b0f-323">Сондықтан, тапсырыстар мен тағайындаулардың бос байланысы икемділікті қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-323">Therefore, the loose coupling of bookings and assignments provides flexibility.</span></span>

<span data-ttu-id="44b0f-324">PSA бағдарламасындағы **Салыстырып тексеру** қойыншасы жоба менеджерлеріне топ мүшелерінің тапсырыстары мен жоба топтарына берілген тағайындауларды салыстырып тексеруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-324">PSA has a **Reconciliation** tab that lets project managers reconcile team members' bookings and their assignments for project teams.</span></span>

![Салыстырып тексеру қойыншасы](media/Resource-Management-image56.png)

<span data-ttu-id="44b0f-326">**Салыстырып тексеру** қойыншасында топтың әр мүшесі үшін жеке тапсырма тағайындауы деңгейіндегі тапсырыстар мен тағайындаулар көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="44b0f-326">The **Reconciliation** tab shows bookings and assignments down to the level of the individual task assignment for each team member.</span></span> <span data-ttu-id="44b0f-327">Онда уақыт кезеңдерін айлардан күндерге дейін көрсететін ұяшықтардағы сағаттар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-327">It shows hours in cells that represent time periods from months down to days.</span></span>

<span data-ttu-id="44b0f-328">Сондай-ақ қойыншада жалпы бағанмен бірге жобаның жалпы таза қорытындысы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-328">The tab also shows an overall net total for the project, together with a total column.</span></span>

<span data-ttu-id="44b0f-329">Әр ресурс үшін қойыншада топ мүшелерінің тапсырыстары мен топ мүшелерінің тапсырма тағайындауларының жиынтығы арасындағы айырмашылық есептеледі.</span><span class="sxs-lookup"><span data-stu-id="44b0f-329">For each resource, the tab calculates the difference between the team member's bookings and a rollup of the team member's task assignments.</span></span> <span data-ttu-id="44b0f-330">Ең дұрысы, бұл айырмашылық 0 (нөл) мәніне тең болуы керек.</span><span class="sxs-lookup"><span data-stu-id="44b0f-330">Ideally, this difference should be 0 (zero).</span></span> <span data-ttu-id="44b0f-331">Басқаша айтқанда, тапсырыстар мен тағайындаулардың арасында ешқандай айырмашылық болмауы керек.</span><span class="sxs-lookup"><span data-stu-id="44b0f-331">In other words, there should be no difference between bookings and assignments.</span></span> <span data-ttu-id="44b0f-332">Айырмашылықтар екі шартқа назар аударту үшін түспен ерекшеленген және көлеңкеленген:</span><span class="sxs-lookup"><span data-stu-id="44b0f-332">Differences are colored and shaded to draw attention to two conditions:</span></span>

- <span data-ttu-id="44b0f-333">**Тапсырыс тапшылығы** – тапсырыс тапшылығы ресурста тапсырыстарға қарағанда тағайындаулар көп болған кезде орын алады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-333">**Booking shortage** – A booking shortage occurs when a resource has more assignments than bookings.</span></span> <span data-ttu-id="44b0f-334">Бұл сыйымдылық сақталмағандықтан, жоба менеджері тапшылықты жабу үшін ресурс тапсырыстарын кеңейту арқылы бұл жағдайды түзетуді қалауы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="44b0f-334">Because this capacity hasn't been reserved, a project manager might want to correct this condition by extending the resource's bookings to cover the deficit.</span></span>
- <span data-ttu-id="44b0f-335">**Артық тапсырыстар** – артық тапсырыс жоба үшін ресурсқа тапсырыс берілген кезде, бірақ тапсырмаларға тағайындалмаған кезде орын алады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-335">**Excess bookings** – Excess bookings occur when a resource has been booked to the project but hasn't been assigned to tasks.</span></span> <span data-ttu-id="44b0f-336">Бұл шарт ресурс тапсырма тағайындалғанға дейін жобаға резервтелген жағдайда қолайлы болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="44b0f-336">This condition might be acceptable in the cases where the resource was booked to the project before task assignment occurred.</span></span> <span data-ttu-id="44b0f-337">Алайда, басқа жағдайларда, ресурс тапсырмаларға тағайындалады деп жоспарланбайды.</span><span class="sxs-lookup"><span data-stu-id="44b0f-337">However, in other cases, the resource isn't planned to be assigned to tasks.</span></span> <span data-ttu-id="44b0f-338">Мұндай жағдайларда жоба менеджері сыйымдылықты басқа жоба үшін пайдалануға болатындай ресурс тапсырыстарынан бас тарту туралы ойлануы керек.</span><span class="sxs-lookup"><span data-stu-id="44b0f-338">In these cases, the project manager should consider canceling the resource's bookings, so that the capacity can be used for another project.</span></span>

<span data-ttu-id="44b0f-339">Кейбір жағдайларда уақытты күн деңгейінен (мысалы, ай деңгейінен) жоғары деңгейде қараған кезде, ресурс үшін нөлдің таза айырмашылығын байқай аласыз (басқаша айтқанда, тапсырмалар = тағайындаулар).</span><span class="sxs-lookup"><span data-stu-id="44b0f-339">In some cases, when you view time at a higher level than the day level (for example, the month level), you might see a net difference of zero for a resource (in other words, bookings = assignments).</span></span> <span data-ttu-id="44b0f-340">Алайда, егер уақытты апта деңгейінде қарасаңыз, онда бірінші аптада нөл сағаттық және 40 сағаттық тағайындаулар бар екенін, ал екінші аптада 40 сағаттық және нөл сағаттық тағайындаулар бар екенін көре аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-340">However, if you view time at the week level, you might see that there are assignments of zero hours and bookings of 40 hours in the first week, but assignments of 40 hours and bookings of zero hours in the second week.</span></span> <span data-ttu-id="44b0f-341">Жалпы, тапсырыстар мен тағайындаулар салыстырып тексерілген, бірақ олар бір аптадан екінші аптаға дейін ерекшеленеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-341">Overall, the bookings and assignments are reconciled, but they differ from one week to the next.</span></span>

<span data-ttu-id="44b0f-342">Уақытты жоғарырақ деңгейде қарасаңыз, **Салыстырып тексеру** қойыншасындағы ұяшықтарда төменгі деңгейлерде айырмашылықтар бар екендігі туралы хабардар ететін индикатор бар болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-342">When you view time at higher levels, cells in the **Reconciliation** tab have an indicator to inform you that there are differences at lower levels.</span></span> <span data-ttu-id="44b0f-343">Ұяшықты екі рет басу арқылы айырмашылықты көру үшін оны үлкейтуге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-343">By double-clicking in a cell, you can zoom in to view the difference.</span></span> <span data-ttu-id="44b0f-344">Кішірейту үшін оны тінтуірдің оң жақ түймешігімен басуға болады. Ресурсты таңдап, тордың құралдар тақтасындағы **Келесі айырмашылық** басқару элементін пайдалану арқылы сол ресурстың тапсырыстары мен тағайындаулары арасындағы келесі айырмашылыққа өтуіңізге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-344">You can then right-click to zoom out. By selecting a resource and then using the **Next difference** control on the grid toolbar, you can go to the next difference between bookings and assignments for that resource.</span></span> <span data-ttu-id="44b0f-345">Содан кейін қайту үшін **Алдыңғы айырмашылық** басқару элементін қолдана аласыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-345">You can then use the **Previous difference** control to go back.</span></span> <span data-ttu-id="44b0f-346">Сондай-ақ айырмашылық индикаторы мен шарлау әрекетін **Параметрлер** тармағында өшіруге болады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-346">You can also turn off the difference indicator and navigation behavior under **Settings**.</span></span>

![Айырмашылық индикаторы](media/Resource-Management-image57.png)

<span data-ttu-id="44b0f-348">Егер ресурсқа арналған тапсырма тағайындаулары бар болса, бірақ тапсырыстар жоқ болса, **Жобалар** бетіндегі **Салыстырып тексеру** қойыншасында тапсырыс тапшылығын, содан кейін **Тапсырыстың мерзімін ұзарту** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="44b0f-348">If you have task assignments for a resource but no bookings, on the **Projects** page, on the **Reconciliation** tab, select the booking shortage, and then select **Extend Booking**.</span></span> <span data-ttu-id="44b0f-349">Сонда **Тапсырыстың мерзімін ұзарту** диалогтық терезесі пайда болады және ресурс тапшылығын жою үшін қажет тапсырысты көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-349">The **Extend Booking** dialog box appears and shows the booking that is needed to address the resource's shortage.</span></span> <span data-ttu-id="44b0f-350">Сондай-ақ бұл барлық жобалар немесе басқа жоспарланатын нысандар бойынша ресурстың бар тапсырыстарын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="44b0f-350">It also shows the resource's existing bookings across all projects or other schedulable entities.</span></span> <span data-ttu-id="44b0f-351">Егер ресурс үшін тапсырысты жасау үшін **OK** опциясын таңдасаңыз, сол ресурстың қолжетімділігіне қарамастан, артық тапсырыстың туындауына себеп болуыңыз мүмкін.</span><span class="sxs-lookup"><span data-stu-id="44b0f-351">If you select **OK** to create the booking for the resource, regardless of that resource's availability, you might cause overbooking.</span></span>

![Тапсырыстың мерзімін ұзарту диалогтық терезесі](media/Resource-Management-image58.png)

<span data-ttu-id="44b0f-353">Кейін жоба менеджері немесе ресурс менеджері ресурстар кестесін ресурс сыйымдылығынан асыра шамадан тыс резервтелген кез келген жағдайларды басқару үшін қолдана алады.</span><span class="sxs-lookup"><span data-stu-id="44b0f-353">The project manager or resource manager can then use the Schedule Board to manage any situations where a resource is overbooked beyond its capacity.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]