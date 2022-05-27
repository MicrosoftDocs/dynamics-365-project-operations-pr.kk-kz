---
title: Белгіленген баға келісіміне нақты әсер ету
description: Бұл тақырып Microsoft корпорациясында тіркелген баға келісімінің өмірлік циклі кезіндегі әртүрлі оқиғалардағы Actuals кестесіне әсер ету туралы ақпаратты береді Dynamics 365 Project Operations.
author: rumant
ms.date: 02/22/2022
ms.topic: overview
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 222e7c5eefd7c619e4d7389cdaff2f96176ff275
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/14/2022
ms.locfileid: "8579235"
---
# <a name="actuals-impact-in-a-fixed-price-engagement"></a>Белгіленген баға келісіміне нақты әсер ету

_**Қолданылу аясы:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Төмендегі кестеде тіркелген баға келісіміндегі әртүрлі оқиғаларда жасалған әртүрлі транзакция түрлерінің нақты деректері берілген.

| Оқиға | Нақты құны | Шот ұсынылмаған сатылымның нақты мәні | Есептелген сату нақты | Мысал |
|---|---|---|---|---|
| Уақыт құрылды. | Қолданылмайды | Қолданылмайды | Қолданылмайды | <p>Сағатына 100 АҚШ доллары (100 АҚШ доллары) құны бар Fabrikam АҚШ ұйымдық бөлімшесінің қызметкері Боб Козак «Адатумда қаруды орнату» деп аталатын жобада жұмыс істеуде. Бұл жоба келісім-шарт жолында тіркелген бағаны есептеу әдісімен салыстырылады. Міне, Боб Козактың уақыт жазбасының үлгісі:</p><p>Боб Козак - 8 сағат</p> |
| Уақыт беріледі. | Қолданылмайды | Қолданылмайды | Қолданылмайды | Уақытты енгізу үшін шығындар журналы жолы жасалады. Әдепкі құн мөлшерлемесі журнал жазбасына енгізіледі. |
| Уақыт жазбасы бекітілгенге дейін кері қайтарылады. | Қолданылмайды | Қолданылмайды | Қолданылмайды | |
| Уақыт бекітілді. | Нақты шығындар жасалады. | Қолданылмайды | Қолданылмайды | <p>Жасалған жаңа нақты:</p><ul><li>**Нақты құны:** Боб Козак, 8 сағат, USD 800</li></ul> |
| Уақытты бекіту жойылды. | <p>Нақты бастапқы құнның түзету күйі жаңартылды **Түзетілген**.</p><p>Түзету күйі бар нақты қалпына келтіру құны жасалады **Реттелмейтін**.</p> | Қолданылмайды | Қолданылмайды | <p>Жаңартылған бар нақты:</p><ul><li>**Нақты құны:** Боб Козак, 8 сағ, USD 800, *Түзетілген*</li></ul><p>Бұрынғы қаржылық әсерді жою үшін жасалған жаңа нақты:</p><ul><li>**Нақты құны:** Боб Козак, (8 сағат), (800 АҚШ доллары), *Реттелмейтін*</li></ul> |
| Уақыт жазбасы бекітілгеннен кейін кері қайтарылады. | <p>Нақты бастапқы құнның түзету күйі жаңартылды **Түзетілген**.</p><p>Түзету күйі бар нақты қалпына келтіру құны жасалады **Реттелмейтін**.</p> | Қолданылмайды | Қолданылмайды | <p>Жаңартылған бар нақты:</p><ul><li>**Нақты құны:** Боб Козак, 8 сағ, USD 800, *Түзетілген*</li></ul><p>Бұрынғы қаржылық әсерді жою үшін жасалған жаңа нақты:</p><ul><li>**Нақты құны:** Боб Козак, (8 сағат), (800 АҚШ доллары), *Реттелмейтін*</li></ul> |
| Келісімшарт бекітілді. | <p>Ескі нақты шығындардың түзету күйі келесіге жаңартылды **Түзетілген**.</p><p>Түзету күйі бар қалпына келтіру құнының нақты деректері жасалады **Реттелмейтін**.</p><p>Жаңа нақты шығындар келісім-шарт ережелерін қайта бағалаудан кейін жасалады.</p> | Қолданылмайды | Қолданылмайды | <p>Жаңартылған бар нақты:</p><ul><li>**Нақты құны:** Боб Козак, 8 сағ, USD 800, *Түзетілген*</li></ul><p>Бұрынғы қаржылық әсерді жою үшін жасалған жаңа нақты:</p><ul><li>**Нақты құны:** Боб Козак, (8 сағат), (800 АҚШ доллары), *Реттелмейтін*</li></ul><p>Қайта бағаланған қаржылық әсер үшін жасалған жаңа нақты:</p><ul><li>**Нақты құны:** Боб Козак, 8 сағат, USD 800</li></ul> |
| Шот-фактура жасалады. | Қолданылмайды | Қолданылмайды | Қолданылмайды | |
| Шот-фактура кезеңмен расталады. | Қолданылмайды | Қолданылмайды | Жаңа кезеңге негізделген есептелген сату фактілері жасалады. | <p>Өзгеріссіз қалатын бар нақты:</p><ul><li>**Нақты құны:** Боб Козак, 8 сағат, USD 800</li></ul><p>Есептелген сату мәндерін жазу үшін жасалған жаңа нақты:</p><ul><li>**Есептелген сатудың нақты көлемі:** Маңызды кезең, USD 5,000</li></ul> |
| Шот-фактура маңызды кезеңді есепке алу үшін түзетіледі. | Қолданылмайды | Қолданылмайды | Кері шотталған сату фактілері жасалады. | <p>Өзгеріссіз қалатын бар нақты:</p><ul><li>**Нақты құны:** Боб Козак, 8 сағат, 800 USD</li></ul><p>Жаңартылған бар нақты:</p><ul><li>**Нақты есептелген сатылымдар:** Маңызды кезең, USD 5,000, *Түзетілген*</li></ul><p>Алдыңғы есептелген сату мәндерін өзгерту үшін жасалған жаңа нақты:</p><ul><li>**Нақты есептелген сатылымдар:** Маңызды кезең, (5 000 АҚШ доллары), *Реттелмейтін*</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]