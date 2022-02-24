---
title: Жобаның баға ұсыныстарын талдау
description: Бұл тақырыпта жобаның баға ұсыныстарын талдау туралы ақпарат берілген.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 361a940261811467c46222c3d58c9504434ec882
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145230"
---
# <a name="analysis-of-project-quotes"></a>Жобаның баға ұсыныстарын талдау

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation қызметі табыстылықты болжау үшін жобаның баға ұсыныстарын талдайды. Сондай-ақ ол баға ұсыныстары тұтынушының жеткізілу күніне немесе аяқталу күніне және бюджетке қатысты болжамдарына қаншалықты сәйкес келетінін талдайды.

## <a name="profitability-analysis"></a>Табыстылық талдауы

Project Service Automation қызметі жиынтық пайда мен реттелген жиынтық пайданы пайдалану арқылы табыстылықты талдайды.

- Жиынтық пайда келесі формула бойынша есептеледі:

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- Реттелген жиынтық пайда келесі формула бойынша есептеледі:

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

Егер жиынтық пайда мен реттелген жиынтық пайда мәндері айтарлықтай өзгешеленсе, баға ұсынудағы жұмыстың көбі ақылы емес ретінде жіктеледі.

## <a name="analysis-of-customer-expectations"></a>Тұтынушы болжамдарын талдау

Келесі өрістер үшін мәндерді енгізу арқылы баға ұсыныстарын талдап, тұтынушының кесте мен бюджетке қатысты болжамдары үшін диаграммалар жасауға болады:

- Баға ұсыну тақырыбындағы **Сұралған жеткізу күні** өрісі.
- Әр баға ұсыну жолының **Тұтынушы бюджеті** өрісі (жобаға негізделген жолдар және өнімге негізделген жолдар үшін).

Тұтынушының кестеге қатысты болжамдарын талдау баға ұсыну жолы мәліметінің соңғы аяқталу күні мен баға ұсынудағы барлық баға ұсыну жолдары бойынша сұралған жеткізу күнін салыстыру арқылы жасалады.

Тұтынушының бюджетке қатысты болжамдарын талдау жалпы тұтынушы бюджетінің сомасын барлық баға ұсыну жолдары бойынша баға ұсыну сомасымен салыстыру арқылы жасалады.
