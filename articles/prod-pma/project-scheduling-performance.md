---
title: Жоба ресурстарын жоспарлау өнімділігі
description: Бұл тақырыпта көптеген жобалар үшін ресурсты жоспарлау өнімділігін жақсарту туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: c3f219ce0635545976a6a4639233f166e18468af
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079643"
---
# <a name="project-resource-scheduling-performance"></a><span data-ttu-id="e922f-103">Жоба ресурстарын жоспарлау өнімділігі</span><span class="sxs-lookup"><span data-stu-id="e922f-103">Project resource scheduling performance</span></span>

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


<span data-ttu-id="e922f-104">Ресурсты жоспарлауға қатысты өнімділік мәселелері жобалар саны мыңға жеткенде пайда болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e922f-104">Performance issues related to resource scheduling can occur when the number of projects reaches into the thousands.</span></span> <span data-ttu-id="e922f-105">Ресурсты жоспарлау өнімділігін жақсарту үшін пайдаланушыларға ресурстың қолжетімділік пішінін іске қосуға кететін уақытты қысқартуға мүмкіндік беретін мүмкіндік бар.</span><span class="sxs-lookup"><span data-stu-id="e922f-105">To improve resource scheduling performance, a feature is available that allows users to reduce the time that it takes to launch the resource availability form.</span></span> <span data-ttu-id="e922f-106">Нақтырақ айтқанда, бұл ресурс мүмкіндігін синхрондау процесін жояды және **ResProjectResource** кестесін ресурстарды іздеуді жылдамдату үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e922f-106">Specifically, this removes the resource capacity roll-up synchronization process and uses the **ResProjectResource** table to speed up the resource lookup.</span></span> <span data-ttu-id="e922f-107">**ResRollup** кестесінің бұдан былай пайдаланылмайтынын ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="e922f-107">Note that the **ResRollup** table will no longer be used.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e922f-108">Егер ресурстар мүмкіндігі жыймаларын синхрондау процесіне немесе **ResProjectResource** кестесіне тәуелділік болса, бұл мүмкіндікті пайдаланбаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-108">If there is a dependency on either the resource capacity roll-up synchronization process or the **ResProjectResource** table, do not use this feature.</span></span>

## <a name="enable-resource-scheduling-performance-enhancement"></a><span data-ttu-id="e922f-109">Ресурстарды жоспарлау өнімділігін жақсарту мүмкіндігін қосу</span><span class="sxs-lookup"><span data-stu-id="e922f-109">Enable resource scheduling performance enhancement</span></span>
<span data-ttu-id="e922f-110">Ресурстарды жоспарлау өнімділігін жақсарту мүмкіндігін қосу үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-110">To enable resource scheduling performance enhancement, complete the following steps.</span></span>

1. <span data-ttu-id="e922f-111">**Мүмкіндіктерді басқару** > **Барлығы** тармағына өтіп, мүмкіндіктер тізімінен **Жоба ресурстарын жоспарлау өнімділігін жақсарту мүмкіндігін қосу** параметрін табыңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-111">Go to **Feature management** > **All** , and in the feature list, locate **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="e922f-112">**Қазір қосу** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-112">Select **Enable now**.</span></span>

> [!NOTE]
> <span data-ttu-id="e922f-113">Егер мүмкіндікті тізімнен таба алмасаңыз, тізімді жаңарту үшін **Жаңартуларды тексеру** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-113">If you can't find the feature in the list, select **Check for updates** to refresh the list.</span></span>

3. <span data-ttu-id="e922f-114">Браузерді жаңартыңыз, содан кейін **Жобаларды басқару және есепке алу** > **Мерзімді** > **Жоба ресурстары** > **Барлық компаниялардағы ресурстың күнтізбелер мүмкіндігін синхрондау** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="e922f-114">Refresh your browser, and then go to **Project management and accounting** > **Periodic** > **Project resources** > **Synchronize resource calendars capacity across all companies**.</span></span>
4. <span data-ttu-id="e922f-115">Алдыңғы деректерді жою үшін **Бұрыннан бар мүмкіндік жазбаларын жою** параметрін **Иә** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-115">Set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="e922f-116">Қосымша деректер жасау керек болса, оны **Жоқ** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-116">If you want generate incremental data, set it to **No**.</span></span>
5. <span data-ttu-id="e922f-117">**Кезең коды** өрісінде деректер жасалуы керек кезеңді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-117">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="e922f-118">Егер кезең кодын таңдасаңыз, басталу мен аяқталу күнін анықтаудың қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="e922f-118">If you select a period code, a start and end date do not need to be defined.</span></span>
6. <span data-ttu-id="e922f-119">**Кезең коды** өрісін бос қалдырсаңыз, деректерді құру үшін нақты басталу және аяқталу күндерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-119">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
7. <span data-ttu-id="e922f-120">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-120">Select **OK**.</span></span>

 > [!NOTE]
 > <span data-ttu-id="e922f-121">Бұл жалпы деректерді ұйымыңыздағы барлық компаниялар бойынша **ResCalendarCapacity** кестесіне таратады, сондықтан топтық тапсырма тек бір заңды нысанда жүргізілуі керек.</span><span class="sxs-lookup"><span data-stu-id="e922f-121">This will distribute general data to the **ResCalendarCapacity** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="e922f-122">Осы топтық тапсырмадағы деректер байланысты күнтізбе арқылы ресурстар мүмкіндігін есептеу үшін қажет.</span><span class="sxs-lookup"><span data-stu-id="e922f-122">The data in this batch job is needed to calculate resource capacity through the associated calendar.</span></span>

8. <span data-ttu-id="e922f-123">**Жобаларды басқару және есепке алу** > **Мерзімді** > **Жоба ресурстары** > **Барлық компаниялардағы жоба ресурстарын толтыру** тармағына өтіп, **OK** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-123">Go to **Project management and accounting** > **Periodic** > **Project resources** > **Populate project resources across all companies** and then select **OK**.</span></span> <span data-ttu-id="e922f-124">Бұл **ResProjectResource** , **ResCalendarDateTimeRange** және **ResEffectiveDateTimeRange** кестелеріндегі жалпы деректерге арналған деректерді жаңарту сценарийі.</span><span class="sxs-lookup"><span data-stu-id="e922f-124">This is the data upgrade script for general data in the **ResProjectResource** , **ResCalendarDateTimeRange** , and **ResEffectiveDateTimeRange** tables.</span></span> <span data-ttu-id="e922f-125">**PSAPRojSchedRole.RootActivity** өрісіне арналған мәндер де жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="e922f-125">Values for the **PSAPRojSchedRole.RootActivity** field are also updated.</span></span> <span data-ttu-id="e922f-126">Егер бұл іске қосылмаған болса, сіз ресурстарды жоспарлау операцияларын орындау кезінде ескерту аласыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-126">If this is not run, you will receive a warning when you try to execute resource scheduling operations.</span></span>
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a><span data-ttu-id="e922f-127">Ресурстарды жоспарлау өнімділігін жақсарту мүмкіндігін өшіру</span><span class="sxs-lookup"><span data-stu-id="e922f-127">Turn off resource scheduling performance enhancement</span></span>

1. <span data-ttu-id="e922f-128">**Мүмкіндіктерді басқару** > **Барлығы** тармағына өтіп, **Жоба ресурстарын жоспарлау өнімділігін жақсарту мүмкіндігін қосу** параметрін іздеңіз.</span><span class="sxs-lookup"><span data-stu-id="e922f-128">Go to **Feature management** > **All**  and search for **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="e922f-129">Функцияны таңдаңыз, содан кейін **Өшіру** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-129">Select the feature, and then select the **Disable** button.</span></span>
3. <span data-ttu-id="e922f-130">Браузерді жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-130">Refresh your browser.</span></span>
4. <span data-ttu-id="e922f-131">**Жобаларды басқару және есепке алу** > **Мерзімді** > **Мүмкіндікті синхрондау** > **Ресурс мүмкіндігі жыймаларын синхрондау** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="e922f-131">Go to **Project management and accounting** > **Periodic** > **Capacity synchronization** > **Synchronize resource capacity roll-ups**.</span></span>
5. <span data-ttu-id="e922f-132">**Мүмкіндік жыймаларын синхрондау** бетінде, алдыңғы деректерді жою үшін **Бұрыннан бар мүмкіндік жазбаларын жою** параметрін **Иә** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-132">On the **Capacity roll-up synchronization** page, set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="e922f-133">Қосымша деректер жасау керек болса, оны **Жоқ** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-133">If you want to generate incremental data, set it to **No**.</span></span>
6. <span data-ttu-id="e922f-134">**Кезең коды** өрісінде деректер жасалуы керек кезеңді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-134">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="e922f-135">Егер кезең кодын таңдасаңыз, басталу мен аяқталу күнін анықтаудың қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="e922f-135">If you select a period code, a start and end date do not need to be defined.</span></span>
7. <span data-ttu-id="e922f-136">**Кезең коды** өрісін бос қалдырсаңыз, деректерді құру үшін нақты басталу және аяқталу күндерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-136">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
8. <span data-ttu-id="e922f-137">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e922f-137">Select **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="e922f-138">Бұл жалпы деректерді ұйымыңыздағы барлық компаниялар бойынша **ResRollup** кестесіне таратады, сондықтан топтық тапсырма тек бір заңды нысанда жүргізілуі керек.</span><span class="sxs-lookup"><span data-stu-id="e922f-138">This will distribute general data to the **ResRollup** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="e922f-139">Бұл топтық тапсырма барлық **Ресурс қолжетімділігі** көріністеріне қажет.</span><span class="sxs-lookup"><span data-stu-id="e922f-139">This batch job is needed for all **Resource Availability** views.</span></span> <span data-ttu-id="e922f-140">Егер бұл топтық тапсырма жүргізілмесе, **ResRollup** деректері ұшу кезінде пайда болады, бұл уақытты алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="e922f-140">If this batch job is not run, the **ResRollup** data will be generated on the fly, which can take time.</span></span>
