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
ms.openlocfilehash: 6ed900620f92e76d293f6b533b101be94b25cff3
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127030"
---
# <a name="analysis-of-project-quotes"></a>Жобаның баға ұсыныстарын талдау

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
