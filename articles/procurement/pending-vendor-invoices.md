---
title: Күтудегі жеткізушінің шот-фактурасын пайдаланып қорда жоқ материалдарды немесе сатып алу санаттарын сатып алыңыз
description: Бұл мақала күтудегі жеткізушінің шот-фактураларын қалай жазу керектігін түсіндіреді.
author: sigitac
ms.date: 09/13/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: b1c05755f6759e90e031a11261f15a2c4b6b716e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921999"
---
# <a name="purchase-non-stocked-materials-or-procurement-categories-using-a-pending-vendor-invoice"></a>Күтудегі жеткізушінің шот-фактурасын пайдаланып қорда жоқ материалдарды немесе сатып алу санаттарын сатып алыңыз

_**Қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Компания жоба үшін қорда жоқ материалдарды немесе сатып алу санаттарын сатып алатындықтан, шығындар жобаға қарсы бірден жазылуы мүмкін. 

Мысалы, Contoso Robotics US компаниясы жабдықты жаңарту жобасын жүзеге асыруда және оған бағдарламалық жасақтама лицензиялары қажет. Бұл лицензиялар үшінші тарапты жеткізушіден сатып алынады.  Dynamics 365 Finance көмегімен Кредиторлық берешектің қызметкері күтудегі жеткізушінің шот-фактура құжатын жазады және лицензия шығындарын жабдықты жаңарту жобасына тікелей жатқызады. 

> [!IMPORTANT]
> Осы мақалада сипатталған функцияны пайдаланбас бұрын, қажетті конфигурацияларды қарап шығыңыз және қолданыңыз. Қосымша ақпаратты қараңыз [Қорда жоқ материалдарды және күтудегі жеткізушінің шот-фактураларын қосыңыз](configure-materials-nonstocked.md) және [Сатып алу санаттарын жобалық сатып алу тапсырыстарымен және күтудегі жеткізушінің шот-фактураларымен пайдаланыңыз](configure-procurement-categories.md)

## <a name="post-a-project-related-pending-vendor-invoice"></a>Жобаға қатысты күтудегі жеткізуші шот-фактурасы 

Күтудегі жеткізуші шот-фактуралары **Күтудегі жеткізуші шот-фактуралары** бетінде (**Несие берушілер** > **Шот-фактуралар** > **Күтудегі жеткізуші шот-фактуралары)** жазылуы мүмкін. Жобаға қатысты күтудегі жеткізуші шот-фактурасын орналастыру үшін келесі қадамдарды орындаңыз:

1. Бару **Кредиторлық қарыз** > **Шот-фактуралар**, және таңдаңыз **Жаңа**. 
1. Ішінде **Шот-фактура шоты** өрісінде жеткізушіні таңдаңыз, содан кейін ішінде **Сан** өрісінде сатушы шот-фактурасының сәйкестендіруін енгізіңіз.
1. Жеткізуші шот-фактурасына жолды, содан кейін жолды қосыңыз **Заттың нөмірі** өрісінде сатушыдан сатып алынған қоймада жоқ элементті таңдаңыз. Немесе, в **Сатып алу санаты** өрісінде сатушыдан сатып алынған сатып алу санатын таңдаңыз.   
1. Сатып алынған соманы қосыңыз. Жүйе қоймада жоқ тауар бағасының конфигурациясына негізделген бірлік бағасын толтырады. 
1. Жолдағы жалпы соманы және басқа қажетті мәліметтерді тексеріңіз.
1. Жол мәліметтерінде, бетінде **Жоба** қойындысында осы элемент жазылатын жобаның идентификаторын таңдаңыз.
1. Қосымша: әрекет нөмірін таңдап, жоба санаты мен жол сипатын жаңартыңыз.
1. Күтудегі жеткізушінің шот-фактурасын жіберіңіз. Шот-фактура жарияланған кезде жүйе келесі ақпаратты жазады:
    
    - Жеткізушінің қалдық сомасы.
    - Сатылым салығы сомасы.
    - Жоба бойынша шығындар сатып алуды біріктіру шотына жазылады.
    - Dataverse бағдарламасындағы жоба нақты құнының транзакциясы.  Бұл транзакция енді [Project Operations біріктіру журналы](../project-accounting/project-operations-integration-journal.md) арқылы өңделеді. Бұл журналды орналастыру сатып алуды біріктіру шотынан соманы жоба құны шотына ауыстырады. 
    - Уақыт пен материалдар бойынша шот ұсыну әдісі көмегімен жоба тұтынушысына шот ұсынылатын сатып алулар. Сонымен қатар Dataverse бағдарламасындағы сатып алулар үшін шот ұсынылмаған сатылым транзакциялары жасалады. Dataverse бағдарламасындағы өнім бағасының тізімі сатылым бағалары мен шот ұсынылмаған сатылым транзакциясының сомасы үшін пайдаланылады.