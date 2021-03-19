---
title: Аяқтау кезіндегі болжамды жаңарту
description: Осы тақырып жоба бойынша ықпал ету проекциясын жаңарту туралы ақпаратты ұсынады.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 0e63bdb815a6f758c57d055c8c03d92e04700445
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286435"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="7fef2-103">Аяқтау кезіндегі болжамды жаңарту</span><span class="sxs-lookup"><span data-stu-id="7fef2-103">Update estimate at completion</span></span>

<span data-ttu-id="7fef2-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="7fef2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7fef2-105">Жоба менеджері үшін тапсырманың бастапқы болжамдарын қайта қарау әдеттегідей болады.</span><span class="sxs-lookup"><span data-stu-id="7fef2-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="7fef2-106">Жобаның қайта болжаулары – бұл жобаның қазіргі күйін ескере отырып, жоба менеджерінің бағалауды қабылдауы.</span><span class="sxs-lookup"><span data-stu-id="7fef2-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="7fef2-107">Алайда, біз жоба менеджерлеріне бастапқы сандарды өзгертуге кеңес бермейміз, себебі жобаның бастапқы мәні жоба кестесі мен құн болжамы үшін шындықтың бекітілген көзі болып табылады және барлық мүдделі тараптар бұған келіскен.</span><span class="sxs-lookup"><span data-stu-id="7fef2-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="7fef2-108">Жоба менеджері үшін тапсырмалар бойынша талпынысты қайта жобалаудың екі жолы бар:</span><span class="sxs-lookup"><span data-stu-id="7fef2-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="7fef2-109">Әдепкі бағалауды жоба бойынша қалған нақты әрекетті жаңа бағалаумен аяқтау (ETC) үшін ауыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="7fef2-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="7fef2-110">Тапсырма бойынша нақты орындалу барысының жаңа болжамын әдепкі орындалу барысының пайызымен ауыстыру.</span><span class="sxs-lookup"><span data-stu-id="7fef2-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="7fef2-111">Осы әдістердің әрбірі тапсырманың ETC, аяқтау кезінде бағалау (ЕАС) және прогресс пайызы, тапсырма бойынша жобаланған әрекет ауытқуын қайта есептеуге әкеледі.</span><span class="sxs-lookup"><span data-stu-id="7fef2-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="7fef2-112">Қорытынды тапсырмалар бойынша ЕАС, ЕТС және прогресс пайызы қайта есептеледі және әрекет ауытқуының жаңа проекциясын шығарады.</span><span class="sxs-lookup"><span data-stu-id="7fef2-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]