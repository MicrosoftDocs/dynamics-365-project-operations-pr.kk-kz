---
title: Компанияаралық есеп-шот ұсынуға шолу
description: Бұл тақырыпта жобалар үшін компанияаралық есеп-шот туралы ақпарат пен мысалдар келтірілген.
author: sigitac
ms.date: 11/19/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: c343c5bf525574e496036793cd4e131394e8b1b471153147a66cfebe1acf3fce
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "7005398"
---
# <a name="intercompany-invoicing-overview"></a>Компанияаралық есеп-шот ұсынуға шолу

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Ұйымыңызда жобалар бойынша бір-біріне өнімдер мен қызметтерді тасымалдайтын бірнеше бөлімдер, еншілес бөлімшелер және басқа заңды тұлғалар болуы мүмкін. Қызмет немесе өнімді ұсынатын заңды тұлға *несие беруші заңды тұлға* деп аталады. Қызмет немесе өнімді алатын заңды тұлға *несие алушы заңды тұлға* деп аталады.

Келесі кескінде екі заңды тұлға, Contoso Robotics USA (қарыз алушы заңды тұлға) және Contoso Robotics UK (несие беретін заңды тұлға) Adventure Works тұтынушысына жобаны ұсыну үшін ресурстарды бөлісетін әдеттегі сценарий көрсетілген. Осы сценарий үшін Contoso Robotics USA компаниясымен Adventure Works тұтынушысы үшін жұмысты орындау келісімшарты жасалды.

![Компанияаралық шот жіберу.](./media/IntercompanyScenario.png) 

Dynamics 365 Project Operations бағдарламасы компанияаралық транзакцияларды өңдеу үшін келесі ағынды пайдаланады:

1. Несие беруші заңды тұлға жазбасындағы ресурстар қарыз алушы заңды тұлғаның жобалары бойынша тапсырыс уақыты мен шығыстар арқылы компанияаралық уақытты немесе шығыс транзакцияларын есепке алады.
2. Уақыт пен шығыс құндары несие беруші компанияда несие алушы компанияның бірлігінің құн бағатізбесін пайдалану арқылы жазылады.
3. Компанияаралық шот ұсынылмаған сатылым транзакциялар несие беруші компанияда несие алушы компанияның бірлігінің құн бағатізбесін пайдалану арқылы жазылады.
4. Шот ұсынылмаған табыс несие алушы компанияда жобаның келісім-шарт сатылым бағатізбесін пайдалана отырып жазылады. Тұтынушыға шот ұсынылмаған табыс жазылған кезде шот ұсынылуы мүмкін. Тұтынушы компанияаралық есеп-шотты өңдеу аяқталғанша күтудің қажеті жоқ.
5. Компанияаралық тұтынушы есеп-шоттары кезеңдік негізде несие теруші компанияда жасалады. Есеп-шоттар қолмен немесе кезеңдік автоматтандырылған процесті пайдалану арқылы жасалады. Әрбір несие алушы заңды тұлға үшін бір есеп-шот немесе жеке есеп-шот жоба бойынша жасалуы мүмкін.
6. Компанияаралық тұтынушының есеп-шоты несие беретін заңды тұлғада жарияланған кезде, тиісті жеткізушінің күтілетін есеп-шоты несие алушы заңды тұлғада жасалады. Жеткізушінің күтілетін есеп-шотындағы құндар есеп-шот жарияланған кезде жоба қосалқы кітабына жазылады.

Төмендегі диаграмма бухгалтерлік оқиғаларға және бас кітапқа күтілетін орналастыруларға қатысты болғандықтан, компанияаралық есеп-шоттарды көрсетеді.

![Компанияаралық ағын.](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a>Қосымша ресурстар

- [Компанияаралық шот ұсынуды конфигурациялау](configure-intercompany-invoicing.md)
- [Компанияаралық транзакцияларды жазу](create-intercompany-transactions.md)
- [Тұтынушылар мен жеткізушілердің компанияаралық есеп-шоттарын жасау](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]