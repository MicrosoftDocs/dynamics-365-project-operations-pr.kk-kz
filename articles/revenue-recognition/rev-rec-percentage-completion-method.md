---
title: Бекітілген бағадағы табыс болжамы жобалары
description: Бұл тақырыпта жобалардағы бекітілген баға табысы туралы ақпарат беріледі.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 639c6a104f2a90366a0f477c0d7cf384f19cdd81
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013808"
---
# <a name="fixed-price-revenue-estimate-projects"></a><span data-ttu-id="c66b6-103">Бекітілген бағадағы табыс болжамы жобалары</span><span class="sxs-lookup"><span data-stu-id="c66b6-103">Fixed price revenue estimate projects</span></span> 

<span data-ttu-id="c66b6-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="c66b6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c66b6-105">Microsoft Dataverse жүйесіндегі Dynamics 365 Project Operations бағдарламасындағы келесі төлсипаттармен жобалық келісім-шарт жолын жасау кезінде жүйе автоматты түрде бекітілген баға табысы болжамының жобасын жасайды.</span><span class="sxs-lookup"><span data-stu-id="c66b6-105">When you create a project contract line with the following attributes in Dynamics 365 Project Operations on Microsoft Dataverse, the system automatically creates a fixed price revenue estimate project.</span></span> <span data-ttu-id="c66b6-106">Бұл жобадағы ақпарат келесіге негізделген:</span><span class="sxs-lookup"><span data-stu-id="c66b6-106">The information in this project is based on the following:</span></span>

  - <span data-ttu-id="c66b6-107">Бекітілген баға бойынша есеп айырысу әдісі.</span><span class="sxs-lookup"><span data-stu-id="c66b6-107">A fixed price billing method.</span></span>
  - <span data-ttu-id="c66b6-108">Байланысты жоба.</span><span class="sxs-lookup"><span data-stu-id="c66b6-108">An associated project.</span></span>
  - <span data-ttu-id="c66b6-109">**Жобалық келісім-шарт жолы** бетіндегі **Есеп-шот кестесі** қойыншасында анықталған кем дегенде бір аралық кезең.</span><span class="sxs-lookup"><span data-stu-id="c66b6-109">At least one milestone defined on the **Invoice schedule** tab on the **Project contract line** page.</span></span>

## <a name="review-fixed-price-revenue-estimates-projects"></a><span data-ttu-id="c66b6-110">Бекітілген бағадағы табыс болжамдары жобаларын қарап шығу</span><span class="sxs-lookup"><span data-stu-id="c66b6-110">Review fixed price revenue estimates projects</span></span>
<span data-ttu-id="c66b6-111">Бекітілген баға табысы болжамдарының жобаларын қарап шығу үшін келесі қадамдарды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="c66b6-111">To review fixed price revenue estimates projects, complete the following steps:</span></span>

1. <span data-ttu-id="c66b6-112">Dynamics 365 Finance ортасында **Жобаларды басқару және есеп** > **Жобалар** > **Бекітілген баға табысы болжамының жобалары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="c66b6-112">In the Dynamics 365 Finance environment, go to **Projects management and accounting** > **Projects** > **Fixed price revenue estimate projects**.</span></span>
2. <span data-ttu-id="c66b6-113">Қарағыңыз келетін жобаны таңдаңыз да, жазбаны ашып, жоба мәліметтерін қарап шығу үшін **Болжам жобасының идентификаторы** түймесін екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="c66b6-113">Select the project that you want to view and double-click the **Estimate project ID** to open the record and review the details of the project.</span></span>
3. <span data-ttu-id="c66b6-114">**Жоба** қойыншасын кеңейтіңіз. **Таңдалған жобалар** торында бір жобаны көресіз.</span><span class="sxs-lookup"><span data-stu-id="c66b6-114">Expand the **Project** tab. You will see one project in the **Selected projects** grid.</span></span> <span data-ttu-id="c66b6-115">Жүйе мұны әдепкі жоба ретінде пайдаланады, себебі бұл жоба келісім-шарт жолымен байланысты жоба.</span><span class="sxs-lookup"><span data-stu-id="c66b6-115">The system uses this as default project because it is the project associated to the project contract line.</span></span> 
4. <span data-ttu-id="c66b6-116">Байланысты өзгерту үшін қосымша жобаларды таңдап, оларды **Таңдалған жобалар** торына қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="c66b6-116">To change the association, select additional projects and add them to the **Selected projects** grid.</span></span> <span data-ttu-id="c66b6-117">Бұл торда бірнеше жобалар таңдалса, барлық таңдалған жобалар үшін жобаның пайыздық орындалуы мен табыс болжамдары бірге есептеледі.</span><span class="sxs-lookup"><span data-stu-id="c66b6-117">If multiple projects are selected in this grid, the project percentage completion and revenue estimates are calculated together for of the all selected projects.</span></span>

  <span data-ttu-id="c66b6-118">Жоба құны, табыс профилі, шығындар үлгісі және кезең кодын қолмен орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="c66b6-118">Project cost, revenue profile, cost template, and the period code can be set manually.</span></span> <span data-ttu-id="c66b6-119">Егер олар қолмен орнатылмаса, мәндер жоба құны мен табыс профильдері үшін конфигурацияланған ережелерді қолдана отырып, жоба бойынша алғашқы болжамды есептеу кезінде әдепкі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="c66b6-119">If they aren't set manually, the values default during the first estimate calculation for the project using the rules configured for project cost and revenue profiles.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]