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
ms.openlocfilehash: 9e4e910d0ff0a5f2603148fcc5daa0d423a4d174
ms.sourcegitcommit: a9dbcd3aff4c6ae495412e4980e105ae160fd1ec
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/10/2020
ms.locfileid: "4483955"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="5b890-103">Бекітулерге арналған әзірлеуші ескертпелері</span><span class="sxs-lookup"><span data-stu-id="5b890-103">Developer notes for Approvals</span></span>

<span data-ttu-id="5b890-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="5b890-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5b890-105">Dynamics 365 Project Operations бағдарламасы бекіту кезеңдері арқылы жазбаның дұрыс өтуін қамтамасыз ететін тексеру логикасын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="5b890-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="5b890-106">Жазбаның дұрыс өтуі келесіні қамтамасыз етеді:</span><span class="sxs-lookup"><span data-stu-id="5b890-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="5b890-107">Барлық қолдау көрсететін жолдар журналдар мен нақты көрсеткіштер сияқты қатысты кестелерде жасалады.</span><span class="sxs-lookup"><span data-stu-id="5b890-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="5b890-108">Жалғастырмас бұрын растаушы жобада **Жоба растаушысы** болып белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="5b890-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>
