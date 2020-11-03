---
title: Project Service бағдарламасындағы бұрыннан бар өрісті бағалар өлшемі ретінде пайдалану
description: Бұл тақырыпта Project Service бағдарламасының бұрыннан бар өрістерін бағалар өлшемі ретінде пайдалану туралы ақпарат берілген.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 415e346f88e60cb064f3327bfb35e21bd1c89014
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079738"
---
# <a name="use-an-existing-field-in-project-service-as-a-pricing-dimension"></a><span data-ttu-id="cd0d9-103">Project Service бағдарламасындағы бұрыннан бар өрісті бағалар өлшемі ретінде пайдалану</span><span class="sxs-lookup"><span data-stu-id="cd0d9-103">Use an existing field in Project Service as a pricing dimension</span></span>

<span data-ttu-id="cd0d9-104">Project Service Automation (PSA) бағдарламасында **Нақты көрсеткіштер** нысанында жоба ұйымдарындағы ресурсқа негізделген бағаға арналған бағалар өлшемі ретінде пайдалануға болатын өрістер бар.</span><span class="sxs-lookup"><span data-stu-id="cd0d9-104">Project Service Automation (PSA) has many fields on the **Actuals** entity that can be used as pricing dimensions for resource-based pricing in project organizations.</span></span> <span data-ttu-id="cd0d9-105">Мысалы, бір жалпы өріс **Тапсырыс беруге болатын ресурс**.</span><span class="sxs-lookup"><span data-stu-id="cd0d9-105">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="cd0d9-106">Шамамен 20-30 шот ұсынылатын ресурстарға ие кішігірім компаниялар әр ресурсқа тән пайыздық мөлшерлеме мен құн мөлшерлемесін қолдану оңайырақ тәсіл деп табуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="cd0d9-106">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="cd0d9-107">Алайда, ақылы жұмыс күші өскен сайын, ресурстар жұмыста ілгерілегенге, қосымша тәжірибе жинағанына немесе басқа дағдыларды үйренуіне байланысты ресурс құны мен құн мөлшерлемесі өзгере бастайтындықтан оны сақтап тұру мүмкін емес болады.</span><span class="sxs-lookup"><span data-stu-id="cd0d9-107">However, as the billable workforce grows, this could become unrealistic to maintain as resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different skill sets.</span></span> <span data-ttu-id="cd0d9-108">Бұл тәсіл Project Service бағдарламасының бұрыннан бар өрісін бағалар өлшемі ретінде пайдалануды түсіну үшін, әлі де белгілі бір көлемдегі компаниялар үшін жұмыс істейді, [Тапсырыс беруге болатын ресурстарды бағалар өлшемі ретінде пайдалану](bookable-resource-pricing-dimension.md) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="cd0d9-108">Because this approach still works for companies of a certain size, see the topic, [Use a bookable resource as a pricing dimension](bookable-resource-pricing-dimension.md) to understand how an existing Project Service field can be used as a pricing dimension.</span></span>

<span data-ttu-id="cd0d9-109">Тағы бір мысал — транзакция санаты.</span><span class="sxs-lookup"><span data-stu-id="cd0d9-109">Another example is that of transaction category.</span></span> <span data-ttu-id="cd0d9-110">Тұтынушылар мен ендірушілер PSA жүйесіндегі транзакция санатын жұмысты жіктеу және баға мен құн өрісін жұмыстың санаты негізінде пайдалану үшін қолданды.</span><span class="sxs-lookup"><span data-stu-id="cd0d9-110">Customers and Implementers have used the transaction category in PSA to classify work and use the field to price and cost based on the category of work.</span></span> <span data-ttu-id="cd0d9-111">Қосымша ақпарат алу үшін, [Транзакция санатын бағалар өлшемі ретінде пайдалану](transaction-category-pricing-dimension.md) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="cd0d9-111">For more information, see [Use transaction category as a pricing dimension](transaction-category-pricing-dimension.md).</span></span>
