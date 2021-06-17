---
title: Бекітулерге арналған әзірлеуші ескертпелері
description: Бұл тақырыпта бекітулермен жұмыс істеу жөніндегі қосымша әзірлеушілер туралы ақпарат берілген.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: a89ea669a262c145b9f391fddc19e79a425fabb5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996798"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="decb8-103">Бекітулерге арналған әзірлеуші ескертпелері</span><span class="sxs-lookup"><span data-stu-id="decb8-103">Developer notes for Approvals</span></span>

<span data-ttu-id="decb8-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="decb8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="decb8-105">Dynamics 365 Project Operations бағдарламасы бекіту кезеңдері арқылы жазбаның дұрыс өтуін қамтамасыз ететін тексеру логикасын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="decb8-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="decb8-106">Жазбаның дұрыс өтуі келесіні қамтамасыз етеді:</span><span class="sxs-lookup"><span data-stu-id="decb8-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="decb8-107">Барлық қолдау көрсететін жолдар журналдар мен нақты көрсеткіштер сияқты қатысты кестелерде жасалады.</span><span class="sxs-lookup"><span data-stu-id="decb8-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="decb8-108">Жалғастырмас бұрын растаушы жобада **Жоба растаушысы** болып белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="decb8-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]