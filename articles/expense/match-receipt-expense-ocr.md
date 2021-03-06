---
title: Түсімді шығысқа OCR арқылы сәйкестендіру
description: Осы тақырып түсімдерге таңбаларды оптикалық түрде тану (OCR) өңдеуі туралы ақпаратты ұсынады.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 02c1bafbe907a657689b610ae792f88085320903
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897008"
---
# <a name="match-a-receipt-to-an-expense-using-ocr"></a>Түсімді шығысқа OCR арқылы сәйкестендіру

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Шығыс жазбасы түсімдерге таңбаларды оптикалық түрде тану (OCR) өңдеуді кірістіру арқылы жақсартылды. Функционалдылық шығыс туралы есептерді жасаған кезде пайдаланушы тәжірибесін жақсартуға арналған.

## <a name="key-features"></a>Негізгі мүмкіндіктер

- Жүйе түсімнен сатушы атын, күнді және жалпы соманы алады.
- Жүйе тіркелмеген түсімдерді тіркелмеген түсімдер транзакцияларымен сәйкестендіруге тырысады.
- Сіз қолмен енгізілген шығыс транзакцияларын түсімдерден жасай аласыз.

## <a name="attach-receipts-to-an-expense-report"></a>Түсімдерді шығыс есебіне тіркеңіз

Шығыс туралы есеп жасалған кезде несиелік карта транзакцияларын қамтитын түсімдерді автоматты түрде тіркеу үшін келесі қадамдарды орындаңыз.

  1. **Шығысты басқару** жұмыс кеңістігін ашыңыз.
  2. **Түсімдер** қойындысында тіркелмеген түсімдердің бар екенін растаңыз. Түсімдерді **Түсімдер** қойындысына да жүктей аласыз.
  3.  **Шығыстар** қойындысында тіркелмеген шығыстардың бар екенін растаңыз. Әдетте шығыс әкімшісі бұл шығыстарды несиелік карта жеткізушісінен импорттайды.
  4. **Шығыс туралы есеп** опциясын таңдаңыз. Енді шығыс туралы есепті жасаған кезде шығыстарды, түсімдерді қоса алатыныңызды ескеріңіз. Егер сіз шығындарды да, түбіртектерді де қоссаңыз, түсімдерді шығындармен автоматты түрде сәйкестендіру іске қосылады.

## <a name="create-or-match-receipts-to-an-expense-report"></a>Түсімдерді шығыс туралы есепке сәйкестендіріңіз немесе жасаңыз
Шығысты жасау немесе түсімнен шығысты сәйкестендіру үшін келесі қадамдарды орындаңыз.

  1. Шығыс туралы есепте **Түсімдер** қойындысында **Түсімдерді қосу** таңдау арқылы түсімді тіркеңіз.
  2. Түсімнің жүктелген кескіні астында **Жасау** және **Сәйкестендіру** опцияларын ескеріңіз.

      - Қолмен енгізілген шығыс операциясын жасау және түсімнен алынған мәндерді толтыру үшін **Жасау** опциясын таңдаңыз.
      - Егер **Сәйкестендіру** опциясы таңдалса, жүйе бар шығысты түсіммен сәйкестендіруге тырысады.

## <a name="installation"></a>Орнату

Осы жетілдірілген шығыс мүмкіндіктерін пайдалану үшін Microsoft Dynamics 365 Finance бағдарламасы үшін шығысты басқару қызметі қондырмасын орнатыңыз және сіздің данаңыздағы мүмкіндіктерді қосыңыз. Microsoft Dynamics өмірлік цикл қызметтері (LCS) жүйесінде жобаңыздан қондырмаға кіруге болады.

1. LCS жүйесіне кіріп, қажетті ортаны ашыңыз.
2. **Толық мәліметтер** бөліміне өтіңіз.
3. **Ұстау** түймесін таңдаңыз немесе **Орта қондырмалары** FastTab қойындысына өтіңіз.
4. **Жаңа қондырманы орнату** опциясын таңдаңыз.
5. **Шығысты басқару қызметі** түймесін басыңыз.
6. Орнату нұсқаулығын ұстанып, шарттар мен талаптарға келісіңіз.
7. **Орнату** пәрменін таңдаңыз.

**Мүмкіндікті басқару** жұмыс кеңістігінде келесі мүмкіндіктерді қосыңыз:

- Шығыс туралы есептерге жаңа көзқарас
- Түсімдерден шығысты автоматты түрде сәйкестендіріңіз немесе жасаңыз

Осы мүмкіндіктерді қосқан кезде келесі әрекеттер орын алады:

- Қолданыстағы **Шығысты басқару** жұмыс кеңістігі жаңа жұмыс кеңістігімен ауыстырылды.
- Шығыс өрісінің көрінуіне арналған мәзірдің жаңа тармағы қосылды.
- **Шығысты басқару > Менің шығыстарым > Шығыс туралы есептер** жолы арқылы бұрынғы **Шығыс туралы есеп** бетін аша аласыз.
- Жұмыс ағындары және кез келген растау сізді шығыс туралы есептер бетіне апарады.
- Түсімдер Microsoft Azure Cognitive Services қызметі арқылы өңделеді және метадеректер алынып, қосылады.
- Сәйкес тіркелмеген түбіртектерді қамтитын шығыс туралы есеп жасауға мүмкіндік беретін опция қосылды.
- Шығыс туралы есептерге қосылатын опция түсімнен шығыс бабын жасауға мүмкіндік береді немесе бар түсімдерді қолданыстағы шығыс бабына сәйкестендіруге тырысады.

## <a name="frequently-asked-questions"></a>Жиі қойылатын сұрақтар

**Microsoft өз үлгілері үшін менің деректерімді пайдаланады ма?**

Жоқ, Microsoft түсімді өңдеу қызметі үшін жалпы машиналық оқыту үлгісін құрды. Бұл үлгі сіз жүктеген түсімдерге негізделмеген.

**Бұл мүмкіндік қайда қолжетімді және қайда өңделеді?**

Қазіргі уақытта Америка Құрама Штаттарына қолдау көрсетіледі.

**Менің түсімдерім қайда жіберіледі?**

Finance бағдарламасы өріс деректерін шығару үшін Cognitive Services қызметтерімен байланысады. Cognitive Services өңдеу кезінде сіздің түсіміңіздің көшірмесін 24 сағатқа дейін сақтайды. Өңдеу аяқталғаннан кейін Cognitive Services түсімдерді жояды. Түбіртектер әлі де Finance жүйесінде сақталады.

Толық ақпарат алу үшін Form Recognizer қызметінің жаңа мүмкіндігімен түсімді түсінуді қосу бөліміне өтіңіз: [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).
