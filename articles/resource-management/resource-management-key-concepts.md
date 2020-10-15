---
title: Ресурстарды басқарудың негізгі тұжырымдамалары
description: Бұл тақырыпта Microsoft Dynamics Project Operations жүйесіндегі ресурстарды басқару туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 124d9bad5cc0c16955417a8213db047a2d8bae1d
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897548"
---
# <a name="resource-management-key-concepts"></a><span data-ttu-id="352f7-103">Ресурстарды басқарудың негізгі тұжырымдамалары</span><span class="sxs-lookup"><span data-stu-id="352f7-103">Resource management key concepts</span></span>

<span data-ttu-id="352f7-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="352f7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="352f7-105">Ресурстар — қызмет көрсетуге негізделген ұйымдардың ең маңызды активі.</span><span class="sxs-lookup"><span data-stu-id="352f7-105">Resources are the most important asset of a service-based organization.</span></span> <span data-ttu-id="352f7-106">Тиісті уақытта тиісті ресурстарды табу, сол ресурстарды жобаларда тіркеу және оларды пайдалану ұйымға табыс мақсаттарына және тұтынушының қанағаттану мақсаттарына жету үшін көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="352f7-106">The ability to find the right resources at the right time, book those resources on projects and keep them utilized, helps the organization meet revenue targets and customer satisfaction goals.</span></span> <span data-ttu-id="352f7-107">Dynamics 365 Project Operations бағдарламасындағы жобаның ресурстық функцияларын келесі тапсырмаларды орындау үшін пайдалануға болады:</span><span class="sxs-lookup"><span data-stu-id="352f7-107">You can use the project resourcing functionality in Dynamics 365 Project Operations to do the following tasks:</span></span>

- <span data-ttu-id="352f7-108">Қолжетімді және білікті ресурстарға тапсырыс беру арқылы жоба топтарын құру.</span><span class="sxs-lookup"><span data-stu-id="352f7-108">Form project teams by booking available and qualified resources.</span></span>
- <span data-ttu-id="352f7-109">Жалпы топ мүшесі жазбаларын жасау және олардың рөлдері мен ресурс ұйымдық бөлімшесін анықтау.</span><span class="sxs-lookup"><span data-stu-id="352f7-109">Create generic team member records and define their roles and resource organization unit.</span></span>
- <span data-ttu-id="352f7-110">Жалпы топ мүшелері үшін олардың тапсырма тағайындамаларынан ресурс талаптарын құру.</span><span class="sxs-lookup"><span data-stu-id="352f7-110">Generate resource requirements for generic team members from their task assignments.</span></span>
- <span data-ttu-id="352f7-111">Ресурс сұранысындағы дағдыларды анықтау арқылы дағдыларды қолжетімді ресурс дағдыларымен сәйкестендіру.</span><span class="sxs-lookup"><span data-stu-id="352f7-111">Match skills by identifying the skills defined on the resource demand against available resource skills.</span></span>
- <span data-ttu-id="352f7-112">Ресурстардың орнын ауыстыру.</span><span class="sxs-lookup"><span data-stu-id="352f7-112">Substitute resources.</span></span>
- <span data-ttu-id="352f7-113">Жобаның жоспар тағайындамаларын және ресурсқа тапсырыс беру әрекеттерін туралау.</span><span class="sxs-lookup"><span data-stu-id="352f7-113">Align project schedule assignments and resource bookings.</span></span>
- <span data-ttu-id="352f7-114">Тапсырыстар мен тағайындамалардағы өзгешеліктерді салыстырып тексеру.</span><span class="sxs-lookup"><span data-stu-id="352f7-114">Reconcile differences in bookings and assignments.</span></span>
- <span data-ttu-id="352f7-115">"Кеңседе жоқ" күйіне сәйкес ресурсқа тапсырыс беру әрекетін өзгерту.</span><span class="sxs-lookup"><span data-stu-id="352f7-115">Change resource bookings in response to out-of-office status.</span></span>
- <span data-ttu-id="352f7-116">Жоба менеджерлері мен ресурс менеджерлерінің бірлесіп жұмыс істеуі.</span><span class="sxs-lookup"><span data-stu-id="352f7-116">Collaborate between project managers and resource managers.</span></span>
- <span data-ttu-id="352f7-117">Ресурсты мақсатқа сәйкес пайдалану тарихын қарау (оның ішінде ресурстардың уақыты қалай қолданылғанын көрсететін үзілістер).</span><span class="sxs-lookup"><span data-stu-id="352f7-117">View the history of resource utilization against a target, including a breakdown of how the resources' time was utilized.</span></span>
- <span data-ttu-id="352f7-118">Дағдылар және біліктілік репозиторийін жүргізу.</span><span class="sxs-lookup"><span data-stu-id="352f7-118">Maintain a skills and proficiency repository.</span></span>


<span data-ttu-id="352f7-119">Жобаңызды Project Operations жүйесіндегі жалпы немесе атауы бар ресурстар тобымен қамтамасыз ете аласыз.</span><span class="sxs-lookup"><span data-stu-id="352f7-119">You can staff your project with a team of generic or named resources in Project Operations.</span></span> <span data-ttu-id="352f7-120">Топ мүшелерін қосу және тағайындау үшін, сондай-ақ олардың тапсырыстары мен тағайындамаларын басқару үшін әртүрлі әдістерді пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="352f7-120">You can use various methods to add and assign team members and to manage their bookings and assignments.</span></span> 