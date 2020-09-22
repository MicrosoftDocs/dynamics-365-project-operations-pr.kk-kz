---
title: Мен неліктен Нақты көрсеткіштер нысанынан жазбаларды жоя алмаймын?
description: Бұл тақырыпта нақты мәндер нысанынан жазбалар неліктен жойылмайтыны туралы ақпарат берілген.
author: JPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.prod: Project Service
ms.technology: Applies to all versions of Project Service
ms.assetid: ff504c34-7337-474f-89e8-d8afdd1e0a98
ms.author: Jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5817940933c161dccac0fe549fabacbe57e7077a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753019"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="46a9a-103">Мен неліктен Нақты көрсеткіштер нысанынан жазбаларды жоя алмаймын?</span><span class="sxs-lookup"><span data-stu-id="46a9a-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="46a9a-104">Project Service Automation (PSA) бағдарламасы нақты фактілерді жоюға мүмкіндік бермейді, себебі олар жалпы бухгалтерлік сияқты төменгі жүйелерге қаржылық әсерін тигізетін транзакциялар үшін шындық көзі ретінде қызмет көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="46a9a-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="46a9a-105">Егер нақты мәндерді жою мүмкін болса, қаржылық есеп беру транзакцияларының тұтастығына күмән келтіруге болады.</span><span class="sxs-lookup"><span data-stu-id="46a9a-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="46a9a-106">Тексеру журналын орнату үшін, тұтынушылар өтемақы транзакцияларын жасау үшін журналдарды пайдалануы керек.</span><span class="sxs-lookup"><span data-stu-id="46a9a-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

