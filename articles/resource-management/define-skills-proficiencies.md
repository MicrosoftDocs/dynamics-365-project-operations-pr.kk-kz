---
title: Қабілеттер мен тиімділіктерді анықтау
description: Осы тақырып бағалау ресурстарды бағалау үшін тиімділік үлгілерін орнату әдісі туралы ақпаратты ұсынады.
author: ruhercul
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 982f64677b74f2195eacc287fc07b80c34f7acc0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6015338"
---
# <a name="define-skills-and-proficiencies"></a><span data-ttu-id="4e2aa-103">Қабілеттер мен тиімділіктерді анықтау</span><span class="sxs-lookup"><span data-stu-id="4e2aa-103">Define skills and proficiencies</span></span>

<span data-ttu-id="4e2aa-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="4e2aa-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4e2aa-105">Дағдылар — Dynamics 365 Project Operations бағдарламасы мен егер бар болса, Dynamics 365 Field Service бағдарламасының арасында ортақ пайдаланылатын ресурс сипаттамалары.</span><span class="sxs-lookup"><span data-stu-id="4e2aa-105">Skills are resource characteristics that are shared between Dynamics 365 Project Operations and if present, Dynamics 365 Field Service.</span></span> 

- <span data-ttu-id="4e2aa-106">Project Operations бағдарламасында дағдылар репозиторийін жүргізу үшін **Ресурстар** \> **Ресурс дағдылары** тармағы бойынша өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="4e2aa-106">To maintain the repository of skills in Project Operations, go to **Resources** \> **Resource Skills**.</span></span> 

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="4e2aa-107">Ресурстарды бағалау үшін кәсіби дағдылар үлгілерін пайдалану</span><span class="sxs-lookup"><span data-stu-id="4e2aa-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="4e2aa-108">Ресурстардың дағдылары кәсіби дағдылар үлгілерімен бағаланады.</span><span class="sxs-lookup"><span data-stu-id="4e2aa-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="4e2aa-109">Жеке бағалар кәсіби дағдылар үлгісінде болады.</span><span class="sxs-lookup"><span data-stu-id="4e2aa-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="4e2aa-110">Кәсіби дағдылар үлгісін жасау үшін, **Ресурстар** \> **Кәсіби дағдылар үлгілері** тармағына өтіп, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="4e2aa-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="4e2aa-111">Жаңа бағалау үлгісінде минималды бағалау мәнін, максималды бағалау мәнін және бағаланып жатқан нысанды көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="4e2aa-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="4e2aa-112">**Бағалау мәндері** қосалқы торында, минималды мәннен максималды мәнге дейінгі әртүрлі бағалау мәндерін анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="4e2aa-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>


<span data-ttu-id="4e2aa-113">Бұл бағалау мәндері **Ресурс талаптары**, **Кесте тақтасы** және **Кесте көмекшісі** сүзгілерінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="4e2aa-113">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]