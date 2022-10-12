---
title: Қосалқы мердігерлерді тапсырыс беруге болатын ресурстар ретінде орнату
description: Бұл мақала жүйедегі пайдаланушылар мен контактілерден жасалған қосалқы мердігер ресурстарын қалай орнату және қолдау керектігін түсіндіреді, осылайша олар Microsoft жүйесіндегі қосалқы мердігерлермен байланыстырылады Dynamics 365 Project Operations.
author: rumant
ms.date: 09/14/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 727508c41c190c3703e9cd1420066fa0e551f147
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522708"
---
# <a name="set-up-subcontractors-as-bookable-resources"></a>Қосалқы мердігерлерді тапсырыс беруге болатын ресурстар ретінде орнату

_**Келесіге қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Microsoft Dynamics 365 Project Operations жүйесінде қосалқы мердігерлерді тапсырыс беруге болатын ресурстар ретінде орнату қадамдарын орындаңыз.

1. **Жоба**\> **Ресурстар** тармағына өтіп, **Жаңа** опциясын таңдаңыз.
2. **Жаңа тапсырыс беруге болатын ресурс** бетінде, **Ресурстар түрі** өрісінде келесі опциялардың бірін таңдаңыз:

    - **Пайдаланушы** — егер қосалқы мердігер уақытты немесе шығындарды енгізу үшін Project Operations қызметіне кіруі тиіс болса, осы ресурс түрін таңдаңыз. Егер **Пайдаланушы** опциясын таңдасаңыз, қосалқы мердігер жүйеге кіру үшін жарамды лицензияны қажет етеді.
    - **Контакт** немесе **Тіркелгі** — егер қосалқы мердігер Project Operations жүйесіне кіруді қажет етпесе, бірақ тапсырма тағайындау немесе жобаларға тапсырыс беру үшін қолжетімді болуы қажет болса, осы ресурстардың бірін таңдаңыз. Бұл ресурстардың ешқайсысы жүйеге кіруді қамтамасыз етпейді. Жеткізуші компаниясын тапсырыс беруге болатын ресурс ретінде көрсету үшін **Тіркелгі** опциясын таңдаңыз. Жеткізушінің жеке қызметкерлерін ұсыну үшін **Контакт** опциясын таңдаңыз.

3. Таңдалған ресурс түріне байланысты сәйкес пайдаланушыны, тіркелгіні немесе контакт жазбасын таңдау ұсынылады.
4. **Жұмысшы түрі** өрісінде қосалқы мердігерді тапсырыс беруге болатын ресурс ретінде орнату үшін "Келісімшарт жұмысшысы" опциясын таңдаңыз.

    > [!NOTE]
    > **Жұмысшы түрі** өрісі бос болса, тапсырыс беруге болатын ресурс қызметкер ретінде қарастырылады.

5. Егер жұмысшы түрі ретінде **Келісімшарт жұмысшысы** опциясын таңдасаңыз, ресурс жұмыс істейтін жеткізушіні таңдаңыз.
6. Ресурстың уақыт белдеуін таңдаңыз, содан кейін **Сақтау** опциясын таңдаңыз. Жұмыс уақыты үлгісін тапсырыс беруге болатын ресурсқа тағайындау үшін **Тапсырыс беруге болатын ресурс** тізім бетінде **Күнтізбені орнату** опциясын таңдауға болады.

Қосалқы келісімшарт жолы ресурсымен байланысу үшін тапсырыс беруге болатын ресурс мына шарттарға сәйкес болуы тиіс:

- Тапсырыс беруге болатын ресурс келісімшарт жұмысшысы болуы тиіс.
- **Контакт** ресурс түрінің тапсырыс беруге болатын ресурсы контакт ретіндегі жеткізуші тіркелгісімен байланысты болуы тиіс. **Пайдаланушы** ресурс түрінің тапсырыс беруге болатын ресурстың контакт ретіндегі жеткізуші тіркелгісімен байланысты болуы міндетті емес.
- Тапсырыс беруге болатын ресурстың **Жеткізуші** мәні қосалқы келісімшарттың **Жеткізуші** өрісінің мәніне сәйкес болуы тиіс.

## <a name="update-the-type-of-worker-and-vendor-mapping-for-bookable-resources"></a>Тапсырыс берілетін ресурстар үшін жұмысшы мен сатушының салыстыру түрін жаңартыңыз

Тапсырыс беруге болатын ресурстың **Жұмысшы түрі** өрісі тапсырыс беруге болатын ресурстың келісімшарт бойынша жұмысшы немесе қызметкер екенін анықтайды. **Сатушы** өрісі тапсырыс беруге болатын ресурс байланыстырылған жеткізуші тіркелгісін анықтайды. Тапсырыс беруге болатын ресурсты жеткізушімен контакт ретінде байланыстыра отырып, контактінің жеткізуші компаниясының қызметкері екенін көрсетесіз.

Егер **Жұмысшы түрі** және **Сатушы** өрістері тапсырыс беруге болатын ресурстың өрістері өзгертілсе, өзгертулер уақыт жазбалары секілді тапсырыс беруге болатын ресурс жасайтын жаңа жазбалардың келешектегі тексерулеріне әсер етеді. Алайда, өзгертулер бар жазбаларды жарамсыз етпейді.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]