---
title: 2021 жылдың мамыр айындағы қосалқы/өндіріске негізделген сценарийлеріне арналған Project Operations бағдарламасындағы жаңалықтар немесе өзгерістер
description: Бұл мақалада жинақталған/өндіріске негізделген сценарийлер үшін Жоба операцияларының 2021 жылдың мамыр айындағы шығарылымында қолжетімді сапа жаңартулары туралы ақпарат берілген.
author: andchoi
ms.date: 07/01/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: andchoi
ms.openlocfilehash: eff34a4e9fc1fc6429f1fa7a3e4b0d5b664222f9
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/18/2022
ms.locfileid: "9029399"
---
# <a name="whats-new-or-changed-in-project-operations-may-2021-for-stockedproduction-based-scenarios"></a>2021 жылдың мамыр айындағы қосалқы/өндіріске негізделген сценарийлеріне арналған Project Operations бағдарламасындағы жаңалықтар немесе өзгерістер

_ **Келесіге қолданылады:** қосалқы/өндіріске негізделген сценарийлеріне арналған Project Operations бағдарламасы

Бұл мақала келесіге қатысты Dynamics 365 Project Operations құрамдас бөліктер мен нұсқалар:

- Dynamics 365 Finance ортасында жобаны басқару және есепке алу 10.0.19 нұсқасында
 
### <a name="quality-updates"></a>Сапа жаңартулары
                                                                                                                                                                                  
| Мүмкіндік аумағы                      | Сілтемелік нөмір| Сапа жаңартуы                                                                                                                                                                          |
|-----------------------------------|--------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Жобаларды басқару және есеп | [529751](https://fix.lcs.dynamics.com/Issue/Details/?bugId=529751) | Жоба элементінің журнал жолы үшін нысанды тексеру өшірулі болған кезде импорттау сәтсіз аяқталады.                                                                                                                                                   |
| Жобаларды басқару және есеп | [550565](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550565) | **GeneralJournalEntry** параметрін іздеумен байланысты WIP тіркелгілері есебінде өнімділік мәселесі бар.                                                                                                                                  |
| Жобаларды басқару және есеп | [539044](https://fix.lcs.dynamics.com/Issue/Details/?bugId=539044) | WIP жобасында қаржылық өлшемдер жоқ.                                                                                                                                                                                                    |
| Жобаларды басқару және есеп | [540903](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540903) | **ProjBudgetReductionHistory** сипаты дұрыс емес **ProjBudgetAllocationLineIdSales** параметрі тағайындалғандықтан есеп‑шот ұсынысын жариялау сәтсіз болады.                                                                                                                           |
| Жобаларды басқару және есеп | [547090](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547090) | XML файлын импорттағаннан кейін, жалпы журнал қате ваучер нөмірлерін көрсетеді.                                                                                                                                                              |
| Жобаларды басқару және есеп | [552160](https://fix.lcs.dynamics.com/Issue/Details/?bugId=552160) | Жұмыс декомпозициясының құрылымы үлгісінде қате орын алды.                                                                                                                                                                                          |
| Жобаларды басқару және есеп | [552976](https://fix.lcs.dynamics.com/Issue/Details/?bugId=552976) | **Пішін ескертпелері** және **Пішінді орнату** параметрлері Project Operations бағдарламасымен біріктірілген кезде Қаржы заңды нысандарындағы жобаны басқаруды орнатуды көрінбейді.                                                                                                             |
| Жобаларды басқару және есеп | [553313](https://fix.lcs.dynamics.com/Issue/Details/?bugId=553313) | Компания аралық сату тапсырысынан бас тарту кезінде келесі қате орын алады: "Сатып алуға тапсырыс жолдарындағы жазбаны өңдеу мүмкін емес (PurchLine). Басқа пайдаланушы процесі жазбаны жоюына немесе жазбадағы бір немесе бірнеше өрісті өзгертуіне байланысты жаңарту қайшылығы орын алды." |
| Жобаларды басқару және есеп | [553775](https://fix.lcs.dynamics.com/Issue/Details/?bugId=553775) | Жоба транзакциясын реттеу жоба құны үшін дұрыс емес қаржылық өлшем жасайды.                                                                                                                                                          |
| Жобаларды басқару және есеп | [556751](https://fix.lcs.dynamics.com/Issue/Details/?bugId=556751) | Жобамен байланысты сатып алу тапсырысын өңдеу кезінде жеткізушінің есеп‑шотында қосымша сұрау болады.                                                                                                                                                 |
| Жобаларды басқару және есеп | [557925](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557925) | Уақыт кестесінің жолдарын бекіту мүмкін емес және келесі қате пайда болады: "Жұмыс ағыны үшін белсендіру шарты жарамсыз. Бұл мәселе туралы жүйе әкімшісіне хабарлаңыз."                                                                          |
| Жобаларды басқару және есеп | [559266](https://fix.lcs.dynamics.com/Issue/Details/?bugId=559266) | Егер сіз "Жоба келісімшартын өзгерту мүмкін емес, өйткені байланысты XXXXXX жобасы үшін транзакция бар" қатесін алсаңыз, сіз келісімшартты жоба деңгейінде әлі де өзгерте аласыз.                                                                           |
| Жобаларды басқару және есеп | [560432](https://fix.lcs.dynamics.com/Issue/Details/?bugId=560432) | Егер сіз "Санын есеп‑шотта көрсету мүмкін емес, себебі шегерілген күйіндегі түгендеу транзакциялар жеткіліксіз" деген қате алсаңыз, қорда қайта есептеу жүргізілгеннен кейін сатып алуға тапсырыс есеп‑шотын жариялау мүмкін емес.                             |
| Жобаларды басқару және есеп | [562013](https://fix.lcs.dynamics.com/Issue/Details/?bugId=562013) | Ресурс сұрауының жұмыс ағыны қосылған кезде, жоба ресурсының қолжетімділігін басқаратын беттерді ашуға әрекет еткен кезде өнімділік мәселелері туындайды.                                                                                                               |
| Жобаларды басқару және есеп | [488320](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488320) | Жоба келісімшартына басқа жобаны көрсету үшін төлем ережесін қосқаннан кейін есеп‑шот күйі **Ақысыз** күйіне өзгереді.                                                                                                                                |
| Жобаларды басқару және есеп | [515219](https://fix.lcs.dynamics.com/Issue/Details/?bugId=515219) | Алдын-ала төлеу есеп‑шотын жобаның сатып алу тапсырыстан алып тастаған кезде қате орын алады және **Жоба бойынша кейінгі алдын-ала төлем құны** параметрі қосылады.                                                                                                        |
| Жобаларды басқару және есеп | [526439](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526439) | Жобаның сатып алу тапсырысының есеп‑шотын жариялаған кезде элементті автоматты белгілеу мүмкіндігі жоқ болғандықтан қате орын алады.                                                                                                                            |
| Жобаларды басқару және есеп | [527970](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527970) | Егер тарату түрі жоба есеп‑шот ваучерлеріне арналған сатылым салығына тең болса, ҚҚС үшін әдепкі сипаттама бос болады.                                                                                                                                           |
| Жобаларды басқару және есеп | [530352](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530352) | Егер сіз қатысты бас тартылған элемент талабының сатылым тапсырысын жойсаңыз, жобаның сатып алу тапсырысы қате көрсетеді.                                                                                                                                 |
| Жобаларды басқару және есеп | [530651](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530651) | Жоба элементінің талабын сатып алу тапсырыстарына құсбелгі қойғанда және алып тастаған кезде сілтемелер жоғалады.                                                                                                                                                               |
| Жобаларды басқару және есеп | [533023](https://fix.lcs.dynamics.com/Issue/Details/?bugId=533023) | Жоба элементтерінің талаптары үшін таңдау тізімін басып шығарған кезде азайтылған санның әдепкі мәнімен мәселе туындайды.                                                                                                                                                 |
| Жобаларды басқару және есеп | [535493](https://fix.lcs.dynamics.com/Issue/Details/?bugId=535493) | Жеткізілім артық болса, есептелген сату бағасы дұрыс емес.                                                                                                                                                                                 |
| Жобаларды басқару және есеп | [541329](https://fix.lcs.dynamics.com/Issue/Details/?bugId=541329) | Ұстап қалу есеп‑шот ұсынысындағы есеп‑шот мөлшерінсіз босатылған кезде дұрыс емес міндеттеме жарияланады.                                                                                                                                                |
| Жобаларды басқару және есеп | [541997](https://fix.lcs.dynamics.com/Issue/Details/?bugId=541997) | Уақыт кестесі кезеңін жасаған кезде бірінші кезең 53-ші апта ретінде көрсетіледі.                                                                                                                                                                         |
| Жобаларды басқару және есеп | [542043](https://fix.lcs.dynamics.com/Issue/Details/?bugId=542043) | Dynamics 365 Project Service Automation біріктіру параметрлеріндегі әдепкі жоба түрлері уақыт пен материал және бекітілген баға болуы керек.                                                                                                         |
| Жобаларды басқару және есеп | [543096](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543096) | Шот ұсыну ережелері бар есеп‑шот ұсынысын жою таратулар тудырады.                                                                                                                                                                              |
| Жобаларды басқару және есеп | [543463](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543463) | Толық орындалу әдісті қолдана отырып жою процесінің қорытынды бағасын жою мүмкін емес, себебі жүйе кірісті мойындамайды.                                                                                                                                      |
| Жобаларды басқару және есеп | [543938](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543938) | Жоба болжамын жариялаған кезде, хабарлама болжамының жазбасы жасалмайды.                                                                                                                                                                            |
| Жобаларды басқару және есеп | [546885](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546885) | Күтудегі жеткізуші есеп-шотындағы негізгі шот компания аралық есеп‑шот кезінде табылмайды.                                                                                                                                                               |
| Жобаларды басқару және есеп | [547885](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547885) | Егер келісімшартта элемент талаптары болса, екінші қаржыландыру көзін қоса алмайсыз.                                                                                                                                                         |
| Жобаларды басқару және есеп | [550379](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550379) | **Жоба** > **Бюджет** > **Түзетулер** > **Жаңа** > **Импорттау** тармағын пайдаланған кезде жүйе барлық жобалар үшін жоба бюджетінде түзетулер жасайды.                                                                                                                         |
| Жобаларды басқару және есеп | [550577](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550577) |  Егер сіз транзакцияны басқа транзакциямен және есеп валюталарымен реттесеңіз, тарату және жалпы кітап жазбалары дұрыс емес болады.                                                                                                                                       |
| Жобаларды басқару және есеп | [557049](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557049) | Бекітілген құн шегерілмейтін салық сомасымен асыра көрсетілген.                                                                                                                                                                                   |
| Жобаларды басқару және есеп | [557376](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557376) | Транзакция үшін тарату есеп‑шотын жасаған кезде өлшемдер алынбайды.                                                                                                                                                                  |
| Жобаларды басқару және есеп | [559416](https://fix.lcs.dynamics.com/Issue/Details/?bugId=559416) | **PurchTotals.purchNewTotalAmount()** әдісі сатып алу тапсырысымен байланыстырылмаған күтудегі жеткізуші есеп‑шотын жасаған кезде шақырылады, нәтижесінде өнімділік мәселесі туындайды.                                                                                   |
| Жобаларды басқару және есеп | [563694](https://fix.lcs.dynamics.com/Issue/Details/?bugId=563694) | **Тұтынылған бюджет** және **Қалған бюджет** бағандары жоба бюджетінің қалдықтарында дұрыс емес сомалар көрсетеді.                                                                                                                                                |
| Жобаларды басқару және есеп | [565089](https://fix.lcs.dynamics.com/Issue/Details/?bugId=565089) | Project Operations бағдарламасы бар Dataverse жүйесінде тапсырмаға негізделген шот ұсыну пайдаланылған кезде транзакция екі рет жарияланады.                                                                                                                                         |
| Жобаларды басқару және есеп | [566869](https://fix.lcs.dynamics.com/Issue/Details/?bugId=566869) | Project Operations бағдарламасын пайдаланған кезде кірісті танудың пайыздық орындалуы дұрыс емес болады.                                                                                                                                                  |
| Жобаларды басқару және есеп | [568107](https://fix.lcs.dynamics.com/Issue/Details/?bugId=568107) | Project Operations біріктірілген сценарийінде күтудегі жеткізуші есеп‑шоты пайдаланылған кезде кіріс екі есе артады.                                                                                                                                          |
| Жобаларды басқару және есеп | [569736](https://fix.lcs.dynamics.com/Issue/Details/?bugId=569736) | Жобаның уақыт кестесін жариялау транзакциялардың қайталануын жасайды.                                                                                                                                                                        |
| Жобаларды басқару және есеп | [569819](https://fix.lcs.dynamics.com/Issue/Details/?bugId=569819) | Жұмысқа тапсырыс үшін элементті тұтыну журналын жариялаған кезде қате орын алады.                                                                                                                                  |
| Жобаларды басқару және есеп | [571197](https://fix.lcs.dynamics.com/Issue/Details/?bugId=571197) | Жобаның өндірістік тапсырысын келесі қатеге байланысты орындау мүмкін емес: "Нысан сілтемесі нысанның данасына орнатылмаған."                                                                                                                           |
| Жобаларды басқару және есеп | [572370](https://fix.lcs.dynamics.com/Issue/Details/?bugId=572370) | Егер кіріс профилінің ережесі **Топты орнату** параметріне орнатылған болса, біріктіру журналын жариялау мүмкін емес.                                                                                                                                                           |
| Жобаларды басқару және есеп | [573596](https://fix.lcs.dynamics.com/Issue/Details/?bugId=573596) | Бірнеше өлшем бірлігімен жолдары бар жобаның сатып алу тапсырысы үшін сатып алу есеп‑шотын жариялау мүмкін емес.                                                                                                                                             |
| Жобаларды басқару және есеп | [573637](https://fix.lcs.dynamics.com/Issue/Details/?bugId=573637) | Жобаның әдепкі қаржылық өлшемін **Жобалар V2** деректер нысанының көмегімен жаңарту мүмкін емес.                                                                                                                                                          |
| Жобаларды басқару және есеп | [573886](https://fix.lcs.dynamics.com/Issue/Details/?bugId=573886) | Салық компания валютасынан басқа валютада болған кезде жобаның сату тапсырысы үшін нота‑кредитін жасау мүмкін емес.                                                                                                                     |
| Жобаларды басқару және есеп | [574104](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574104) | Есеп‑шот ұсынысы 100-ден астам шот ұсыну ережелерімен жасалған кезде мәселе туындайды.                                                                                                                                                                  |
| Жобаларды басқару және есеп | [577211](https://fix.lcs.dynamics.com/Issue/Details/?bugId=577211) | Жоба болжамын құру процесінің аяқталуы тым ұзақ уақытты алады.                                                                                                                                                                      |
| Жобаларды басқару және есеп | [577785](https://fix.lcs.dynamics.com/Issue/Details/?bugId=577785) | **Барлық компаниялар бойынша жоба ресурстарын толтыру** функциясын іске қосқан кезде келесі қате орын алды: "ResRollupCalendar нысан атауы жарамсыз."                                                                                                                                   |
| Жобаларды басқару және есеп | [582329](https://fix.lcs.dynamics.com/Issue/Details/?bugId=582329) | Келісімшартты жойған кезде тұтынушымен байланысты мекенжай да жойылады.                                                                                                                                                                    |
| Сапар және шығыс                  | [514930](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514930) | Шығындар есебін мақұлдаудың жұмыс ағынының шарты дұрыс бағаланбаған.                                                                                                                                                                           |
| Сапар және шығыс                  | [519304](https://fix.lcs.dynamics.com/Issue/Details/?bugId=519304) | Шығындар туралы есеп саясаты жоба идентификаторын дұрыс бағаламайды.                                                                                                                                                                                   |
| Сапар және шығыс                  | [522463](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522463) | Компанияаралық шығын транзакциялары үшін **Жекеге бөлу** әрекеті дұрыс жұмыс істемейді.                                                                                                                                                                |
| Сапар және шығыс                  | [534702](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534702) | Кейде шығындар туралы есептер жолының негіздемелері сапар өтінімдері жойылған кезде жойылады. Бұл шығындар туралы есептің recid идентификаторы пен сапар өтінімі бірдей болған кезде орын алады.                                                            |
| Сапар және шығыс                  | [544368](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544368) | Шығындар туралы есеп саясаттары **Жоба идентификаторы** өрісін қажет еткен кезде, шығын мобильді бағдарламасында мәселе туындайды.                                                                                                                                                |
| Сапар және шығыс                  | [545331](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545331) | Жобамен байланысты компанияаралық шығынды өңдеуге әрекет еткен кезде, келесі қате туралы хабар пайда болады: "Нысан сілтемесі нысанның данасына орнатылмаған."                                                                           |
| Сапар және шығыс                  | [548659](https://fix.lcs.dynamics.com/Issue/Details/?bugId=548659) | Шығындар туралы есеп жарияланғаннан кейін банктің қосалқы кітабында дұрыс емес валюта және сома көрсетілген.                                                                                                                                                                |
| Сапар және шығыс                  | [555462](https://fix.lcs.dynamics.com/Issue/Details/?bugId=5355462) | Жобаның белгіленген құны сапар өтінімін белгіленген құнмен жапқаннан кейін босатылмайды.                                                                                                                                              |
| Сапар және шығыс                  | [558336](https://fix.lcs.dynamics.com/Issue/Details/?bugId=558336) | Несиелік карта бойынша транзакцияларды жою функциясы жақсартылды.                                                                                                                                                                                           |
| Сапар және шығыс                  | [525070](https://fix.lcs.dynamics.com/Issue/Details/?bugId=525070) | Шығындар туралы есептегі сату салығы заңды нысанда басқа есеп беру валютасы көрсетілген кезде дәйекті түрде есептелмейді.                                                                                                         |
| Сапар және шығыс                  | [527779](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527779) | Жаңа қолма‑қол сапар шығынын қосқан кезде өнімділікке әсер етеді.                                                                                                                                                                                         |
| Сапар және шығыс                  | [537841](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537841) | Шығындар саясаты ережесі шығындар туралы есепте іске қосылмайды.                                                                                                                                                                                            |
| Сапар және шығыс                  | [566386](https://fix.lcs.dynamics.com/Issue/Details/?bugId=566386) | Деректерді басқару құрылымын пайдаланып жаңа ортақ санатты жүктеп салу барлық ортақ санаттар үшін барлық ішкі санаттарды жояды.                                                                                                                         |
| Сапар және шығыс                  | [574131](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574131) | Шығындар жолын жасап және санатты таңдаған кезде келесі қате пайда болады: "Сатылым салығының DOM тобы мен сатылым салығының STD тобының тіркесімі жарамсыз."                                                                  |
| Сапар және шығыс                  | [574900](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574900) | Шығын мобильді бағдарламасында синхрондау мәселелері бар. 

### <a name="regulatory-updates"></a>Нормативтік жаңартулар
Қаржы және операциялық қолданбаларға арналған нормативтік жаңартулар туралы ақпаратты қараңыз [Нормативтік жаңартулар](/dynamics365/finance/localizations/regulatory-updates). Сондай‑ақ Lifecycle Services (LCS) қызметіне кіріп, мәселе іздеу құралының көмегімен жоспарланған нормативтік жаңартуларды көруге болады. Мәселені іздеу сізге ел, мүмкіндік түрі және шығарылым бойынша іздеуге мүмкіндік береді.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]