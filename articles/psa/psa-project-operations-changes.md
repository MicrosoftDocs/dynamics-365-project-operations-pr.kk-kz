---
title: Project Service Automation - Project Operations функция өзгерістері
description: Бұл мақалада Project Service Automation бағдарламасынан Dynamics 365 Project Operations бағдарламасына жаңарту кезіндегі функциялардың өзгерістері туралы жалпы ақпарат берілген.
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
ms.openlocfilehash: a9c69fc4296d30763f3994a4955e64ab258ceb4f
ms.sourcegitcommit: 675e9f3615e701c5f998de3a5ea3e25df11ae107
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/09/2022
ms.locfileid: "9459933"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Project Service Automation - Project Operations функция өзгерістері

Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Project Operations Lite бағдарламасына жаңарту үш кезең арқылы жеткізіледі. Бұл мақалада жаңарту аяқталған кезде көруге болатын негізгі өзгерістер туралы ақпарат берілген.

| Жаңартуды жеткізу | 1-кезең <br>(Қаңтар, 2022) | 2-кезең <br>(Қараша, 2022) | 3-кезең  |
|------------------|------------------------|---------------------------|---------------------------|
| Жобалар үшін жұмыс декомпозициясының құрылымына (WBS) тәуелділік жоқ. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBS Project Operations бағдарламасының ағымдағы қолдау көрсетілетін шектеулеріне кіреді. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| WBS Project Desktop Client бағдарламасына қолдаумен қоса Project Operations бағдарламасының ағымдағы қолдау көрсетілетін шектеулерінен тыс. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Жобаны басқару

Пайдаланушы тәжірибесіндегі ең маңызды өзгерістер жобаны жоспарлау саласында болады. Project Operations бағдарламасы [Project for the Web](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) ұсынған жоспарлау мүмкіндіктерін пайдалану арқылы жұмыс декомпозициясының құрылымын (WBS) басқарудың жаңа заманауи тәжірибесін қолданады.

## <a name="differences-in-the-scheduling-experience"></a>Жоспарлау тәжірибесіндегі айырмашылықтар

Келесі кестеде Project Service Automation және Project Operations арасындағы жоспарлау айырмашылықтары көрсетілген.

|  Жоспарлау     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| Жоба үлгілері - жоба жасалғанда жоба үлгілерін анықтау және қолдану мүмкіндігі  |  &nbsp;    | :heavy_check_mark: |
| Жұмыс үстелі клиенті мен жоба бойынша жұмыс декомпозициясының құрылымын (WBS) біріктіру   |    &nbsp;  | :heavy_check_mark: |
| Шектеулер - ерте бастамау, кешіктірмей аяқтау  | :heavy_check_mark: |   &nbsp;  |
| Кезеңдер - нөлдік ұзақтыққа ие тапсырмалар   | :heavy_check_mark:  |  &nbsp;  |
| Ресурсқа негізделген тапсырмалар тағайындалған ресурстардың қолжетімділігіне сәйкес келеді   | :heavy_check_mark: |  &nbsp;    |
| Кезеңді өңдеу - жоспарларды өңдеу және күнделікті жұмыс істеу   |   &nbsp;  | :heavy_check_mark: |
| Автоматты/қолмен жоспарлау - тапсырмаларды автоматты түрде немесе қолмен жоспарлау үшін жобаны жоспарлау механизмін пайдалану |  &nbsp; | :heavy_check_mark:  |
| Үлкен жобаларды тікелей пайдаланушы интерфейсінде өңдеу: өңдеуге болатын жоспарлардың өлшеміне шектеу жоқ  | Шектеу: 500 тапсырма  | :heavy_check_mark:       |
| Орындалу пайызы - тапсырманың орындалу барысын белгілеу   | :heavy_check_mark:  |  &nbsp;  |
| [Жобаны жоспарлау режимдері](../project-management/scheduling-modes.md) - жобаны тұрақты бірліктер, бекітілген еңбек шығыны немесе белгіленген ұзақтық ретінде анықтау | :heavy_check_mark: | &nbsp; |
| Уақыт шкаласы - кесте мәліметтерін визуализациялау және мүдделі тараптармен байланысу үшін уақыт шкаласы көрінісін жасау және реттеу. | :heavy_check_mark:  | &nbsp; |
| Еңбек шығынына негізделген тапсырмалар - тапсырманы еңбек шығыны ретінде жоспарлауға арналған механизмге қолдау көрсету  | :heavy_check_mark:  | &nbsp; |
| **Тапсырма туралы ақпарат** диалогтік терезесі - диалогтік терезені пайдаланып тапсырма мәліметтерін сақтау | :heavy_check_mark:  |  &nbsp;  |
| Сүйреп апару - бірнеше тапсырманы таңдау және олардың WBS жүйесіндегі орнын өзгерту | :heavy_check_mark: | &nbsp;  |
| Икемді тұрақты көріністер - тапсырма атрибуттарының түйіршікті көріністерін анықтау   | :heavy_check_mark:  | &nbsp; |
| WBS сұрыптау және сүзгілеу  | :heavy_check_mark:  | &nbsp; |
| "Сарқырама" үлгісінлегі емес жобаны жеткізуге арналған тақталар көрінісі  | :heavy_check_mark:   | &nbsp; |
| Уақыт шкаласы көрінісі - WBS құрылымын визуализациялау және өңдеу үшін пайдаланылатын интерактивті Гант диаграммасы   | :heavy_check_mark:  | &nbsp; |
| Пернелер тіркесімдері - шегініс немесе кірістіру сияқты жалпы әрекеттер үшін пернелер тіркесімін пайдалану  | :heavy_check_mark:  |  &nbsp; |
| Көп деңгейлі бас тарту - әрекеттердің бүкіл жинағын кері қайтару және қайта қолдану арқылы өзгерістердің әсерін толық түсіну үшін түрлі сценарийлер талдауын орындау | :heavy_check_mark: | &nbsp; |
| Қиып алу/көшіру/қою - қолданбалар арасында кесте мәліметтерін көшіру және қою арқылы кестені әзірлеу бойынша бірлесіп жұмыс жасау  | :heavy_check_mark: | &nbsp; |
| Тапсырмаларды тексеру тізімдері - тапсырмаға 20-ға дейін тексеру тізімі элементін қосу   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Жобаны жоспарлау

Project Operations бағдарламасындағы **Жоба** бетінің Project Service Automation бағдарламасындағы **Жоба** бетімен салыстырғанда айтарлықтай айырмашылықтары бар.

Келесі әрекеттер 1-кезең жаңартуының бөлігі ретінде **Жобалар** бетінен жойылды:

  - **MS Project ішінде ашу**
  - **Үлгі жасау**
  - **MS Project бағдарламасынан ажырату**

Project Operations бағдарламасындағы **Жоба** беті келесі жаңа қойыншаларды қамтиды.

- **Материал болжамдары**
- **Тапсырма шотын ұсынуды реттеу**

**Күй** қойыншасы жойылды және **Күй** өрісі енді **Қорытынды** қойыншасында орналасқан және ол жобаның жоспарлау режимінде жұмыс істейді.

   ![Жоба бетіндегі жаңартулар.](media/projectform.png)

**Кесте** қойыншасының атауы **Тапсырма** деп өзгертілді және жобаны Project for the Web бағдарламасыны жаңа жоспарлау тәжірибесін ұсынады.

   ![Жаңа жоба тапсырмалары қойыншасы.](media/tasktab.png)

## <a name="scheduling-modes"></a>Жоспарлау режимдері

Project Operations бағдарламасына жаңа функция қосылды: [жоспарлау режимдері](../project-management/scheduling-modes.md). Барлық бұрыннан бар Project Service Automation жобалары Project Operations бағдарламасында әдепкі бойынша **Бекітілген ұзақтық** режимінде болады. Алайда жаңа жобаларға арналған әдепкі режимді **Параметрлер** > **Параметрлер** > **Параметр** > **Жоспарлау режимі** тармағына өту арқылы басқаруға болады.

   ![Жоспарлау режиміне арналған жоба параметрлері.](media/projectparameter.png)

## <a name="project-planning-limits"></a>Жобаны жоспарлау бойынша шектеулер

Project Operations жобаны жоспарлау бойынша барлық операциялар үшін Project for the Web бағдарламасын пайдаланады. Project for the Web келесі кестедегі шектеулерді пайдалана отырып жұмыс декомпозициясының құрылымын басқарады.

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

## <a name="project-planning-extensibility-and-development"></a>Жобаны жоспарлауды әзірлеу және оның кеңейтімділігі

Project Operations нұсқасына жаңартқаннан кейін, келесі нысандарда жасау, жаңарту және жою әрекеттерін орындау үшін Project Scheduling API интерфейстерін пайдалануыңыз керек:

|   Нысан атауы           |   Нысанның логикалық атауы       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Жоба тапсырмасы            | msdyn_projecttask           |
| Жоба тапсырмасы тәуелділігі | msdyn_projecttaskdependency |
| Ресурс тағайындауы     | msdyn_resourceassignment    |
| Жоба контейнері          | msdyn_projectbucket         |
| Жоба тобы мүшесі     | msdyn_projectteam           |

Ағымдағы уақытта осы нысандарды қамтитын реттеулер бар болса, мына бөлімнен ендіру нұсқаулығын қараңыз: [ Жоспарлау нысандарымен әрекеттерді орындау үшін жобаны жоспарлауға арналған API интерфейстерін пайдалану](../project-management/schedule-api-preview.md).

## <a name="data-model-changes"></a>Деректер үлгісінің өзгерістері

Жаңартудың 1-кезеңі шеңберінде деректер үлгісіне өзгерістер енгізіледі. Ең алдымен, бұрыннан бар нысандардағы өрістерге өзгерістер енгізіледі. 1-кезеңде **msydn_project** және **msdyn_projectteam** нысандары реттеулер рефакторингі болып табылады. 

> [!IMPORTANT]
> Бұл бөлім болашақ жаңарту кезеңдері аяқталған сайын қосымша нысандармен жаңартылады.

Келесі өрістер жаңа өрістермен ауыстырылады.

|   Entity          |   Ескі логикалық атауы   |   Жаңа логикалық атауы    |
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
| msdyn_project     | msdyn_actualfeesales                         | Жоба бойынша сатылымның нақты жиынтық алымдарын көрсетеді. Тек Project Service Automation қызметінде пайдалануға арналған. |
| msdyn_project     | msdyn_actualmaterialcost                     | Жоба бойынша материалдардың нақты жиынтық құнын көрсетеді. Тек Project Service Automation қызметінде пайдалануға арналған. |
| msdyn_project     | msdyn_actualmaterialsales                    | Жоба бойынша материалдардың нақты жиынтық сатылымын көрсетеді. Тек Project Service Automation қызметінде пайдалануға арналған. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Осы жобамен байланысты келісім-шарт жолы. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Бұл — өзара қатынас идентификаторына қатысты **Жобаны көшіру** үшін пайдаланылатын ішкі жүйелік өріс. Тек Project Service Automation қызметінде пайдалануға арналған. |
| msdyn_project     | msdyn_copyprojectsessionid                   | Бұл — өзара сеанс идентификаторына қатысты **Жобаны көшіру** үшін пайдаланылатын ішкі жүйелік өріс. Тек Project Service Automation қызметінде пайдалануға арналған. |
| msdyn_project     | msdyn_globalrevisiontoken                    | Жобаны жоспарлау қызметіндегі соңғы синхрондалған xRM нұсқасындағы глобалды токен. |
| msdyn_project     | msdyn_msprojectdocument                      | Жобаға тиесілі Microsoft Project құжаты. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Жоба бойынша материалдардың жоспарланған жиынтық құнын көрсетеді. Тек Project Service Automation қызметінде пайдалануға арналған. |
| msdyn_project     | msdyn_plannedmaterialsales                   | Жоба бойынша материалдардың жоспарланған жиынтық сатылымын көрсетеді. Тек Project Service Automation қызметінде пайдалануға арналған. |
| msdyn_project     | msdyn_program                                | Бұл жобамен байланысты бағдарлама. |
| msdyn_project     | msdyn_quotelineproject                       | Осы жобамен байланысты баға ұсыну жолы. |
| msdyn_project     | msdyn_replaylogheader                        | Ойнату журналдарының жоғарғы деректемесі. |
| msdyn_project     | msdyn_schedulemode                           | Жобада барлық тапсырмалар үшін әдепкі жоспарлау режимі пайдаланылады.  |
| msdyn_project     | msdyn_taskearlieststart                      | Жобадағы тапсырманың ең ерте басталу күні.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Осы жоба тобының мүшесі көшірілген жоба тобының мүшесі. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | Жаңадан жасалған жалпы топ мүшесі үшін ресурс талабын жасау керектігін көрсетеді.  |
| msdyn_projectteam | msdyn_deletestatus                           | Project Scheduling Service қызметіне жіберілген жою сұрауы бар-жоғын және оның күтілетін уақыт аралығында жауап қайтарған-қайтармағанын бақылауға арналған топ мүшесінің жою сұрауы. |
| msdyn_projectteam | msdyn_effortcompleted                        | Тағайындалған тапсырмаларда топ мүшесі жасаған еңбек шығындарын бақылайды. |
| msdyn_projectteam | msdyn_effortremaining                        | Тағайындалған тапсырмаларда топ мүшесі аяқтамаған еңбек шығындарын бақылайды. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Топ мүшесі Project Scheduling Service қызметіне жою сұрауын жібергеннен бастап топ мүшесі Microsoft Dataverse бағдарламасында нақты жойылғанға дейінгі күту кезеңі.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Project Scheduling Service қызметіне топ мүшесін жою сұрауының жіберілуін жазуға арналған уақыт белгісі. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Осы жоба тобының мүшесі көшірілген жоба тобының мүшесін көрсетеді.  |

## <a name="project-templates"></a>Жоба үлгілері

Project Operations жоба үлгілеріне қолдау көрсетпейді. Алайда [жобаны көшірудің API интерфейсіндегі](../project-management/dev-copy-project.md) негізгі функциялардың көбісін қайталай аласыз.

## <a name="desktop-add-in-support"></a>Жұмыс үстелі қондырмасына қолдау көрсету

Microsoft Project Desktop қондырмасына қолдау жаңартудың алғашқы 2 кезеңінде қолжетімді болмайды. 3-кезеңде Project for the Web бағдарламасының ағымдағы қолдау көрсетілетін шектеулерінен асатын жобалары бар тұтынушылар жұмыс үстелі қондырмасын пайдалана алатын болады.

## <a name="editing-resource-assignment-contours"></a>Ресурсты тағайындау контурларын өңдеу

Ресурсты тағайындау контурларын өңдеу мүмкіндігі жаңартудың 2-кезеңі қолжетімді болғанда қолжетімді болады.

## <a name="billing-and-pricing"></a>Есеп-шот ұсыну және баға белгілеу

Project Operations бағдарламасына келесі жаңа мүмкіндіктер қосылды. Бұл мүмкіндіктер аддитивті сипатқа ие және Project Service Automation деректер үлгісіне әсер етпейді.

- [Жобалар мен жоба тапсырмалары бойынша материал қолданысын жазу](../material/material-usage-log.md)
- [Қосалқы мердігерлікті басқару](../pro/subcontracting/managing-subcontracts-overview.md)
- [Аванстар және қаламақыға негізделген келісім-шарттар](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Келісім-шарттың асырмау күйі мен тексерулер](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Тапсырма негізінде шот ұсыну](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Ескірген құрамдастар

Келесі кестелерде жаңартудан кейін ескірген құрамдастар шешіміне жылжытылған барлық ескірген өрістер берілген. Қосымша ақпаратты және шешімге сілтемені алу үшін мына бөлімді қараңыз: [Dynamics 365 Project Service Automation 3x нұсқасынан Project Operations 4x нұсқасына жаңарту кезіндегі ескірген құрамдастар](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>invoicedetail

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

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

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
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

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

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

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

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

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
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicantsavailable                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hoursrequested                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

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

### <a name="salesorderdetail"></a>salesorderdetail

| Өрістер                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

