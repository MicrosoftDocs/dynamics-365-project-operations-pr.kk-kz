---
title: Project Finder Mobile бағдарламасының мүмкіндіктерін қосу
description: Project Service жүйесіне арналған Project Finder Mobile бағдарламасы мүмкіндіктерін қосу жолы
author: JohnPBurrows
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
ms.openlocfilehash: 749c5682dc2e639843a0a8a085fe8af65502d433
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079667"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a><span data-ttu-id="4d544-103">Project Finder Mobile бағдарламасының мүмкіндіктерін қосу (Project Service)</span><span class="sxs-lookup"><span data-stu-id="4d544-103">Enable Project Finder Mobile app features (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="4d544-104">Жұмыс істейтін жаңа жобаларды іздеу және дағдылар жиынтығын жаңарту үшін ресурстар телефондағы Project Finder Mobile бағдарламасын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесімен пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="4d544-104">Your resources can use the Project Finder Mobile app on their phone with [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to find new projects to work on and update their skill sets.</span></span>  
  
 <span data-ttu-id="4d544-105">Бағдарлама [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] телефондарына және [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)] жүйесіне қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="4d544-105">The app is available for [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] phones, and [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].</span></span>  
  
 <span data-ttu-id="4d544-106">Пайдаланушылардың жоба ресурсының талаптарын қарауы және дағдыларын жаңартуы үшін ұйымдық бірлік параметрлеріндегі екі опцияны орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="4d544-106">You need to set a couple of options in the parameters setting for your organizational unit to allow users to view projects' resource requirements and update their skills.</span></span>  
  
> [!NOTE]
>  <span data-ttu-id="4d544-107">Project Finder Mobile бағдарламасы тек [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] жүйесімен (жергілікті орнатымдармен емес) жұмыс істейді.</span><span class="sxs-lookup"><span data-stu-id="4d544-107">The Project Finder Mobile app only works with [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], not with on-premises installations.</span></span>  
  
1. <span data-ttu-id="4d544-108">**Project Service > Параметрлер** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="4d544-108">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="4d544-109">Project Finder Mobile бағдарламасы мүмкіндіктеріне рұқсат беру үшін пайдаланылатын параметрлерді басыңыз.</span><span class="sxs-lookup"><span data-stu-id="4d544-109">Click the parameters setting you want to use for allowing the Project Finder Mobile app features.</span></span>  
  
3. <span data-ttu-id="4d544-110">**Жалпы** аумағында **Ресурстарға көрінетін ресурс талаптары** параметрін **Иә** мәніне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="4d544-110">In the **General** area, set **Resource requirements visible to resources** to **Yes**.</span></span>  
  
4. <span data-ttu-id="4d544-111">**Ресурс бойынша дағды жаңартуына рұқсат беру** пәрменін **Иә** мәніне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="4d544-111">Set **Allow skill update by resource** to **Yes**.</span></span>  
  
   <span data-ttu-id="4d544-112">![ProjectService_ProjectFinderEnable](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")</span><span class="sxs-lookup"><span data-stu-id="4d544-112">![ProjectService_ProjectFinderEnable](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")</span></span>  
  
   <span data-ttu-id="4d544-113">Бұл глобалдық параметр.</span><span class="sxs-lookup"><span data-stu-id="4d544-113">This is a global setting.</span></span> <span data-ttu-id="4d544-114">Жоба реттеушілері жеке жобаның осы жобаның **Жоба тобы** бетінде көрінуін орната алады.</span><span class="sxs-lookup"><span data-stu-id="4d544-114">Project managers can set whether an individual project will be visible on that project's **Project Team** page.</span></span>  
  
   <span data-ttu-id="4d544-115">![ProjectService_ProjectTeamVisible](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")</span><span class="sxs-lookup"><span data-stu-id="4d544-115">![ProjectService_ProjectTeamVisible](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")</span></span>  
  
## <a name="email-notifications"></a><span data-ttu-id="4d544-116">Электрондық пошта хабарландырулары</span><span class="sxs-lookup"><span data-stu-id="4d544-116">Email notifications</span></span>  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="4d544-117">қызметі мына уақыттарда төмендегі алушыларға ресурс сұрауларына қатысты электрондық хабарлар жібереді:</span><span class="sxs-lookup"><span data-stu-id="4d544-117">sends emails regarding resource requests to the following recipients at the following times:</span></span>  
  
|<span data-ttu-id="4d544-118">Қабылдаушы</span><span class="sxs-lookup"><span data-stu-id="4d544-118">Recipient</span></span>|<span data-ttu-id="4d544-119">Оқиға</span><span class="sxs-lookup"><span data-stu-id="4d544-119">Event</span></span>|  
|---------------|-----------|  
|<span data-ttu-id="4d544-120">Жоба менеджері</span><span class="sxs-lookup"><span data-stu-id="4d544-120">Project manager</span></span>|<span data-ttu-id="4d544-121">-   Ресурс Project Finder Mobile бағдарламасымен жобаға тіркелген кезде.</span><span class="sxs-lookup"><span data-stu-id="4d544-121">-   When a resource signs up for a project with the Project Finder Mobile app.</span></span>|  
|<span data-ttu-id="4d544-122">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4d544-122">Resource</span></span>|<span data-ttu-id="4d544-123">-   Ресурс тіркелген жоба жұмысын басқа ресурс орындаған кезде.</span><span class="sxs-lookup"><span data-stu-id="4d544-123">-   When the project work the resource has signed up for has already been fulfilled by another resource.</span></span><br /><span data-ttu-id="4d544-124">-   Дағдыны бекіту сұрауы бекітілген немесе қабылданбаған кезде.</span><span class="sxs-lookup"><span data-stu-id="4d544-124">-   When their skill approval request has been approved or rejected.</span></span><br /><span data-ttu-id="4d544-125">-   Жобаға тіркелу сұрауы бекітілген немесе қабылданбаған кезде.</span><span class="sxs-lookup"><span data-stu-id="4d544-125">-   When their project sign up request has been approved or rejected.</span></span>|  
  
## <a name="privacy-notice"></a><span data-ttu-id="4d544-126">Құпиялылық ескертпесі</span><span class="sxs-lookup"><span data-stu-id="4d544-126">Privacy notice</span></span>  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a><span data-ttu-id="4d544-127">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="4d544-127">See Also</span></span>  
 [<span data-ttu-id="4d544-128">Ресурстарды реттеу</span><span class="sxs-lookup"><span data-stu-id="4d544-128">Set up resources</span></span>](../psa/set-up-resources.md)
