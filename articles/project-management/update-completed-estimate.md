---
title: Аяқтау кезіндегі болжамды жаңарту
description: Осы тақырып жоба бойынша ықпал ету проекциясын жаңарту туралы ақпаратты ұсынады.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 42824cc4cfc2b934f69d319944fe7ee43183955c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897773"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="86f2c-103">Аяқтау кезіндегі болжамды жаңарту</span><span class="sxs-lookup"><span data-stu-id="86f2c-103">Update estimate at completion</span></span>

<span data-ttu-id="86f2c-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="86f2c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="86f2c-105">Жоба менеджері үшін тапсырманың бастапқы болжамдарын қайта қарау әдеттегідей болады.</span><span class="sxs-lookup"><span data-stu-id="86f2c-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="86f2c-106">Жобаның қайта болжаулары – бұл жобаның қазіргі күйін ескере отырып, жоба менеджерінің бағалауды қабылдауы.</span><span class="sxs-lookup"><span data-stu-id="86f2c-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="86f2c-107">Алайда, біз жоба менеджерлеріне бастапқы сандарды өзгертуге кеңес бермейміз, себебі жобаның бастапқы мәні жоба кестесі мен құн болжамы үшін шындықтың бекітілген көзі болып табылады және барлық мүдделі тараптар бұған келіскен.</span><span class="sxs-lookup"><span data-stu-id="86f2c-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="86f2c-108">Жоба менеджері үшін тапсырмалар бойынша талпынысты қайта жобалаудың екі жолы бар:</span><span class="sxs-lookup"><span data-stu-id="86f2c-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="86f2c-109">Әдепкі бағалауды жоба бойынша қалған нақты әрекетті жаңа бағалаумен аяқтау (ETC) үшін ауыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="86f2c-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="86f2c-110">Тапсырма бойынша нақты орындалу барысының жаңа болжамын әдепкі орындалу барысының пайызымен ауыстыру.</span><span class="sxs-lookup"><span data-stu-id="86f2c-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="86f2c-111">Осы әдістердің әрбірі тапсырманың ETC, аяқтау кезінде бағалау (ЕАС) және прогресс пайызы, тапсырма бойынша жобаланған әрекет ауытқуын қайта есептеуге әкеледі.</span><span class="sxs-lookup"><span data-stu-id="86f2c-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="86f2c-112">Қорытынды тапсырмалар бойынша ЕАС, ЕТС және прогресс пайызы қайта есептеледі және әрекет ауытқуының жаңа проекциясын шығарады.</span><span class="sxs-lookup"><span data-stu-id="86f2c-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>
