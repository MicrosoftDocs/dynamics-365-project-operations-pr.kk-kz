---
title: Мен неліктен Нақты көрсеткіштер нысанынан жазбаларды жоя алмаймын?
description: Бұл тақырыпта нақты мәндер нысанынан жазбалар неліктен жойылмайтыны туралы ақпарат берілген.
author: JPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
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
ms.openlocfilehash: 36cd241c7c7a2ff6ae018c94d691bc95d1f0c912
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148965"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="4f526-103">Мен неліктен Нақты көрсеткіштер нысанынан жазбаларды жоя алмаймын?</span><span class="sxs-lookup"><span data-stu-id="4f526-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="4f526-104">Project Service Automation (PSA) бағдарламасы нақты фактілерді жоюға мүмкіндік бермейді, себебі олар жалпы бухгалтерлік сияқты төменгі жүйелерге қаржылық әсерін тигізетін транзакциялар үшін шындық көзі ретінде қызмет көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="4f526-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="4f526-105">Егер нақты мәндерді жою мүмкін болса, қаржылық есеп беру транзакцияларының тұтастығына күмән келтіруге болады.</span><span class="sxs-lookup"><span data-stu-id="4f526-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="4f526-106">Тексеру журналын орнату үшін, тұтынушылар өтемақы транзакцияларын жасау үшін журналдарды пайдалануы керек.</span><span class="sxs-lookup"><span data-stu-id="4f526-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

