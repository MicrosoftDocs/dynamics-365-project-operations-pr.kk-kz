---
title: Топ мүшесі торынан топ мүшелерін қосу
description: Бұл бөлімде топ мүшесі ресурстарын басқару жолы туралы ақпарат берілген.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 0f975d295b4c0ccef9827767beabd32ffd761faa
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897728"
---
# <a name="add-team-members-from-the-team-member-grid"></a>Топ мүшесі торынан топ мүшелерін қосу

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Dynamics 365 Project Operations бүкіл ұйым бойынша ресурс сұрауы және пайдалану жолының визуалды шолуын қамтамасыз ететін ресурс менеджерінің бақылау тақтасын қамтиды. Осы бақылау тақтасындағы диаграммаларды келесі ақпаратты визуализациялау үшін пайдалануға болады:

- **Ресурс сұрауы**: **Белсенді ресурс сұрауы** диаграммасында жіберілген ресурстар көрсетіледі. Ресурстар рөл немесе жоба бойынша біріктіріледі.
- **Жіберілмеген ресурс сұрауы**: **Тағайындалмаған ресурс сұрауы** диаграммасында жіберілмеген барлық ресурстар талаптары көрсетіледі. Бұл диаграмма ресурс менеджерлеріне берік емес және ресурс сұрауы арқылы жіберілуі мүмкін сұрауды көруге көмектеседі.
- **Өткен аптада шот ұсынылған қолданыс**: **Рөл бойынша қолданыс** диаграммасында рөл арқылы ұйымның мақсатты шот ұсынылған қолданысы бойынша рөл арқылы нақты шот ұсынылған қолданыстың пайыздық көрсеткіші көрсетіледі.

    > [!NOTE]
    > **Рөл бойынша қолданыс** диаграммасын қолжетімді ету үшін, **UpdateRoleUtilization** жұмыс ағынын іске қосатын тапсырманы жасаңыз. Бұл қайталанатын тапсырма әр жеті күн сайын алдыңғы жеті күн бойынша шот ұсынылған қолданысты есептеу үшін орындалады. Нәтижелер рөл бойынша біріктіріледі.

## <a name="manage-project-team-members"></a>Жоба тобының мүшелерін басқару

Жоба менеджерлері жобалардағы ресурстарды басқару үшін, ресурс менеджерінің бақылау тақтасын қолдана алады. Мысалы, олар топ мүшесін жобаға тікелей қосып, жалпы ресурс арқылы алынған ресурстарға қойылатын талаптарды орындау үшін топ мүшелерін резервтей алады.

### <a name="add-a-team-member-directly-to-a-project"></a>Топ мүшесін жобаға тікелей қосу

Топ мүшесін жобаға тікелей қосу үшін, **Жобалар** пішініндегі **Топ** қойыншасында **Жаңа** параметрін таңдаңыз. Сонда **Жылдам құру: жоба тобының мүшесі** диалогтық терезесі пайда болады. Осы диалогтық терезеде келесі тапсырмаларды орындауға болады:

- **Аталған ресурсты резервтеу**: **Резервтеу үшін қолжетімді ресурс** өрісінде ресурс атауын таңдаңыз. Содан кейін рөлді таңдап, кезеңді белгілеңіз де бөлу әдісін таңдаңыз. Таңдалған атаулы ресурс жобаға таңдалған бөлу әдісі мен ресурстар күнтізбесін қолдану арқылы қосылады.
- **Жалпы ресурс қосу**: **Резервтеу үшін қолжетімді ресурс** өрісін бос қалдырып, рөлді таңдаңыз да, кезеңді белгілеңіз және бөлу әдісін таңдаңыз. Жалпы ресурс топқа толтырғыш ретінде қосылады. Толтырғыш командадағы атаулы ресурстарды брондау үшін пайдаланылатын сұраныстың үлгісіне ие. Талап жоба күнтізбесі бойынша жасалады.
- **Аталған ресурсты ресурс сыйымдылығын пайдаланбай топқа қосу**: **Резервтеу үшін қолжетімді ресурс** өрісінде ресурсты таңдаңыз. Кезеңді таңдап, содан кейін бөлу әдісі ретінде **Жоқ** мәнін таңдаңыз. Сонда ресурс топқа қосылады, бірақ ресурс сыйымдылығы резервтеу арқылы пайдаланылмайды.

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a>Жалпы ресурсқа арналған ресурс талаптарын орындау үшін топ мүшелерін резервтеу

Project Operations ішінде жобалық топта жалпы ресурстарға тапсырыс бере аласыз. Сондай-ақ рөлді, қажетті сыйымдылықты және ол сыйымдылықтың қалай бөлінетінін көрсете аласыз. Ресурсқа қойылатын талап үшін жалпы ресурстармен байланысты атрибуттарды көрсете аласыз. Бұл атрибуттарға қажетті дағдылар, таңдаулы ұйымдық бөлімше және таңдаулы ресурстар кіреді.

Әзірлеушіге арналған жалпы ресурс бойынша қажетті дағдыларды көрсету үшін, келесі қадамдарды орындаңыз.

1. **Жобалар** пішініндегі **Топ** қойыншасында жалпы ресурсты резервтеу үшін **Жаңа** параметрін таңдаңыз.
2. **Барлық топ мүшелері** көрінісіндегі **Ресурс талабы** бағанында жалпы ресурсқа қажетті дағдыларды қосу үшін сілтемені таңдаңыз.
3. **Ресурс талабы** пішініндегі **Дағдылар** торында эллипсті (**...**) таңдап, әзірлеушіге қажетті дағдыларды қосу үшін **Жаңа талап сипаттамасын қосу** параметрін таңдаңыз.
4. **Жылдам жасау: талап сипаттамасы** диалогтық пішініндегі **Сипаттама** өрісінде қажетті дағдыны таңдаңыз.
5. **Бағалау мәні** өрісінде сол дағдының кәсіби деңгейін таңдаңыз. 
6.  **Ресурс талабы** өрісінде ұйымдық бөлімшелерден немесе тіпті аталған ресурстардан алынған бастапқы ресурстарға қойылатын талапты орнатыңыз. Аяқтағаннан кейін, **Сақтау** түймешігін таңдаңыз.
7. **Ресурс талабы** пішінінде ресурсқа қойылатын талапты орындау үшін, **Резервтеу** параметрін таңдаңыз. Сондай-ақ жалпы ресурсты **Барлық топ мүшелері** торынан таңдап, **Резервтеу** параметрін таңдай аласыз.

    > [!NOTE]
    > Бұл мысалда талап етілетін 40 сағат бар, бірақ нақты резервтелген сағаттар жоқ, себебі жалпы ресурстарда резервтеу мүмкіндігі жоқ. Сонымен қатар тағайындалған сағаттар жоқ, себебі жалпы ресурс тапсырма тағайындауы арқылы қосылудың орнына топқа тікелей қосылған.

    **Жоспарлау бойынша көмекші** пішінінде қолжетімді ресурстарды ресурсқа қойылатын талапта көрсетілген талаптар бойынша сүзгілеуге болады. Ресурстар кесте тақтасында көрсетілген сұрыптау параметрлері бойынша сұрыпталады.

   Кейбір жиі пайдаланылатын сүзгілер:

    - **Бағалау бойынша сипаттама**: біліктілік бағалауына қосымша ретінде, дағдылары, сертификаттары және басқа ресурстық қасиеттері бойынша сүзгілеу.
    - **Рөлдер**: резервтеу үшін қолжетімді ресурстарға тағайындалған әдепкі рөлдер бойынша сүзгілеу.
    - **Ұйымдық бөлімшелер**: резервтеу үшін қолжетімді ресурстарды тағайындалған ұйымдық бөлімшелер бойынша сүзгілеу.

8. Егер алғашқы талаптарды іздеудің нәтижелеріне қанағаттанбасаңыз, сүзгілеу шарттарын өзгерте аласыз. Сол жақтағы **Сүзгі көрінісі** тақтасын кеңейтіп, қосымша ресурстар табу үшін **Іздеу** параметрін таңдаңыз. Нәтижелерді сұрыптау әдісін өзгерту үшін, **Сұрыптау** параметрін таңдаңыз.
9. Тордың жоғарғы жағында көрсетілгендей, ресурстарды талапта көрсетілген сұрауға сәйкес таңдаңыз. Тордағы ұяшықтардың таңдау белгісін алып тастап, ресурс сыйымдылығын ашық қалдыруға болады. Бір уақытта резервтелген ретінде тек бір ресурсты таңдауға болады.
10. Таңдалған ресурсты резервтеу үшін **Резервтеу** параметрін таңдап, кестелер тақтасын ашық қалдырыңыз, осылайша қосымша ресурстарды таңдай аласыз. Не болмаса, таңдалған ресурсты резервтеу және кесте тақтасын жабу үшін **Резервтеу және шығу** параметрін таңдаңыз.
11. **Барлық топ мүшелері** көрінісіне оралыңыз. Торда жалпы ресурстың аталған ресурсқа ауыстырылғанын және 40 сағаттың сол ресурс үшін резервтелгенін ескеріңіз.

    > [!NOTE]
    > Тағайындалған сағаттар көрсетілмейді, себебі олар тікелей топта резервтелген. Олар тапсырма тағайындауын қолдану арқылы резервтелмеді.

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a>Жалпы ресурстарды тапсырмаларға тағайындау және ресурс талаптарын жасау

Project Operations бағдарламасында тапсырмалар жасап, оларға жалпы ресурстар тағайындауға болады. Кестеңізді және қаржылық нөмірлеріңізді бағалау кезінде, ресурс сұрауын толтырғыштар арқылы ұсынуға болады. Содан кейін жалпы ресурстарға қойылатын талаптарды құрып, оларды орындай аласыз.

1. **Жобалар** пішіндегі **Кесте** қойыншасында тапсырма құру үшін **Қосу** параметрін таңдаңыз.
2. **Ресурстар** өрісінде **Ресурс таңдау құралы** белгісін таңдаңыз. Сонда ресурс таңдау құралы пайда болып, жоба бойынша топ мүшелерін көрсетеді.
3. Жаңа жалпы ресурстың атауын енгізіп, **Жасау** параметрін таңдаңыз.
4. Пайда болатын **Жылдам жасау: жоба тобының мүшесі** диалогтық терезесіндегі **Рөл** өрісінде жалпы ресурс рөлін таңдаңыз. 
5. **Ресурс бірлігі** өрісінде жалпы ресурс үшін ұйымдық бөлімшені таңдаңыз. Содан кейін **Сақтау** опциясын таңдаңыз. Жалпы топ мүшесі енді тапсырмаға тағайындалды.

   **Топ** қойыншасында жалпы топтың жаңа мүшесін көресіз. Оның тағайындалған сағаттарды ғана қамтитынын ескеріңіз. Бұл сағаттар жалпы топ мүшесіне тағайындалған барлық тапсырмалардың қосындысы болып табылады. Жалпы топ мүшесінің қажетті сағаттары немесе ресурс талабы жоқ.

6. Енді ресурс таңдау құралы арқылы жалпы топ мүшесін басқа тапсырмаларға тағайындауға болады.

   Тапсырмаларға жалпы ресурсты тағайындауды аяқтағаннан кейін, жалпы ресурс үшін ресурс талабын жасай аласыз.

7. **Топ** қойыншасында жалпы ресурсты, содан кейін **Талапты жасау** параметрін таңдаңыз. Талап жасалған кезде, жалпы топ мүшесінде қажетті сағаттар мен ресурс талабына сілтеме бар болады.

  Аталған ресурсты резервтегеннен кейін, жалпы ресурс топтан жойылады да аталған ресурспен алмастырылады. **Кесте** қойыншасындағы жалпы ресурс тағайындаулары жойылып, аталған ресурспен алмастырылады.

  > [!NOTE]
  > Бұл әрекет аталған ресурс жалпы ресурс талабы үшін толығымен резервтелгенде ғана пайда болады. Аталған ресурс жалпы ресурс талабын ішінара алмастырғанда немесе аталған бірнеше ресурс жалпы ресурс талабын алмастырғанда, жалпы ресурс тапсырмаға тағайындалған күйінде қалады.

Project Operations бағдарламасы ресурстың екеуін де тапсырмаға тағайындамайды, себебі бұл әрекеттен болжамдылығы төмен кесте жасалады. Бұл қарапайым мысалда сағаттарды екі ресурсқа тең бөлген оңай. Алайда, бірнеше тапсырманы және бірнеше ресурсты қамтитын әлдеқайда күрделі сценарийлерде PSA бағдарламасы бірнеше тапсырма бойынша бірнеше ресурстан алынған тапсырыстарды бөлу жолы туралы болжам жасауы керек.

Сондықтан, осы сценарийлерде жоба менеджері бірнеше тапсырысты талдауға және қажет болған жағдайда оларды тағайындауға жауап береді. Тапсырыстарды бөлектеу үшін, жоба менеджері жалпы ресурстардың тапсырмаларын аталған ресурстарға тағайындайды, содан кейін **Салыстырып тексеру** көрінісін бөлектеу әрекетінің тапсырыспен бірге жұмыс істейтініне көз жеткізу үшін қолданады.

### <a name="edit-a-resource-requirement"></a>Ресурс талабын өңдеу

Ресурс талабы жасалғаннан кейін, жоба менеджері немесе ресурс менеджері кесте тақтасы қолданылған кезде, іздеу шарттарын нақтылау үшін мәліметтерді өңдеуді қалауы мүмкін. Ресурс талабын өңдеу үшін, келесі қадамдарды орындаңыз.

1. **Жобалар** пішініндегі **Топ** қойыншасында жалпы ресурс бойынша кез келген талап сілтемесін таңдаңыз.
2. Пайда болатын **Ресурс талабы** пішінінде қажетті өріс туралы ақпаратты енгізіңіз

   **Ресурс талабы** пішінінде, жоба менеджері немесе ресурс менеджері дағдыларды, рөлдерді, ресурстардың артықшылықтарын және таңдаулы ұйымдық бөлімді анықтай алады.

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a>Ресурс тапсырыстарын жобада резервтелгеннен кейін жаңарту

Жоба тобына жалпы немесе аталған ресурсты қосқаннан кейін, ресурс тапсырыстарын өзгертуге болады.

1. **Жобалар** пішініндегі **Топ** қойыншасында топ мүшесін, содан кейін **Тапсырыстарды жүргізу** параметрін таңдаңыз.
 
   Кесте тақтасы пайда болады және жоба тобы мүшесінің тапсырыстарын көрсетеді. Осы жоба және топ мүшесінің мүмкіндігін пайдаланатын басқа жобалар бойынша резервтелген сағаттарды көру үшін, топ мүшесінің жазбасын кеңейтіңіз.

2. Тапсырысты кеңейту немесе қысқарту үшін, оны таңдап сүйреңіз. Сонда тапсырысты реттеуге мүмкіндік беретін **Ресурс тапсырысын жасау** диалогтық терезесі пайда болады.
3. Тапсырысты тінтуірдің оң жақ түймешігімен басыңыз. Келесі әрекеттерді орындау үшін, контекстік мәзірді пайдалануға болады:

    - Тапсырыс күйін өзгерту
    - Тапсырысты өңдеңіз
    - Жоба тобындағы ресурсты алмастыру

### <a name="change-the-booking-status"></a>Тапсырыс күйін өзгерту

Кез келген әдепкі немесе реттелмелі тапсырыс күйін өзгертуге болады.

Келесі күйлер Project Operations бағдарламасында қамтылған:

- **Бас тартылды**: ресурстың тапсырысын болдырмайды және ресурс сыйымдылығын босатады.
- **Қорытынды резервтеу**: ресурс сыйымдылығын пайдаланады. Әдетте **Жобалар** пішініндегі **Барлық топ мүшелері** торынан **Тапсырыстарды жүргізу** параметрін ашқан кезде, тапсырыс осы күйге ие болады.
- **Алдын ала резервтеу**: топқа ресурсты қосады, бірақ ресурстың сыйымдылығын пайдаланбайды. Бұл күй ресурстың ықтимал тапсырма үшін сақталғанын, бірақ басқа тапсырмалар үшін қажет болса, сыйымдылығы бар екенін көрсетеді. Ресурстың жалпы қолжетімділігі тұрғысынан, алдын ала резервтеулер қорытынды резервтеулерге қарағанда басқа күйге ие.
- **Ұсынылған**: ресурс менеджері немесе жоба менеджерінің ресурс туралы ұсынысын білдіреді. Ұсыныстар ресурстың сыйымдылығын пайдаланбайды және ресурс жоба тобына қосылмайды. Топтағы ресурсты түпкілікті резервтеу үшін, жоба менеджері ұсынысты қабылдауы керек.

### <a name="submit-resource-requests"></a>Ресурс сұрауларын жіберу

Ресурс сұраулары ресурс менеджері орындауы керек сұранысты немесе ресурс талабын орындау үшін қолданылады. Топта әлдеқашан бар жалпы ресурс үшін ресурс сұрауын тікелей жіберуге болады. Ресурс сұрауы екі жолмен орындалуы мүмкін:

- Ресурс менеджері сұрауды тікелей орындайды. Бұл жағдайда, жалпы ресурс аталған ресурсы бар қорытынды резервтеумен ауыстырылады.
- Ресурс менеджері жоба менеджеріне ресурсты ұсынады, ал жоба менеджері ұсынылған ресурсты мақұлдайды немесе қабылдамайды.

#### <a name="direct-fulfillment-of-resource-requests"></a>Ресурс сұрауларын тікелей орындау

Ресурс талабы жасалған кезде, жоба менеджері ресурсты таңдап, **Сұрау жіберу** пәрменін таңдау арқылы жалпы ресурсқа сұрау жібере алады. Ресурс туралы пікірлер сұрауды орындайтын ресурс менеджеріне берілуі мүмкін. Сұрау жіберілгеннен кейін, топ мүшесінің **Күй** өрісі **Жіберілді** күйіне өзгертіледі. Ресурс менеджері сұрауды орындаған кезде, жалпы топ мүшесі **Барлық топ мүшелері** торындағы аталған ресурспен алмастырылады.

#### <a name="use-a-resource-proposal-for-resource-requests"></a>Ресурс сұраулары үшін ресурс ұсынысын пайдалану

Ресурс сұрауы бойынша тікелей резервтеудің орнына, ресурс менеджері жоба менеджеріне ресурсты ұсына алады. Ресурс менеджері талаптарға дәл сәйкестік болмаған кезде осы опцияны қолдана алады. Ресурс менеджері ресурсты ұсынған кезде, жоба менеджері жалпы топ мүшесінің **Күй** өрісі **Қарап шығуды талап етеді** күйіне өзгертілгенін көреді.

Сіз ұсынылған ресурстарды ұсынысты резервтеу әсерінің визуализациясымен бірге көре аласыз. 

1. **Қарап шығуды талап етеді** күйіне ие топ мүшесін екі рет басыңыз. 
2. **Ұсынылатын ресурстар** қойыншасын таңдаңыз.
3. Барлық ұсынылған ресурстарды қабылдау **Барлық ұсыныстарды қабылдау** параметрін немесе оларды қабылдамау үшін **Барлық ұсыныстарды қабылдамау** параметрін таңдаңыз. Егер ұсынылған ресурстарды қабылдасаңыз, онда олар жобада топ мүшелері ретінде түпкілікті резервтеледі және жалпы ресурстарды алмастырады.

> [!NOTE]
> Барлық ұсынылған ресурстарды қабылдауыңыз немесе қабылдамауыңыз керек. Оларды ішінара қабылдасаңыз немесе қабылдамасаңыз болады.

### <a name="substitute-a-resource-on-the-project-team"></a>Жоба тобындағы ресурсты алмастыру

Кейде жоба менеджері резервтелген топ мүшесін жоба бойынша алмастыруы керек.

1. **Жобалар** пішініндегі **Топ** қойыншасында алмастыру керек ресурсты, содан кейін **Тапсырыстарды жүргізу** параметрін таңдаңыз.
2. Тағайындалған жобаларын көру үшін ресурсты кеңейтіңіз.
3. Жобаны тінтуірдің оң жақ түймешігімен басып, **Орын басушы ресурс** параметрін таңдаңыз.
4. Егер ағымдағы ресурсты алмастырғыңыз келетін ресурсты білсеңіз, атауын таңдаңыз немесе теріңіз де, **Қайта тағайындау** параметрін таңдаңыз.

Немесе. егер сізге ресурс іздеу қажет болса, келесі қадамдарды орындаңыз.

1. **Ауыстырылатын элементті табу** параметрін таңдаңыз.

   Кесте көмекшісі қолжетімді орын басушылар тізімін қайтарады. Кесте көмекшісінде қолайлы орын басушыны табу үшін қолжетімді ресурстарды одан әрі сүзгілей аласыз.

2. Ресурсты ауыстыру үшін, қажетті ресурсты басып, **Ауыстыру** параметрін таңдаңыз.   

   Тапсырыстар мен тағайындаулар жаңа ресурспен алмастырылды.

## <a name="reconcile-team-member-bookings-and-assignments"></a>Топ мүшесінің тапсырыстары мен тағайындауларын салыстырып тексеру

Топ мүшелері үшін тапсырыстар мен тағайындаулар бір-бірімен тығыз байланысқан. Басқаша айтқанда, ресурстарда тағайындаулар бар болуы, бірақ тапсырыстар жоқ болуы немесе тапсырыстар бар болуы, бірақ тағайындаулар жоқ болуы мүмкін. Ең дұрысы, тапсырыстар мен тағайындаулар ресурстар тапсырма тағайындауларын орындауға қабілетті болатындай туралануы керек. Алайда, тапсырыстар қолжетімділікке негізделуі мүмкін және жоба жалғасқан кезде тапсырма мерзімі өзгеруі мүмкін. Сондықтан, тапсырыстар мен тағайындаулардың бос байланысы икемділікті қамтамасыз етеді.

Project Operations бағдарламасындағы **Салыстырып тексеру** қойыншасы жоба менеджерлеріне топ мүшелерінің тапсырыстары мен жоба топтарына берілген тағайындауларды салыстырып тексеруге мүмкіндік береді.

**Салыстырып тексеру** қойыншасында топтың әр мүшесі үшін жеке тапсырма тағайындауы деңгейіндегі тапсырыстар мен тағайындаулар көрсетілген. Онда уақыт кезеңдерін айлардан күндерге дейін көрсететін ұяшықтардағы сағаттар көрсетіледі.

Сондай-ақ қойыншада жалпы бағанмен бірге жобаның жалпы таза қорытындысы көрсетіледі.

Әр ресурс үшін қойыншада топ мүшелерінің тапсырыстары мен топ мүшелерінің тапсырма тағайындауларының жиынтығы арасындағы айырмашылық есептеледі. Ең дұрысы, бұл айырмашылық 0 (нөл) мәніне тең болуы керек. Басқаша айтқанда, тапсырыстар мен тағайындаулардың арасында ешқандай айырмашылық болмауы керек. Айырмашылықтар екі шартқа назар аударту үшін түспен ерекшеленген және көлеңкеленген:

- **Тапсырыс тапшылығы**: ресурста тапсырыстарға қарағанда тағайындаулар көп болған кезде орын алады. Бұл сыйымдылық сақталмағандықтан, жоба менеджері тапшылықты жабу үшін ресурс тапсырыстарын кеңейту арқылы бұл жағдайды түзетуді қалауы мүмкін.
- **Артық тапсырыстар**: жоба үшін ресурсқа тапсырыс берілген кезде, бірақ тапсырмаларға тағайындалмаған кезде орын алады. Бұл шарт ресурс тапсырма тағайындалғанға дейін жобаға резервтелген жағдайда қолайлы болуы мүмкін. Алайда, басқа жағдайларда, ресурс тапсырмаларға тағайындалады деп жоспарланбайды. Мұндай жағдайларда жоба менеджері сыйымдылықты басқа жоба үшін пайдалануға болатындай ресурс тапсырыстарынан бас тарту туралы ойлануы керек.

Кейбір жағдайларда уақытты күн деңгейінен, мысалы, ай деңгейінен, жоғары деңгейде қараған кезде, ресурс үшін нөлдің таза айырмашылығын байқай аласыз. Басқаша айтқанда, тапсырыстар = тағайындаулар. Алайда, егер уақытты апта деңгейінде қарасаңыз, онда бірінші аптада нөл сағаттық және 40 сағаттық тағайындаулар бар екенін, ал екінші аптада 40 сағаттық және нөл сағаттық тағайындаулар бар екенін көре аласыз. Жалпы, тапсырыстар мен тағайындаулар салыстырып тексерілген, бірақ олар бір аптадан екінші аптаға дейін ерекшеленеді.

Уақытты жоғарырақ деңгейде қарасаңыз, **Салыстырып тексеру** қойыншасындағы ұяшықтарда төменгі деңгейлерде айырмашылықтар бар екендігі туралы хабардар ететін индикатор бар болады. Айырмашылықты көру үшін ұяшықты екі рет басыңыз. Кішірейту үшін оны тінтуірдің оң жақ түймешігімен басуға болады. Ресурсты таңдап, тордың құралдар тақтасындағы **Келесі айырмашылық** басқару элементін таңдау арқылы сол ресурстың тапсырыстары мен тағайындаулары арасындағы келесі айырмашылыққа өтуіңізге болады. Кері қайту үшін **Алдыңғы айырмашылық** параметрін таңдаңыз. Сондай-ақ айырмашылық индикаторы мен шарлау әрекетін **Параметрлер** тармағында өшіруге болады.

Егер ресурсқа арналған тапсырма тағайындаулары бар болса, бірақ тапсырыстар жоқ болса, **Жобалар** пішініндегі **Салыстырып тексеру** қойыншасында тапсырыс тапшылығын, содан кейін **Тапсырыстың мерзімін ұзарту** параметрін таңдаңыз. Сонда **Тапсырыстың мерзімін ұзарту** диалогтық терезесі пайда болады және ресурс тапшылығын жою үшін қажет тапсырысты көрсетеді. Сондай-ақ диалогтік терезеде барлық жобалар немесе басқа жоспарланатын нысандар бойынша ресурстың бар тапсырыстары көрсетіледі. Егер ресурс үшін тапсырысты жасау үшін **OK** опциясын таңдасаңыз, сол ресурстың қолжетімділігіне қарамастан, артық тапсырыстың туындауына себеп болуыңыз мүмкін.

Кейін жоба менеджері немесе ресурс менеджері ресурстар кестесін ресурс сыйымдылығынан асыра шамадан тыс резервтелген кез келген жағдайларды басқару үшін қолдана алады.
