---
title: Несиелік карта бойынша транзакцияларды импорттау және сақтау
description: Бұл тақырып шығыспен байланысты несиелік карта транзакцияларын қалай импорттау және ұстану туралы түсіндіреді. Бұл транзакциялар автоматты түрде қайталанатын кесте бойынша импортталатындай етіп орнатылуы мүмкін немесе қажет болған жағдайда қолмен импортталуы мүмкін.
author: KimANelson
manager: AnnBe
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPbsMainDataLines
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 274023
ms.assetid: 3605eda1-a7ed-4675-8031-5279c5a8f5e4
ms.search.region: Global
ms.author: suvaidya
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: df5c6bce8a534f4f8b1872e2bd5cc8a58ef11189
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271585"
---
# <a name="import-and-maintain-credit-card-transactions"></a>Несиелік карта бойынша транзакцияларды импорттау және сақтау

Шығыспен байланысты несиелік карта транзакциялары автоматты түрде қайталанатын кесте бойынша импортталатын етіп орнатуға болады. Сонымен қатар қажет болған жағдайда транзакцияларды қолмен импорттауға болады. Несиелік карта бойынша транзакциялар несиелік карта бойынша транзакция деректері заңды тұлға арқылы импортталады.

Деректер нысандары туралы қосымша ақпаратты [Мәліметтер нысандары](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities) бөлімінен қараңыз.

## <a name="import-credit-card-transactions"></a>Несие картасының транзакцияларын импорттау

1. **Несие картасының транзакциялары** бетінде **Транзакцияларды импорттау** опциясын таңдаңыз. Егер сіз деректерді басқаруды бірінші рет ашып отырсаңыз, жалғастыру үшін жүйе деректер нысандарының тізімін жаңартуы тиіс.
2. **Атауы** өрісінде импорттау тапсырмасының бірегей сипаттамасын енгізіңіз.
3. **Дереккөз пішімі** өрісінде импортталатын несие картасының транзакцияларын қамтитын файл пішімін таңдаңыз.
4. **Жүктеп салу** түймесін таңдап, жүктеп салғыңыз келетін файлды тауып, тізімнен таңдаңыз.
5. Файл жүктелініп салынғаннан кейін, плиткадағы **Картаны қарау** сілтемесін таңдау арқылы несие картасымен жасалған транзакция файлының картасын және несие картасының транзакция деректерін салыстыру бағандарын тексеріңіз. Егер салыстыру қателіктері болса немесе салыстыруды өзгерту керек болса, **Салыстыруды визуализациялау** қойыншасынан немесе **Салыстыру мәліметтері** қойыншасынан өзгертуіңіз керек.
6. Несие карталарының транзакцияларын автоматтандыру үшін **Қайталанатын деректер тапсырмасын жасау** пәрменін таңдаңыз. Содан кейін несиелік картаның транзакциялары қаншалықты жиі импортталатынын анықтайтын қайталануды орнатуға болады. Аяқтаған кезде **OK** түймесін басыңыз.
7. Таңдалған файлды қазір импорттау үшін **Import** (Импорттау) опциясын таңдаңыз.
8. Егер импорттау кезінде қателіктер орын алса, сәтті импорттауға кепілдік беру үшін түзету керек қателерді көру үшін орындау журналын немесе кезеңдік деректерді қарауға болады.

> [!NOTE]
> Егер сіз бірнеше файл пішімін импорттауыңыз керек болса, әр пішін түрі үшін бөлек импорттау тапсырмаларын жасауыңыз керек.

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a>Қызметі тоқтатылған жұмысшылар үшін несиелік карта транзакцияларын қайта тағайындаңыз

Жұмысшының жазбасы тоқтатылғаннан кейін жұмысшының Active Directory Domain Services (AD DS) тіркелгісі өшіріледі. Дегенмен несиелік карта белсенді транзакциялар болуы мүмкін, олар әлі де шығындарға жазылып, өтелуі керек. **Несие картасының транзакциялары** бетінен байланысты жұмысшының тоқтатылған кез келген несие карта транзакциясы үшін жұмыскерді қайта тағайындай аласыз.

Несие картасымен бір немесе бірнеше транзакцияны таңдаңыз, содан кейін **Транзакцияларды қайта тағайындау** пәрменін таңдаңыз. Содан кейін несие картасымен транзакцияларды тағайындау үшін басқа жұмыскерді таңдауға болады. Несиелік карта транзакциялары қайта тағайындалғаннан кейін оларды шығыс туралы есеп үшін таңдап алуға болады және шығысты өтеу үшін әдеттегі процесс арқылы төлеуге болады.


[!INCLUDE[footer-include](../includes/footer-banner.md)]