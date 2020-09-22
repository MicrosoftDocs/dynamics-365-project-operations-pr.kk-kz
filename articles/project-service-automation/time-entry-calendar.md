---
title: Уақыт жазбасының күнтізбесі
description: Бұл тақырыпта уақыт жазбасының күнтізбесін пайдалану жолы туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: cc78d9ae-9f1b-4bd4-8cdf-41406f859ff7
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: ea8c5113b9ba89e2255218e6a53f062c25badc98
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753107"
---
# <a name="time-entry-calendar"></a><span data-ttu-id="4c570-103">Уақыт жазбасының күнтізбесі</span><span class="sxs-lookup"><span data-stu-id="4c570-103">Time entry calendar</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="4c570-104">**Уақыт жазбалары** бетінде күнтізбедегі уақыт жазбаларын **Басқаша көрсету**\>**Күнтізбені басқару** түймешігін таңдау арқылы көруге болады.</span><span class="sxs-lookup"><span data-stu-id="4c570-104">On the **Time Entries** page, you can view the time entries on the calendar by selecting **Show as** \> **Calendar Control**.</span></span>

## <a name="updated-calendar-control"></a><span data-ttu-id="4c570-105">Жаңартылған күнтізбені басқару элементі</span><span class="sxs-lookup"><span data-stu-id="4c570-105">Updated calendar control</span></span>

<span data-ttu-id="4c570-106">Dynamics 365 Project Service Automation уақыт жазбасының жаңа және кеңейтілетін тәжірибесін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="4c570-106">Dynamics 365 Project Service Automation offers a new and extensible time entry experience.</span></span> <span data-ttu-id="4c570-107">Бұл жаңа тәжірибе алдыңғы нұсқаларда пайдаланылған Реттелетін күнтізбені басқару элементін алмастырады.</span><span class="sxs-lookup"><span data-stu-id="4c570-107">This new experience replaces the Custom Calendar Control that was used in earlier versions.</span></span> <span data-ttu-id="4c570-108">Дегенмен уақыт жазбаларын тек оқуға арналған күнтізбені бақылау элементі арқылы көруге болады. Бұны Бірыңғай интерфейс құрылымы күнделікті, апталық немесе айлық көріністер үшін қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="4c570-108">However, you can still view time entries through a read-only calendar control that the Unified Interface Framework provides for daily, weekly, or monthly views.</span></span>

<span data-ttu-id="4c570-109">Күнтізбе жеке күнтізбе элементтеріндегі әрекеттерге қолдау көрсетпейді және жіберілетін немесе жойылатын бір немесе бірнеше күнтізбе элементтерін таңдау мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="4c570-109">The calendar doesn't support actions on individual calendar items, and you can't select one or more calendar items for submission or deletion.</span></span> <span data-ttu-id="4c570-110">Оның орнына қажетті әрекеттерді орындауға болатын **Уақыт жазбасы** нысан бетін ашу үшін күнтізбе элементін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="4c570-110">Instead, select a calendar item to open the **Time Entry** entity page, where you can complete the required actions.</span></span>

## <a name="extensibility"></a><span data-ttu-id="4c570-111">Кеңейтімділік</span><span class="sxs-lookup"><span data-stu-id="4c570-111">Extensibility</span></span>

<span data-ttu-id="4c570-112">Уақыт жазбасы торы бар **Уақыт жазбалары** бетінде реттелетін өрістерді қосуға, іздеу өрістерін орнатуға және реттелетін көріністер жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="4c570-112">On the **Time Entries** page that has the time entry grid, you can add custom fields, set up lookup fields, and create custom views.</span></span> <span data-ttu-id="4c570-113">Сондай-ақ реттелетін өрістерде таңдалған немесе енгізілген мәндерге негізделген реттелетін бизнес-логиканы орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="4c570-113">You can also set up custom business logic that is based on the values that are selected or entered in custom fields.</span></span>
