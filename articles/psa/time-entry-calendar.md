---
title: Уақыт жазбасының күнтізбесі
description: Бұл тақырыпта уақыт жазбасының күнтізбесін пайдалану жолы туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 413aba735a5011a9b40c1d5b0bf43c6771db0f7b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131200"
---
# <a name="time-entry-calendar"></a><span data-ttu-id="750b2-103">Уақыт жазбасының күнтізбесі</span><span class="sxs-lookup"><span data-stu-id="750b2-103">Time entry calendar</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="750b2-104">**Уақыт жазбалары** бетінде күнтізбедегі уақыт жазбаларын **Басқаша көрсету**\>**Күнтізбені басқару** түймешігін таңдау арқылы көруге болады.</span><span class="sxs-lookup"><span data-stu-id="750b2-104">On the **Time Entries** page, you can view the time entries on the calendar by selecting **Show as** \> **Calendar Control**.</span></span>

## <a name="updated-calendar-control"></a><span data-ttu-id="750b2-105">Жаңартылған күнтізбені басқару элементі</span><span class="sxs-lookup"><span data-stu-id="750b2-105">Updated calendar control</span></span>

<span data-ttu-id="750b2-106">Dynamics 365 Project Service Automation уақыт жазбасының жаңа және кеңейтілетін тәжірибесін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="750b2-106">Dynamics 365 Project Service Automation offers a new and extensible time entry experience.</span></span> <span data-ttu-id="750b2-107">Бұл жаңа тәжірибе алдыңғы нұсқаларда пайдаланылған Реттелетін күнтізбені басқару элементін алмастырады.</span><span class="sxs-lookup"><span data-stu-id="750b2-107">This new experience replaces the Custom Calendar Control that was used in earlier versions.</span></span> <span data-ttu-id="750b2-108">Дегенмен уақыт жазбаларын тек оқуға арналған күнтізбені бақылау элементі арқылы көруге болады. Бұны Бірыңғай интерфейс құрылымы күнделікті, апталық немесе айлық көріністер үшін қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="750b2-108">However, you can still view time entries through a read-only calendar control that the Unified Interface Framework provides for daily, weekly, or monthly views.</span></span>

<span data-ttu-id="750b2-109">Күнтізбе жеке күнтізбе элементтеріндегі әрекеттерге қолдау көрсетпейді және жіберілетін немесе жойылатын бір немесе бірнеше күнтізбе элементтерін таңдау мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="750b2-109">The calendar doesn't support actions on individual calendar items, and you can't select one or more calendar items for submission or deletion.</span></span> <span data-ttu-id="750b2-110">Оның орнына қажетті әрекеттерді орындауға болатын **Уақыт жазбасы** нысан бетін ашу үшін күнтізбе элементін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="750b2-110">Instead, select a calendar item to open the **Time Entry** entity page, where you can complete the required actions.</span></span>

## <a name="extensibility"></a><span data-ttu-id="750b2-111">Кеңейтімділік</span><span class="sxs-lookup"><span data-stu-id="750b2-111">Extensibility</span></span>

<span data-ttu-id="750b2-112">Уақыт жазбасы торы бар **Уақыт жазбалары** бетінде реттелетін өрістерді қосуға, іздеу өрістерін орнатуға және реттелетін көріністер жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="750b2-112">On the **Time Entries** page that has the time entry grid, you can add custom fields, set up lookup fields, and create custom views.</span></span> <span data-ttu-id="750b2-113">Сондай-ақ реттелетін өрістерде таңдалған немесе енгізілген мәндерге негізделген реттелетін бизнес-логиканы орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="750b2-113">You can also set up custom business logic that is based on the values that are selected or entered in custom fields.</span></span>
