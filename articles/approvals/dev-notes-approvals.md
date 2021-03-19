---
title: Бекітулерге арналған әзірлеуші ескертпелері
description: Бұл тақырыпта бекітулермен жұмыс істеу жөніндегі қосымша әзірлеушілер туралы ақпарат берілген.
author: stsporen
manager: Annbe
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: d58c776b0341c08b0292e1b459a7d7ebac550bcc
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290276"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="2b530-103">Бекітулерге арналған әзірлеуші ескертпелері</span><span class="sxs-lookup"><span data-stu-id="2b530-103">Developer notes for Approvals</span></span>

<span data-ttu-id="2b530-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="2b530-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2b530-105">Dynamics 365 Project Operations бағдарламасы бекіту кезеңдері арқылы жазбаның дұрыс өтуін қамтамасыз ететін тексеру логикасын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="2b530-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="2b530-106">Жазбаның дұрыс өтуі келесіні қамтамасыз етеді:</span><span class="sxs-lookup"><span data-stu-id="2b530-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="2b530-107">Барлық қолдау көрсететін жолдар журналдар мен нақты көрсеткіштер сияқты қатысты кестелерде жасалады.</span><span class="sxs-lookup"><span data-stu-id="2b530-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="2b530-108">Жалғастырмас бұрын растаушы жобада **Жоба растаушысы** болып белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="2b530-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]