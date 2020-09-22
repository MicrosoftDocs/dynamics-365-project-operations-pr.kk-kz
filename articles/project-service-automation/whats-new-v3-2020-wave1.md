---
title: Project Service Automation бағдарламасының 3.x нұсқасының 1-толқынындағы (2020) жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 3 нұсқасының 1-толқынындағы (2020) жаңалықтар мен өзгерістер туралы ақпарат беріледі.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 01/24/2020
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x wave 1 2020
author: stsporen
ms.assetid: 48b408c1-11e7-4005-abac-8fd7c0b064b1
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 478080c0570b71188c9f1e12b18b5aadc13903e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753061"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="d71e8-103">Project Service Automation бағдарламасының 3 нұсқасының 1-толқынындағы (2020) жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="d71e8-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>
<span data-ttu-id="d71e8-104">Бұл тақырып Project Service Automation (PSA) бағдарламасының 3.x нұсқасының 1-толқынындағы (2020) соңғы шығарылымына көшу кезіндегі негізгі жаңарту мәселелеріне назар аударады.</span><span class="sxs-lookup"><span data-stu-id="d71e8-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="d71e8-105">Уақыт жазбасы</span><span class="sxs-lookup"><span data-stu-id="d71e8-105">Time entry</span></span>
<span data-ttu-id="d71e8-106">Уақытты енгізу тәжірибесі тұтынушылардың көп сценарийлеріне уақытты енгізуді ұзартуға мүмкіндік беру үшін кеңейтілген.</span><span class="sxs-lookup"><span data-stu-id="d71e8-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="d71e8-107">Бұл **Уақыт көзі** ретінде көрсетілетін және **Уақыт жазбасының параметрлері** деп аталатын өріс схемасына негізделген нақты әрекетті басқаратын жазба түрлерін қосу мүмкіндігін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="d71e8-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings**, displayed as **Time Source**.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="d71e8-108">Ұсынысты жетілдіру</span><span class="sxs-lookup"><span data-stu-id="d71e8-108">Upgrade consideration</span></span>
<span data-ttu-id="d71e8-109">Бұл функцияны қолдау үшін, PSA құрамындағы рөлдер жаңа артықшылықтарды қамту үшін жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="d71e8-109">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="d71e8-110">Бұл артықшылықтар **Уақыт жазбасының параметрлері** деген жаңа нысанға оқу қатынасы құқығын береді.</span><span class="sxs-lookup"><span data-stu-id="d71e8-110">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="d71e8-111">Уақытты тіркеу мүмкіндігін талап ететін пайдаланушыларға бар рөлдерге қосымша ретінде **Уақыт жазбасының пайдаланушысы** пайдаланушы рөлі берілуі керек.</span><span class="sxs-lookup"><span data-stu-id="d71e8-111">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="d71e8-112">Бұл рөл жаңа функцияны қамтиды және уақыт жазбасының жұмысын жалғастырады.</span><span class="sxs-lookup"><span data-stu-id="d71e8-112">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="d71e8-113">Қазіргі уақытта ұзартылған уақыт жазбасы өзгертілуде</span><span class="sxs-lookup"><span data-stu-id="d71e8-113">Currently extended time entry changes</span></span>
<span data-ttu-id="d71e8-114">Уақыт жазбасының қазіргі пайдаланушыларына әсерін азайту үшін, бұл рөлді өзгерту уақытты енгізуді пайдалануды жалғастыру үшін қажет жалғыз қажеттілік болып табылады.</span><span class="sxs-lookup"><span data-stu-id="d71e8-114">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="d71e8-115">Егер сіз жеке көріністеріңізді немесе жеке уақыт жазбасының тәжірибелерін жасасаңыз, онда **Уақыт жазбасының параметрі** өрістерін дұрыс PSA мәніне орнатуыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="d71e8-115">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>
