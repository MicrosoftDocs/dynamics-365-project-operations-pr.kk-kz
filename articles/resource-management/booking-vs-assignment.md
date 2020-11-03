---
title: Тапсырыстар және тағайындаулар
description: Бұл тақырыпта ресурстарды резервтеу мен ресурстарды тағайындау арасындағы айырмашылықтар туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fa99783e52dbcdeaf80bbfd03df0f458f86b5e99
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079509"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="dd5a9-103">Тапсырыстар және тағайындаулар</span><span class="sxs-lookup"><span data-stu-id="dd5a9-103">Bookings vs assignments</span></span>

<span data-ttu-id="dd5a9-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="dd5a9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="dd5a9-105">Тапсырыстар — жобаға ресурсты түпкілікті немесе алдын ала тағайындау.</span><span class="sxs-lookup"><span data-stu-id="dd5a9-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="dd5a9-106">Қорытынды резервтеулер ресурс сыйымдылығын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="dd5a9-106">Hard bookings consume a resource's capacity.</span></span> 

<span data-ttu-id="dd5a9-107">Тағайындаулар — жоба кестесіндегі жоба тапсырмаларына ресурстарды тағайындау.</span><span class="sxs-lookup"><span data-stu-id="dd5a9-107">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="dd5a9-108">Ресурстар нақты немесе жалпы болады.</span><span class="sxs-lookup"><span data-stu-id="dd5a9-108">The resources can be real or generic.</span></span> 

<span data-ttu-id="dd5a9-109">Ең дұрысы, нақты ресурстар үшін тапсырмалар мен тағайындаулар келісілуі керек, себебі олар бір-бірінен ерекшеленбейді.</span><span class="sxs-lookup"><span data-stu-id="dd5a9-109">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="dd5a9-110">Дегенмен Microsoft Dynamics Project Operations жүйесі бұл келісімді қамтамасыз етпейді.</span><span class="sxs-lookup"><span data-stu-id="dd5a9-110">However, Microsoft Dynamics Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="dd5a9-111">**Салыстырып тексеру** көрінісі жоба менеджеріне ресурстың тапсырыстары мен тағайындаулары келіспейтін жерлерді көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="dd5a9-111">The **Reconciliation** view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>
