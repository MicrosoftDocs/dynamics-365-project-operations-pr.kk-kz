---
title: Тапсырыстар және тағайындаулар
description: Бұл тақырыпта ресурстарды резервтеу мен ресурстарды тағайындау арасындағы айырмашылықтар туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8fe6937dfdfe137f28917c16da1d7dc6155284ae
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130225"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="37520-103">Тапсырыстар және тағайындаулар</span><span class="sxs-lookup"><span data-stu-id="37520-103">Bookings vs assignments</span></span>

<span data-ttu-id="37520-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="37520-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="37520-105">Тапсырыстар — жобаға ресурсты түпкілікті немесе алдын ала тағайындау.</span><span class="sxs-lookup"><span data-stu-id="37520-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="37520-106">Қорытынды резервтеулер ресурс сыйымдылығын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="37520-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="37520-107">Тапсырыстар топтар үшін әртүрлі жобалар бойынша ресурстардың қалай тартылатындығын түсіну үшін ұйымдастырушылық тұжырымдамаларды ұсынады.</span><span class="sxs-lookup"><span data-stu-id="37520-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="37520-108">Dynamics 365 Project Operations бағдарламасы тапсырмаларды жоба деңгейіндегі тұжырымдама ретінде қарастырады.</span><span class="sxs-lookup"><span data-stu-id="37520-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="37520-109">Тапсырыстарға қарағанда, тағайындаулар жоба кестесіндегі жоба тапсырмалары үшін ресурстар міндеттемесі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="37520-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="37520-110">Ресурстар аталған немесе жалпы болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="37520-110">The resources can be named or generic.</span></span> 

<span data-ttu-id="37520-111">Әдетте, ресурстарға арналған тапсырыстардың сомасы ресурстардың бір немесе бірнеше тапсырмалар бойынша тағайындауларының сомасына тең болады.</span><span class="sxs-lookup"><span data-stu-id="37520-111">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="37520-112">Дегенмен Project Operations бағдарламасы бұл келісімді қамтамасыз етпейді.</span><span class="sxs-lookup"><span data-stu-id="37520-112">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="37520-113">**Салыстырып тексеру** көрінісі жоба менеджеріне ресурс тапсырыстары мен тағайындаулары келіспейтін жерлерді көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="37520-113">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>
