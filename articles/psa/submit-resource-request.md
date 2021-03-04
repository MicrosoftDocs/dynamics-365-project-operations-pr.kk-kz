---
title: Ресурс сұрауын жіберу
description: Бұл тақырыпта жоба ресурсына сұрау жіберу туралы ақпарат берілген.
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 173572be43149aea253bf7beddb993f8c50ab337
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149730"
---
# <a name="submitting-a-resource-request"></a><span data-ttu-id="8828f-103">Ресурс сұрауын жіберу</span><span class="sxs-lookup"><span data-stu-id="8828f-103">Submitting a resource request</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8828f-104">Жасалған ресурс талабын ресурс сұрауы ретінде жіберуге болады.</span><span class="sxs-lookup"><span data-stu-id="8828f-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="8828f-105">Содан кейін сұрау орындау үшін ресурс менеджеріне жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="8828f-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="8828f-106">Project Service Automation (PSA) бағдарламасында, тіркелетін ресурстарды көру үшін **Жобалар** бетінде **Топ** қойыншасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8828f-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="8828f-107">Тізімнен ресурс талабы бар жалпы ресурсты таңдап, **Сұрау жіберу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="8828f-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![Ресурс сұрауын жіберу](media/RM-how-to-18.png)

<span data-ttu-id="8828f-109">Жалпы топ мүшесінің сұрау күйі **Жіберілді** күйіне өзгереді.</span><span class="sxs-lookup"><span data-stu-id="8828f-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="8828f-110">Ресурс менеджері сұрауды орындағаннан кейін, ол аталған ресурсты тіркеу сұрауын орындаса, жалпы ресурс аталған ресурспен ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="8828f-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="8828f-111">Әйтпесе, ресурс менеджері аталған ресурсты ұсынған болса, жалпы ресурс топта қалып, сұрау күйі **Қарап шығуды талап етеді** күйіне өзгереді.</span><span class="sxs-lookup"><span data-stu-id="8828f-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review**, if the resource manager has proposed a named resource.</span></span>
