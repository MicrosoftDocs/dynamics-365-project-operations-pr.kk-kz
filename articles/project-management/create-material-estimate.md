---
title: Жобалар бойынша материалдарға қатысты қаржылық болжамдар
description: Бұл мақалада жобаға негізделген материалдарды анықтау немесе бағалау туралы ақпарат берілген.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: eb33c8e2ead2a558bf53256095645011212ff343
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925708"
---
# <a name="financial-estimates-for-materials-on-projects"></a>Жобалар бойынша материалдарға қатысты қаржылық болжамдар

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Dynamics 365 Project Operations бағдарламасы жоба менеджерлеріне әр жоба немесе тапсырма бойынша жобалық материалдар құнын анықтауға мүмкіндік береді. Әрбір материал болжамын белгілі бір жоба тапсырмасымен байланыстыруға болады. Жобаларда қолданылатын материалдар жазылатын өнімдер немесе өнім каталогындағы өнімдер болуы мүмкін. Өнім мен бірліктің әрбір комбинациясы үшін бағаны сатуға арналған жобаның прейскуранттарында және өзіндік құн бойынша жобаның прейскуранттарында анықтауға болады.  

Жобалық материал болжамын қарау, қосу немесе жою үшін келесі әрекеттерді орындаңыз.

1. **Жобалар** бетіне өтіп, жаңартқыңыз келетін жобаны таңдаңыз.
2. **Материал болжамдары** қойыншасында жобалық материал болжамдарының тізімін қараңыз.
3. Жаңа материал болжамын жасау үшін **Жаңа материал болжамы** опциясын таңдаңыз. Немесе жойылатын материал болжамын таңдап, **Материал болжамын жою** опциясын таңдаңыз.

Келесі кестеде жобадағы **Материал болжамының жолы** туралы ақпарат берілген. 

| **Өріс** | **Сипаттамасы** | **Төменгі әсер** |
| --- | --- | --- |
| Тапсырма | Жобадағы тапсырмалардың тізімі. Бұл қорытынды мен соңғы түйін бойынша тапсырмаларды қамтиды. | Материалды бағалау жолы үшін тапсырманы таңдау, болжалды материал құны мен тапсырмаға арналған болжалды материал сатылымына әсер етеді. Егер бұл өріс бос болса, материал болжамы тек жоба деңгейінде бақыланады және қорытындылады. |
| Өнім таңдау |  Осы болжам жолы бұрыннан бар (каталог) немесе енгізілген өніміне арналғанын көрсетуге болады. | Бұл өріс өнімді каталогтан немесе енгізілген өнімді таңдайтыныңызды анықтайды. |
| Өнім  | Өнім каталогындағы өнімнің идентификаторы. Өнім идентификаторын таңдаған кезде **Өнімді таңдаңыз** өрісіндегі мән **Бұрыннан бар өнім** мәніне автоматты түрде жаңартылады. Идентификатор баға мен сату бағасын бағатізбеден алу үшін қолданылады. | Бұл өріс үшін төменгі әсері жоқ. |
| Енгізілген өнім сипаттамасы | Өнімнің атын жазуға арналған мәтін өрісі. Бұл өріс тек **Өнімді таңдаңыз** өрісінде **Енгізілген** өнімін таңдаған кезде пайдаланылуы тиіс.| Бұл өріс үшін төменгі әсері жоқ. |
| Басталу күні | Материал пайдаланылатын болжалды күн. | Бұл өріс үшін төменгі әсері жоқ. |
| Бірлік тобы | Бұл өрістегі әдепкі мән каталог өнімінде әдепкі бірліктер тобынан алынады. Бұл өрісті басқа бірлік тобын таңдау үшін жаңартуға болады. | Бұл өріс үшін төменгі әсері жоқ. |
| Бірлік | Бұл өрістегі мән таңдалған өнімнің әдепкі бірлігінен алынады. Бұл өрісті басқа бірлікті таңдау үшін жаңартуға болады. | Әртүрлі бірлік бағасы мен құнда бірлік нәтижелерін өзгерту. |
| Шама | Жобада пайдаланылатын өнімнің болжалды саны. | Бұл өріс үшін төменгі әсері жоқ. |
| Бірлік құны | Қолданылатын шығын бағатізбелерінде белгіленген таңдалған өнім мен бірлік тіркесімінің бірлік құны. | Бірлік құны әрқашан жобаның өзіндік құнымен көрсетіледі. Егер бағатізбеде біріккен өнім мен бірлік орнатылымы үшін бірлік құны орнатылмаса, бірлік құны 0,00 мәніне дейін әдепкі болады. |
| Бірлік бағасы | Қолданылатын сатылым бағатізбелерінде белгіленген таңдалған өнім мен бірлік тіркесімінің бағасы. | Бірлік бағасы әрқашан жобаның сатылым валютасымен көрсетіледі. Егер бағатізбеде біріккен өнім мен бірлік орнатылымы үшін бірлік бағасы орнатылмаса, бірлік бағасы 0,00 мәніне дейін әдепкі болады.|
| Жалпы құны | Мөлшер \* бірлік құны ретінде есептелген құн мөлшері.| Құн мөлшері әрқашан жобаның өзіндік құнымен көрсетіледі. |
| Жалпы сатылым | Мөлшер \* бірлік бағасы ретінде есептелген сатылым мөлшері. | Сатылым мөлшері әрқашан жобаның сатылым валютасымен көрсетіледі. |


[!INCLUDE[footer-include](../includes/footer-banner.md)]