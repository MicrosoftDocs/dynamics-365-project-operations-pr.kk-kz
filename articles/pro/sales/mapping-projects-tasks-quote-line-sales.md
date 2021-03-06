---
title: Жобалар мен тапсырмаларды жобаға негізделген баға ұсыну жолымен салыстыру
description: Бұл тақырып жобалар мен тапсырмаларды жобаға негізделген тапсырмалар жолымен салыстыру туралы ақпарат береді.
author: rumant
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d726ab09da0e502da99191f7e7469c47f79b6e7c
ms.sourcegitcommit: 6b396ccf5e76230a42a2f933a3aaa5b8149790bb
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "3964914"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a>Жобалар мен тапсырмаларды жобаға негізделген баға ұсыну жолымен салыстыру

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Жобаға негізделген баға ұсыну жолдарында әлдеқашан баға ұсыну жолына байланысты жобаның нақты тапсырмаларын салыстыруға болады.

Тапсырмаларды баға ұсыну жолымен салыстырған кезде, баға ұсыну жолында анықтаған келесі элементтер тек осы тапсырмаларға қатысты болады:

- Төлем әдісі
- Төлем қабілеттілігі параметрлері
- Асырмау шектері
- Тұтынушылар

Мысалы, бір кезеңі белгіленген баға, ал қалған барлық кезеңдері уақыт пен материал болатын жоба болуы мүмкін. Бұл жағдайда бірінші кезеңді және оның барлық еншілес тапсырмаларын осы кезеңнің бекітілген бағаның төлем әдісімен баға ұсыну жолына байланыстыруға болады. Содан кейін барлық басқа кезеңдерді уақыт пен материалдарға негізделген баға ұсыну жолына байланыстыруға болады.

## <a name="associate-tasks-to-project-based-quote-lines"></a>Тапсырмаларды жобаға негізделген баға ұсыну жолдарымен байланыстыру

Тапсырмаларды келесі орындардан баға ұсыну жолдарымен байланыстыруға болады:

- **Жоба** беті > **Тапсырма шоты** қойыншасы (оңтайлы)
- **Баға ұсыну жолы** беті > **Ақылы тапсырмалар** қойыншасы 

### <a name="from-the-project-page"></a>Жоба бетінен:

**Жоба** беті тапсырмаларды баға ұсыну жолдарымен байланыстырудың оңтайлы тәжірибесін ұсынады. Бұл бетті бірнеше тапсырмаларды таңдау үшін және олардың барлығын, сонымен қатар олардың еншілес тапсырмаларын, таңдалған баға ұсыну жолымен байланыстыру үшін пайдалануға болады.

1. Жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасында **Жоба** өрісінің толтырылғанына көз жеткізіңіз.
2. **Қосылған тапсырмалар** өрісінде **Тек таңдалған тапсырмалар** түймешігін таңдаңыз.
3. Жобаға негізделген баға ұсыну жолын сақтаңыз. Пішін жаңарған кезде **Ақылы тапсырмалар** қойыншасы көрсетіледі.
4. **Жалпы** қойыншасында **Жоба** өрісінен жобаның сілтемесін таңдаңыз.
5. **Жоба** бетінде **Тапсырма шоты** қойыншасын таңдаңыз.
6. Тапсырмаға сәйкес шот ұсынысын орнатуға қолданылатын екінші торда бір немесе бірнеше тапсырмаларды таңдап, содан кейін **Баға ұсыну жолдарын байланыстыру** түймешігін таңдаңыз.
7. Пайда болған диалогтік бетте баға ұсынысында жобаға негізделген баға ұсыну жолдарын көрсететін баға ұсыну жолын таңдаңыз.
8. **Есеп-шот ұсыну түрі** өрісінде осы тапсырмалардың ақылы немесе ақысыз екендігін көрсетіңіз.
9. Байланысқа таңдалған тапсырмалардың еншілес тапсырмаларын қосу керектігін көрсету үшін құсбелгіні қойыңыз. Құсбелгіні қою таңдалған тапсырмалардың еншілес тапсырмаларын баға ұсыну жолымен байланыстырады.
10. Диалогтік терезені жабу үшін **OK** түймешігін таңдаңыз.

### <a name="from-the-quote-line-page"></a>Баға ұсыну жолы бетінен

Жоба тапсырмаларын баға ұсыну жолдарына **Баға ұсыну жолы** бетіндегі **Ақылы тапсырмалар** қойыншасынан байланыстыруға болады.

>[!NOTE]
>Жоба тапсырмаларын баға ұсыну жолдарына байланыстырудың оңтайлы орны - **Жоба** бетіндегі **Тапсырма шоты** қойыншасы. Тапсырмаларды **Баға ұсыну жолы** бетіндегі **Ақылы тапсырмалар** қойыншасынан байланыстырсаңыз, әр жобаны қолмен байланыстыру қажет.

1. Жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасында **Жоба** өрісінде жобаның таңдалғанына көз жеткізіңіз.
2. **Қосылған тапсырмалар** өрісінде **Тек таңдалған тапсырмалар** түймешігін таңдаңыз.
3. Жобаға негізделген баға ұсыну жолын сақтаңыз. Пішін жаңарған кезде **Ақылы тапсырмалар** қойыншасы көрсетіледі.
4. **Ақылы тапсырмалар** қойыншасында **Баға ұсыну жолының тапсырмасын қосу** түймешігін таңдаңыз.
5. **Баға ұсыну жолының тапсырмасы** бетіндегі **Тапсырмалар** өрісінде тапсырманы таңдаңыз және **Есеп-шот ұсыну түрі** өрісінде **Сақтау** түймешігін таңдаңыз. 
6. Бетті жабыңыз. Таңдалған тапсырма енді баға ұсыну жолымен байланысты.

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a>Тапсырмалардың жобаға негізделген баға ұсыну жолдарымен байланысын жою

### <a name="from-the-project-page"></a>Жоба бетінен:

Бұл әдіс тапсырмалардың баға ұсыну жолдарымен байланыстын жоюдың ең оңтайлы тәжірибесін ұсынады. Бірнеше тапсырмаларды таңдап, олардың барлығының, сонымен қатар олардың еншілес тапсырмаларының, таңдалған баға ұсыну жолымен байланысын жоюға болады.

1. Жобаға негізделген баға ұсыну жолының **Жалпы** қойыншасында **Жоба** өрісінде жоба сілтемесін таңдаңыз.
2. **Жоба** бетінде **Тапсырма шоты** қойыншасын таңдаңыз.
3. Тапсырмаға сәйкес шот ұсынысын орнатуға қолданылатын екінші торда бір немесе бірнеше тапсырмаларды таңдап, содан кейін **Баға ұсыну жолдарымен байланысты жою** түймешігін таңдаңыз.
4. Пайда болған диалогтік бетте баға ұсыну жолын таңдаңыз.
5. Байланысқа таңдалған тапсырмалардың еншілес тапсырмаларынан жою керектігін де көрсету үшін құсбелгіні қойыңыз. Құсбелгіні қою сондай-ақ таңдалған тапсырмалардың еншілес тапсырмаларының баға ұсыну жолымен байланысын жояды.
6. **OK** пәрменін таңдаңыз. Ескерту хабары осы байланысты жойсаңыз, тапсырмада бұрын жазылған кез келген нақты көрсеткішті қалпына келтіруге болатынын хабарлайды. 
7. Жалғастыру үшін **OK** түймешігін таңдап, тапсырма мен жобаға негізделген баға ұсыну жолы арасындағы байланысты жойыңыз.

### <a name="from-the-quote-line-page"></a>Баға ұсыну жолы бетінен

Сондай-ақ жоба тапсырмаларының баға ұсыну жолдарымен байланысын **Баға ұсыну жолы** бетіндегі **Ақылы тапсырмалар** қойыншасынан жоюға болады.

1. **Ақылы тапсырмалар** қойыншасында **Баға ұсыну жолының тапсырмасын жою** түймешігін таңдаңыз.
2. **OK** пәрменін таңдаңыз. Ескерту хабары осы байланысты жойсаңыз, тапсырмада бұрын жазылған кез келген нақты көрсеткішті қалпына келтіруге болатынын хабарлайды. 
3. Жалғастыру үшін **OK** түймешігін таңдап, тапсырма мен жобаға негізделген баға ұсыну жолы арасындағы байланысты жойыңыз.

>[!NOTE]
> Бұл процедура тапсырманы жобадан жоймайды. Ол тек тапсырмалардың жобаға негізделген баға ұсыну жолымен байланысын жояды.
