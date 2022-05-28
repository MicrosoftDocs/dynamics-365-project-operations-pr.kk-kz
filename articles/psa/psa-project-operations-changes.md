---
title: Жоба қызметін автоматтандырудан жобалық операцияларға мүмкіндік өзгертулері
description: Бұл тақырып Project Service Automation параметрінен параметрге өзгертулер шолуын береді Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 7e41b381d6da267f58174305f33fc229c66cd7b7
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/14/2022
ms.locfileid: "8595413"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Жоба қызметін автоматтандырудан жобалық операцияларға мүмкіндік өзгертулері

Жаңарту Dynamics 365 Project Service Automation дейін Dynamics 365 Project Operations Lite үш кезеңде жеткізіледі. Бұл тақырып жаңарту аяқталған кезде көруге болатын негізгі өзгерістер туралы ақпаратты береді.

| Жеткізуді жаңарту | 1-кезең <br>(2022 ж. қаңтар) | 2-кезең <br>(Сәуір толқыны 2022) | 3-кезең  |
|------------------|------------------------|---------------------------|---------------------------|
| Жобалар үшін жұмысты бөлу құрылымына (WBS) тәуелділік жоқ. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBS жоба операцияларының қазіргі уақытта қолдау көрсетілетін шектеулеріне кіреді. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| WBS Жобаның жұмыс үстелі клиентіне қолдауды қоса алғанда, Жоба операцияларының қазіргі уақытта қолдау көрсетілетін шектеулерінен тыс. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Жобаны басқару

Пайдаланушы тәжірибесіндегі ең маңызды өзгерістер жобаны жоспарлау саласында болады. Project Operations бағдарламасы ұсынған жоспарлау мүмкіндіктерін пайдалана отырып, жұмысты бөлу құрылымын (WBS) басқарудың жаңа заманауи тәжірибесін қабылдайды.[Интернетке арналған жоба](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>Жоспарлау тәжірибесіндегі айырмашылықтар

Келесі кестеде Project Service Automation және Project Operations арасындағы жоспарлау айырмашылықтары жинақталған.

|  Жоспарлау     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| Жоба үлгілері - жоба жасалған кезде жоба үлгілерін анықтау және қолдану мүмкіндігі  |  &nbsp;    | :heavy_check_mark: |
| Жұмыс үстелі клиентімен жоба жұмысын бөлу құрылымы (WBS) интеграциясы   |    &nbsp;  | :heavy_check_mark: |
| Шектеулер - ерте емес бастаңыз, кешіктірмей аяқтаңыз  | :heavy_check_mark: |   &nbsp;  |
| Маңызды кезең - ұзақтығы нөлдік тапсырмалар   | :heavy_check_mark:  |  &nbsp;  |
| Ресурсқа негізделген тапсырмалар тағайындалған ресурстардың қолжетімділігін құрметтейді   | :heavy_check_mark: |  &nbsp;    |
| Уақыт кезеңді өңдеу - жоспарларды өңдеңіз және күн сайын жұмыс жасаңыз   |   &nbsp;  | :heavy_check_mark: |
| Автоматты/қолмен жоспарлау - тапсырмаларды автоматты түрде немесе қолмен жоспарлау үшін жобаны жоспарлау механизмін пайдаланыңыз |  &nbsp; | :heavy_check_mark:  |
| Үлкен жобаларды тікелей пайдаланушы интерфейсінде өңдеңіз: Өңдеуге болатын жоспарлардың өлшемдерінде шектеу жоқ  | 500 тапсырма шегі  | :heavy_check_mark:       |
| Орындалу пайызы - тапсырманың орындалу барысын белгілеңіз   | :heavy_check_mark:  |  &nbsp;  |
| [Жоба кестесі режимдері](../project-management/scheduling-modes.md) - Жобаны тұрақты бірлік, белгіленген күш немесе белгіленген ұзақтық ретінде анықтаңыз | :heavy_check_mark: | &nbsp; |
| Уақыт кестесі - кесте мәліметтерін визуализациялау және мүдделі тараптармен байланысу үшін уақыт шкаласы көрінісін жасаңыз және теңшеңіз. | :heavy_check_mark:  | &nbsp; |
| Күшке негізделген тапсырмалар - Тапсырманы күш ретінде жоспарлауға арналған қозғалтқышты қолдауды жоспарлау  | :heavy_check_mark:  | &nbsp; |
| **Тапсырма туралы ақпарат** диалогтық терезе - диалогтық терезені пайдаланып тапсырма мәліметтерін сақтаңыз | :heavy_check_mark:  |  &nbsp;  |
| Сүйреп апарып тастаңыз - Тапсырмаларды бірнеше рет таңдаңыз және олардың WBS жүйесіндегі орнын өзгертіңіз | :heavy_check_mark: | &nbsp;  |
| Икемді тұрақты көріністер - тапсырма атрибуттарының түйіршікті көріністерін анықтаңыз   | :heavy_check_mark:  | &nbsp; |
| WBS сұрыптау және сүзгілеу  | :heavy_check_mark:  | &nbsp; |
| Сарқырамасыз жобаны жеткізуге арналған тақталар көрінісі  | :heavy_check_mark:   | &nbsp; |
| Уақыт шкаласы көрінісі - WBS визуализациясы және өңдеу үшін пайдаланылатын интерактивті Гант диаграммасы   | :heavy_check_mark:  | &nbsp; |
| Пернелер тіркесімдері - шегініс немесе кірістіру сияқты жалпы әрекеттер үшін пернелер тіркесімін пайдаланыңыз  | :heavy_check_mark:  |  &nbsp; |
| Көп деңгейлі кері қайтару - әрекеттердің бүкіл жинағын кері қайтару және қайта қолдану арқылы өзгерістердің әсерін толық түсіну үшін не-егер талдауды орындаңыз | :heavy_check_mark: | &nbsp; |
| Қиып алу/көшіру/қою - қолданбалар арасында кесте мәліметтерін көшіру және қою арқылы кестені әзірлеуде бірлесіп жұмыс жасаңыз  | :heavy_check_mark: | &nbsp; |
| Тапсырмаларды тексеру тізімдері - тапсырмаға 20-ға дейін бақылау тізімі элементтерін қосыңыз   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Жобаны жоспарлау

The **Жоба** Project Operations бетіндегімен салыстырғанда айтарлықтай айырмашылықтар бар **Жоба** Project Service Automation бетінде.

Келесі әрекеттер файлдан жойылды **Жобалар** 1-кезең жаңартуының бөлігі ретінде бет:

  - **MS Project ішінде ашу**
  - **Үлгі жасау**
  - **MS Project бағдарламасынан ажырату**

The **Жоба** Жоба әрекеттеріндегі бет келесі жаңа қойындыларды қамтиды.

- **Материал болжамдары**
- **Тапсырма шотын ұсынуды реттеу**

The **Күй** қойындысы жойылды және **Күй** өріс қазірде **Түйіндеме** жобаның жоспарлау режимі бар қойынды.

   ![Жоба бетіндегі жаңартулар.](media/projectform.png)

The **Кесте** қойындысының атауы өзгертілді **Тапсырма** қойындысын ашады және жобаны вебке арналған жобамен жаңа жоспарлау тәжірибесін ұсынады.

   ![Жаңа жоба тапсырмалары қойындысы.](media/tasktab.png)

## <a name="scheduling-modes"></a>Жоспарлау режимдері

Project Operations жаңа мүмкіндікті енгізді, [Жоспарлау режимдері](../project-management/scheduling-modes.md). Барлық бар Project Service Automation жобалары әдепкі бойынша болады **Бекітілген ұзақтығы** Жоба операцияларында. Дегенмен, жаңа жобалар үшін әдепкі параметрді келесіге өту арқылы басқаруға болады **Параметрлер** > **Параметрлер** > **Параметр** > **Кесте режимі**.

   ![Жоспар режиміне арналған жоба параметрінің параметрлері.](media/projectparameter.png)

## <a name="project-planning-limits"></a>Жобаны жоспарлау шектеулері

Жоба операциялары жобаны жоспарлаудың барлық операциялары үшін Project for the Web қызметіне сүйенеді. Вебке арналған жоба келесі кестедегі шектеулерді пайдаланып жұмыстың бөліну құрылымын басқарады.

| **Өріс**                                          | **Шек**             |
|----------------------------------------------------|-----------------------|
| Жобаға арналған максималды жалпы тапсырмалар                  | 500                   |
| Жобаға арналған максималды жалпы ұзақтығы               | 3650 күн (10 жыл)  |
| Жобаға арналған максималды жалпы ресурстар              | 300                   |
| Жобаға арналған максималды жалпы сілтемелер (тек кейінгі элемент) | 600                   |
| Жобаға арналған максималды жалпы реттелетін өрістер          | 10                    |
| Максималды иерархиялық деңгей                            | 10 деңгей             |
| Максималды сілтемелер (кейінгі элемент + алдыңғы элемент)            | 20                    |
| Парақшалы тапсырманың максималды ұзақтығы                      | 1250 күн             |
| Жиынтық тапсырманың максималды ұзақтығы                 | 3650 күн (10 жыл)  |
| Тапсырмаға тағайындалған ең көп ресурстар               | 20 ресурс          |
| Тапсырма үшін қолдау көрсетілетін күн ауқымы                    | 1/1/2000 - 12/31/2149 |
| Бақылау тізімінің элементтері                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>Жобаны жоспарлаудың кеңеюі және дамуы

Project Operations нұсқасына жаңартқаннан кейін, келесі нысандарда жасау, жаңарту және жою әрекеттерін орындау үшін Project Scheduling API интерфейстерін пайдалануыңыз керек:

|   Нысан атауы           |   Нысанның логикалық атауы       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Жоба тапсырмасы            | msdyn_projecttask           |
| Жоба тапсырмасы тәуелділігі | msdyn_projecttaskdependency |
| Ресурс тағайындауы     | msdyn_resourceassignment    |
| Жоба контейнері          | msdyn_projectbucket         |
| Жоба тобы мүшесі     | msdyn_projectteam           |

Қазіргі уақытта осы нысандарды қамтитын теңшеулеріңіз болса, қараңыз [Жоспарлау нысандарымен әрекеттерді орындау үшін Жоба кестесі API интерфейстерін пайдаланыңыз](../project-management/schedule-api-preview.md) іске асыру бойынша нұсқаулық үшін.

## <a name="data-model-changes"></a>Деректер үлгісінің өзгеруі

Жаңарту кезеңінің 1 бөлігі ретінде деректер үлгісіне өзгерістер енгізілді. Бұл өзгертулер, ең алдымен, бар нысандардағы өріс өзгерістері болып табылады. 1-кезеңде субъектілер, **msydn_project** және **msdyn_projectteam** теңшеулердің рефакторингі болып табылады. 

> [!IMPORTANT]
> Бұл бөлім болашақ жаңарту кезеңдері аяқталған сайын қосымша нысандармен жаңартылады.

Келесі өрістер жаңа өрістермен ауыстырылды.

|   Entity          |   Ескі логикалық атау   |   Жаңа логикалық атау    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

Келесі өрістер қосылды.

|   Entity          |   Логикалық атау                               |   Сипаттама |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | Жоба бойынша нақты комиссиялық сату жиынын көрсетеді. Тек Project Service Automation жүйесінде пайдалануға арналған. |
| msdyn_project     | msdyn_actualmaterialcost                     | Жоба бойынша нақты материалдық шығындардың жиынтығын көрсетеді. Тек Project Service Automation жүйесінде пайдалануға арналған. |
| msdyn_project     | msdyn_actualmaterialsales                    | Жоба бойынша нақты материалды сату жиынын көрсетеді. Тек Project Service Automation жүйесінде пайдалануға арналған. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Осы жобамен байланысты келісімшарт желісі. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Бұл ішкі жүйе өрісі үшін пайдаланылады **Жобаны көшіру** Корреляция идентификаторына қатысты. Тек Project Service Automation жүйесінде пайдалануға арналған. |
| msdyn_project     | msdyn_copyprojectsessionid                   | Бұл ішкі жүйе өрісі үшін пайдаланылады **Жобаны көшіру** сеанс идентификаторына қатысты. Тек Project Service Automation жүйесінде пайдалануға арналған. |
| msdyn_project     | msdyn_globalrevisiontoken                    | Соңғы синхрондау xRM жаһандық қайта қарау таңбалауышы Жобаны жоспарлау қызметінен. |
| msdyn_project     | msdyn_msprojectdocument                      | Жобаға жататын Microsoft Project құжаты. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Жоба бойынша жоспарланған материалдық шығындардың жиынтығы. Тек Project Service Automation жүйесінде пайдалануға арналған. |
| msdyn_project     | msdyn_plannedmaterialsales                   | Жоба бойынша жоспарланған материалды сату жиыны. Тек Project Service Automation жүйесінде пайдалануға арналған. |
| msdyn_project     | msdyn_program                                | Бұл жобамен байланысты бағдарлама. |
| msdyn_project     | msdyn_quotelineproject                       | Осы жобамен байланысты дәйексөз жолы. |
| msdyn_project     | msdyn_replaylogheader                        | Қайталау журналдарына арналған тақырып. |
| msdyn_project     | msdyn_schedulemode                           | Жобадағы барлық тапсырмалар үшін пайдаланылатын әдепкі жоспарлау режимі.  |
| msdyn_project     | msdyn_taskearlieststart                      | Жобадағы тапсырманың ең ерте басталу күні.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Осы жоба тобының мүшесі көшірілген жоба командасының мүшесі. |
| msdyn_projectteam | msdyn_creategenericteammember with талап | Жаңадан жасалған жалпы топ мүшесі үшін ресурс талабын жасау керек пе екенін көрсетеді.  |
| msdyn_projectteam | msdyn_deletestatus                           | Жобаны жоспарлау қызметіне жіберілген жою сұрауының бар-жоғын және оның күтілетін уақыт терезесінде жауапты сәтті қайтаруын бақылау үшін топ мүшесінің жою күйі. |
| msdyn_projectteam | msdyn_effortcompleted                        | Топ мүшелерінің тапсырмалары бойынша орындаған күш-жігерін қадағалайды. |
| msdyn_projectteam | msdyn_effortremaining                        | Топ мүшелерінің тапсырмалары бойынша әлі орындамаған күш-жігерін қадағалайды. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Топ мүшесі жобаны жоспарлау қызметіне жою сұрауын жібергеннен бастап топ мүшесі нақты жойылғанға дейінгі күту кезеңі Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Топ мүшесі жою сұрауы Жобаны жоспарлау қызметіне жіберілген кезде жазылатын уақыт белгісі. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Осы жоба тобының мүшесі көшірілген жоба тобының мүшесін көрсетеді.  |

## <a name="project-templates"></a>Жоба үлгілері

Project Operations жоба үлгілеріне қолдау көрсетпейді. Дегенмен, негізгі функциялардың көпшілігін пайдалану арқылы қайталауға болады [Project Copy API](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>Жұмыс үстелі қондырмасын қолдау

Microsoft Project Desktop қондырмасына қолдау жаңартудың алғашқы 2 кезеңінде қол жетімді болмайды. 3-кезеңде жобаны вебке арналған жобаның қазіргі уақытта қолдау көрсетілетін шектеулерінен үлкенірек тұтынушылар жұмыс үстелі қондырмасын пайдалана алады.

## <a name="editing-resource-assignment-contours"></a>Ресурс тағайындау контурларын өңдеу

Ресурс тағайындау контурларын өңдеу мүмкіндігі жаңартудың 2-кезеңі қолжетімді болғанда қолжетімді болады.

## <a name="billing-and-pricing"></a>Есеп-шот ұсыну және баға белгілеу

Жоба операцияларында келесі жаңа мүмкіндіктер қосылды. Бұл мүмкіндіктер қосымша сипатта болады және Project Service Automation деректер үлгісіне әсер етпейді.

- [Жобалар мен жоба тапсырмалары бойынша материалды пайдалануды тіркеу](../material/material-usage-log.md)
- [Қосалқы мердігерлік басқару](../pro/subcontracting/managing-subcontracts-overview.md)
- [Аванстар және қаламақыға негізделген келісім-шарттар](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Келісімшарттың орындалмаған күйі және тексерулері](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Тапсырмаға негізделген есепшот](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Ескірген құрамдас бөліктер

Келесі кестелер жаңартудан кейін ескірген құрамдастардың шешіміне жылжытылған барлық ескірген өрістерді құжаттайды. Қосымша ақпаратты және шешімге сілтемені қараңыз [Dynamics 365 Project Service Automation Project Operations 4x ескірген құрамдастарға 3x](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>шот-фактураның детальдары

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinescheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunityline транзакциясы

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transaction классификациясы                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransaction санаты

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassicatio

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransaction классификациясы

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_istemplate                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduleddurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatuser

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocomplete                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatuserid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicants қолжетімді                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hoursrequested                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammemberтіркелу

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransaction санаты

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinescheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransactioncategory.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_name                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>сату тапсырысының егжей-тегжейі

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

