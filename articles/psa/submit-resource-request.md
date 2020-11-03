---
title: Ресурс сұрауын жіберу
description: Бұл тақырыпта жоба ресурсына сұрау жіберу туралы ақпарат берілген.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: bcea3d640d7e9ee2b071c55bff9ade3268edb319
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079753"
---
# <a name="submitting-a-resource-request"></a><span data-ttu-id="d3a69-103">Ресурс сұрауын жіберу</span><span class="sxs-lookup"><span data-stu-id="d3a69-103">Submitting a resource request</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="d3a69-104">Жасалған ресурс талабын ресурс сұрауы ретінде жіберуге болады.</span><span class="sxs-lookup"><span data-stu-id="d3a69-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="d3a69-105">Содан кейін сұрау орындау үшін ресурс менеджеріне жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="d3a69-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="d3a69-106">Project Service Automation (PSA) бағдарламасында, тіркелетін ресурстарды көру үшін **Жобалар** бетінде **Топ** қойыншасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d3a69-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="d3a69-107">Тізімнен ресурс талабы бар жалпы ресурсты таңдап, **Сұрау жіберу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d3a69-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![Ресурс сұрауын жіберу](media/RM-how-to-18.png)

<span data-ttu-id="d3a69-109">Жалпы топ мүшесінің сұрау күйі **Жіберілді** күйіне өзгереді.</span><span class="sxs-lookup"><span data-stu-id="d3a69-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="d3a69-110">Ресурс менеджері сұрауды орындағаннан кейін, ол аталған ресурсты тіркеу сұрауын орындаса, жалпы ресурс аталған ресурспен ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="d3a69-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="d3a69-111">Әйтпесе, ресурс менеджері аталған ресурсты ұсынған болса, жалпы ресурс топта қалып, сұрау күйі **Қарап шығуды талап етеді** күйіне өзгереді.</span><span class="sxs-lookup"><span data-stu-id="d3a69-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review** , if the resource manager has proposed a named resource.</span></span>
