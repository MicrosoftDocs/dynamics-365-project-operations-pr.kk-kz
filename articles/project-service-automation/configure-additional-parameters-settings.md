---
title: Қосымша параметрді конфигурациялау
description: Project Service жүйесінде қосымша параметрлерді теңшеу жолы
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: de2fe830-4313-4711-b03b-76d56bf56cb6
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: f3e110163088f8e3b78da9f273113d74775bf24c
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753159"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="9cf53-103">Қосымша параметрлерді конфигурациялау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="9cf53-103">Configure additional parameter settings (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="9cf53-104">Алдыңғы бөлімдердегі элементтерді теңшегеннен кейін, жобаларға пайдаланылатын қосымша жоба параметрлерін орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="9cf53-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="9cf53-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметін бірінші рет орнатқан кезде алдымен [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жұмыс істеуі үшін қажетті барлық жазбаларды жасау параметрін жасадыңыз.</span><span class="sxs-lookup"><span data-stu-id="9cf53-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="9cf53-106">Енді оралып, осы параметрлердің қосымша өрістерін конфигурациялау уақыты келді.</span><span class="sxs-lookup"><span data-stu-id="9cf53-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="9cf53-107">Мына параметрлерді теңшеу қажет болады:</span><span class="sxs-lookup"><span data-stu-id="9cf53-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="9cf53-108">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="9cf53-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="9cf53-109">Есеп-шот жиілігі</span><span class="sxs-lookup"><span data-stu-id="9cf53-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="9cf53-110">Жұмыс сағаттары үлгісі</span><span class="sxs-lookup"><span data-stu-id="9cf53-110">Work hours template</span></span>  
  
-   <span data-ttu-id="9cf53-111">Бағатізбе</span><span class="sxs-lookup"><span data-stu-id="9cf53-111">Price list</span></span>  
 
<span data-ttu-id="9cf53-112">Осы қадамда әрі қажетті ресурстың бөліну түрін көрсетесіз:</span><span class="sxs-lookup"><span data-stu-id="9cf53-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="9cf53-113">**Орталық**.</span><span class="sxs-lookup"><span data-stu-id="9cf53-113">**Central**.</span></span> <span data-ttu-id="9cf53-114">Тек ресурс реттеушілері ресурстарды жобаларға бөле алады.</span><span class="sxs-lookup"><span data-stu-id="9cf53-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="9cf53-115">**Гибридті**.</span><span class="sxs-lookup"><span data-stu-id="9cf53-115">**Hybrid**.</span></span> <span data-ttu-id="9cf53-116">Ресурс реттеушілері, жоба реттеушілері және тіркелгі реттеушілері ресурстарды жобаларға бөле алады.</span><span class="sxs-lookup"><span data-stu-id="9cf53-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="9cf53-117">Жоба параметрлерін орнату үшін:</span><span class="sxs-lookup"><span data-stu-id="9cf53-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="9cf53-118">**Project Service > Параметрлер** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="9cf53-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="9cf53-119">Конфигурациялау қажет параметрлерді басыңыз ([!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметін бірінші рет орнатқан кезде жасалған) немесе жаңасын жасау үшін **Жаңа** пәрменін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="9cf53-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="9cf53-120">**Жалпы** аумағында барлық жоба параметрлерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="9cf53-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="9cf53-121">**Бағатізбе** аумағында бағатізбені қосу үшін **+** түймешігін басыңыз, **Жоба параметрінің бағатізбесі** ашылмалы тізімінде бағатізбені таңдап, **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="9cf53-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="9cf53-122">Экранның астыңғы оң бұрышында **Сақтау** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="9cf53-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="9cf53-123">Project Service қызметінің тиісті түрде жұмыс істеуі үшін жоба параметрінің жазбасы жасалуы керек.</span><span class="sxs-lookup"><span data-stu-id="9cf53-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="9cf53-124">Бұл жазба жойылмауы керек.</span><span class="sxs-lookup"><span data-stu-id="9cf53-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="9cf53-125">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="9cf53-125">See Also</span></span>  
 [<span data-ttu-id="9cf53-126">Ресурстарды реттеу</span><span class="sxs-lookup"><span data-stu-id="9cf53-126">Set up resources</span></span>](../project-service/set-up-resources.md)
