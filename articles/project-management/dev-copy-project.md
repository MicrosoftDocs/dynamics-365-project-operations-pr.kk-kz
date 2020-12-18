---
title: Copy Project көмегімен жоба үлгілерін жасау
description: Бұл тақырыпта Copy Project реттелетін әрекеті көмегімен жоба үлгілерін жасау жолы туралы ақпарат берілген.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 22976730ef3c8c22ea028b27a6eb5f14fb88993e
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642415"
---
# <a name="develop-project-templates-with-copy-project"></a>Copy Project көмегімен жоба үлгілерін жасау

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations бағдарламасы жобаны көшіру және кез келген тапсырманы рөлді көрсететін жалпы ресурстарға қайтару мүмкіндігін қолдайды. Тұтынушылар бұл функцияны жобаның негізгі үлгілерін құру үшін пайдалана алады.

**Copy Project** таңдалған кезде, мақсатты жобаның күйі жаңартылады. Көшіру әрекеті қашан аяқталғанын анықтау **Күй себебі** пәрменін пайдаланыңыз. **Copy Project** таңдау мақсатты жоба нысанында ешқандай мақсатты күн анықталмаса, жобаның басталу күнін ағымдағы басталу күніне дейін жаңартады.

## <a name="copy-project-custom-action"></a>Copy Project реттелетін әрекеті 

### <a name="name"></a>Атауы 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>Кіріс параметрлер
Үш кіріс параметрі берілген:

| Параметр          | Түр   | Мәндер                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** немесе **{"clearTeamsAndAssignments":true}** |
| SourceProject      | Нысан анықтамасы | Бастапқы жоба |
| Мақсатты мән             | Нысан анықтамасы | Мақсатты жоба |


- **{"clearTeamsAndAssignments":true}**: интернетке арналған жобаның әдепкі әрекеті және барлық тапсырмалар мен топ мүшелерін жояды.
- **{"removeNamedResources":true}** Project Operation бағдарламасына арналған әдепкі әрекет және тағайындауларды жалпы ресурстарға қайтарады.

Әрекеттердегі әдепкі параметрлер туралы ақпарат алу үшін [Веб API әрекеттерін пайдалану](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions) бөлімін қараңыз

## <a name="specify-fields-to-copy"></a>Көшіру үшін өрістерді көрсетіңіз 
Әрекет шақырылған кезде, **Copy Project** жоба көшірілгенде қандай өрістер көшірілетінін анықтау үшін **Жоба бағандарын көшіру** жоба көрінісін қарастырады.
