---
title: Дағдылар мен кәсіби дағдылар үлгілері
description: Бұл тақырыпта дағдылар мен кәсіби дағдылар үлгілерін пайдалану жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/13/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c7da8b2a7eda51b2aa7cf04e325a92f33d834efc
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147480"
---
# <a name="skills-and-proficiency-models"></a><span data-ttu-id="9de8f-103">Дағдылар мен кәсіби дағдылар үлгілері</span><span class="sxs-lookup"><span data-stu-id="9de8f-103">Skills and proficiency models</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="9de8f-104">Дағдылар — Dynamics 365 Project Service Automation бағдарламасы мен егер бар болса, Dynamics 365 Field Service бағдарламасының арасында ортақ пайдаланылатын ресурс сипаттамалары.</span><span class="sxs-lookup"><span data-stu-id="9de8f-104">Skills are resource characteristics that are shared between Dynamics 365 Project Service Automation and if present, Dynamics 365 Field Service.</span></span> 

<span data-ttu-id="9de8f-105">Project Service Automation бағдарламасында дағдылар репозиторийін жүргізу үшін, **Ресурстар** \> **Ресурс дағдылары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="9de8f-105">To maintain the repository of skills in Project Service Automation, go to **Resources** \> **Resource Skills**.</span></span> 

> ![Ресурс дағдылары](media/Resource-Management-image84.png)

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="9de8f-107">Ресурстарды бағалау үшін кәсіби дағдылар үлгілерін пайдалану</span><span class="sxs-lookup"><span data-stu-id="9de8f-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="9de8f-108">Ресурстардың дағдылары кәсіби дағдылар үлгілерімен бағаланады.</span><span class="sxs-lookup"><span data-stu-id="9de8f-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="9de8f-109">Жеке бағалар кәсіби дағдылар үлгісінде болады.</span><span class="sxs-lookup"><span data-stu-id="9de8f-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="9de8f-110">Кәсіби дағдылар үлгісін жасау үшін, **Ресурстар** \> **Кәсіби дағдылар үлгілері** тармағына өтіп, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9de8f-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="9de8f-111">Жаңа бағалау үлгісінде минималды бағалау мәнін, максималды бағалау мәнін және бағаланып жатқан нысанды көрсетіңіз.</span><span class="sxs-lookup"><span data-stu-id="9de8f-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="9de8f-112">**Бағалау мәндері** қосалқы торында, минималды мәннен максималды мәнге дейінгі әртүрлі бағалау мәндерін анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="9de8f-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>

> ![Анықталған минималды және максималды бағалар](media/Resource-Management-image85.png)

<span data-ttu-id="9de8f-114">Бұл бағалау мәндері **Ресурс талаптары**, **Кесте тақтасы** және **Кесте көмекшісі** сүзгілерінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="9de8f-114">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>
