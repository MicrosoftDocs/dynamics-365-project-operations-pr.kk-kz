---
title: Мен неліктен Нақты көрсеткіштер нысанынан жазбаларды жоя алмаймын?
description: Бұл тақырыпта нақты мәндер нысанынан жазбалар неліктен жойылмайтыны туралы ақпарат берілген.
author: JPBurrows
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
ms.openlocfilehash: 434be93cedb4772616b1e6d5cbe15fc715eed19a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993108"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="ce8e0-103">Мен неліктен Нақты көрсеткіштер нысанынан жазбаларды жоя алмаймын?</span><span class="sxs-lookup"><span data-stu-id="ce8e0-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ce8e0-104">Project Service Automation (PSA) бағдарламасы нақты фактілерді жоюға мүмкіндік бермейді, себебі олар жалпы бухгалтерлік сияқты төменгі жүйелерге қаржылық әсерін тигізетін транзакциялар үшін шындық көзі ретінде қызмет көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="ce8e0-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="ce8e0-105">Егер нақты мәндерді жою мүмкін болса, қаржылық есеп беру транзакцияларының тұтастығына күмән келтіруге болады.</span><span class="sxs-lookup"><span data-stu-id="ce8e0-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="ce8e0-106">Тексеру журналын орнату үшін, тұтынушылар өтемақы транзакцияларын жасау үшін журналдарды пайдалануы керек.</span><span class="sxs-lookup"><span data-stu-id="ce8e0-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]