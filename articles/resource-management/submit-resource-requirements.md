---
title: Ресурс сұрауын жіберу
description: Жасалған ресурс талабын ресурс сұрауы ретінде жіберуге болады. Содан кейін сұрау орындау үшін ресурс менеджеріне жіберіледі.
author: ruhercul
manager: Annbe
ms.date: 10/04/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 94cf0f0d88e9be2522936b45122ed0037434d4f3
ms.sourcegitcommit: 2cf93d8bf0be5b61a739195a41334c34d910e9ba
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961722"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="48c11-104">Ресурс сұрауын жіберу</span><span class="sxs-lookup"><span data-stu-id="48c11-104">Submit a resource request</span></span>

<span data-ttu-id="48c11-105">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="48c11-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="48c11-106">Жасалған ресурс талабын ресурс сұрауы ретінде жіберуге болады.</span><span class="sxs-lookup"><span data-stu-id="48c11-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="48c11-107">Содан кейін сұрау орындау үшін ресурс менеджеріне жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="48c11-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="48c11-108">Dynamics 365 Project Operations бағдарламасында, тіркелетін ресурстарды көру үшін **Жобалар** бетінде **Топ** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="48c11-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="48c11-109">Тізімнен ресурс талабы бар жалпы ресурсты таңдап, **Сұрау жіберу** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="48c11-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="48c11-110">Жалпы топ мүшесінің сұрау күйі **Жіберілді** күйіне өзгереді.</span><span class="sxs-lookup"><span data-stu-id="48c11-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="48c11-111">Сұрау орындалғаннан кейін, ресурс менеджері аталған ресурсты тіркеу сұрауын орындаса, жалпы ресурс аталған ресурспен ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="48c11-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="48c11-112">Әйтпесе, ресурс менеджері аталған ресурсты ұсынса, жалпы ресурс топта қалып, сұрау күйі **Қарап шығуды талап етеді** күйіне өзгереді.</span><span class="sxs-lookup"><span data-stu-id="48c11-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>
