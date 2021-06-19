---
title: Ресурс сұрауын жіберу
description: Жасалған ресурс талабын ресурс сұрауы ретінде жіберуге болады. Содан кейін сұрау орындау үшін ресурс менеджеріне жіберіледі.
author: ruhercul
ms.date: 10/04/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 6ac0044a27d1e506c9c62c477014017fd0ca06cb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014033"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="0d257-104">Ресурс сұрауын жіберу</span><span class="sxs-lookup"><span data-stu-id="0d257-104">Submit a resource request</span></span>

<span data-ttu-id="0d257-105">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="0d257-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0d257-106">Жасалған ресурс талабын ресурс сұрауы ретінде жіберуге болады.</span><span class="sxs-lookup"><span data-stu-id="0d257-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="0d257-107">Содан кейін сұрау орындау үшін ресурс менеджеріне жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="0d257-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="0d257-108">Dynamics 365 Project Operations бағдарламасында тіркелетін ресурстарды көру үшін **Жобалар** бетінде **Топ** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="0d257-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="0d257-109">Тізімнен ресурс талабы бар жалпы ресурсты таңдап, **Сұрау жіберу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="0d257-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="0d257-110">Жалпы топ мүшесінің сұрау күйі **Жіберілді** күйіне өзгереді.</span><span class="sxs-lookup"><span data-stu-id="0d257-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="0d257-111">Сұрау орындалғаннан кейін, ресурс менеджері аталған ресурсты тіркеу сұрауын орындаса, жалпы ресурс аталған ресурспен ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="0d257-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="0d257-112">Әйтпесе, ресурс менеджері аталған ресурсты ұсынса, жалпы ресурс топта қалып, сұрау күйі **Қарап шығуды талап етеді** күйіне өзгереді.</span><span class="sxs-lookup"><span data-stu-id="0d257-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]