---
title: Ресурс талаптарынан аталған ресурстарды тіркеу
description: Бұл тақырыпта жалпы ресурс талабы үшін аталған ресурстарды тіркеу туралы ақпарат берілген.
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: c2f97107de938975491770ab4e2ed18a3145d0e3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013403"
---
# <a name="book-named-resources-from-resource-requirements"></a><span data-ttu-id="66c38-103">Ресурс талаптарынан аталған ресурстарды тіркеу</span><span class="sxs-lookup"><span data-stu-id="66c38-103">Book named resources from resource requirements</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="66c38-104">Ресурс талабы бар жалпы ресурсты ауыстыру үшін аталған ресурсты тіркеуге болады.</span><span class="sxs-lookup"><span data-stu-id="66c38-104">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="66c38-105">Project Service Automation (PSA) жүйесінің **Жобалар** бетінде **Топ** қойыншасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="66c38-105">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab.</span></span>
2. <span data-ttu-id="66c38-106">Тізімнен ресурс талабы бар жалпы ресурсты таңдап, **Тіркеу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="66c38-106">Select the generic resource that has a resource requirement from the list and then click **Book**.</span></span> <span data-ttu-id="66c38-107">Немесе ресурс талабын ашып, **Тіркеу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="66c38-107">Or, open the resource requirement and then click **Book**.</span></span>


![Жалпы топ мүшесін тіркеу](media/RM-how-to-14.png)


3. <span data-ttu-id="66c38-109">**Кесте көмекшісі** бетінде жобаға тіркелетін аталған ресурсты таңдап, **Тіркеу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="66c38-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then click **Book**.</span></span>

![Кесте көмекшісінің көмегімен жалпы топ мүшесін тіркеу](media/RM-how-to-15.png)

<span data-ttu-id="66c38-111">Тіркеу аяқталған және аталған ресурспен орындалған кезде, жалпы ресурс аталған ресурспен ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="66c38-111">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

![Аталған топ мүшесіне ауыстырылатын жалпы топ мүшесі](media/RM-how-to-16.png)

<span data-ttu-id="66c38-113">Аталған ресурспен бірге кестедегі тағайындаулар да жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="66c38-113">The assignments on the schedule are updated with the named resource as well.</span></span>

![Жобалық тапсырмаларға тағайындалған аталған топ мүшесі](media/RM-how-to-17.png)

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="66c38-115">Жалпы ресурсты бірнеше аталған ресурстармен толықтырыңыз</span><span class="sxs-lookup"><span data-stu-id="66c38-115">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="66c38-116">Бірнеше аталған ресурстары бар жалпы ресурсқа сұранысты орындау жалғыз аталған ресурсты тағайындаумен бірдей.</span><span class="sxs-lookup"><span data-stu-id="66c38-116">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="66c38-117">Мысалы, ұзақтығы бес күн және 120 сағаттық жұмысты қажет ететін тапсырма бар.</span><span class="sxs-lookup"><span data-stu-id="66c38-117">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="66c38-118">Бұл тапсырманы әдетте аптасына бес күн, сегіз сағат жұмыс істейтін бір ресурс аяқтай алмайды.</span><span class="sxs-lookup"><span data-stu-id="66c38-118">This task can't be completed by one resource that works a typical eight-hour day over a five day week.</span></span> 

![Бес күн ішінде 120 сағаттық жұмысты қажет ететін тапсырма](media/RM-how-to-21.png)

<span data-ttu-id="66c38-120">Бес күн ішінде 120 сағат, яғни күніне 24 сағат роботты техника жұмысы талап етіледі.</span><span class="sxs-lookup"><span data-stu-id="66c38-120">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

![Бір күн ішіндегі талап](media/RM-how-to-22.png)

<span data-ttu-id="66c38-122">Бұл жалпы ресурстық сұранысты орындау үшін бірнеше аталған ресурстар қажет болған кездегі мысал.</span><span class="sxs-lookup"><span data-stu-id="66c38-122">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="66c38-123">Талапты орындау үшін бірнеше ресурсты тіркеу қажет.</span><span class="sxs-lookup"><span data-stu-id="66c38-123">You will need to book multiple resources to fulfill the requirement.</span></span>

![Талапты орындау үшін бірнеше ресурсты тіркеу](media/RM-how-to-23.png)

<span data-ttu-id="66c38-125">Бұл сценарийдегі басты айырмашылық — жалпы ресурс тапсырмаға тағайындалған топта қалады, ал тіркелген аталған ресурс тобының мүшелері лауазым бөлігі ретінде тағайындалмайды.</span><span class="sxs-lookup"><span data-stu-id="66c38-125">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="66c38-126">Жоба менеджері жұмысты аталған ресурстарға сәйкес тағайындай алады.</span><span class="sxs-lookup"><span data-stu-id="66c38-126">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="66c38-127">**Салыстырып тексеру** көрінісі жоба менеджеріне бірнеше ресурстар бойынша тапсырыстарды тапсырма тағайындауларына бөлуге көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="66c38-127">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="66c38-128">Бұл автоматты түрде жасалмайды, себебі кез келген жоғарыдағы қарапайым мысалға қарағанда күрделірек сценарийде, мысалы, сізде талапты құрайтын тапсырмалар жинағы бар болған кезде, жоба менеджерінің тағайындау жолы жүйемен қарастырылуы керек.</span><span class="sxs-lookup"><span data-stu-id="66c38-128">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement, the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="66c38-129">Жүйе мақсатты түсінбейтіндіктен, жорамалдар мақсатты жорамалдардан өзгеше болуы мүмкін және дұрыс емес немесе болжауға келмейтін нәтиже орын алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="66c38-129">Because the system can't understand intent, chances are that the assumptions will be different than intended and an incorrect or unpredictable result will happen.</span></span> <span data-ttu-id="66c38-130">Болжауға болатын нәтиже — жоба менеджері **Салыстырып тексеру** көрінісінің көмегімен тағайындауларды әдейі жасамайынша жалпы ресурстың тағайындалған күйде қалуы.</span><span class="sxs-lookup"><span data-stu-id="66c38-130">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]