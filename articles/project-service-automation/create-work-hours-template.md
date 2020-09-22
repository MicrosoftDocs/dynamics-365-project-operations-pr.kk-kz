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
ms.prod: ''
ms.technology: ''
ms.assetid: 1a519487-25f1-4e9d-b739-1c1becf1d649
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5e7ef4af5f22419cccd8f29ea2a0a0a21a75875a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753093"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="1261c-103">Жұмыс сағаттары үлгісін жасау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="1261c-103">Create a work hours template (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="1261c-104">Жоба кестелерін жасау алдында кестедегі әр күн бойынша жұмыс сағаттары санын анықтайтын жоба күнтізбесін және қызмет есептейтін күндерді орнату керек.</span><span class="sxs-lookup"><span data-stu-id="1261c-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="1261c-105">Күнделікті жұмыс сағаттары, демалыс күндері және басқа қызмет етпейтін күндер туралы мәліметтерден тұратын жұмыс сағаттары үлгісімен осыны істеңіз.</span><span class="sxs-lookup"><span data-stu-id="1261c-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="1261c-106">Жобаны жасау кезінде жоба кестесін қолдану үшін жұмыс үлгісін жоба күнтізбесімен байланыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="1261c-107">Жұмыс сағаттары үлгісін жасаудың екі жолы бар:</span><span class="sxs-lookup"><span data-stu-id="1261c-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="1261c-108">Ресурс күнтізбесі негізінде жұмыс сағаттары үлгісін жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="1261c-109">Жаңа жұмыс сағаттары үлгісін жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="1261c-110">Ресурс күнтізбесі негізінде жұмыс сағаттары үлгісін жасау үшін</span><span class="sxs-lookup"><span data-stu-id="1261c-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="1261c-111">**Project Service > Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="1261c-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="1261c-112">Жұмыс сағаттары негізделетін ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="1261c-113">**Күнтізбені басқаша сақтау** түймешігін басып, жұмыс сағаттары үлгісінің атауын енгізіңіз, содан кейін **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="1261c-114">Параметрлерді өзгертуді аяқтағаннан кейін **Сақтау және жабу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="1261c-115">Экранның астыңғы оң бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="1261c-116">Жаңа жұмыс сағаттары үлгісін жасау үшін</span><span class="sxs-lookup"><span data-stu-id="1261c-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="1261c-117">**Project Service > Жұмыс сағаттары үлгілері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="1261c-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="1261c-118">**Жаңа** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="1261c-119">Жұмыс сағаттары үлгісінің атауын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="1261c-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="1261c-120">Жұмыс сағаттары негізделетін ресурсты таңдап, **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="1261c-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="1261c-121">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="1261c-121">See Also</span></span>  
 [<span data-ttu-id="1261c-122">Ресурстарды реттеу</span><span class="sxs-lookup"><span data-stu-id="1261c-122">Set up resources</span></span>](../project-service/set-up-resources.md)
