---
title: Тапсырыстар және тағайындаулар
description: Бұл тақырыпта ресурстарды резервтеу мен ресурстарды тағайындау арасындағы айырмашылықтар туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 01/08/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 9e346766e6ccbb3dff59ef12072a1cd63f1e4231
ms.sourcegitcommit: 260ce052fed760bb44c514517806049ca13a5459
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 01/08/2021
ms.locfileid: "4841179"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="32b3a-103">Тапсырыстар және тағайындаулар</span><span class="sxs-lookup"><span data-stu-id="32b3a-103">Bookings vs assignments</span></span>

<span data-ttu-id="32b3a-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="32b3a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="32b3a-105">Тапсырыстар — жобаға ресурсты түпкілікті немесе алдын ала тағайындау.</span><span class="sxs-lookup"><span data-stu-id="32b3a-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="32b3a-106">Қорытынды резервтеулер ресурс сыйымдылығын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="32b3a-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="32b3a-107">Тапсырыстар топтар үшін әртүрлі жобалар бойынша ресурстардың қалай тартылатындығын түсіну үшін ұйымдастырушылық тұжырымдамаларды ұсынады.</span><span class="sxs-lookup"><span data-stu-id="32b3a-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="32b3a-108">Dynamics 365 Project Operations бағдарламасы тапсырыстарды жоба деңгейіндегі тұжырымдама ретінде қарастырады.</span><span class="sxs-lookup"><span data-stu-id="32b3a-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="32b3a-109">Тапсырыстарға қарағанда, тағайындаулар жоба кестесіндегі жоба тапсырмалары үшін ресурстар міндеттемесі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="32b3a-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="32b3a-110">Ресурстар аталған немесе жалпы болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="32b3a-110">The resources can be named or generic.</span></span>  <span data-ttu-id="32b3a-111">Ресурс талабы жобалық тапсырма тағайындауларынан алынған кезде, Project Operations бағдарламасы ресурс талабы деректерінің контурын құру үшін ресурстар тағайындамасының талпыныс контурларын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="32b3a-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="32b3a-112">Дегенмен ресурс тағайындаулары анықтамасы сақталмайды.</span><span class="sxs-lookup"><span data-stu-id="32b3a-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="32b3a-113">Ресурс талабынан алынған тапсырыстардың жаңартулары кез келген ресурс тағайындауларын жаңартпайды.</span><span class="sxs-lookup"><span data-stu-id="32b3a-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="32b3a-114">Әдетте, ресурстарға арналған тапсырыстардың сомасы ресурстардың бір немесе бірнеше тапсырмалар бойынша тағайындауларының сомасына тең болады.</span><span class="sxs-lookup"><span data-stu-id="32b3a-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="32b3a-115">Дегенмен Project Operations бағдарламасы бұл келісімді қамтамасыз етпейді.</span><span class="sxs-lookup"><span data-stu-id="32b3a-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="32b3a-116">**Салыстырып тексеру** көрінісі жоба менеджеріне ресурс тапсырыстары мен тағайындаулары келіспейтін жерлерді көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="32b3a-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>


