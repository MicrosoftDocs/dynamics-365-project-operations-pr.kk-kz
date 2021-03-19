---
title: Ресурсты пайдалануға шолу
description: Бұл тақырыпта ресурсты Project Operations бағдарламасында пайдалану туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4d66b5fc642ef53adf1169ce891a7a5fa26b07d6
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279325"
---
# <a name="resource-utilization-overview"></a><span data-ttu-id="05077-103">Ресурсты пайдалануға шолу</span><span class="sxs-lookup"><span data-stu-id="05077-103">Resource utilization overview</span></span>

<span data-ttu-id="05077-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="05077-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="05077-105">Ресурстардың мақсатты шот ұсынылған қолданысы болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="05077-105">Resources can have a target billable utilization.</span></span> <span data-ttu-id="05077-106">Осы мақсатты пайдалану ресурстың әдепкі рөліндегі атрибут ретінде анықталады немесе жеке тіркелетін ресурстың жазбасында орнатылады.</span><span class="sxs-lookup"><span data-stu-id="05077-106">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="05077-107">Пайдалану есептеулері ресурстар бекітілген уақыт жазбаларын пайдалану арқылы есеп берген нақты сағат санына негізделген.</span><span class="sxs-lookup"><span data-stu-id="05077-107">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="05077-108">Пайдалануды есептеу үшін келесі формулалар пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="05077-108">The following formulas are used to calculate utilization:</span></span>

  - <span data-ttu-id="05077-109">Шот ұсынылған қолданыс = ақылы нақты сағаттар ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="05077-109">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
  - <span data-ttu-id="05077-110">Шот ұсынылмайтын қолданыс = шот ұсыну түрінің идентификаторы бар нақты уақыт = ақысыз, қосымша немесе қолжетімді емес ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="05077-110">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
  - <span data-ttu-id="05077-111">Ішкі = сатылым келісім-шарты жоқ нақты уақыт ÷ ресурс сыйымдылығы</span><span class="sxs-lookup"><span data-stu-id="05077-111">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
  - <span data-ttu-id="05077-112">Ресурс сыйымдылығы = ресурстың жұмыс сағаттары – кеңседен тыс – жұмыс істемейтін күндер</span><span class="sxs-lookup"><span data-stu-id="05077-112">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="05077-113">**Ресурсты пайдалану** көрінісін **Ресурстар** тақтасынан табуға болады.</span><span class="sxs-lookup"><span data-stu-id="05077-113">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="05077-114">Тордағы әрбір ұяшық ресурстың күн, апта немесе ай сияқты кезеңдегі шот ұсынылған қолданысының пайыздық мөлшерін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="05077-114">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="05077-115">Ұяшықтарды бояу үшін келесі формулалар пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="05077-115">The following formulas are used to color the cells:</span></span>

  - <span data-ttu-id="05077-116">**Жасыл**: шот ұсынылған қолданыс >= ресурстың мақсатты қолданысы</span><span class="sxs-lookup"><span data-stu-id="05077-116">**Green**: Billable utilization >= Resource target utilization</span></span>
  - <span data-ttu-id="05077-117">**Сары**: мақсатты қолданыс – 20 <= шот ұсынылған қолданыс < мақсатты қолданыс</span><span class="sxs-lookup"><span data-stu-id="05077-117">**Yellow**: Target utilization – 20 <= Billable utilization < Target utilization</span></span>
  - <span data-ttu-id="05077-118">**Қызыл**: шот ұсынылған қолданыс < мақсатты қолданыс – 20</span><span class="sxs-lookup"><span data-stu-id="05077-118">**Red**: Billable utilization < Target utilization – 20</span></span>

<span data-ttu-id="05077-119">**Ресурсты пайдалану** көрінісі кесте тақтасына негізделгендіктен, нәтижелерді сүзгілеу үшін кесте тақтасының сүзгілеу мүмкіндіктерін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="05077-119">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="05077-120">Тор рөлге немесе жеке ресурсқа мақсатты қолданысты орнатуды талап етеді.</span><span class="sxs-lookup"><span data-stu-id="05077-120">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="05077-121">Бұл орнатуды орындау үші, **Ресурстар** > **Ресурс рөлдері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="05077-121">To do this setup, go to **Resources** > **Resource roles**.</span></span>

<span data-ttu-id="05077-122">Сонымен қатар әрбір тіркелетін ресурсқа әдепкі рөлді тағайындау керек.</span><span class="sxs-lookup"><span data-stu-id="05077-122">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="05077-123">**Ресурстар** > **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="05077-123">Go to **Resources** > **Resources**.</span></span> <span data-ttu-id="05077-124">**Project Service** қойыншасында ресурс рөлінің анықталғанын және оның **Әдепкі** өрісі **Иә** параметріне орнатылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="05077-124">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field is set to **Yes**.</span></span> <span data-ttu-id="05077-125">**Әдепкі** = **жоқ** параметріне орнатылған қосымша рөлдерді қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="05077-125">You can add additional roles where **Is Default** = **No**.</span></span> <span data-ttu-id="05077-126">**Әдепкі** = **иә** параметріне орнатылған рөл ресурсты сол рөлдің мақсаты бойынша пайдалануды бағалау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="05077-126">The role where the **Is Default** = **Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="05077-127">**Project Service** қойыншасында, ресурс үшін жеке мақсатты қолданысты орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="05077-127">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="05077-128">Сонда пайдалануды есептеу ресурстың әдепкі рөлінің орнына ресурстың мақсатын бағалау үшін мақсатты қолданысты пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="05077-128">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="05077-129">Қолдану ресурсқа егер оның торда көрсетілген уақыт кезеңінде бекітілген, ақылы уақыты болса ғана көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="05077-129">Utilization is only shown for a resource if that resource has approved, chargeable time during the period shown in the grid.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]