---
title: Заманауи мақұлдауларға арналған жаңартулар
description: Мақалада әкімшілер Заманауи бекітулер функциясын қосқанда ескеруі керек мәселелер қарастырылады.
author: stsporen
ms.date: 01/31/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 44a933c92d4ef8dff40f20200d74c4bbdf8caa76
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931751"
---
# <a name="upgrade-considerations-for-modern-approvals"></a>Заманауи мақұлдауларға арналған жаңартулар 

_**Келесіге қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

2022 жылдың сәуір айындағы 1-толқын шығарылымының бөлігі ретінде Заманауи бекітулер функциясы әдепкі бойынша қосылады. Бұл функция бекіту логикасының сенімділігін жақсартады және бекіту логикасы сәтсіз болған жағдайда оның себебін анықтауға мүмкіндік береді.

Осы өзгертудің бөлігі ретінде жобаны бекітуге арналған күй өзгерістері жаңартылады. Күй енді мына жерден шығады **Жіберілді** дейін **Бекітілген**. **Күтуде** бұдан былай мақұлдау мәртебесі емес. Бекіту күтілуде екенін анықтау үшін мақұлдау мақұлдау жиынының бөлігі екенін және тіркелген бекіту жиынының күйін қарап шығыңыз.

## <a name="before-you-upgrade"></a>Жаңарту алдында

Заманауи мақұлдауларға жаңартпас бұрын, күтпеген мақұлдауларыңыз жоқ екеніне көз жеткізіңіз. Қазіргі мақұлдаулар қолданбайды **Күтуде** күй. Сондықтан әлі де белгіленген рұқсаттар **Күтуде** жаңартудан кейін өңделмейді.

## <a name="after-you-upgrade"></a>Жаңартқаннан кейін

Заманауи мақұлдауларға жаңартқаннан кейін әкімші бекітулерді өңдейтін бұлт ағынының қосылғанын тексеруі керек.

1. кіру [flow.microsoft.com](https://flow.microsoft.com)
2. Беттің жоғарғы оң жағында ортаңызды жаңартылған ортаға ауыстырыңыз.
3. таңдаңыз **Шешімдер** ортада орнатылған шешімдерді тізімдеу үшін.
4. Шешім тізімінде таңдаңыз **Жоба операциялары** немесе **Жоба қызметі**.
5. Сүзгіні келесіден өзгертіңіз **Барлық** дейін **Бұлт ағындары**.
6. екенін тексеріңіз **Жоба қызметі – Жобаны мақұлдау жиындарын қайталап жоспарлау** опциясы орнатылған **Қосулы**. Егер олай болмаса, ағынды таңдап, содан кейін таңдаңыз **Қосу**.
7. шолу арқылы өңдеудің әрбір бес минут сайын орындалатынын тексеріңіз **Жүйе тапсырмалары** ішіндегі тізім **Параметрлер** аумақ.

## <a name="short-term-rollback"></a>Қысқа мерзімді кері қайтару

Өзгерістерді қабылдай алмасаңыз немесе осы мүмкіндікке қатысты күрделі мәселеге тап болсаңыз, келесі қадамдарды орындау арқылы бастапқы бекіту ағынына уақытша оралуға болады:
1. Ортаңызға кіріп, күтудегі мақұлдаулардың жоқтығын тексеріңіз.
2. Бару **Параметрлер** > **Жоба параметрлері**.
3. таңдаңыз **Функцияны басқару** содан кейін таңдаңыз **Заманауи бекітулер** мүмкіндікті өшіру үшін.

## <a name="removing-the-feature-flag"></a>Мүмкіндік жалаушасын жою

2022 жылдың қазан айындағы 2-толқын жаңартуында бұл мүмкіндікті өшіру мүмкіндігі жойылады.

[!INCLUDE[footer-include](../includes/footer-banner.md)]