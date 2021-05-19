---
title: Ішкі жобалар үшін есепті конфигурациялау
description: Бұл тақырып Project Operations жүйесінде ішкі жобалар үшін бухгалтерлік есеп тәжірибелерін құру жолдары туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 65d05e3a6321dc32aee55c28b3eaa4bd0bae2f86
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "5857985"
---
# <a name="configure-accounting-for-internal-projects"></a>Ішкі жобалар үшін есепті конфигурациялау

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Ішкі жобалар компанияларға тұтынушыға есеп айырыспайтын әрекеттерге байланысты шығындарды бақылауға мүмкіндік береді. Ішкі жобалардың мысалдары:

- Мобильді құрылғы бағдарламасы сияқты өнімді әзірлеу және оны әзірлеуге байланысты шығындарды қадағалау.
- Сату алдындағы уақыт пен шығындарды басқару. Бұл сату алдындағы ішкі жоба, егер баға ұсынысы жеңіске жетсе, кейінірек ақылы жобаға айналуы мүмкін.

Dynamics 365 Project Operations бағдарламасында келісім-шартпен байланысты емес кез келген жоба ішкі ретінде қарастырылады. Жоба құны мен түсім профильдері жоба бойынша есеп ережелерін анықтау үшін пайдаланылмайды. Жобаның ішкі құны әрқашан пайда мен шығын ережелерін пайдалана отырып орналастырылады. Енгізу деректеріне арналған бухгалтерлік кітап шоттары **Бас кітапқа енгізу деректерін орнату** бетінде анықталады.

- Мерзімдік мәмілелер **Шығын** шотын дебеттеп, сондай-ақ **Жалақының жалпы сомасын бөлу** шотын есептеу арқылы орналастырылады.
- Шығыс операциялары **Шығын** шотын дебеттеп, сондай-ақ **Шығыстың өтемақы шотын** есептеу арқылы орналастырылады.
- Элемент транзакциялары **Құны** тіркелгісін дебеттеу және **Құны - элемент** тіркелгісін кредиттеу арқылы орналастырылады.

Операциялар жобаға орналастырылғаннан кейін, егер жоба жобалық келісім-шартпен байланысты болса, жүйе барлық жинақталған операцияларды кері қайтарып, жаңа ақылы операцияларды жасайды. Ақылы операциялар жобаның шығындары мен кірістерінің тиісті профилінде айқындалған бухгалтерлік есеп ережелеріне сәйкес орындалады.




[!INCLUDE[footer-include](../includes/footer-banner.md)]