---
title: Project Service Automation бағдарламасының 3.x нұсқасының 1-толқынындағы (2020) жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 3 нұсқасының 1-толқынындағы (2020) жаңалықтар мен өзгерістер туралы ақпарат беріледі.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/15/2020
ms.topic: article
author: stsporen
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 16b51995f863d9ee54172625dacbf081c51c8556
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079606"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="8de41-103">Project Service Automation бағдарламасының 3 нұсқасының 1-толқынындағы (2020) жаңалықтар немесе өзгерістер</span><span class="sxs-lookup"><span data-stu-id="8de41-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>
<span data-ttu-id="8de41-104">Бұл тақырып Project Service Automation (PSA) бағдарламасының 3.x нұсқасының 1-толқынындағы (2020) соңғы шығарылымына көшу кезіндегі негізгі жаңарту мәселелеріне назар аударады.</span><span class="sxs-lookup"><span data-stu-id="8de41-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="8de41-105">Уақыт жазбасы</span><span class="sxs-lookup"><span data-stu-id="8de41-105">Time entry</span></span>
<span data-ttu-id="8de41-106">Уақытты енгізу тәжірибесі тұтынушылардың көп сценарийлеріне уақытты енгізуді ұзартуға мүмкіндік беру үшін кеңейтілген.</span><span class="sxs-lookup"><span data-stu-id="8de41-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="8de41-107">Бұл **Уақыт көзі** ретінде көрсетілетін және **Уақыт жазбасының параметрлері** деп аталатын өріс схемасына негізделген нақты әрекетті басқаратын жазба түрлерін қосу мүмкіндігін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="8de41-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings** , displayed as **Time Source**.</span></span> <span data-ttu-id="8de41-108">Осы функционалдыққа қолдау көрсету үшін «Уақыт», «Шығыс», «Күй» және «Растаулар» (TESA) деп аталатын жаңа шешім қосылды.</span><span class="sxs-lookup"><span data-stu-id="8de41-108">A new solution, called Time, Expense, Statusing, and Approvals (TESA) has been added to support this functionality.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="8de41-109">Ұсынысты жетілдіру</span><span class="sxs-lookup"><span data-stu-id="8de41-109">Upgrade consideration</span></span>
<span data-ttu-id="8de41-110">Бұл функцияны қолдау үшін, PSA құрамындағы рөлдер жаңа артықшылықтарды қамту үшін жаңартылды.</span><span class="sxs-lookup"><span data-stu-id="8de41-110">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="8de41-111">Бұл артықшылықтар **Уақыт жазбасының параметрлері** деген жаңа нысанға оқу қатынасы құқығын береді.</span><span class="sxs-lookup"><span data-stu-id="8de41-111">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="8de41-112">Уақытты тіркеу мүмкіндігін талап ететін пайдаланушыларға бар рөлдерге қосымша ретінде **Уақыт жазбасының пайдаланушысы** пайдаланушы рөлі берілуі керек.</span><span class="sxs-lookup"><span data-stu-id="8de41-112">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="8de41-113">Бұл рөл жаңа функцияны қамтиды және уақыт жазбасының жұмысын жалғастырады.</span><span class="sxs-lookup"><span data-stu-id="8de41-113">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

<span data-ttu-id="8de41-114">Сонымен қоса, уақыт жазбасы нысаны үшін барлық пішіндерді қамтитын қандай да бір реттелмелі бағдарлама модульдері болса, модульден **TESA уақыт жазбасының жылдам жасау пішінін** жою қажет болады.</span><span class="sxs-lookup"><span data-stu-id="8de41-114">Additionally, if you have any custom app modules that include all forms for the time entry entity, you will be required to remove the **TESA time Entry Quick Create Form** from the module.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="8de41-115">Қазіргі уақытта ұзартылған уақыт жазбасы өзгертілуде</span><span class="sxs-lookup"><span data-stu-id="8de41-115">Currently extended time entry changes</span></span>
<span data-ttu-id="8de41-116">Уақыт жазбасының қазіргі пайдаланушыларына әсерін азайту үшін, бұл рөлді өзгерту уақытты енгізуді пайдалануды жалғастыру үшін қажет жалғыз қажеттілік болып табылады.</span><span class="sxs-lookup"><span data-stu-id="8de41-116">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="8de41-117">Егер сіз жеке көріністеріңізді немесе жеке уақыт жазбасының тәжірибелерін жасасаңыз, онда **Уақыт жазбасының параметрі** өрістерін дұрыс PSA мәніне орнатуыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="8de41-117">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>