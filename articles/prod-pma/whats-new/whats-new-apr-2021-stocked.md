---
title: Қосалқы/өндіріске негізделген сценарийлерге арналған 2021 жылдың сәуір айындағы Project Operations бағдарламасындағы жаңалықтар немесе өзгерістер
description: Бұл мақалада жинақталған/өндіріске негізделген сценарийлер үшін Жоба операцияларының 2021 жылдың сәуір айындағы шығарылымында қолжетімді сапа жаңартулары туралы ақпарат берілген.
author: andchoi
ms.date: 04/22/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: andchoi
ms.openlocfilehash: 74cace069e0b5a982e6ea1df0607ff72f1911a0f
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028201"
---
# <a name="whats-new-or-changed-in-project-operations-april-2021-for-stockedproduction-based-scenarios"></a>Қосалқы/өндіріске негізделген сценарийлерге арналған 2021 жылдың сәуір айындағы Project Operations бағдарламасындағы жаңалықтар немесе өзгерістер

_**Келесіге қолданылады:** қосалқы/өндіріске негізделген сценарийлеріне арналған Project Operations жүйесі_

Бұл мақала келесіге қатысты Dynamics 365 Project Operations құрамдас бөліктер мен нұсқалар:

- Dynamics 365 Finance ортасында жобаны басқару және есепке алу 10.0.18 нұсқасында
 
### <a name="quality-updates"></a>Сапа жаңартулары
                                                                                                                                                                                  
| Мүмкіндік аумағы                      | Сілтемелік нөмір| Сапа жаңартуы                                                                                                                                                                          |
|-----------------------------------|--------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Жобаларды басқару және есеп | [534393](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534393) | **Жобаны сұрыптау** торында қате пайда болады.                                                                                                                                                      |
| Жобаларды басқару және есеп | [542850](https://fix.lcs.dynamics.com/Issue/Details/?bugId=542850) | Жобаны сатып алу тапсырысында бірлік бағасы мен саны түзетілгеннен кейін жасалған сома артық болады.                                                                                    |
| Жобаларды басқару және есеп | [543645](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543645) | **ProjParameters** айнымалысы жарияланады, бірақ оны пайдаланар алдында ешқашан жазба буферін тағайындамайды.                                                                                     |
| Жобаларды басқару және есеп | [543674](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543674) | **Барлық компанияларда жоба ресурстарын толтыру** топтық тапсырмасы шығарылған кезде **ResRollup** кестелері жойылады.                                                                          |
| Жобаларды басқару және есеп | [544417](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544417) | **V2 тапсырыс жолдарын сатып алу** нысаны арқылы сатып алу тапсырысында **Жобаның сатылым бағасы** өрісін жаңарту кезінде мәселе туындайды.                                                                           |
| Жобаларды басқару және есеп | [547652](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547652) | Идентификатор нөмірлеріне байланысты қосалқы жобалар жасалмайды.   Келесі қате пайда болады: “Function Global::int642int пәрмені дұрыс емес шақырылды."                                         |
| Жобаларды басқару және есеп | [484274](https://fix.lcs.dynamics.com/Issue/Details/?bugId=484274) | Тұтынушы бір шот-фактурада сатып алу санаты мен элементімен сатып алу тапсырысына шот ұсыну кезінде қате шоттарды алады.                                                                      |
| Жобаларды басқару және есеп | [509920](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509920) | Жобаның транзакциясын жанама шығындармен шот ұсынылатын түрінен ұсынылмайтын түріне және қайтадан ұсынылатынына дейін түзету WIP тіркелгісін дұрыс тазартпайды.                                       |
| Жобаларды басқару және есеп | [511274](https://fix.lcs.dynamics.com/Issue/Details/?bugId=511274) | Сатылым тапсырысында сақтау және жалпы жеңілдік пайдаланылған кезде шот-фактура сомалары дұрыс емес.                                                                                          |
| Жобаларды басқару және есеп | [511315](https://fix.lcs.dynamics.com/Issue/Details/?bugId=511315) | Жол туралы мәліметтердегі мекенжай атауы басқа транзакция түрі таңдалған кезде өзгермейді.                                                                           |
| Жобаларды басқару және есеп | [522983](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522983) | Өнімнің ішінара түбіртегі мен ішінара шот-фактураны сатып алу тапсырысы бойынша есеп айырысу процесінде элемент талаптары мен сатып алу тапсырысы бар расталған шығындар дұрыс емес.                       |
| Жобаларды басқару және есеп | [524226](https://fix.lcs.dynamics.com/Issue/Details/?bugId=524226) | Жобаның қаржылық өлшемдері өзгерген кезде, сатып алу тапсырысының тақырыбы өзгерістерді көрсетпейді.                                                                                                  |
| Жобаларды басқару және есеп | [524979](https://fix.lcs.dynamics.com/Issue/Details/?bugId=524979) | Жасалған **Белгіленген баға жобасы** есебі бос.                                                                                                         |
| Жобаларды басқару және есеп | [529445](https://fix.lcs.dynamics.com/Issue/Details/?bugId=529445) | Шот-фактура жеткізушінің шот-фактураларын қарау кезінде жоба идентификаторы **Төлем қабылданғаннан кейінгі төлем** бетінде таңдамайды.                                                                          |
| Жобаларды басқару және есеп | [529982](https://fix.lcs.dynamics.com/Issue/Details/?bugId=529982) | Кіру **HR менеджері** рөліндегі бір заңды нысан үшін шектеулі болатын пайдаланушы үшін уақыт кестесінің жазбасы дұрыс емес, өйткені әдепкі санат дұрыс көрсетілмеген.                                         |
| Жобаларды басқару және есеп | [530008](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530008) | **Реттеу күнін жобаның жаңа күні ретінде пайдалану** өрісі **Жоқ** мәніне орнатылғанда жобаның бастапқы күні түзетуге қосылмайды және бұл қате тудырады.                                             |
| Жобаларды басқару және есеп | [530788](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530788) | Жобалық бағалаулар топтаманы пайдаланып есептелген кезде нәтижелер қате болады.                                                                                                         |
| Жобаларды басқару және есеп | [530834](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530834) | Жоба келісімшартына жұмсалған сома жобадағы шоттағы сомаға сәйкес келмейді.                                                                             |
| Жобаларды басқару және есеп | [530883](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530883) | Жоба бойынша есепші мен жоба менеджерінің рөлі мақұлдау тобының орнатылымы бар сағаттық журнал жасай алмайды.                                                                                 |
| Жобаларды басқару және есеп | [531974](https://fix.lcs.dynamics.com/Issue/Details/?bugId=531974) | Microsoft Excel импортталған шығын журналын орналастыру мүмкін емес.                                                                                                                                       |
| Жобаларды басқару және есеп | [532548](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532548) | Жеткізушілердің шот-фактуралары мен шығындар туралы есептерді қоса алғанда, жеткізушілер транзакциясын компанияаралық сценарийлерден өзгертуге рұқсат етіледі.                                                                     |
| Жобаларды басқару және есеп | [533426](https://fix.lcs.dynamics.com/Issue/Details/?bugId=533426) | Жобаны түзету жанама шығындармен сату көлемін дұрыс жаңартпайды.                                                                                                    |
| Жобаларды басқару және есеп | [534869](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534869) | Белгіленген жобалық шот-фактура үшін несиелік жазба жасалған кезде және жеткізілім шоттары ережесінің бірлігін пайдаланған кезде, шығарылған бірліктер қайта шот ұсыну бойынша қолжетімді емес. |
| Жобаларды басқару және есеп | [535428](https://fix.lcs.dynamics.com/Issue/Details/?bugId=535428) | Басқа валютамен жасалған жоба келісімшартында элемент журналындағы немесе шот-фактура ұсынысындағы есеп валютасы дұрыс есептелмейді.                                                   |
| Жобаларды басқару және есеп | [537158](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537158) | Элементке қойылатын талапты ауыстыру үшін сатып алуға тапсырыс жолағындағы жобаны өзгертіңіз.                                                                                                                          |
| Жобаларды басқару және есеп | [540603](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540603) | Болжамнан жобаның бюджетіне импорттау дұрыс емес мөлшерге әкеледі.                                                                                                                    |
| Жобаларды басқару және есеп | [540622](https://fix.lcs.dynamics.com/Issue/Details/?bugId=5406222) | Транзакцияны шот ұсынылатын түрінен шот ұсынылмайтынға дейін түзету кезінде бас кітап жазбалары жасалмайды.                                                                                            |
| Жобаларды басқару және есеп | [540633](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540633) | **Жобаның жеткізуші шот-фактурасын сақтау шарты үшін шығын сомасын есептеуді іске қосу мүмкіндігін қосу** параметрі қосылған кезде жоба транзакциялары төлем қабылданғаннан кейінгі төлеммен жасалмайды.                  |
| Жобаларды басқару және есеп | [541421](https://fix.lcs.dynamics.com/Issue/Details/?bugId=541421) | **Шот-фактура ұсынысын жасау** бетіндегі көптеген мәселелер.                                                                                                                             |
| Жобаларды басқару және есеп | [543390](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543390) | **Барлық жобалар** беті жаңа тіл коды бар тізімді көрсетпейді.                                                                                                            |
| Жобаларды басқару және есеп | [543803](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543803) | Жоба бюджетінің қалдығында бекітілмеген бюджет сомасы бюджетті екі реттен артық қайта қарау кезінде дұрыс емес.                                                                |
| Жобаларды басқару және есеп | [543968](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543968) | **Сатып алу туралы келісім** беті Project Operations арқылы біріктірілген Finance заңды нысандарда көрінбейді.                                                                               |
| Жобаларды басқару және есеп | [545456](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545456) | Тиісті ваучер күні жоба сағаттарының журнал жолдарына жүктелмеген.                                                                                                            |
| Жобаларды басқару және есеп | [545878](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545878) | Ресурсқа негізделген сценарийлерге арналған Project Operations бағдарламасында біріктіру қатесіне байланысты баға ұсыныстарын Project Operations ішіндегі жеңіске ауыстыра алмайсыз.                                                                      |
| Жобаларды басқару және есеп | [546604](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546604) | Project Operations бағдарламасында қате туралы хабар қабаттасқан келісімшарт жолдары мен транзакция түрлерін тексеруге байланысты келісім-шарт жолы мен жоба идентификаторы арасында байланыс жасауға әрекеттенгенде жіберіледі.                        |
| Жобаларды басқару және есеп | [546949](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546949) | **ProjValEmplProjSetup** кестесінде 14000-нан астам жазба болғанда **Ресурс-жобалық тексеру топтары** бетінде өнімділік мәселелері болады.                                                                     |
| Жобаларды басқару және есеп | [547440](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547440) | **ProjCDSProjectContractEntity** басқа тұтынушыдан қаржыландыру көзі шот-фактурасының мекенжайын орната алады.                                                                                   |
| Жобаларды басқару және есеп | [547606](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547606) | 10.0.15 шығарылымынан кейін ресурстарды стандартты іздеу қолжетімді емес.                                                                                          |
| Жобаларды басқару және есеп | [547831](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547831) | Сатып алу тапсырысы бойынша шот-фактура ваучеріндегі бас кітап шоты мен орналастыру түрі қызметтік элементке сәйкес келмейді. Жоба тобы **Қалдық** күйіне орнатылады, ал бас кітап шоты дұрыс емес.                   |
| Жобаларды басқару және есеп | [550030](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550030) | **Негізгі әрекетін таңдауды бұғаттау** параметрі **Жоқ** мәніне орнатылса да, әрекет нөмірі күтудегі сатушы шот-фактурасында көрсетілмеген.                                            |
| Жобаларды басқару және есеп | [550379](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550379) | **Жоба** > **Бюджет** > **Түзетулер** > **Жаңа** > **Импорттау** навигация жолын пайдалану кезінде жүйе барлық жобалар үшін жобалық бюджетті қайта қарау әрекетін жасайды.                                                            |
| Жобаларды басқару және есеп | [550577](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550577) | Транзакцияны басқа транзакция және есеп валюталарымен реттеу кезінде қате орналастыру және жалпы бас кітап жазбалары туындайды.                                                                        |
| Жобаларды басқару және есеп | [557376](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557376) | Транзакция үшін орналастыру шот-фактурасын жасау кезінде өлшемдер қосылмайды.                                                                                                   |
| Жобаларды басқару және есеп | [559416](https://fix.lcs.dynamics.com/Issue/Details/?bugId=559416) | **PurchTotals.purchNewTotalAmount()** әдісі өнімділікке байланысты кез келген сатып алу тапсырысымен байланысты емес күтудегі жеткізуші шот-фактурасын жасау кезінде шақырылады.                    |
| Сапар және шығыс                | [480451](https://fix.lcs.dynamics.com/Issue/Details/?bugId=480451) | Жүріс параметріне қатысты орналастыру қатесі бар.                                                                                                                                          |
| Сапар және шығыс                | [522084](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522084) | Бөгде валюта шығысының транзакцияларына арналған **Жекеге бөлу** мүмкіндігі жұмыс істемейді.                                                                                                         |
| Сапар және шығыс                | [523938](https://fix.lcs.dynamics.com/Issue/Details/?bugId=523938) | Шығындар санатының ашылмалы мәзірі **Өкілдер** параметрі ресурс ретінде орнатылғанына қарамастан дұрыс емес санаттарды көрсетеді.                                         |
| Сапар және шығыс                | [539266](https://fix.lcs.dynamics.com/Issue/Details/?bugId=539266) | Ресурс/санатты растау қателігіне байланысты компанияаралық шығындар туралы есепті сақтау мүмкін емес.                                                                                             |
| Сапар және шығыс                | [532610](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532610) | Шығындар туралы есепті есепке алудағы жүріс мөлшерлемесінің қате есептелуі бөлінген жолдарға ие болады.                                                                                                        |
| Сапар және шығыс                | [537404](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537404) | Сатылым салығы енгізілгенде және төлем әдісіндегі өзара есеп айырысу шотының түрі **Қызметкер** болса, компанияаралық шығындар туралы есепті орналастыру мүмкін емес.                                                   |
| Сапар және шығыс                | [542927](https://fix.lcs.dynamics.com/Issue/Details/?bugId=542927) | Өзгерістер **TrvRequisitionLine** деректер нысанына және нысанмен байланысты бірегей индекске қайтарылды.                                                                                            |
| Сапар және шығыс                | [543239](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543239) | Бастапқы құжат жолдарын құруды және жаңартуды қолдау үшін шығындар туралы есепте нақты нүктелерде журналға тіркеу.                                                                                           |
| Сапар және шығыс                | [544323](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544323) | Сату салығы мақсатты заңды нысанға орналастырылса, компанияаралық сценарийлерде қате қосалқы журнал ұсынылады.                                              |
| Сапар және шығыс                | [546877](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546877) | Project Operations жүйесінде шығын болжамы Dataverse ішінен жойылған кезде Finance бағдарламасында жойылмайды.                                                                                         |
| Сапар және шығыс                | [550575](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550575) | Шығындар санаты жобалық емес санатта болса, **Шығындар** бетінде таңдалған қаржылық өлшемдер шығындар есебіне көшірілмейді.                                          |

### <a name="regulatory-updates"></a>Нормативтік жаңартулар
Қаржы және операциялық қолданбаларға арналған нормативтік жаңартулар туралы ақпаратты қараңыз [Нормативтік жаңартулар](/dynamics365/finance/localizations/regulatory-updates). Сондай-ақ LCS жүйесіне кіріп, мәселені іздеу құралы арқылы жоспарланған нормативтік жаңартуларды көруге болады. Мәселені іздеу сізге ел, мүмкіндік түрі және шығарылым бойынша іздеуге мүмкіндік береді.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]