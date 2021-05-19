---
title: Баға орнатуы және транзакциялық нысандарға реттелетін өрістер қосу
description: Бұл тақырыпта баға орнатуы және транзакциялық нысандарға реттелетін өрістер қосу туралы ақпарат беріледі.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: e1a8d6319788ee73e0e2837a47cba89108c32572
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5275320"
---
# <a name="add-custom-fields-to-price-setup-and-transactional-entities"></a>Баға орнатуы және транзакциялық нысандарға реттелетін өрістер қосу 

[!include [banner](../includes/psa-now-project-operations.md)]

Бұл тақырып осы тақырыптағы процедураларды аяқтағаныңызды білдіреді, [Реттелетін өрістер мен нысандарды жасау](create-custom-fields-entities.md). Егер сіз бұл процедураларды орындамасаңыз, кері қайтып, оларды орындаңыз, содан кейін осы тақырыпқа оралыңыз. 

Бұл тақырыптағы процедураларда нысандарға және пішіндер мен көріністер сияқты пайдаланушылық интерфейс (ПИ) элементтеріне қажетті реттелетін өріс сілтемелерін қосу жолы көрсетіледі.

## <a name="add-custom-pricing-dimension-fields"></a>Реттелетін бағалар өлшемінің өрістерін қосу 
Реттелетін өрістер мен нысандар жасалғаннан кейін, келесі қадам бағаны белгілеу және сілтеме өрістерін құру арқылы кез келген реттелетін немесе параметрлер жиыны туралы хабарланған транзакциялық нысандарды жасау болып табылады. Баға өлшемдеріңіздің тізіміне параметрлер жиыны өлшемдері немесе нысан өлшемдері немесе екеуінің де кіретініне байланысты **Параметрлер жиыны негізіндегі реттелетін баға өлшемдері** немесе **Нысан негізіндегі реттелетін баға өлшемдері** бөліміндегі немесе екеуіндегі қадамдарды ғана сәйкесінше орындаңыз.

### <a name="option-set-based-custom-pricing-dimensions"></a>Параметрлер жиыны негізіндегі реттелетін баға өлшемдері
Реттелетін баға өлшемі параметрлер жиыны негізінде болғанда, оны Project Service негізгі нысандарына өріс ретінде қосыңыз. Келесі процедурада **Ресурстың жұмыс орны** және **Ресурстың жұмыс сағаттары** параметрлер жиыны негізіндегі баға өлшемдері ретінде пайдаланылады. Алдымен олар баға нысандарына өріс ретінде қосылуы керек, **Рөл бағасы** және **Рөлдің үстеме бағасы**.

1. Project Service Automation (PSA) бағдарламасында **Параметрлер** > **Шешімдер** тармағын таңдап, содан кейін **\<your organization name>баға өлшемдері** пәрменін екі рет басыңыз. 
2. Шешім жетектеушісіндегі сол жақ шарлау аумағында **Нысандар > Рөл бағасы** тармағын таңдаңыз.
3. **Рөл бағасы** нысанын кеңейтіп, **Өрістер** опциясын таңдаңыз.
4. **Ресурстың жұмыс орны** деп аталатын жаңа өрісті жасау үшін **Жаңа** опциясын басып, өріс түрі ретінде **Параметрлер жиыны** түрін таңдаңыз. 
5. **Бар параметрлер жиынын қолдану** параметрін, содан кейін **Ресурстың жұмыс орны** параметрлер жиынын таңдап, **Сақтау** түймешігін басыңыз.
6. Осы өрісті **Рөлдің үстеме бағасы** нысанына қосу үшін 1 - 5 қадамдарды қайталаңыз. 
7. **Ресурстың жұмыс сағаттары** параметрлер жиыны үшін 1 - 5 қадамдарды қайталаңыз.

> [!IMPORTANT]
> Өрісті бірнеше нысанға қосқан кезде, барлық нысандар үшін бірдей өрісті қолданыңыз. 

> ![Рөл бағасына ресурстың жұмыс орнын қосу](media/RWL-Field.png)

Жобаны сату және бағалау кезеңдерінде, **Тұрақты сағаттар** және **Үстеме жұмыс уақыты** ішіндегі **Жергілікті** және **Ішкі** жұмысын аяқтау үшін қажет жұмыс қарқындылығының болжамдары, баға ұсыну/жоба мәнін бағалау үшін қолданылады. **Ресурстың жұмыс орны** және **Ресурстың жұмыс сағаттары** бағалау нысандарына қосылады, **Баға ұсыну жолының мәліметі**, **Келісім-шарт жолының мәліметі**, **Жоба тапсырмасы**, **Жоба тобының мүшесі** және **Болжам жолы**.

1. PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын таңдап, содан кейін **\<your organization name> баға өлшемдері** пәрменін екі рет басыңыз. 
2. Шешім жетектеушісіндегі сол жақ шарлау аумағында **Нысандар > Баға ұсыну жолының мәліметі** тармағын таңдаңыз.
3. **Баға ұсыну жолының мәліметі** нысанын кеңейтіп, **Өрістер** параметрін таңдаңыз.
4. **Ресурстың жұмыс орны** деп аталатын жаңа өрісті жасау үшін **Жаңа** опциясын басып, **Параметрлер жиыны** өріс түрін таңдаңыз. 
5. **Бар параметрлер жиынын қолдану** параметрін, содан кейін **Ресурстың жұмыс орны** параметрін таңдап, **Сақтау** түймешігін басыңыз.
6. Осы өрісті **Жоба келісім-шартының жолы туралы мәлімет**, **Жоба тапсырмасы**, **Жоба тобының мүшесі** және **Болжам жолы** нысандарына қосу үшін 1 - 5 қадамдарды қайталаңыз.
7. **Ресурстың жұмыс сағаттары** параметрлер жиыны үшін 1 - 6 қадамдарды қайталаңыз. 

> ![Болжам жолына ресурстың жұмыс орнын қосу](media/RWL-Default-Value.png)


Жеткізу және шот-фактураны ұсыну үшін, аяқталған жұмыстың **Жергілікті** немесе **Ішкі** түрде орындалғанын және оның "Жобаның нақты көрсеткіштері" тармағындағы **Тұрақты сағаттар** немесе **Үстеме жұмыс** кезінде аяқталғанын таңдау үшін аяқталған жұмыс бағасын дәл анықтау қажет. **Ресурстың жұмыс орны** және **Ресурстың жұмыс уақыты** өрістері **Уақыт жазбасы**, **Нақты**, **Есеп-шот жолының мәліметі** және **Журнал жолы** нысандарына қосылуы керек.

1. PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын таңдап, содан кейін **\<your organization name> баға өлшемдері** пәрменін екі рет басыңыз.
2. Шешім жетектеушісіндегі сол жақ шарлау аумағында **Нысандар > Уақыт жазбасы** тармағын таңдаңыз.
3. **Баға ұсыну жолының мәліметі** нысанын кеңейтіп, **Өрістер** параметрін таңдаңыз.
4. **Ресурстың жұмыс орны** деп аталатын жаңа өрісті жасау үшін **Жаңа** опциясын басып, өріс түрі ретінде **Параметрлер жиыны** түрін таңдаңыз. 
5. **Бар параметрлер жиынын қолдану** параметрін, содан кейін **Ресурстың жұмыс орны** параметрлер жиынын таңдап, **Сақтау** түймешігін басыңыз.
6. Осы өрісті **Нақты**, **Есеп-шот жолының мәліметі** және **Журнал жолы** нысандарына қосу үшін 1 - 5 қадамдарды қайталаңыз.
7. **Ресурстың жұмыс сағаттары** параметрлер жиыны үшін 1 - 6 қадамдарды қайталаңыз. 

> ![Уақыт жазбасына ресурстың жұмыс орнын қосу](media/RWL-time-entry.png)

Бұл параметрлер жиыны негізіндегі реттелетін өлшемдер үшін қажет схемалық өзгертулерді аяқтайды.

## <a name="entity-based-custom-pricing-dimensions"></a>Нысан негізіндегі реттелетін баға өлшемдері

Реттелетін баға өлшемі нысан болған кезде, сіз өлшем нысаны мен Project Service негізгі нысандары арасындағы 1:N қатынасын қосасыз. Жоғарыда келтірілген "Стандартты тақырып" мысалын қолдана отырып, әр қызметкерге стандартты тақырып тағайындалады деп күтуге болады. Нәтижесінде резервтеу үшін қолжетімді ресурстың стандартты тақырыбындағы 1:N қатынасы немесе ол стандартты тақырыптың резервтеу үшін қолжетімді ресурсынан жасалған жағдайда N:1 қатынасы керек болады.

1. PSA бағдарламасында **Параметрлер** > **Шешімдер** тармағын таңдап, содан кейін **\<your organization name> баға өлшемдері** пәрменін екі рет басыңыз. 
2. Шешім жетектеушісіндегі сол жақ шарлау аумағында **Нысандар > Стандартты тақырып** тармағын таңдаңыз.
3. **Стандартты тақырып** нысанын кеңейтіп, **1:N қатынастары** опциясын таңдаңыз.
4. **Резервтеу үшін қолжетімді ресурстың стандартты тақырыбы** деп аталатын жаңа 1:N қатынасын құру үшін **Жаңа** параметрін басыңыз. Қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.

> ![Стандартты тақырыпты резервтеу үшін қолжетімді ресурсқа сілтеме өріс ретінде қосу](media/ST-BR.png)

Стандартты тақырып, сонымен қатар Project Service қызметінің **Рөл бағасы** және **Рөл бағасын белгілеу** сияқты баға нысандарына қосылуы керек. Бұл сонымен қатар **Стандартты тақырып** және **Рөл бағасы** нысандары және **Стандартты тақырып** және **Рөл бағасын белгілеу** нысандары арасындағы 1:N қатынастарын қолдана отырып орындалады.

1. Шешім жетектеушісіндегі сол жақ шарлау аумағында **Нысандар > Стандартты тақырып** тармағын таңдаңыз.
2. **Стандартты тақырып** нысанын кеңейтіп, **1:N қатынастары** опциясын таңдаңыз.
3. **Рөл бағасының стандартты тақырыбы** деп аталатын жаңа 1:N қатынасын құру үшін **Жаңа** параметрін басыңыз. Қажетті ақпаратты енгізіп, **Сақтау** түймешігін басыңыз.
4. **Стандартты тақырып** және **Рөл бағасын белгілеу** нысандары арасындағы 1:N қатынастарын құру үшін 1 - 4 қадамдарды қайталаңыз.

Баға ұсынуды/Жобаны бағалау үшін жобаны сату және бағалау кезеңдерінде әрбір стандартты тақырып үшін жұмыс қарқындылығының болжамдары талап етіледі. Бұл дегеніміз стандартты тақырыптың 1:N қатынастары Project Service қызметіндегі осы бағалау нысандарының әрқайсысына қажет: 

- **Баға ұсыну жолының мәліметі**
- **Жобалық келісім-шарт жолы мәліметі**
- **Жоба тапсырмасы**
- **Жоба тобы мүшесі**
- **Болжам жолы**

5. **Стандартты тақырып** және **Баға ұсыну жолының мәліметі**, **Жоба келісім-шартының жолы туралы мәлімет**, **Жоба тапсырмасы**, **Жоба тобының мүшесі** және **Болжам жолы** арасында 1:N қатынастарын құру үшін 1 - 5 қадамдарды қайталаңыз.

> ![Стандартты тақырыпты болжам жолына сілтеме өріс ретінде қосу](media/ST-Estimate-Line.png)

Жеткізу және шот-фактуралар ұсыну кезеңдерінде әр стандартты тақырыппен аяқталған жұмыс "Жобаның нақты көрсеткіштері" тармағында дәл бағалануы керек. Бұл **Стандартты тақырып** және **Уақыт жазбасы**, **Нақты**, **Есеп-шот жолы мәліметі** және **Журнал жолы нысандары** арасында 1:N қатынасы болуы керек дегенді білдіреді.

6. **Стандартты тақырып** және **Уақыт жазбасы**, **Нақты**, **Есеп-шот жолы мәліметі** және **Журнал жолы нысандары** арасында 1:N қатынастарын құру үшін 1 - 6 қадамдарды қайталаңыз.

> ![Стандартты тақырыпты уақыт жазбасына сілтеме өріс ретінде қосу](media/ST-Mapping.png)

### <a name="set-up-dimension-value-defaulting-using-the-mappings-features-of-the-platform"></a>Платформаның салыстыру мүмкіндіктерін қолданып, өлшем мәнін әдепкі бойынша орнату
Уақыт жазбасы үшін уақыт жазбасын жазатын резервтеу үшін қолжетімді ресурстан алынған уақыт жазбасының стандартты тақырыбын әдепкі бойынша пайдалану жүйеге пайдалы болар еді. **Резервтеу үшін қолжетімді ресурс** және **Уақыт жазбасы** арасындағы 1:N қатынасына өріс салыстыруларын қосу үшін келесі қадамдарды қолданыңыз.

1. Шешім жетектеушісіндегі сол жақ шарлау аумағында **Нысандар > Стандартты тақырып** тармағын таңдаңыз.
2. **Стандартты тақырып** нысанын кеңейтіп, **1:N қатынастары** опциясын таңдаңыз.
3. **Резервтеу үшін қолжетімді ресурс және уақыт жазбасы** параметрін екі рет басыңыз. **Қарым-қатынас** бетінде **Өріс салыстыруларын қолдану** параметрін басыңыз. 
4. **Резервтеу үшін қолжетімді ресурс** нысанындағы **Стандартты тақырып** өрісі және **Уақыт жазбасы** нысанындағы **Стандартты тақырып** сілтеме өрісі арасындағы жаңа өріс салыстыруларын жасау үшін **Жаңа** параметрін басыңыз. 

> ![Резервтеу үшін қолжетімді ресурстағы стандартты тақырыпты уақыт жазбасында әдепкі бойынша пайдалануға мүмкіндік беру үшін өріс салыстыруларын орнату](media/ST-Mapping2.png)


Бұл нысан негізіндегі реттелетін өлшемдер үшін қажет схемалық өзгертулерді аяқтайды.

##  <a name="add-custom-fields-to-forms-views-and-business-rules"></a>Реттелетін өрістерді пішіндерге, көріністер мен бизнес ережелерге қосу

Барлық қажетті схемалық өзгертулерді жасағаннан кейін, келесі қадам – өрістерді пішіндер мен көріністерге қосу арқылы пайдаланушылық интерфейсте көрінетіндей етіп жасау.

1. Пішінді немесе көріністі ашыңыз. Оң жақ шарлау аумағында өрісті таңдап, оны пішін кенебіне сүйреңіз. 
2. Егер көріністі өңдесеңіз, оң жақ шарлау аумағын пайдаланып, **Өрістер қосу** түймешігін басыңыз және **Өрістер тізімі** диалогтық терезесінде қажетті өрістерді таңдап, **Ok** опциясын басыңыз.

Төмендегі кестеде нысанмен тізімделген кірістірілген формалар мен көріністердің жаңа өрістермен жаңартылуы қажет жиынтық тізімі беріледі. Осы нысандардың реттеулерінде қандай да бір қосымша көріністер немесе формалар бар болса, жаңа өрістерді сол көріністер мен формаларға да қосыңыз.

| Project Service нысаны        | Жаңа өрісті қажет ететін формалар   |Жаңа өрісті қажет ететін көріністер      |
| ------------------------------|---------------------------------|----------------------------------|
|  Рөл бағасы|• Ақпарат |• Белсенді ресурс санатының бағалары<br> • Ресурс санаты бағасының байланысты көрініс|
|  Рөлдің үстеме бағасы|• Ақпарат|• Белсенді рөлдің үстеме бағасы<br>• Рөл үстеме бағасының байланысты көрінісі|
|  Баға ұсыну жолы мәліметі|• Жоба ақпараты<br>• Жобаны жылдам жасау|• Белсенді баға ұсыну жолы мәліметі<br>• Біріктірілген баға ұсыну жолы мәліметтері<br>• Баға ұсыну жолы мәліметінің байланысты көрінісі|
|  Жоба келісім-шартының жолы туралы мәлімет|• Жоба ақпараты<br>• Жобаны жылдам жасау|• Біріктірілген келісім-шарт жолының мәліметтері<br>• Белсенді келісімшарт жолының мәліметтері<br>• Келісім-шарт жолы мәліметтерінің байланысты көрінісі|
|  Жоба тапсырмасы|• Ақпарат<br>• Жаңа форма||
|  Жоба тобы мүшесі|• Ақпарат<br>• Жаңа форма|• Белсенді жоба тобы мүшелері<br>• Жоба тобы мүшелері<br>• Жоба тобы мүшелерінің байланысты көрінісі|
|  Уақыт жазбасы|• Ақпарат<br>• Уақыт жазбасын жасау|• Күн бойынша уақыт жазбаларым<br>• Осы апталық уақыт жазбаларым<br>• Бекітілетін уақыт жазбалары|
|  Журнал жолы|• Ақпарат<br>• Жылдам жасау|• Белсенді журнал жолдары<br>• Журнал жолының байланысты көрінісі|
|  Есеп-шот жолы мәліметі|• Ақпарат<br>• Жылдам жасау|• Белсенді есеп-шот жолы мәліметтері<br>• Ақылы есеп-шот транзакциялары<br>• Қосымша есеп-шот транзакциялары<br>• Есеп-шот жолы мәліметінің байланысты көрінісі<br>• Ақысыз есеп-шот транзакциялары|
|  Нақты|• Ақпарат<br>• Белсенді нақты көрсеткіштер|• Нақты байланысты көрініс|

Анықтаған нәрсеге байланысты реттелетін өрістерді бизнес ережелеріне қосу қажет болуы мүмкін. Бір дайын мысал **Күйге негізделген уақыт жазбасын өңдеу мүмкіндігі** бизнес ережесіне арналған. Бұл ереже "Уақытты жазбасы" **Бекітілген** сияқты өңделмейтін күйде болған кезде қай өрістерді құлыптау керектігін анықтайды. Уақытты жазбасы **Жоба** немесе **Қайтарылған** күйінен басқа күйде болған кезде, өрістер өңдеу үшін құрсаулы болатындай етіп, осы ережеге өрістер қосыңыз.


[!INCLUDE[footer-include](../includes/footer-banner.md)]