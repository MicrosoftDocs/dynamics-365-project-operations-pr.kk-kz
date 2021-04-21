---
title: Жоспарлау нысандары операцияларын орындау үшін жоспарлау API интерфейстерін пайдалану
description: Бұл тақырыпта жоспарлау API интерфейстерін қолдануға арналған ақпарат пен үлгілері берілген.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868136"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Жоспарлау нысандары операцияларын орындау үшін жоспарлау API интерфейстерін пайдалану

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

> [!IMPORTANT] 
> Осы бөлімде айтылған кейбір немесе барлық мүмкіндіктер алдын ала қарау бөлігі ретінде қолжетімді. Мазмұны мен функциялар өзгеруі мүмкін. 

## <a name="scheduling-entities"></a>Жоспарлау нысандары

Жоспарлау API интерфейстері **Жоспарлау нысандары** арқылы операцияларды жасау, жаңарту және жою мүмкіндіктерін ұсынады. Бұл нысандар веб-нұсқаға арналған жобада жоспарлау механизмі арқылы басқарылады. **Жоспарлау нысандары** көмегімен операцияларды жасау, жаңарту және жою алдыңғы Dynamics 365 Project Operations шығарылымдарында шектеулі болды.

Келесі кестеде **Жоспарлау нысандарының** толық тізімі берілген.

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

## <a name="schedule-apis"></a>Жоспарлау API интерфейстері

Төменде қазіргі жоспарлау API интерфейстерінің тізімі берілген.

- **msdyn_CreateProjectV1**: бұл API интерфейсін жобаны құру үшін қолдануға болады. Жоба және әдепкі жоба контейнері дереу жасалады.
- **msdyn_CreateTeamMemberV1**: бұл API интерфейсін жоба тобының мүшесін құру үшін қолдануға болады. Топ мүшелерінің жазбасы дереу жасалады.
- **msdyn_CreateOperationSetV1**: бұл API интерфейсін транзакция кезінде орындалуы керек бірнеше сұраныстарды жоспарлау үшін қолдануға болады.
- **msdyn_PSSCreateV1**: бұл API интерфейсін нысанды құру үшін пайдалануға болады. Нысан құру операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.
- **msdyn_PSSUpdateV1**: бұл API интерфейсін нысанды жаңарту үшін пайдалануға болады. Нысанды жаңарту операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.
- **msdyn_PSSDeleteV1**: бұл API интерфейсін нысанды жою үшін пайдалануға болады. Нысанды жою операциясын қолдайтын кез келген жоспарлау нысаны болуы мүмкін.
- **msdyn_ExecuteOperationSetV1**: бұл API берілген операциялар жиынтығындағы барлық әрекеттерді орындау үшін қолданылады.

## <a name="using-schedule-apis-with-operationset"></a>OperationSet көмегімен жоспарлау API интерфейстерін пайдалану

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

## <a name="limitations-and-known-issues"></a>Шектеулер мен белгілі қателер
Төменде шектеулер мен белгілі мәселелер тізімі берілген:

- Жоспарлау API интерфейстерін тек **Microsoft жоба лицензиясы бар пайдаланушылар** пайдалана алады. Оларды пайдалана алмайды:
    - Бағдарлама пайдаланушылары
    - Жүйе пайдаланушылары
    - Интеграция пайдаланушылары
    - Қажетті лицензиясы жоқ басқа пайдаланушылар
- Әр **OperationSet** ең көбі 100 операция жасай алады.
- Әрбір пайдаланушыда ең көбі 10 ашық **OperationSets** бола алады.
- Қазіргі уақытта Project Operations жобадағы ең көбі 500 тапсырманы қолдайды.
- **OperationSet** ақаулық күйі және сәтсіздік журналдары қазіргі уақытта қолжетімді емес.
- Жоспарлау API интерфейстері жалпыға қолжетімді алдын ала қарау нұсқасында орналасқан. Бұл API интерфейстерін жұмыс ортасында пайдалануға Microsoft қолдау көрсетпейді.

## <a name="sample-scenario"></a>Үлгі сценарий

Бұл сценарийде сіз жоба, топ мүшесі, төрт тапсырма және екі ресурстық тағайындама жасайсыз. Әрі қарай бір тапсырманы жаңартасыз, жобаны жаңартасыз, бір тапсырманы жоясыз, ресурстардың бір тағайындамасын жоясыз және тапсырмаға тәуелділікті жасайсыз.

```C#
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
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>Қосымша үлгілер

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
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
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
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
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
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
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
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
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
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
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
