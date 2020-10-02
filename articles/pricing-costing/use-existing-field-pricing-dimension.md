---
title: Project Operations өрістері баға өлшемдері ретінде
description: Осы тақырыпта өрістерді Dynamics 365 Project Operations бағдарламасындағы бағалау өлшемдері ретінде пайдалану туралы ақпарат ұсынылған.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
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
ms.openlocfilehash: 3ddf3098e45fdc9b99067b64df05e2adc0b6ad05
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896423"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="cb95c-103">Project Operations өрістері баға өлшемдері ретінде</span><span class="sxs-lookup"><span data-stu-id="cb95c-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="cb95c-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="cb95c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cb95c-105">**Шектеулер** нысанында ресурсқа негізделген бағалау үшін бағалау өлшемдері ретінде пайдалануға болатын көптеген өрістер бар.</span><span class="sxs-lookup"><span data-stu-id="cb95c-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="cb95c-106">Мысалы, бір жалпы өріс **Тапсырыс беруге болатын ресурс**.</span><span class="sxs-lookup"><span data-stu-id="cb95c-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="cb95c-107">Шамамен 20-30 шот ұсынылатын ресурстарға ие кішігірім компаниялар әр ресурсқа тән пайыздық мөлшерлеме мен құн мөлшерлемесін қолдану оңайырақ тәсіл деп табуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="cb95c-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="cb95c-108">Алайда, есеп айырысатын жұмыс күшінің өсуіне байланысты ресурстарға тән мөлшерлемелерді сақтау шындыққа сәйкес келмеуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="cb95c-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="cb95c-109">Ресурс шығыны мен вексель мөлшерлемесі ресурстар ілгері жылжып, көп тәжірибе жинақтағанда немесе басқа дағдыларды игергенде өзгере бастайды.</span><span class="sxs-lookup"><span data-stu-id="cb95c-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="cb95c-110">Тағы бір мысал — транзакция санаты.</span><span class="sxs-lookup"><span data-stu-id="cb95c-110">Another example is that of transaction category.</span></span> <span data-ttu-id="cb95c-111">Тұтынушылар мен ендіру құралдары транзакция санатын жұмысты жіктеу үшін пайдаланды және өрісті жұмыс санатының негізінде баға мен шығынды анықтау үшін пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="cb95c-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>
