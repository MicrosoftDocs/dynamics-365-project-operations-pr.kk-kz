---
title: Жоспарлау нысандарымен операцияларды орындау үшін жоба кестесінің API интерфейстерін пайдалану
description: Бұл тақырып жоба кестесінің API интерфейсін пайдалану үшін ақпарат пен үлгілерді ұсынады.
author: sigitac
ms.date: 09/09/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6be35b1c52996f4f94dc429974ef47343a027c8c
ms.sourcegitcommit: bbe484e58a77efe77d28b34709fb6661d5da00f9
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/10/2021
ms.locfileid: "7487692"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Жоспарлау нысандарымен операцияларды орындау үшін жоба кестесінің API интерфейстерін пайдалану

_**Келесіге қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_



## <a name="scheduling-entities"></a>Жоспарлау нысандары

Жоба кестесінің API интерфейстері **Жоспарлау нысандары** арқылы операцияларды жасау, жаңарту және жою мүмкіндіктерін ұсынады. Бұл нысандар веб-нұсқаға арналған жобада жоспарлау механизмі арқылы басқарылады. **Жоспарлау нысандары** көмегімен операцияларды жасау, жаңарту және жою алдыңғы Dynamics 365 Project Operations шығарылымдарында шектеулі болды.

Келесі кестеде жоба кестесі нысандарының толық тізімі келтірілген.

| Нысан атауы  | Нысанның логикалық атауы |
| --- | --- |
| Project | msdyn_project |
| Жоба тапсырмасы  | msdyn_projecttask  |
| Жоба тапсырмасы тәуелділігі  | msdyn_projecttaskdependency  |
| Ресурс тағайындауы | msdyn_resourceassignment |
| Жоба контейнері  | msdyn_projectbucket |
| Жоба тобы мүшесі | msdyn_projectteam |

## <a name="operationset"></a>OperationSet

OperationSet — транзакция шеңберінде бірнеше кестеге әсер ететін сұраныстарды өңдеу қажет болған кезде қолдануға болатын жұмыс бірлігінің үлгісі.

## <a name="project-schedule-apis"></a>Жоба кестесінің API интерфейстері

Төменде ағымдағы жоба кестесінің API интерфейстерінің тізімі келтірілген.

- **msdyn_CreateProjectV1**: бұл API интерфейсін жобаны құру үшін қолдануға болады. Жоба және әдепкі жоба контейнері дереу жасалады.
- **msdyn_CreateTeamMemberV1**: бұл API интерфейсін жоба тобының мүшесін құру үшін қолдануға болады. Топ мүшелерінің жазбасы дереу жасалады.
- **msdyn_CreateOperationSetV1**: бұл API интерфейсін транзакция кезінде орындалуы керек бірнеше сұраныстарды жоспарлау үшін қолдануға болады.
- **msdyn_PSSCreateV1**: бұл API интерфейсін нысанды құру үшін пайдалануға болады. Нысан жасау операциясына қолдау көрсететін кез келген жобаны жоспарлау нысандары болуы мүмкін.
- **msdyn_PSSUpdateV1**: бұл API интерфейсін нысанды жаңарту үшін пайдалануға болады. Нысан жаңарту операциясына қолдау көрсететін кез келген жобаны жоспарлау нысандары болуы мүмкін.
- **msdyn_PSSDeleteV1**: бұл API интерфейсін нысанды жою үшін пайдалануға болады. Нысан жою операциясына қолдау көрсететін кез келген жобаны жоспарлау нысандары болуы мүмкін.
- **msdyn_ExecuteOperationSetV1**: бұл API берілген операциялар жиынтығындағы барлық әрекеттерді орындау үшін қолданылады.

## <a name="using-project-schedule-apis-with-operationset"></a>Жоба кестесінің API интерфейстерін OperationSet көмегімен пайдалану

**CreateProjectV1** және **CreateTeamMemberV1** дереу жасалатындықтан, бұл API интерфейстерін тікелей **OperationSet** жинағында пайдалануға болмайды. Алайда API интерфейсін қажетті жазбаларды, **OperationSet** жасау үшін, содан кейін осы алдын ала жасалған жазбаларды **OperationSet** ішінде пайдалана аласыз.

## <a name="supported-operations"></a>Қолдау көрсетілетін операциялар

| Жоспарлау нысаны | Жасау | Жаңарту | Delete | Маңызды жайттар |
| --- | --- | --- | --- | --- |
Жоба тапсырмасы | Иә | Иә | Иә | Ешқайсысы |
| Жоба тапсырмасы тәуелділігі | Иә | Иә | | Жоба тапсырмасына тәуелділік туралы жазбалар жаңартылмайды. Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады. |
| Ресурс тағайындауы | Иә | Иә | | Келесі өрістермен операцияларға қолдау көрсетілмейді: **BookableResourceID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining** және **PlannedWork**. Ресурстарды тағайындау туралы жазбалар жаңартылмайды. Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады. |
| Жоба контейнері | Қолданылмайды | Қолданылмайды | Қолданылмайды | Әдепкі контейнер **CreateProjectV1** API интерфейсі арқылы жасалады. |
| Жоба тобының мүшесі | Иә | Иә | Иә | Жасау операциясы үшін **CreateTeamMemberV1** API интерфейсін пайдаланыңыз. |
| Project | Иә | Иә | Қолданылмайды | Келесі өрістермен операцияларға қолдау көрсетілмейді: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining**, **Орындалу барысы**, **Аяқтау**, **TaskEarliestStart** және **Ұзақтығы**. |

Бұл API интерфейсін реттелетін өрістерді қамтитын нысан объектілерімен шақыруға болады.

ID сипаты міндетті емес. Егер ол қарастырылған болса, жүйе оны қолдануға әрекет жасайды және оны пайдалану мүмкін болмаса, ерекше жағдай жасайды. Егер ол қарастырылмаған болса, жүйе оны жасайды.

## <a name="restricted-fields"></a>Шектеулі өрістер

Келесі кестелер **Жасау** және **Өңдеу** параметрлерінен шектелген өрістерді анықтайды.

### <a name="project-task"></a>Жоба тапсырмасы

| **Логикалық атау**                       | **Жасалады** | **Өңделеді**     |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | жоқ             | жоқ               |
| msdyn_actualcost_base                  | жоқ             | жоқ               |
| msdyn_actualend                        | жоқ             | жоқ               |
| msdyn_actualsales                      | жоқ             | жоқ               |
| msdyn_actualsales_base                 | жоқ             | жоқ               |
| msdyn_actualstart                      | жоқ             | жоқ               |
| msdyn_costatcompleteestimate           | жоқ             | жоқ               |
| msdyn_costatcompleteestimate_base      | жоқ             | жоқ               |
| msdyn_costconsumptionpercentage        | жоқ             | жоқ               |
| msdyn_effortcompleted                  | жоқ             | жоқ               |
| msdyn_effortestimateatcomplete         | жоқ             | жоқ               |
| msdyn_iscritical                       | жоқ             | жоқ               |
| msdyn_iscriticalname                   | жоқ             | жоқ               |
| msdyn_ismanual                         | жоқ             | жоқ               |
| msdyn_ismanualname                     | жоқ             | жоқ               |
| msdyn_ismilestone                      | жоқ             | жоқ               |
| msdyn_ismilestonename                  | жоқ             | жоқ               |
| msdyn_LinkStatus                       | жоқ             | жоқ               |
| msdyn_linkstatusname                   | жоқ             | жоқ               |
| msdyn_msprojectclientid                | жоқ             | жоқ               |
| msdyn_plannedcost                      | жоқ             | жоқ               |
| msdyn_plannedcost_base                 | жоқ             | жоқ               |
| msdyn_plannedsales                     | жоқ             | жоқ               |
| msdyn_plannedsales_base                | жоқ             | жоқ               |
| msdyn_pluginprocessingdata             | жоқ             | жоқ               |
| msdyn_progress                         | жоқ             | жоқ (P4W үшін "иә") |
| msdyn_remainingcost                    | жоқ             | жоқ               |
| msdyn_remainingcost_base               | жоқ             | жоқ               |
| msdyn_remainingsales                   | жоқ             | жоқ               |
| msdyn_remainingsales_base              | жоқ             | жоқ               |
| msdyn_requestedhours                   | жоқ             | жоқ               |
| msdyn_resourcecategory                 | жоқ             | жоқ               |
| msdyn_resourcecategoryname             | жоқ             | жоқ               |
| msdyn_resourceorganizationalunitid     | жоқ             | жоқ               |
| msdyn_resourceorganizationalunitidname | жоқ             | жоқ               |
| msdyn_salesconsumptionpercentage       | жоқ             | жоқ               |
| msdyn_salesestimateatcomplete          | жоқ             | жоқ               |
| msdyn_salesestimateatcomplete_base     | жоқ             | жоқ               |
| msdyn_salesvariance                    | жоқ             | жоқ               |
| msdyn_salesvariance_base               | жоқ             | жоқ               |
| msdyn_scheduleddurationminutes         | жоқ             | жоқ               |
| msdyn_scheduledend                     | жоқ             | жоқ               |
| msdyn_scheduledstart                   | жоқ             | жоқ               |
| msdyn_schedulevariance                 | жоқ             | жоқ               |
| msdyn_skipupdateestimateline           | жоқ             | жоқ               |
| msdyn_skipupdateestimatelinename       | жоқ             | жоқ               |
| msdyn_summary                          | жоқ             | жоқ               |
| msdyn_varianceofcost                   | жоқ             | жоқ               |
| msdyn_varianceofcost_base              | жоқ             | жоқ               |

### <a name="project-task-dependency"></a>Жоба тапсырмасы тәуелділігі

| **Логикалық атау**              | **Жасалады** | **Өңделеді** |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | жоқ             | жоқ           |
| msdyn_linktypename            | жоқ             | жоқ           |
| msdyn_predecessortask         | иә            | жоқ           |
| msdyn_predecessortaskname     | иә            | жоқ           |
| msdyn_project                 | иә            | жоқ           |
| msdyn_projectname             | иә            | жоқ           |
| msdyn_projecttaskdependencyid | иә            | жоқ           |
| msdyn_successortask           | иә            | жоқ           |
| msdyn_successortaskname       | иә            | жоқ           |

### <a name="resource-assignment"></a>Ресурс тағайындауы

| **Логикалық атау**             | **Жасалады** | **Өңделеді** |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | иә            | жоқ           |
| msdyn_bookableresourceidname | иә            | жоқ           |
| msdyn_bookingstatusid        | жоқ             | жоқ           |
| msdyn_bookingstatusidname    | жоқ             | жоқ           |
| msdyn_committype             | жоқ             | жоқ           |
| msdyn_committypename         | жоқ             | жоқ           |
| msdyn_effort                 | жоқ             | жоқ           |
| msdyn_effortcompleted        | жоқ             | жоқ           |
| msdyn_effortremaining        | жоқ             | жоқ           |
| msdyn_finish                 | жоқ             | жоқ           |
| msdyn_plannedcost            | жоқ             | жоқ           |
| msdyn_plannedcost_base       | жоқ             | жоқ           |
| msdyn_plannedcostcontour     | жоқ             | жоқ           |
| msdyn_plannedsales           | жоқ             | жоқ           |
| msdyn_plannedsales_base      | жоқ             | жоқ           |
| msdyn_plannedsalescontour    | жоқ             | жоқ           |
| msdyn_plannedwork            | жоқ             | жоқ           |
| msdyn_projectid              | иә            | жоқ           |
| msdyn_projectidname          | жоқ             | жоқ           |
| msdyn_projectteamid          | жоқ             | жоқ           |
| msdyn_projectteamidname      | жоқ             | жоқ           |
| msdyn_start                  | жоқ             | жоқ           |
| msdyn_taskid                 | жоқ             | жоқ           |
| msdyn_taskidname             | жоқ             | жоқ           |
| msdyn_userresourceid         | жоқ             | жоқ           |

### <a name="project-team-member"></a>Жоба тобының мүшесі

| **Логикалық атау**                                 | **Жасалады** | **Өңделеді** |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | жоқ             | жоқ           |
| msdyn_creategenericteammemberwithrequirementname | жоқ             | жоқ           |
| msdyn_deletestatus                               | жоқ             | жоқ           |
| msdyn_deletestatusname                           | жоқ             | жоқ           |
| msdyn_effort                                     | жоқ             | жоқ           |
| msdyn_effortcompleted                            | жоқ             | жоқ           |
| msdyn_effortremaining                            | жоқ             | жоқ           |
| msdyn_finish                                     | жоқ             | жоқ           |
| msdyn_hardbookedhours                            | жоқ             | жоқ           |
| msdyn_hours                                      | жоқ             | жоқ           |
| msdyn_markedfordeletiontimer                     | жоқ             | жоқ           |
| msdyn_markedfordeletiontimestamp                 | жоқ             | жоқ           |
| msdyn_msprojectclientid                          | жоқ             | жоқ           |
| msdyn_percentage                                 | жоқ             | жоқ           |
| msdyn_requiredhours                              | жоқ             | жоқ           |
| msdyn_softbookedhours                            | жоқ             | жоқ           |
| msdyn_start                                      | жоқ             | жоқ           |

### <a name="project"></a>Project

| **Логикалық атау**                       | **Жасалады** | **Өңделеді** |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | жоқ             | жоқ           |
| msdyn_actualexpensecost_base           | жоқ             | жоқ           |
| msdyn_actuallaborcost                  | жоқ             | жоқ           |
| msdyn_actuallaborcost_base             | жоқ             | жоқ           |
| msdyn_actualsales                      | жоқ             | жоқ           |
| msdyn_actualsales_base                 | жоқ             | жоқ           |
| msdyn_contractlineproject              | иә            | жоқ           |
| msdyn_contractorganizationalunitid     | иә            | жоқ           |
| msdyn_contractorganizationalunitidname | иә            | жоқ           |
| msdyn_costconsumption                  | жоқ             | жоқ           |
| msdyn_costestimateatcomplete           | жоқ             | жоқ           |
| msdyn_costestimateatcomplete_base      | жоқ             | жоқ           |
| msdyn_costvariance                     | жоқ             | жоқ           |
| msdyn_costvariance_base                | жоқ             | жоқ           |
| msdyn_duration                         | жоқ             | жоқ           |
| msdyn_effort                           | жоқ             | жоқ           |
| msdyn_effortcompleted                  | жоқ             | жоқ           |
| msdyn_effortestimateatcompleteeac      | жоқ             | жоқ           |
| msdyn_effortremaining                  | жоқ             | жоқ           |
| msdyn_finish                           | иә            | иә          |
| msdyn_globalrevisiontoken              | жоқ             | жоқ           |
| msdyn_islinkedtomsprojectclient        | жоқ             | жоқ           |
| msdyn_islinkedtomsprojectclientname    | жоқ             | жоқ           |
| msdyn_linkeddocumenturl                | жоқ             | жоқ           |
| msdyn_msprojectdocument                | жоқ             | жоқ           |
| msdyn_msprojectdocumentname            | жоқ             | жоқ           |
| msdyn_plannedexpensecost               | жоқ             | жоқ           |
| msdyn_plannedexpensecost_base          | жоқ             | жоқ           |
| msdyn_plannedlaborcost                 | жоқ             | жоқ           |
| msdyn_plannedlaborcost_base            | жоқ             | жоқ           |
| msdyn_plannedsales                     | жоқ             | жоқ           |
| msdyn_plannedsales_base                | жоқ             | жоқ           |
| msdyn_progress                         | жоқ             | жоқ           |
| msdyn_remainingcost                    | жоқ             | жоқ           |
| msdyn_remainingcost_base               | жоқ             | жоқ           |
| msdyn_remainingsales                   | жоқ             | жоқ           |
| msdyn_remainingsales_base              | жоқ             | жоқ           |
| msdyn_replaylogheader                  | жоқ             | жоқ           |
| msdyn_salesconsumption                 | жоқ             | жоқ           |
| msdyn_salesestimateatcompleteeac       | жоқ             | жоқ           |
| msdyn_salesestimateatcompleteeac_base  | жоқ             | жоқ           |
| msdyn_salesvariance                    | жоқ             | жоқ           |
| msdyn_salesvariance_base               | жоқ             | жоқ           |
| msdyn_scheduleperformance              | жоқ             | жоқ           |
| msdyn_scheduleperformancename          | жоқ             | жоқ           |
| msdyn_schedulevariance                 | жоқ             | жоқ           |
| msdyn_taskearlieststart                | жоқ             | жоқ           |
| msdyn_teamsize                         | жоқ             | жоқ           |
| msdyn_teamsize_date                    | жоқ             | жоқ           |
| msdyn_teamsize_state                   | жоқ             | жоқ           |
| msdyn_totalactualcost                  | жоқ             | жоқ           |
| msdyn_totalactualcost_base             | жоқ             | жоқ           |
| msdyn_totalplannedcost                 | жоқ             | жоқ           |
| msdyn_totalplannedcost_base            | жоқ             | жоқ           |


## <a name="limitations-and-known-issues"></a>Шектеулер мен белгілі қателер
Төменде шектеулер мен белгілі мәселелер тізімі берілген:

- Жоба кестесінің API интерфейстерін тек **Microsoft Project лицензиясы бар пайдаланушылар** ғана пайдалана алады. Оларды пайдалана алмайды:
    - Бағдарлама пайдаланушылары
    - Жүйе пайдаланушылары
    - Интеграция пайдаланушылары
    - Қажетті лицензиясы жоқ басқа пайдаланушылар
- Әр **OperationSet** ең көбі 100 операция жасай алады.
- Әрбір пайдаланушыда ең көбі 10 ашық **OperationSets** бола алады.
- Қазіргі уақытта Project Operations жобадағы ең көбі 500 тапсырманы қолдайды.
- **OperationSet** ақаулық күйі және сәтсіздік журналдары қазіргі уақытта қолжетімді емес.
- [Жобалар мен тапсырмалар шектеулері мен шекаралары](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a>Қатені өңдеу

   - Операциялық жиындардан туындаған қателерді қарап шығу үшін **Параметрлер** \> **Кесте интеграциясы** \> **Операциялар жиындары** бөліміне өтіңіз.
   - Жоба кестесіндегі қызметтен туындаған қателерді қарап шығу үшін **Параметрлер** \> **Кестені біріктіру** \> **PSS қателер журналдары** тармағына өтіңіз.

## <a name="sample-scenario"></a>Үлгі сценарий

Бұл сценарийде сіз жоба, топ мүшесі, төрт тапсырма және екі ресурстық тағайындама жасайсыз. Әрі қарай бір тапсырманы жаңартасыз, жобаны жаңартасыз, бір тапсырманы жоясыз, ресурстардың бір тағайындамасын жоясыз және тапсырмаға тәуелділікті жасайсыз.

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>Қосымша үлгілер

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;

    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
