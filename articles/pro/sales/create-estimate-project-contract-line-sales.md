---
title: Жобаға негізделген келісім-шарт жолын есептеңіз - жеңілдетілген
description: Бұл тақырып жобаға негізделген келісім-шарт жолын есептеу туралы ақпарат береді.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: bf7941a627375604dca778ab293756bed2536049
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858096"
---
# <a name="estimate-a-projectbased-contract-line---lite"></a>Жобаға негізделген келісім-шарт жолын есептеңіз - жеңілдетілген

_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_

Dynamics 365 Project Operations бағдарламасында жобаға негізделген келісім-шарт жолының келісім-шарт жолын жеткізуге қатысатын жұмыстың құнын және ықтимал табысын есептеуге көмектесетін мәліметтер бар.

Жоба негізіндегі келісім-шарт жолын есептеу үшін жоба негізіндегі **Келісім-шарт жолы** ішінде **Келісім-шарт жолы мәліметтері** қойыншасына өтіңіз.  Жоба негізіндегі келісім-шарт жолы бойынша есепті жасаудың екі әдісі бар:

   - Есепті келісім-шарт жолының мәліметтерін қолмен қосу арқылы тікелей келісім-шарт жолында жасаңыз.
   - Жоба мен жоба жоспарын жасаңыз, содан кейін жоба мен тапсырмаларды жобаның келісім-шарт жолымен байланыстырыңыз. Бұл келісім-шарт жолында қамтылған құрамдастар негізінде жоба жоспарының есебін келісім-шарт жолына импорттауға болатын процесті іске қосады.

## <a name="create-an-estimation-directly-on-a-projectbased-contract-line"></a>Есепті тікелей жобаға негізделген келісім-шарт жолында жасаңыз

Болжамды тікелей жобаға негізделген келісім-шарт жолына жасау үшін келесі қадамдарды орындаңыз:

1. Келісім-шарт жолына өтіп, **Келісім-шарт жолы мәліметтері** қойындысын таңдаңыз. Қойыншада жасалған жолдар жинақталып, осы **Келісім-шарт желісі** үшін **Келісім-шарт мәні** ретінде көрсетіледі. 
2. **Келісім-шарт жолы мәліметтері** қосалқы торында **Жаңа келісім-шарт жолының мәліметтері** параметрін таңдаңыз. Жылдам жасау жүгірткісі ашылады. **Келісім-шарт жолы мәліметтері** бетінде келесі өрістер қолжетімді.

| Өріс | Орналасқан жері | Сипаттамасы | Төменгі әсер |
| --- | --- | --- | --- |
| **Сипаттамасы** | **Жылдам жасау** | Арнайы болжам сипаттамасы. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Транзакция класы** | **Жылдам жасау** | Бұл транзакциялық жіктемелердің тізімі жобаға негізделген келісім-шарт жолындағы **Жалпы мәліметтер** қойыншасында қамтылған. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Өнім таңдау** | **Жылдам жасау** | Транзакция класы **Материал** болған кезде қолданылады. Осы болжам жолы **Бұрыннан бар** (каталог) өнім немесе **Енгізілген** өніміне арналғанын көрсетуге болады. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Өнім** | **Жылдам жасау** | Өнім каталогындағы өнімнің идентификаторы. Бұл өріс тек **Өнімді таңдаңыз** өрісінде **Бұрыннан бар өнім** өнімін таңдаған кезде қолжетімді болады. Идентификатор сату бағасын келісім-шарттағы сатылым жобасының бағатізбесінен алу үшін қолданылады. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Енгізілген өнім** | **Жылдам жасау** | Өнімнің атын енгізу арналған мәтін өрісі. Бұл өріс тек **Өнімді таңдаңыз** өрісінде **Енгізілген** өнімін таңдаған кезде қолжетімді болады.| Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Рөл** | **Жылдам жасау** | Осы жұмысты орындап жатқан немесе осы шығысты төлейтін адамның рөлі. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді.|
| **Санат** | **Жылдам жасау** | Жұмыстың немесе шығыстың санаты. |Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді.|
| **Басталу күні** | **Жылдам жасау** | Жұмыстың басталу күні. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Аяқталу күні** | **Жылдам жасау** | Жұмыстың аяқталу күні. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Ресурс бірлігі** | **Жылдам жасау** | Бұл шығындарға әкелетін және онымен жұмыс істеу үшін ресурстарды қамтамасыз ететін ресурстар бірлігі. |Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді және шығын алуда пайдаланылады. |
| **Бірлік кестесі** | **Жылдам жасау** | Жұмыс, өнім немесе шығынның бірлік тобы. Бірліктер бірлік кестесіне немесе бірліктер тобына тиесілі. Мысалы, *миль* және *километр (км)* қашықтықты сипаттайтын бірліктер тобына жататын бірліктер болып саналады. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Бірлік** | **Жылдам жасау** | Жұмыс, өнім немесе шығын бірлігі. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Шама** | **Жылдам жасау** | Жұмыс, өнім немесе шығын саны. | Бұл мән автоматты түрде жасалатын шығындар үшін сәйкес келісім-шарт жолы мәліметіне сәйкес келеді. |
| **Бірлік бағасы** | **Жылдам жасау** | Жұмысты орындайтын рөлдің есеп-шот мөлшерлемесі немесе өнімнің бірлік бағасы не өнімнің сатылым бағасы немесе шығын санаты. **Уақыт** параметріне арналған осы өрістің әдепкі мәндері басталу күнінен бастап күшіне енетін жобаның бағатізбесіндегі рөлдің баға жолындағы баға өлшемі мәндерінің тіркесіміне негізделген. **Шығындар** үшін бұл өрістің әдепкі мәні басталу күнінен бастап күшіне енетін жобаның бағатізбесіндегі транзакция санаты үшін бағаны орнатудан алынады. Егер транзакция санатындағы бағалау әдісі **бірлік бағасы** мәніне сәйкес болмаса, әдепкі шарт жоқ және бұл өріс бос қалдырылады. Өнімдер үшін осы өрістің әдепкі мәні басталу күнінен бастап күшіне енетін жоба бағатізбесіндегі **Бағатізбе элементі** жолына негізделген.| Жұмысты орындайтын рөлдің шығын мөлшерлемесі немесе шығындар санаты бірлігінің құны немесе өнімнің бірлік құны. Бұл өріс әдепкі бойынша басталу күнінен бастап күшіне енетін келісім-шарт бірлігіне бекітілген құн бағатізбесіндегі рөлдің баға жолындағы баға өлшемі мәндерінің тіркесімі негізінде **Уақыт** мәніне орнатылады. Шығындар үшін бұл өрістің әдепкі мәні басталу күнінен бастап күшіне енетін келісім-шарт бірлігіне тіркелген шығын бағатізбесінің санат бағасы жолына негізделеді. Егер транзакция санатындағы бағалау әдісі бірлік бағасына сәйкес болмаса, әдепкі шарт жоқ және бұл өріс бос қалдырылады. Өнімдер үшін бұл өрістің әдепкі мәні басталу күнінен бастап күшіне енетін құн бағатізбесіндегі **Бағатізбе элементі** жолына негізделген.|
| **Болжалды салық** | **Жылдам жасау** | Осы жұмыс немесе шығындар үшін болжалды салық. | Осы жұмыс немесе шығындар үшін болжалды салық. |
| **Сомасы** | **Жылдам жасау** | Бұл өрістегі мәнді **Саны** және **Бағасы** өрістері бос қалдырылған болса қосуға болады. **Саны** және **Бағасы** өрістері толтырылған болса, **Сома** өрісі тек оқуға арналады және **(Саны \* Бірлік бағасы) + Салық** бойынша есептеледі. | &nbsp; |

## <a name="update-prices-on-contract-line-details"></a>Келісім-шарт жолының мәліметтеріндегі бағаларды жаңарту

Келісім-шартқа немесе келісім-шарт бірлігінің құн бағатізбесіне тіркелген жоба бағатізбесіндегі бағаларды өзгертсеңіз, өзгерісті көрсету үшін жеке келісім-шарт жолының мәліметтеріндегі бағаларды жаңарта аласыз. **Келісім-шарт** бетінде **Қайта есептеу** пәрменін таңдаңыз. Осы келісім-шарттағы барлық келісім-шарт жолдары қалпына келтірілгені туралы ескерту пайда болады. Сатылым және құн келісім-шарт жолының мәліметтерінің бағаларын жаңарту үшін **Иә** параметрін таңдаңыз.

## <a name="access-contract-line-details-for-cost"></a>Құн бойынша келісім-шарт жолының мәліметтеріне кіру

**Келісім-шарт жолының мәліметтері** қойыншасында қосалқы тордың құралдар тақтасындағы әрекеттерді көрсету үшін тордың ішіндегі жолды таңдаңыз. Қосалқы тор құралдар тақтасындағы бірінші әрекет — **Шығын мәліметін ашу**. Осы келісім-шарт жолының мәліметі үшін қатысты құн мөлшерлемесін және сомасын көру үшін **Шығын мәліметін ашу** параметрін таңдаңыз. 

> [!NOTE]
> **Құны** өрісі үшін ресурс компаниясын, ресурс бірлігін, санын, күндерді, рөлді немесе келісім-шарт жолының мәліметіндегі санат мәндерін өзгерту **Сатылым** өрісі үшін келісім-шарт жолының мәліметіндегі сәйкес мәндерді өзгертеді.

## <a name="currency-on-contract-line-details-for-cost-and-sales"></a>Құн мен сатылым бойынша келісім-шарт жолының мәліметіндегі валюта

**Сатылым** өрісі үшін келісім-шарт жолының мәліметі әдепкі валютаны келісім-шарт жолы мәліметінің басталу күнінен бастап күшіне енетін жобаның бағатізбесінен белгілейді.

**Құн** өрісі үшін келісім-шарт жолының мәліметі әдепкі валютаны **Құн** өрісі үшін келісім-шарт жолы мәліметінің басталу күнінен бастап күшіне енетін келісім-шарттың келісім-шарт бірлігінің бағатізбесінен белгілейді.

Келісім-шарттағы жалпы нақты және болжалды шектерді есептеу мақсатында табыс есептеулері келісім-шарт жолының мәліметтері үшін сомаларды **Құн** және **Сатылым** өрістері үшін ортаның негізгі валютасына түрлендіреді.

> [!NOTE]
> Валюталарды дөңгелектеу қателері және өзгертілген шектер жарамды күн бойынша айырбас бағамдарының жеткіліксіз болуына байланысты орын алуы мүмкін. Бұл есептеулерді тек жобалық келісім-шарттарда пайдаланыңыз, өйткені бұл есептеулер шамамен алынған және нақты заңды немесе басқа есеп беру үшін қажет емес, бұл дөңгелектеудің жоғары дәлдігін және валюта бағамдары үшін күннің тиімділігі туралы білуді қажет етеді.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]