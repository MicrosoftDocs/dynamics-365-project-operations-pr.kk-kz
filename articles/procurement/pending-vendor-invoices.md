---
title: Биржадан тыс материалдарды күтудегі жеткізуші есеп-шоты арқылы сатып алу
description: Бұл бөлімде күтудегі жеткізуші шот-фактураларын жазу жолы түсіндіріледі.
author: sigitac
ms.date: 09/13/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e95f7dabe597968707fdd2dead40bfb93d7f1f95
ms.sourcegitcommit: 74a7e1c9c338fb8a4b0ad57c5560a88b6e02d0b2
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/23/2021
ms.locfileid: "7547296"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a>Биржадан тыс материалдарды күтудегі жеткізуші есеп-шоты арқылы сатып алу

_**Келесіге қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Компания жоба үшін биржадан тыс материалдарды сатып алатындықтан, шығындар жобаға қатысты дереу жазылуы мүмкін. 

Мысалы, Contoso Robotics US компаниясы жабдықты жаңарту жобасын жүзеге асыруда және оған бағдарламалық жасақтама лицензиялары қажет. Бұл лицензиялар үшінші тарапты жеткізушіден сатып алынады.  Dynamics 365 Finance арқылы несие берушілермен есеп айырысу жөніндегі қызметкер жеткізушінің күтілетін шот-фактура құжатын жазады және лицензия шығындарын жабдықты жаңарту жобасына тікелей жатқызады. 

> [!IMPORTANT]
> Осы тақырыпта сипатталған функцияны пайдаланар алдында, қажетті конфигурацияларды қарап шығыңыз. Қосымша ақпарат алу үшін [Биржадан тыс материалдарды және күтудегі жеткізуші шот-фактуралары](configure-materials-nonstocked.md) тақырыбын қараңыз. 

## <a name="post-a-project-related-pending-vendor-invoice"></a>Жобаға қатысты күтудегі жеткізуші шот-фактурасы 

Күтудегі жеткізуші шот-фактуралары **Күтудегі жеткізуші шот-фактуралары** бетінде (**Несие берушілер** > **Шот-фактуралар** > **Күтудегі жеткізуші шот-фактуралары)** жазылуы мүмкін. Жобаға қатысты күтудегі жеткізуші шот-фактурасын орналастыру үшін келесі қадамдарды орындаңыз:

1. **Несие берушілер** > **Шот-фактуралар** және **Жаңа** опцияларын таңдаңыз. 
2. **Шот-фактура шоты** өрісінде жеткізушіні таңдап, **Нөмір** өрісінде жеткізушінің шот-фактура идентификациясын енгізіңіз.
3. Жеткізуші шот-фактурасына және **Элемент нөмірі** өрісіне жол қосып, жеткізушіден сатып алынған биржадан тыс элементті таңдаңыз. 

    > [!NOTE]
    > Сатып алу санатына негізделген жеткізуші шот-фактурасының жолдарын жобаға қарсы жазу мүмкін емес. 
    
5. Сатып алынған санын қосыңыз. Жүйе биржадан тыс элемент бағасының конфигурациясы негізінде бірлік бағасын толтырады. 
6. Жолдағы жалпы соманы және басқа қажетті мәліметтерді тексеріңіз.
7. Жол мәліметтерінде **Жоба** қойыншасында осы элемент жазылатын жобаның идентификаторын таңдаңыз.
8. Қажет болса, әрекет нөмірін таңдап, жоба санаты мен жол сипатын жаңартыңыз.
9. Күтудегі жеткізуші шот-фактурасын орналастырыңыз. Шот-фактура орналастырылған кезде жүйе келесілерді жазады:
    
    - Жеткізушінің қалдық сомасы.
    - Сатылым салығы сомасы.
    - Жоба бойынша шығындар сатып алуды біріктіру шотына жазылады.
    - Dataverse бағдарламасындағы жоба нақты құнының транзакциясы.  Бұл транзакция енді [Project Operations біріктіру журналы](../project-accounting/project-operations-integration-journal.md) арқылы өңделеді. Бұл журналды орналастыру сатып алуды біріктіру шотынан соманы жоба құны шотына ауыстырады. 
    - Уақыт пен материалдар бойынша шот ұсыну әдісі көмегімен жоба тұтынушысына шот ұсынылатын сатып алулар. Сонымен қатар Dataverse бағдарламасындағы сатып алулар үшін шот ұсынылмаған сатылым транзакциялары жасалады. Dataverse бағдарламасындағы өнім бағасының тізімі сатылым бағалары мен шот ұсынылмаған сатылым транзакциясының сомасы үшін пайдаланылады.