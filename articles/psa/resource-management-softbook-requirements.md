---
title: Талаптарды алдын ала тіркеу
description: Бұл тақырыпта талаптарды алдын ала тіркеу жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 861e484ea2fc251e0082b4cb0cd5409a45a74057
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079870"
---
# <a name="soft-book-requirements"></a><span data-ttu-id="250c7-103">Талаптарды алдын ала тіркеу</span><span class="sxs-lookup"><span data-stu-id="250c7-103">Soft-book requirements</span></span>

<span data-ttu-id="250c7-104">Ресурс талаптарын түпкілікті тіркеуге болады.</span><span class="sxs-lookup"><span data-stu-id="250c7-104">A resource requirement can be hard-booked.</span></span> <span data-ttu-id="250c7-105">Түпкілікті тіркеу ресурс мүмкіндігін пайдаланатын ұсынысты жасайды.</span><span class="sxs-lookup"><span data-stu-id="250c7-105">A hard booking creates a proposal that consumes a resource's capacity.</span></span> <span data-ttu-id="250c7-106">Содан кейін ұсыныс бекіту үшін сұрау салушыға қайта жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="250c7-106">The proposal is then sent back to the requester for approval.</span></span> <span data-ttu-id="250c7-107">Алдын ала тіркеу ресурсты жоба тобына алдын ала қосады және оның кесте тақтасындағы күйі өзгеше болады, бірақ ол ресурс мүмкіндігін пайдаланбайды.</span><span class="sxs-lookup"><span data-stu-id="250c7-107">A soft booking tentatively adds a resource to a project team and has a different status on the Schedule Board, but it doesn't consume the resource's capacity.</span></span> <span data-ttu-id="250c7-108">Ресурсты кесте тақтасынан алдын ала тіркеу үшін, **Тапсырыс беру күйі** өрісін **Алдын ала** параметріне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="250c7-108">To soft-book a resource from the Schedule Board, set the **Booking Status** field to **Soft**.</span></span>

!["Алдын ала" параметріне орнатылған тапсырыс беру күйі](media/Resource-Management-image77.png)

<span data-ttu-id="250c7-110">**Топ** қойыншасы **Аталған топ мүшелері** көрінісінде болған кезде, ресурс сол жерде пайда болады.</span><span class="sxs-lookup"><span data-stu-id="250c7-110">When the **Team** tab is in the **Named Team Members** view, the resource appears there.</span></span> <span data-ttu-id="250c7-111">Алдын ала тіркелген сағаттар **Алдын ала тіркелген сағаттар** бағанында беріледі.</span><span class="sxs-lookup"><span data-stu-id="250c7-111">The soft-booked hours are reported in the **Soft Booked Hours** column.</span></span>

!["Аталған топ мүшелері" көрінісіндегі алдын ала тіркелген сағаттар](media/Resource-Management-image78.png)

<span data-ttu-id="250c7-113">Алдын ала тіркелген топ мүшелерін жоба тапсырмаларына тағайындауға болады.</span><span class="sxs-lookup"><span data-stu-id="250c7-113">Soft-booked team members can be assigned to tasks.</span></span>

![Тапсырмаға тағайындалған алдын ала тіркелген топ мүшесі](media/Resource-Management-image79.png)

<span data-ttu-id="250c7-115">**Салыстырып тексеру** қойыншасында, алдын ала тіркелген ресурс үшін тапсырыстар көрсетілмейді, себебі **Салыстырып тексеру** қойыншасы тек түпкілікті тіркеуді қарастырады.</span><span class="sxs-lookup"><span data-stu-id="250c7-115">On the **Reconciliation** tab, no bookings are shown for a soft-book resource, because the **Reconciliation** tab considers only hard-bookings.</span></span>

![Салыстырып тексеру қойыншасындағы тапсырысы жоқ алдын ала резервтелген ресурс](media/Resource-Management-image80.png)

> [!NOTE]
> <span data-ttu-id="250c7-117">Жалпы топ мүшесінен жасалған талаптан ресурсты алдын ала резервтеу мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="250c7-117">You can't soft-book a resource from a requirement that was generated from a generic team member.</span></span>

<span data-ttu-id="250c7-118">Кесте тақтасында ресурсқа арналған алдын ала резервтеулер үшін басқа түс пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="250c7-118">On the Schedule Board, a different coloring is used for soft bookings for a resource.</span></span>

![Кесте тақтасындағы алдын ала резервтеулер](media/Resource-Management-image81.png)

<span data-ttu-id="250c7-120">Алдын ала резервтеуді қорытынды резервтеуге түрлендіру үшін, кесте тақтасында алдын ала резервтеуді басып, **Күйді өзгерту** \> **Қорытынды резервтеу** \> **Қорытынды** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="250c7-120">To convert a soft booking to a hard booking, on the Schedule Board, right-click the soft booking, and then select **Change Status** \> **Hard Book** \> **Hard**.</span></span>

![Резервтеу күйін "Қорытынды" күйіне өзгерту](media/Resource-Management-image82.png)

<span data-ttu-id="250c7-122">Резервтеу өзгертіліп, кесте тақтасында күйі өзгертілді.</span><span class="sxs-lookup"><span data-stu-id="250c7-122">The booking is changed, and the status is changed on the Schedule Board.</span></span> <span data-ttu-id="250c7-123">Резервтеу күйі енді **Қорытынды** болғандықтан, ресурс резервтелген ретінде көрсетіледі және оның сыйымдылығы мен қолжетімділігі реттеледі.</span><span class="sxs-lookup"><span data-stu-id="250c7-123">Because the booking status is now **Hard** , the resource is shown as booked, and its capacity and availability are adjusted.</span></span>

<span data-ttu-id="250c7-124">Кесте тақтасынан қорытынды резервтеуден немесе алдын ала резервтеуден бас тарту үшін осы әдісті пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="250c7-124">You can use the same method to cancel a hard booking or a soft booking from the Schedule Board.</span></span>

<span data-ttu-id="250c7-125">Жобаның **Топ** қойыншасында алдын ала резервтелген ресурсты қорытынды резервтелген ресурсқа түрлендіру үшін, ресурсты таңдап, **Растау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="250c7-125">To convert a resource that is soft-booked to hard-booked on the project's **Team** tab, select the resource, and then select **Confirm**.</span></span>

![Растау пәрмені](media/Resource-Management-image83.png)
