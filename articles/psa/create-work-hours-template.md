---
title: Жұмыс сағаттары үлгісін жасау
description: Project Service жүйесінде жұмыс уақыты үлгісін жасау жолы
author: ruhercul
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
ms.openlocfilehash: c34634817fc8e4c993261024a8b19d45052bf5e5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079670"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="d9dc3-103">Жұмыс сағаттары үлгісін жасау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="d9dc3-103">Create a work hours template (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="d9dc3-104">Жоба кестелерін жасау алдында кестедегі әр күн бойынша жұмыс сағаттары санын анықтайтын жоба күнтізбесін және қызмет есептейтін күндерді орнату керек.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="d9dc3-105">Күнделікті жұмыс сағаттары, демалыс күндері және басқа қызмет етпейтін күндер туралы мәліметтерден тұратын жұмыс сағаттары үлгісімен осыны істеңіз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="d9dc3-106">Жобаны жасау кезінде жоба кестесін қолдану үшін жұмыс үлгісін жоба күнтізбесімен байланыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="d9dc3-107">Жұмыс сағаттары үлгісін жасаудың екі жолы бар:</span><span class="sxs-lookup"><span data-stu-id="d9dc3-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="d9dc3-108">Ресурс күнтізбесі негізінде жұмыс сағаттары үлгісін жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="d9dc3-109">Жаңа жұмыс сағаттары үлгісін жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="d9dc3-110">Ресурс күнтізбесі негізінде жұмыс сағаттары үлгісін жасау үшін</span><span class="sxs-lookup"><span data-stu-id="d9dc3-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="d9dc3-111">**Project Service > Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="d9dc3-112">Жұмыс сағаттары негізделетін ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="d9dc3-113">**Күнтізбені басқаша сақтау** түймешігін басып, жұмыс сағаттары үлгісінің атауын енгізіңіз, содан кейін **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-113">Click **Save Calendar As** , enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="d9dc3-114">Параметрлерді өзгертуді аяқтағаннан кейін **Сақтау және жабу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="d9dc3-115">Экранның астыңғы оң бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="d9dc3-116">Жаңа жұмыс сағаттары үлгісін жасау үшін</span><span class="sxs-lookup"><span data-stu-id="d9dc3-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="d9dc3-117">**Project Service > Жұмыс сағаттары үлгілері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="d9dc3-118">**Жаңа** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="d9dc3-119">Жұмыс сағаттары үлгісінің атауын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="d9dc3-120">Жұмыс сағаттары негізделетін ресурсты таңдап, **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d9dc3-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="d9dc3-121">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="d9dc3-121">See Also</span></span>  
 [<span data-ttu-id="d9dc3-122">Ресурстарды реттеу</span><span class="sxs-lookup"><span data-stu-id="d9dc3-122">Set up resources</span></span>](../psa/set-up-resources.md)
