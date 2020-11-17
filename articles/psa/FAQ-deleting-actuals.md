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
ms.openlocfilehash: b9b45e3ae0cd9273af4d2a5cd9cce30502c0aa78
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127165"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="9946f-103">Мен неліктен Нақты көрсеткіштер нысанынан жазбаларды жоя алмаймын?</span><span class="sxs-lookup"><span data-stu-id="9946f-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="9946f-104">Project Service Automation (PSA) бағдарламасы нақты фактілерді жоюға мүмкіндік бермейді, себебі олар жалпы бухгалтерлік сияқты төменгі жүйелерге қаржылық әсерін тигізетін транзакциялар үшін шындық көзі ретінде қызмет көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="9946f-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="9946f-105">Егер нақты мәндерді жою мүмкін болса, қаржылық есеп беру транзакцияларының тұтастығына күмән келтіруге болады.</span><span class="sxs-lookup"><span data-stu-id="9946f-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="9946f-106">Тексеру журналын орнату үшін, тұтынушылар өтемақы транзакцияларын жасау үшін журналдарды пайдалануы керек.</span><span class="sxs-lookup"><span data-stu-id="9946f-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

