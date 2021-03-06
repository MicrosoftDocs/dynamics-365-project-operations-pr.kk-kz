---
title: Шығысты басқару параметрлерін конфигурациялау
description: Бұл тақырып шығыстарды басқарудағы жалпы тәртіпті басқаратын параметрлерді сипаттайды.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 8ecbd0abc16d0a29eea47d6bd1653a204a83de4c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897278"
---
# <a name="configure-expense-management-parameters"></a>Шығысты басқару параметрлерін конфигурациялау

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Бұл тақырып шығыстарды басқарудағы жалпы тәртіпті басқаратын параметрлерді сипаттайды.

## <a name="general"></a>Жалпы мәліметтер 

| Өріс                                                    | Сипаттамасы |
|----------------------------------------------------------|-------------|
| Жүрістің стандартты жылдамдығы                                 | Жүріс шығыстарын өтеу мөлшерлемесін енгізіңіз. Бұл мөлшерлеме жол шығындары үшін өтелетін соманы есептеу үшін шығыстарға енгізілген жүріске көбейтіледі. |
| Шығыс мақсатын растау                                 | Бұл параметрді пайдаланушылар шығыс есептерін жасағанда оларды **Шығыс есебінің мақсаты** өрісінде конфигурацияланған мәндер жиынына шектеу үшін қосыңыз. |
| Жеке шығыстарды төлеуші                                | Жеке тұлғалар санатына жатқызылған несиелік карта бойынша кез келген транзакция сомаларын төлеуге кім жауапты екенін таңдаңыз. |
| Барлық шығындар туралы есепті көрсету               | Шығындар туралы есеп орналастырылған кезде пайда болған белгілі бір ваучер үшін бастапқы құжаттың егжей-тегжейлері қаралған кезде шығыстар туралы есеп бойынша барлық шығындарды көрсету үшін осы опцияны таңдаңыз. |
| Сапарды алдын ала авторизациялау міндетті болып табылады                 | Қызметкер шығыстар туралы есеп бергенге дейін сапарға өтініш беруді және бекітуді талап ету үшін осы параметрді таңдаңыз. |
| Орналастыруға дейін таратылымдарды өңдеуге рұқсат ету            | Шығыстар туралы есепті орналастырудан бұрын оны өңдеуге болатындығын таңдаңыз. |
| Шығыстарды басқару саясатын бағалаңыз                     | Шығыс саясаты бұзылғанын анықтау үшін шығыстар қашан бағаланатынын таңдаңыз. Шығыстарды енгізу және сақтау кезінде немесе шығыстарды бекітуге ұсыну кезінде шығындарды бұзушылықтар бойынша бағалауға болады. Қажетті түсімдерге қатысты саясат ережелері шығыстар үнемделген кезде бағаланады. |
| Компанияаралық шығыстар желісіне рұқсат етіңіз                         | Басқа заңды тұлғалар үшін шығыстарды шығыстар туралы есепке енгізуге болатындығын таңдаңыз. |
| Несиелік карта бойынша шығындардың айырбас бағамын өзгертуге рұқсат етіңіз | Пайдаланушыға импортталған несиелік картаға арналған айырбас бағамын түзетуге мүмкіндік беру үшін осы параметрді таңдаңыз. |
| Көрсетілетін көп деңгейлі иерархия өрістері                  | Жұмыс ағынының тағайындау түрі иерархия ретінде орнатылғанда және **Иерархия** таңдау мақұлдау иерархиясын, шығындардың көп деңгейлі мақұлдауын пайдалану үшін орнатылғанда қандай мақұлдаушы өрістер көрсетілетінін таңдаңыз. Көп деңгейлі мақұлдау иерархиясы жұмыс процесінде пайдаланылған кезде таңдалған өрістер шығыстар туралы есепте көрсетіледі және оларды өңдеуге болады. |
| Қызметкердің несиелік картасы нөмірін енгізіңіз                        | Қызметкердің **Несие карталары** бетіндегі **Карта идентификаторы** өрісінде 15 таңбалы немесе 16 таңбалы нөмірді енгізуге және сақтауға болатынын таңдаңыз. |
| Сапар туралы сұраныстың мақсатын растаңыз                      | Бұл параметрді пайдаланушылар сапар сұраныстарын жасағанда оларды **Шығыс есебінің мақсаты** өрісінде конфигурацияланған мәндер жиынына шектеу үшін қосыңыз. |

## <a name="financial"></a>Қаржы қызметі

| Өріс                                                                                    | Сипаттамасы |
|------------------------------------------------------------------------------------------|-------------|
| Кітаптың күнделікті журнал атауы                                                                | Шығыстар туралы есептер орналастырылған кітап журналының атауын таңдаңыз. |
| Шығыстардан салықты қалпына келтіруге мүмкіндік беру                                                        | Сәйкес шығыстар үшін шығыстар салығын қалпына келтіруді қосу үшін осы опцияны таңдаңыз. Егер АҚШ сату салығы мен салық салу ережелері қосылса, бұл опцияны таңдау мүмкін емес. |
| Ақшалай аванстарды дереу жариялаңыз                                                           | Төлеу және аудару процесі аяқталғаннан кейін бекітілген ақшалай авансты орналастыру үшін осы опцияны таңдаңыз. Егер бұл опция таңдалмаса, төлеу және аудару процесі жарияланбаған жалпы журнал жасайды. |
| Орналастыру кезіндегі дұрыс есептік күн                                                   | Ағымдағы кезең тоқтатылған немесе жабық болса, шығыстар орналастырылған кезде есептік күнді жаңарту үшін осы опцияны таңдаңыз. Есепке алу күні келесі ашық кезеңге қойылады. |
| Төлем әдісінде көрсетілген шығындарды есепке алу шоты негізінде транзакцияларды топтауға рұқсат ету       | Шығындарды төлеу әдісінде көрсетілген өзара есепке алу шоты негізінде шығындар туралы есепке арналған шығындар туралы есептерді жинақтау үшін осы опцияны таңдаңыз. |
| Салық қосылған                                                                             | Сату салығын әдепкі бойынша шығындар сомасына қосу үшін осы опцияны таңдаңыз. |
| Сапар сұраныстарын жабу бойынша ауыртпалықтардан босату                                      | Бекітілген сапар сұранысы жабылған кезде ауыртпалықтағы қаражатты босату үшін осы опцияны таңдаңыз. |
| Сапар сұранысына бюджеттік тіркелім мен жобаның бюджеті үшін бюджеттің асып кетуіне рұқсат ету | Бюджеттік тіркелімде белгіленген бюджеттен немесе жобаның рұқсат етілген бюджетінен асып кетсе де, қызметкерлерге сапар сұраныстарын бекітуге жіберуге мүмкіндік беру үшін осы опцияны таңдаңыз. |
| Шығыстар есебіне бюджеттік тіркелім мен жобаның бюджеті үшін бюджеттің асып кетуіне рұқсат ету     | Бюджеттік тіркелімде белгіленген бюджеттен немесе жобаның рұқсат етілген бюджетінен асып кетсе де, қызметкерлерге шығыстар есептерін бекітуге жіберуге мүмкіндік беру үшін осы опцияны таңдаңыз. |
| Шығыстар есебін бекітуді тек бюджеттік тіркелім үшін бюджеттің асып кетуіне рұқсат ету                 | Бекітушілерге бюджеттік тізілімде белгіленген рұқсат етілген бюджеттен асатын шығындар туралы есептерді бекітуге мүмкіндік беру үшін осы параметрді таңдаңыз. |

## <a name="per-diem"></a>Тәуліктік

| Өріс                                 | Сипаттамасы |
|---------------------------------------|-------------|
| Бір тәуліктегі минималды сағат            | Қызметкер сапарға байланысты шығындар үшін тәуліктік ақы алу үшін бір күнде жұмыс істеуі керек болатын әдепкі ең аз сағат санын енгізіңіз. Бұл мән тәуліктік ставкалар деңгейіне арналған **Минималды сағаттар** өрісі үшін әдепкі мән ретінде пайдаланылады. |
| Тамақтану пайызы                          | **Тамақтануды азайтуды есептеу** өрісі **Күнделікті тағам түрі** немесе **Күнделікті тамақтану саны** параметріне орнатылғанда, іссапар шығындарының бірінші және соңғы күндерінде пайдаланылатын тағам үшін әдепкі тәуліктік пайызды енгізіңіз. Бірінші және соңғы күндердегі жұмыс күні әдеттегі жұмыс күніне қарағанда қысқа болуы мүмкін. Сондықтан сол күндері тәуліктік төлемнің мөлшері стандартты мөлшерден өзгеше болуы мүмкін. Егер пайыздық мәні **0** (нөл) мәніне орнатылған болса, алғашқы және соңғы күндердегі аударымдар 0,00 құрайды. |
| Қонақ үй пайызы                         | Іссапар шығындарының бірінші және соңғы күндерінде пайдаланылатын қонақүйлер үшін тәуліктік төлемнің әдепкі пайызын енгізіңіз. Бірінші және соңғы күндердегі жұмыс күні әдеттегі жұмыс күніне қарағанда қысқа болуы мүмкін. Сондықтан сол күндері тәуліктік төлемнің мөлшері стандартты мөлшерден өзгеше болуы мүмкін. Егер пайыздық мәні **0** (нөл) мәніне орнатылған болса, алғашқы және соңғы күндердегі аударымдар 0,00 құрайды. |
| Басқа пайыздар                         | Іссапар шығындарының бірінші және соңғы күндерінде пайдаланылатын әр түрлі шығындар үшін тәуліктік төлемнің әдепкі пайызын енгізіңіз. Бірінші және соңғы күндердегі жұмыс күні әдеттегі жұмыс күніне қарағанда қысқа болуы мүмкін. Сондықтан сол күндері тәуліктік төлемнің мөлшері стандартты мөлшерден өзгеше болуы мүмкін. Егер пайыздық мәні **0** (нөл) мәніне орнатылған болса, алғашқы және соңғы күндердегі аударымдар 0,00 құрайды. |
| Таңғы асқа пайызбен төмендету | Таңертеңгілік тамақтану күніне азайтылатын соманы енгізіңіз. Мысалы, егер қызметкер тегін таңғы ас алса, сіз тәуліктік төлем мөлшерін 10 пайызға азайтуды қалауыңыз мүмкін. |
| Түскі асқа пайызбен төмендету     | Түскі уақыттағы тамақтану күніне азайтылатын соманы енгізіңіз. Мысалы, егер қызметкер тегін түскі ас алса, сіз тәуліктік төлем мөлшерін 15 пайызға азайтуды қалауыңыз мүмкін. |
| Кешкі асқа пайызбен төмендету    | Кешкі уақыттағы тамақтану күніне азайтылатын соманы енгізіңіз. Мысалы, егер қызметкер тегін кешкі ас алса, сіз тәуліктік төлем мөлшерін 25 пайызға азайтуды қалауыңыз мүмкін. |
| Тамақты азайтуды есептеу           | Бұл азайту бір реттік сапар немесе бір күндік тамақтану түріне негізделгенін немесе ол күніне рұқсат етілген тамақтану санына негізделгенін таңдау арқылы жүйенің тәуліктік тамақтануды төмендетуді қалай есептеу керектігін көрсетіңіз. |
| Тәуліктік дөңгелектеу                     | Тәуліктің шығындар үшін пайдаланылатын дөңгелектеу түрін таңдаңыз. Егер сіз қалыпты дөңгелектеуді таңдасаңыз, тәуліктік шығындар 0,50 болса, 1,00-ге дейін, ал күндізгі шығындар 0,50-ден аз болса, 0,00-ге дейін дөңгелектенеді. |
| Тәуліктік есептеу негізі          | Тәуліктік төлем күнтізбелік күнге немесе 24-сағаттық мерзімге негізделгендігін таңдаңыз. |

## <a name="fax-cover-pages"></a>Факстың мұқаба беттері

| Өріс                          | Сипаттамасы |
|--------------------------------|-------------|
| Нұсқаулар                   | Қызметкерлер шығындар туралы есеппен байланысты түбіртектерді жіберу үшін пайдаланылатын факс үшін мұқаба бетін жасаған кезде орындауы керек нұсқауларды енгізіңіз. Көрсетілетін белгілі бір мәтінді қолданушы тіліне сүйене отырып енгізу үшін **Аудармалар** опциясын таңдаңыз. |
| Пайдаланушының идентификаторы (штрих-код туралы ақпарат) | Қызметкердің бірегей идентификаторын факстың мұқаба бетінде пайдаланылатын штрих-кодта сақтау үшін осы опцияны таңдаңыз. |
| Штрих-код                       | Факстың мұқаба бетінде пайдаланылатын штрих-кодты таңдаңыз. 39 және 128 штрих-кодтарына шығыстарды басқаруда қолдау көрсетіледі. |

## <a name="anti-corruption"></a>Сыбайлас жемқорлыққа қарсы іс-қимыл

| Өріс                                 | Сипаттамасы |
|---------------------------------------|-------------|
| Сыбайлас жемқорлыққа қарсы аттестаттауды көрсету   | Шығындар туралы есеп жасалған кезде сыбайлас жемқорлыққа қарсы мәтінді көрсету үшін осы опцияны таңдаңыз. Содан кейін шығындар туралы есепте сыбайлас жемқорлыққа қарсы аттестаттауды таңдауды талап ететін шығындардың нақты санаттарын қосуға болады. Мысалы, үкіметтің ресми шығындарымен байланысты сыйлық категориясы қызметкерден шығындардың мемлекеттік қызметкерлерге қатысты компания саясатына сәйкес келетіндігін растауын талап етуі мүмкін. |
| Жіберушіге арналған сыбайлас жемқорлыққа қарсы хабарлама | Шығындар туралы есеп құратын қызметкерге көрсетілуі керек мәтінді енгізіңіз. Көрсетілетін белгілі бір мәтінді қолданушы тіліне сүйене отырып енгізу үшін **Аудармалар** опциясын таңдаңыз. |
| Бекітушіге арналған сыбайлас жемқорлыққа қарсы хабарлама  | Шығыстар туралы есеп жасалғанда бекітушіге көрсетілетін мәтінді енгізіңіз. Көрсетілетін белгілі бір мәтінді қолданушы тіліне сүйене отырып енгізу үшін **Аудармалар** опциясын таңдаңыз. |
