---
title: Microsoft Project Client біріктіруі
description: Жобаны жоспарлау және жүргізу күрделі болуы мүмкін, сондықтан жоба басқарушылары осы тапсырманы басқаруға көмектесетін құралдарды пайдалануы қажет. Microsoft Project Client бағдарламасымен біріктіру жоба жұмысын бөлу құрылымын басқару және ашуға қолдау көрсетумен қамтамасыз етеді.
author: Yowelle
ms.date: 06/16/2021
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: b312ec5b1f4e6a98a2cbf1667b2f55b758b2d613
ms.sourcegitcommit: 3a4b181be08ef0428104d72b54a3e61ac2782f14
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "6269842"
---
# <a name="microsoft-project-client-integration"></a><span data-ttu-id="2b9e0-104">Microsoft Project Client біріктіруі</span><span class="sxs-lookup"><span data-stu-id="2b9e0-104">Microsoft Project client integration</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="2b9e0-105">Жобаны жоспарлау және жүргізу күрделі болуы мүмкін, сондықтан жоба басқарушылары осы тапсырманы басқаруға көмектесетін құралдарды пайдалануы қажет.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-105">Planning and maintaining a project schedule can be complex, so project managers need to use tools that help them manage this task.</span></span> <span data-ttu-id="2b9e0-106">Microsoft Project Client бағдарламасымен біріктіру жоба жұмысын бөлу құрылымын басқару және ашуға қолдау көрсетумен қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-106">Integration with Microsoft Project Client provides support to open and manage a project work breakdown structure.</span></span> <span data-ttu-id="2b9e0-107">Жоба басқарушысы кез келген өзгерістерді Dynamics 365 Finance жоба жұмысын бөлу құрылымына жариялай алады.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-107">The project manager can publish any changes back to the Dynamics 365 Finance project work breakdown structure.</span></span>

> [!NOTE]
> <span data-ttu-id="2b9e0-108">Шілде жаңартуын (10.0.4 нұсқасы) пайдаланатын болсаңыз, 4054797 және 4055884 білім қорын орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-108">If you are using the July update (version 10.0.4), you must install KB 4054797 and 4055884.</span></span>

## <a name="configure-the-microsoft-project-client-add-in"></a><span data-ttu-id="2b9e0-109">Microsoft Project Client қондырмасын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="2b9e0-109">Configure the Microsoft Project Client add-in</span></span>
<span data-ttu-id="2b9e0-110">Microsoft Project Client бағдарламасымен біріктіруді қосу үшін Microsoft Dynamics 365 қондырмасын пайдаланушы клиентінің Microsoft Project бағдарламасында орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-110">To enable the integration with Microsoft Project Client, a Microsoft Dynamics 365 add-in is required to be installed in the user’s client Microsoft Project application.</span></span> <span data-ttu-id="2b9e0-111">Бұл әрекет **Жобаны басқару жұмыс кеңістігін** ашу арқылы жасалады.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-111">This is done by opening the **Project management workspace**.</span></span>

<span data-ttu-id="2b9e0-112">•   Жұмыс кеңістігінің **Сілтемелер** > **Параметр** бөлімінен **Жоба клиентінің қондырмасын конфигурациялау** опциясын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-112">•   Click **Configure project client add-in** from the **Links** > **Setup** section of the workspace.</span></span>

<span data-ttu-id="2b9e0-113">•   **Ашу** опциясын, содан соң сұралғанда **Іске қосу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-113">•   Click **Open**, then click **Run** when prompted.</span></span>

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a><span data-ttu-id="2b9e0-114">Microsoft Project Client бағдарламасында қолданыстағы жобалық жұмысты бөлу құрылымын ашып, өңдеңіз</span><span class="sxs-lookup"><span data-stu-id="2b9e0-114">Open and edit an existing draft work breakdown structure in Microsoft Project Client</span></span>
<span data-ttu-id="2b9e0-115">Dynamics 365 Finance бағдарламасындағы жобада жасалған жұмысты бөлу құрылымы болса, жұмысты бөлу құрылымы жобалық күйде болса Microsoft Project Client бағдарламасында жұмысты бөлу құрылымы ашылады.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-115">If a project in Dynamics 365 Finance already has a work breakdown structure created, the work breakdown structure can be opened in the Microsoft Project Client application if the work breakdown structure is in a draft status.</span></span> <span data-ttu-id="2b9e0-116">**Жоба** бетінен ашу үшін **Жоспар** қойыншасынан **Microsoft Project бағдарламасында ашу** түймешігін басыңыз. Бұл бетті **Microsoft Dynamics 365** қойыншасында **Ашу** түймешігін басу арқылы Microsoft Project Client бағдарламасында ашуға болады. Тізімнен **Заңды нысан** және **Жоба** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-116">To open from the **Project** page, click **Open in Microsoft Project** link from the **Plan** tab. This page can also be opened from within the Microsoft Project Client application by clicking **Open** in the **Microsoft Dynamics 365** tab. Select the **Legal entity** and **Project** from the list.</span></span>

> [!NOTE]
> <span data-ttu-id="2b9e0-117">Internet Explorer бағдарламасын шолғыш ретінде пайдаланатын болсаңыз, файл жүктелетін орыннан қолмен ашу үшін **Сақтау** опциясын басу қажет.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-117">If you're using Internet Explorer as your browser, you will need to click **Save** to manually open from the location that the file is downloaded to.</span></span> <span data-ttu-id="2b9e0-118">Не болмаса, файлды Microsoft Project Client бағдарламасында ашу үшін **Сақтау және ашу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-118">Or, click **Save and open** to open the file in Microsoft Project Client.</span></span> <span data-ttu-id="2b9e0-119">Сақтау кезінде файлдың атауын өзгертпеңіз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-119">Do not rename the file name when saving.</span></span>

<span data-ttu-id="2b9e0-120">Microsoft Project Client бағдарламасы арқылы файлға өзгертулер жасау алдында оны тексеру қажет. **Microsoft Dynamics 365** қойыншасында **Тексеру** опциясын басыңыз. Бұл басқа пайдаланушылардың Finance жүйесіндегі жұмысты бөлу құрылымын бір уақытта өңдеуін болдырмайды.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-120">Before making any edits to the file using Microsoft Project Client, you need to check it out. Click **Check out** in the **Microsoft Dynamics 365** tab. This will prevent other users from editing the work breakdown structure from within Finance at the same time.</span></span> <span data-ttu-id="2b9e0-121">Өзгертулерді аяқтағаннан кейін жұмысты бөлу құрылымын жариялау үшін **Microsoft Dynamics 365** қойыншасында **Тексеру** опциясын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-121">To publish the work breakdown structure after completing any edits, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

<span data-ttu-id="2b9e0-122">Жоба тобы Finance бағдарламасындағы жобаға қосылған болса, ресурстар тізімі топ мүшелерімен толтырылады.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-122">If a project team has already been added to the project in Finance, the resource list will be populated with the team members.</span></span> <span data-ttu-id="2b9e0-123">Егер жобаға жоба тобы әлі де қосылмаған болса, **Microsoft Dynamics 365** қойыншасында **Ресурстар** түймешігін басу арқылы Microsoft Project Client бағдарламасында ресурстарды таңдап, топ құруға болады.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-123">If a project team has not yet been added to the project, you can select resources and build the team within Microsoft Project Client by clicking the **Resources** button on the **Microsoft Dynamics 365** tab.</span></span> 

<span data-ttu-id="2b9e0-124">Келесі деректер Finance бағдарламасына тексеру процесінің бөлігі ретінде қайта синхрондалады:</span><span class="sxs-lookup"><span data-stu-id="2b9e0-124">The following data will be synced back to Finance as part of the check-in process:</span></span>

<span data-ttu-id="2b9e0-125">•   Тапсырма атауы</span><span class="sxs-lookup"><span data-stu-id="2b9e0-125">•   Task name</span></span>

<span data-ttu-id="2b9e0-126">•   Басталу күні</span><span class="sxs-lookup"><span data-stu-id="2b9e0-126">•   Start date</span></span>

<span data-ttu-id="2b9e0-127">•   Аяқталу күні</span><span class="sxs-lookup"><span data-stu-id="2b9e0-127">•   Finish date</span></span>

<span data-ttu-id="2b9e0-128">•   Алдындағы элементтер</span><span class="sxs-lookup"><span data-stu-id="2b9e0-128">•   Predecessors</span></span>

<span data-ttu-id="2b9e0-129">•   Ресурс атаулары</span><span class="sxs-lookup"><span data-stu-id="2b9e0-129">•   Resource names</span></span>

<span data-ttu-id="2b9e0-130">•   Санат</span><span class="sxs-lookup"><span data-stu-id="2b9e0-130">•   Category</span></span>

<span data-ttu-id="2b9e0-131">•   Ресурс санаты</span><span class="sxs-lookup"><span data-stu-id="2b9e0-131">•   Resource category</span></span>

<span data-ttu-id="2b9e0-132">•   Жұмыс сағаттары</span><span class="sxs-lookup"><span data-stu-id="2b9e0-132">•   Work hours</span></span>

<span data-ttu-id="2b9e0-133">•   Ескертулер</span><span class="sxs-lookup"><span data-stu-id="2b9e0-133">•   Notes</span></span>

<span data-ttu-id="2b9e0-134">•   Басымдық</span><span class="sxs-lookup"><span data-stu-id="2b9e0-134">•   Priority</span></span>

> [!NOTE]
> <span data-ttu-id="2b9e0-135">Microsoft Project Client файлына басқа бағандарды қосатын болсаңыз, олар файлға сақталмайды және файл қайта ашылғанда көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-135">If you add any other columns to your Microsoft Project Client file, they will not be saved to the file and will not be displayed when the file is opened again.</span></span>

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="2b9e0-136">Microsoft Project Client бағдарламасы арқылы қолданыстағы жоба үшін жұмысты бөлу құрылымын жасаңыз</span><span class="sxs-lookup"><span data-stu-id="2b9e0-136">Create the work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="2b9e0-137">Microsoft Project Client бағдарламасы арқылы жаңа жұмысты бөлу құрылымын жасау үшін мына қадамдарды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="2b9e0-137">To create a new work breakdown structure using Microsoft Project Client, follow these steps:</span></span>


1.  <span data-ttu-id="2b9e0-138">Microsoft Project Client бағдарламасын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-138">Open Microsoft Project Client.</span></span>

2.  <span data-ttu-id="2b9e0-139">**Microsoft Dynamics 365** қойыншасында **Ашу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-139">On the **Microsoft Dynamics 365** tab, click **Open**.</span></span>

3.  <span data-ttu-id="2b9e0-140">Жобаға арналған **Заңды нысан** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-140">Select the **Legal entity** for the project.</span></span>

4.  <span data-ttu-id="2b9e0-141">**Жоба** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-141">Select the **Project**.</span></span>

5.  <span data-ttu-id="2b9e0-142">**Microsoft Dynamics 365** қойыншасында **Тексеру** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-142">Click **Check out** on the **Microsoft Dynamics 365** tab.</span></span>

6.  <span data-ttu-id="2b9e0-143">Finance бағдарламасына жариялауға дайын болғанда **Microsoft Dynamics 365** қойыншасында **Тексеру** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-143">When ready to publish to Finance, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="2b9e0-144">Microsoft Project Client бағдарламасы арқылы қолданыстағы жоба үшін қолданыстағы жұмысты бөлу құрылымын ауыстырыңыз</span><span class="sxs-lookup"><span data-stu-id="2b9e0-144">Replace the existing work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="2b9e0-145">Microsoft Project Client бағдарламасы арқылы жаңа жұмысты бөлу құрылымын жасап, қолданыстағы жоба үшін қолданыстағы жұмысты бөлу құрылымын ауыстыру үшін мына қадамдарды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="2b9e0-145">To create a new work breakdown structure using Microsoft Project Client and replace an existing work breakdown structure for an existing project, follow these steps:</span></span>

1.  <span data-ttu-id="2b9e0-146">Microsoft Project Client бағдарламасын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-146">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="2b9e0-147">Microsoft Project Client бағдарламасында кесте жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-147">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="2b9e0-148">**Microsoft Dynamics 365** қойыншасында **Өзгертулерді сақтау** > **Қолданыстағы жобаны ауыстыру** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-148">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Replace existing project**.</span></span>

4.  <span data-ttu-id="2b9e0-149">Жобаға арналған **Заңды нысан** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-149">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="2b9e0-150">**Жоба** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-150">Select the **Project**.</span></span>

6.  <span data-ttu-id="2b9e0-151">**OK** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-151">Click **OK**.</span></span>

## <a name="create-a-new-project-from-within-microsoft-project-client"></a><span data-ttu-id="2b9e0-152">Microsoft Project Client бағдарламасында жаңа жоба жасаңыз</span><span class="sxs-lookup"><span data-stu-id="2b9e0-152">Create a new project from within Microsoft Project Client</span></span>


1.  <span data-ttu-id="2b9e0-153">Microsoft Project Client бағдарламасын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-153">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="2b9e0-154">Microsoft Project Client бағдарламасында кесте жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-154">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="2b9e0-155">**Microsoft Dynamics 365** қойыншасында **Өзгертулерді сақтау** > **Жаңа жобаға сақтау** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-155">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Save to new Project**.</span></span>

4.  <span data-ttu-id="2b9e0-156">Жобаға арналған **Заңды нысан** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-156">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="2b9e0-157">Қажет болса, **Жоба идентификаторын** енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-157">Enter the **Project ID**, if necessary.</span></span>

6.  <span data-ttu-id="2b9e0-158">Қажет болса, **Жоба атауын** енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-158">Enter the **Project name**.</span></span>

7.  <span data-ttu-id="2b9e0-159">**Жоба түрі**, **Жоба тобы** және **Жобалық келісім-шарт идентификаторы** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-159">Select the **Project type**, **Project group** and the **Project contract ID**.</span></span> <span data-ttu-id="2b9e0-160">Балама ретінде **Жаңа** опциясын басу арқылы жаңа жобалық келісім-шартты жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-160">Alternatively, you can create a new project contract by clicking **New**.</span></span>

8.  <span data-ttu-id="2b9e0-161">Ресурсқа пайдаланылатын **Күнтізбе** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-161">Select the **Calendar** to be used for resourcing.</span></span>

11. <span data-ttu-id="2b9e0-162">**OK** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b9e0-162">Click **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="2b9e0-163">Project Client қондырмасы жоба идентификаторы пішіміндегі келесі таңбаларға қолдау көрсетпейді:</span><span class="sxs-lookup"><span data-stu-id="2b9e0-163">The Project Client add-in doesn’t support the following characters in the project ID format:</span></span>
> 
>   - <span data-ttu-id="2b9e0-164">Астыңғы сызық</span><span class="sxs-lookup"><span data-stu-id="2b9e0-164">Underscore</span></span>
>   - <span data-ttu-id="2b9e0-165">Кезең</span><span class="sxs-lookup"><span data-stu-id="2b9e0-165">Period</span></span>
>   - <span data-ttu-id="2b9e0-166">Бос орын</span><span class="sxs-lookup"><span data-stu-id="2b9e0-166">Space</span></span>
>   - <span data-ttu-id="2b9e0-167">Қиғаш сызық</span><span class="sxs-lookup"><span data-stu-id="2b9e0-167">Slash</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
