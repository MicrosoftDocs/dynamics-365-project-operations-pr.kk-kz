---
title: Тапсырыс беруге болатын ресурс жобадағы бірнеше рөлді орындаған кезде, жоба сатылымдары мен шығындарын болжау
description: Бұл тақырыпта жобада бірнеше рөлді орындайтын ресурс үшін баға мен шығындар болжамын қолдау үшін баға өлшемдерін пайдалану жолы түсіндірілген.
author: rumant
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 28a67e79b03dfbc38e9786350c931838ef27891a3d26787fc0334e0572528228
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "6990143"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-on-a-project"></a>Тапсырыс беруге болатын ресурс жобадағы бірнеше рөлді орындаған кезде, жоба сатылымдары мен шығындарын болжау 

_**Келесіге қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі, қосалқы/өндіріске негізделген сценарийлеріне арналған Project Operations_ 

Жобаға негізделген компаниялар көбінесе жобада бірнеше рөлді орындау үшін бір ресурсты қажет етеді. Әр рөл әртүрлі бағалануы мүмкін. Бұл дегеніміз, жобадағы бір ресурстың уақыты әр рөл үшін төлем мен шығындар мөлшерлемелеріне байланысты әртүрлі қаржылық болжамды ала алады. Топ мүшесінің жазбасында мәндерді топ мүшесіне тағайындалған әрбір тапсырма бойынша әртүрлі алдын ала жасалған анықтамалармен аталған ресурс үшін орнатуға болады.

Төмендегі мысал сізге мәннің қарапайым алдын ала жасалған анықтамасы ресурстың жобада әртүрлі шығындар мен төлемдер мөлшерлемелерімен бірнеше рөлге ие болуына мүмкіндік береді.

## <a name="create-tasks"></a>Тапсырмаларды жасау
Тапсырмаларды құру үшін тапсырмаларды, сонымен қатар қорытынды тапсырмаларды қосу керек, содан кейін тапсырманың ұзақтығын қоспас бұрын тапсырма тағайындау қажет. 

### <a name="add-tasks-and-summary-tasks"></a>Тапсырмалар мен қорытынды тапсырмаларды қосу
Тапсырма қосу үшін келесі қадамдарды орындаңыз.

1. **Жобалар** қойыншасына өтіп, тапсырмалар қосу керек жобаны ашыңыз.
2. **Жаңа тапсырма қосу** пәрменін таңдаңыз. Тапсырма атын өзгертіңіз, содан кейін **Енгізу** түймесін басыңыз.
3. Басқа тапсырма атын енгізіп, **Енгізу** түймесін басыңыз. Тапсырмалардың толық тізімі болғанша осыны қайталаңыз.
3. **Қорытынды** тапсырмалары астындағы тапсырмаларды туралау үшін тапсырма атауы бойынша үш тік нүктені таңдап, содан кейін **Ішкі тапсырма жасау** пәрменін таңдаңыз. 

  > [!TIP]
  > Бірнеше тапсырманы таңдау үшін тапсырманы таңдап, **Ctrl** пернесін басып тұрыңыз, содан кейін басқа тапсырманы таңдаңыз.
  >
  > Сондай-ақ **Қорытынды** тапсырмалары астынан тапсырмаларды шығару үшін **Ішкі тапсырманы жариялау** пәрменін таңдауға болады.

### <a name="assign-tasks"></a>Тапсырмаларды тағайындау

Тапсырмаларды тағайындау үшін келесі қадамдарды орындаңыз.

1. Тапсырмаға арналған **Тағайындалған** бағанын таңдап, адам белгішесін басыңыз.
2. Тізімнен топ мүшесін таңдаңыз немесе атау іздеу үшін мәтін енгізіңіз.

### <a name="add-task-duration-and-columns"></a>Тапсырманың ұзақтығы мен бағандарын қосу

Жобаның құрылымын көбінде ұзақтығымен бастау оңай. Тапсырма ұзақтығын қосу үшін келесі қадамдарды орындаңыз.

1. Тапсырмаға арналған **Ұзақтық** бағанында, тапсырманы орындау үшін қажет күн санын енгізіңіз. Егер сіз басқа уақыт бірлігін пайдаланғыңыз келсе, онда **сағат**, **апта** немесе **ай** сөздеріне санды қосып жазыңыз.
2. Егер тапсырмаңыздың **Уақыт шкаласы** көрінісінде алмас пішінді кезең ретінде көрінуін қаласаңыз, **Ұзақтық** бағанында **0 күн** мәнін енгізіңіз.
3. Келесі тапсырманың **Ұзақтық** өрісіне өту үшін **Енгізу** пернесін басып, ұзақтықтарды енгізуді жалғастырыңыз.

  > [!NOTE]
  > Қорытынды тапсырмалардың ұзақтығын енгізу мүмкін емес.

Қосымша мәліметтер ұсыну үшін жобаңызға бағандар қосуға болады. Ол үшін **Баған қосу** параметрін таңдаңыз. 

Қосымша ақпарат алу үшін [Жоба жасау](https://support.microsoft.com/en-us/office/create-a-project-a5b5e823-fb2e-45fd-be00-7d84422d9749) бөлімін қараңыз.

## <a name="set-up-the-role-and-organization-unit-for-a-generic-project-team-member"></a>Жалпы жобаның топ мүшесі үшін рөл мен ұйымдық бірлік орнату
Жалпы топ мүшесіне арналған рөл және ұйымдық бірлік орнату үшін келесі қадамдарды орындаңыз.

1. **Тапсырмалар** бетінде **А тапсырмасы** үшін **Тапсырма** қатарын таңдаңыз. 
2. **Тағайындалған** қойыншасында **Жалпы ресурс қосу** параметрін таңдаңыз. Бұл **Топ мүшесін жылдам жасау** бетін ашады.
3. **Топ мүшесін жылдам жасау** бетінде, осы тапсырманы орындай алатын жалпы топ мүшесінің төлсипаттарын көрсетіңіз.
4. Тиісті рөл мен бөлімшені таңдап, содан кейін **Сақтау және жабу** пәрменін таңдаңыз. Бұл тапсырмаға жалпы топ мүшесі құрылады және тағайындалады. 
5. **В тапсырмасы** үшін 1-4 қадамдарын қайталаңыз. Алайда **В тапсырмасы** **А тапсырмасы** параметріне қарағанда жалпы топ мүшесі үшін тағайындалған басқа рөлі мен ұйымдық бірлігі болуы керек. 

## <a name="set-up-the-role-and-organization-unit-for-a-project-task"></a>Жоба тапсырмасы үшін рөл мен ұйымдық бірлік орнату
Тапсырмаға арналған рөл және ұйымдық бірлік орнату үшін келесі қадамдарды орындаңыз.

1. **А тапсырмасы** жасалғаннан кейін, тапсырманы таңдаңыз, содан кейін **Тапсырма туралы мәліметтер** бөлігін ашу үшін **i** белгішесін басыңыз. 
2. **Тапсырма туралы мәліметтер** бөлігінде төменгі жағына айналдырып, **Тапсырма туралы мәліметтер** бетін ашу үшін **Мәліметтерді қарау** параметрін таңдаңыз.
3. **Тапсырма туралы мәліметтер** бетіндегі **Рөл** және **Ұйымдық бірлік** параметрінде осы тапсырманы орындау үшін қажетті мәндерді қосыңыз. 

  > [!NOTE]
  > Егер сіз осы сценарийді Project Operations демо-деректері көмегімен аяқтасаңыз, рөлге арналған **Кеңес беруші ықтимал тұтынушы** және ұйымдық бірлік ретінде **Fabrikam US** таңдаңыз.

4. **В тапсырмасы** параметрін таңдап, содан кейін тапсырманы таңдаңыз.
5. **Тапсырма туралы мәліметтер** бөлігін ашу үшін **i** белгішесін таңдаңыз. 
6. **Тапсырма туралы мәліметтер** бөлігінде төменгі жағына айналдырып, **Тапсырма туралы мәліметтер** бетін ашу үшін **Мәліметтерді қарау** параметрін таңдаңыз.
7. **Тапсырма туралы мәліметтер** бетіндегі **Рөл** және **Ұйымдық бірлік** параметрінде, ресурсқа арналған осы тапсырманы орындау үшін қажетті мәндерді қосыңыз. **В тапсырмасына** параметріне арналған **Рөл** және **Ұйымдық бірлік** мәндері **А тапсырмасы** параметріне қарағанда өзгеше болуы тиіс. 

  > [!NOTE]
  > Егер сіз осы сценарийді Project Operations демо-деректері көмегімен аяқтасаңыз, рөлге арналған **Желі технигі** және ұйымдық бірлік ретінде **Fabrikam US** таңдаңыз.

8. **Тапсырма туралы мәліметтер** бетін сақтап, жабыңыз. 

## <a name="team-member-and-estimates-behavior"></a>Топ мүшесі және болжамдар әрекеті 
**Топ мүшесі** торындағы әрекетті және болжамдарды түсіну үшін келесі қадамдарды орындаңыз.

1. **Топ мүшесі** торында екі жалпы топ мүшесін таңдап, содан кейін **Талаптарды қалыптастыру** параметрін таңдаңыз. Бұл ресурс талаптарын құрады. 
2. **Кеңес беруші ықтимал тұтынушы** үшін топ мүшесінің жолын таңдаңыз, содан кейін **Брондау** пәрменін таңдаңыз. Кесте тақтасы ресурстар тізімімен ашылады. Ресурсты таңдаңыз, содан кейін сол талапқа сай ресурсты брондау үшін **Брондау** параметрін таңдаңыз.
3. **Желі технигі** үшін топ мүшесінің жолын таңдаңыз, содан кейін **Брондау** пәрменін таңдаңыз. Кесте тақтасы ресурстар тізімімен ашылады. Жоғарыдағыдай бірдей ресурсты таңдаңыз, содан кейін сол талапқа сай ресурсты брондау үшін **Брондау** параметрін таңдаңыз.

### <a name="team-member-grid"></a>Топ мүшесі торы 

**Топ мүшесі** торында, жалпы екі топ мүшесінің жазбасы жойылады және бір ресурспен ғана ауыстырылады. Сол ресурсқа арналған мәндердің бір жиыны бар, олар **Рөл** және **Ұйымдық бірлік** үшін әдепкі мәндер жиыны болып саналады.

Топ мүшесі жазбасының жолын кеңейткенде, топ мүшесі жазбасында екі тапсырма үшін де бөлек тағайындауларды көруге болады. Әрбір тағайындау жолында **Рөл** және **Ұйымдық бірлік** үшін тапсырмаға сәйкес мәндер бар. 

### <a name="estimates-grid"></a>Болжамдар торы 

**Болжамдар** торында, бір ресурсқа арналған екі тағайындау да әртүрлі бағаланады. **А тапсырмасы** параметріндегі ресурсқа арналған тағайындау **Кеңес беруші ықтимал тұтынушы** параметрінің **Рөл** төлсипат мәні арқылы бағаланады. **В тапсырмасы** параметріндегі бірдей ресурсқа арналған тағайындау **Желі технигі** параметрінің **Рөл** төлсипат мәні арқылы бағаланады.


[!INCLUDE[footer-include](../includes/footer-banner.md)]