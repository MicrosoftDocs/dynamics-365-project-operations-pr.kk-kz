---
title: Dynamics 365 Project Operations бағдарламасын жою
description: Бұл мақалада Dynamics 365 Project Operations бағдарламасын жою жолы туралы ақпарат берілген.
author: stsporen
ms.date: 11/09/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 33a505594d6db47b4f8a0c8a630a0836f424e7d5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8911971"
---
# <a name="uninstall-dynamics-365-project-operations"></a>Dynamics 365 Project Operations бағдарламасын жою 

_**Қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Dynamics 365 Project Operations бағдарламасын жою үшін сізге әкімші рөлі тағайындалуы тиіс.

1. **Параметрлер** > **Шешімдер** бөліміне өтіңіз.

    ![Параметрлер беті.](./media/uninstall-proj-ops-solutions.png)
  
2. Шешімдерді келесі кестеде көрсетілген нақты ретпен алып тастаңыз. 

    | Қадам | Шешім атауы                                    | Ескертпе                                                                                         |
    |------|----------------------------------------------------|----------------------------------------------------------------------------------------------|
    | 1-көше | msdyn_ProjectServiceUpgrade_managed.cab            | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 2-көше | ProjectOperations_Anchor                           | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 3-көше | Dynamics365ProjectOperationsDualWriteEntityMaps    | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 4 | Dynamics365ProjectOperationsDualWrite              | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 5 | ProjectService                                     | Қосымша ескертпелер жоқ.                                                                         |
    | 6 | ProjectServiceCore_Patch                           | Қосымша ескертпелер жоқ.                                                                         |
    | 7 | ProjectServiceCore                                 | Қосымша ескертпелер жоқ.                                                                         |
    | 8 | ProjectServiceDeprecatedComponents                 | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 9 | FieldServiceCommon                                 | Dynamics 365 Finance немесе Dynamics 365 Supply Chain Management жүйесімен қос жазу үшін қажет.   |
    | 10 | msdyn_AssetCommon                                  | Dynamics 365 Finance немесе Dynamics 365 Supply Chain Management жүйесімен қос жазу үшін қажет.   |
    | 11 | msdyn_TESA_Anchor                                  | Dynamics 365 Field Service үшін қажет.                                                     |
    | 12 | msdyn_TESA_Patch                                   | Dynamics 365 Field Service үшін қажет.                                                     |
    | 13 | msdyn_TESA                                         | Dynamics 365 Field Service үшін қажет.                                                     |
    | 14 | ResourceSchedulingControls                         | Dynamics 365 Field Service үшін қажет.                                                     |
    | 15 | MicrosoftDynamicsScheduling3_CumulativePatch       | Dynamics 365 Field Service үшін қажет.                                                     |
    | 16 | MicrosoftDynamicsScheduling_Patch_xx               | Dynamics 365 Field Service үшін қажет.                                                     |
    | 17 | MicrosoftDynamicsScheduling                        | Dynamics 365 Field Service үшін қажет.                                                     |
    | 18 | Dynamics365FinanceAndOperationsAnchor              | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 19 | Dynamics365Notes                                   | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 20 | Dynamics365FinanceAndOperationsDualWriteEntityMaps | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 21 | DualWriteCore                                      | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 22 | Dynamics365AssetManagementApp                      | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 23 | Dynamics365AssetManagement                         | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 24 | Dynamics365SupplyChainExtended                     | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 25 | Dynamics365FinanceExtended                         | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 26 | HCMCommon                                          | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 27 | Dynamics365FinanceAndOperationsCommon              | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 28 | Тарап                                              | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 29 | Dynamics365Company                                 | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 30 | CurrencyExchangeRates                              | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
    | 31 | AssetCommon                                        | Егер табылмаса, бұл шешімді өткізіп жіберіңіз.                                                            |
