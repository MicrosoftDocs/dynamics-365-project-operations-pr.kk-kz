---
title: Жоспарлау нысандарымен операцияларды орындау үшін жоба кестесінің API интерфейстерін пайдалану
description: Бұл мақалада Жоба кестесі API интерфейстерін пайдалану үшін ақпарат пен үлгілер берілген.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 159d395efff98f2af780e5ed1e5ab3d6483cba89
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541131"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Жоспарлау нысандарымен операцияларды орындау үшін жоба кестесінің API интерфейстерін пайдалану

_**Келесіге қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_


**Жоспарлау нысандары**

Жоба кестесінің API интерфейстері **Жоспарлау нысандары** арқылы операцияларды жасау, жаңарту және жою мүмкіндіктерін ұсынады. Бұл нысандар веб-нұсқаға арналған жобада жоспарлау механизмі арқылы басқарылады. **Жоспарлау нысандары** көмегімен операцияларды жасау, жаңарту және жою алдыңғы Dynamics 365 Project Operations шығарылымдарында шектеулі болды.

Келесі кестеде жоба кестесі нысандарының толық тізімі келтірілген.

| **Нысан аты**         | **Нысанның логикалық атауы**     |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Жоба тапсырмасы            | msdyn_projecttask           |
| Жоба тапсырмасы тәуелділігі | msdyn_projecttaskdependency |
| Ресурс тағайындауы     | msdyn_resourceassignment    |
| Жоба контейнері          | msdyn_projectbucket         |
| Жоба тобы мүшесі     | msdyn_projectteam           |
| Жобаны тексеру тізімдері      | msdyn_projectchecklist      |
| Жоба белгісі           | msdyn_projectlabel          |
| Белгілеуге арналған жоба тапсырмасы   | msdyn_projecttasktolabel    |
| Жоба спринті          | msdyn_projectsprint         |

**OperationSet**

OperationSet — транзакция шеңберінде бірнеше кестеге әсер ететін сұраныстарды өңдеу қажет болған кезде қолдануға болатын жұмыс бірлігінің үлгісі.

**Жоба кестесінің API интерфейстері**

Төменде ағымдағы жоба кестесінің API интерфейстерінің тізімі келтірілген.

| **API**                                 | Сипаттама                                                                                                                       |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **msdyn_CreateProjectV1**               | Бұл API жобаны жасау үшін пайдаланылады. Жоба және әдепкі жоба шелегі бірден жасалады.                         |
| **msdyn_CreateTeamMemberV1**            | Бұл API жоба тобы мүшесін жасау үшін пайдаланылады. Топ мүшелерінің жазбасы дереу жасалады.                                  |
| **msdyn_CreateOperationSetV1**          | Бұл API транзакция ішінде орындалуы керек бірнеше сұрауларды жоспарлау үшін пайдаланылады.                                        |
| **msdyn_PssCreateV1**                   | Бұл API нысанды жасау үшін пайдаланылады. Нысан жасау операциясына қолдау көрсететін кез келген жобаны жоспарлау нысандары болуы мүмкін. |
| **msdyn_PssUpdateV1**                   | Бұл API нысанды жаңарту үшін пайдаланылады. Нысан жаңарту әрекетін қолдайтын Жобаны жоспарлау нысандарының кез келгені болуы мүмкін  |
| **msdyn_PssDeleteV1**                   | Бұл API нысанды жою үшін пайдаланылады. Нысан жою операциясына қолдау көрсететін кез келген жобаны жоспарлау нысандары болуы мүмкін. |
| **msdyn_ExecuteOperationSetV1**         | Бұл API берілген операциялар жиынындағы барлық операцияларды орындау үшін пайдаланылады.                                                 |
| **msdyn_PssUpdateResourceAssignmentV1** | Бұл API Resource Assignment жоспарланған жұмыс контурын жаңарту үшін пайдаланылады.                                                        |



**Жоба кестесінің API интерфейстерін OperationSet көмегімен пайдалану**

**CreateProjectV1** және **CreateTeamMemberV1** дереу жасалатындықтан, бұл API интерфейстерін тікелей **OperationSet** жинағында пайдалануға болмайды. Алайда API интерфейсін қажетті жазбаларды, **OperationSet** жасау үшін, содан кейін осы алдын ала жасалған жазбаларды **OperationSet** ішінде пайдалана аласыз.

**Қолдау көрсетілетін операциялар**

| **Жоспарлау нысаны**   | **Жасау** | **Жаңарту** | **Delete** | **Маңызды жайттар**                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------|------------|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Жоба тапсырмасы            | Иә        | Иә        | Иә        | The **Прогресс**, **аяқталды**, және **Қалған күш** өрістерді Project for the Web қолданбасында өңдеуге болады, бірақ оларды Project Operations ішінде өңдеу мүмкін емес.                                                                                                                                                                                             |
| Жоба тапсырмасы тәуелділігі | Иә        | No         | Иә        | Жоба тапсырмасына тәуелділік туралы жазбалар жаңартылмайды. Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады.                                                                                                                                                                                                                                 |
| Ресурс тағайындауы     | Иә        | Иә\*      | Иә        | Келесі өрістермен операцияларға қолдау көрсетілмейді: **BookableResourceID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining** және **PlannedWork**. Ресурстарды тағайындау туралы жазбалар жаңартылмайды. Оның орнына ескі жазбаны жоюға және жаңа жазба жасауға болады. Ресурстарды тағайындау контурларын жаңарту үшін бөлек API қамтамасыз етілді. |
| Жоба контейнері          | Иә        | Иә        | Иә        | Әдепкі шелек көмегімен жасалады **CreateProjectV1** API. Жоба шелектерін жасау және жою үшін қолдау 16-шығарылым жаңартуына қосылды.                                                                                                                                                                                                   |
| Жоба тобының мүшесі     | Иә        | Иә        | Иә        | Жасау операциясы үшін **CreateTeamMemberV1** API интерфейсін пайдаланыңыз.                                                                                                                                                                                                                                                                                           |
| Project                 | Иә        | Иә        |            | Келесі өрістермен операцияларға қолдау көрсетілмейді: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Талпыныс**, **EffortCompleted**, **EffortRemaining**, **Орындалу барысы**, **Аяқтау**, **TaskEarliestStart** және **Ұзақтығы**.                                                                                       |
| Жобаны тексеру тізімдері      | Иә        | Иә        | Иә        |                                                                                                                                                                                                                                                                                                                                                         |
| Жоба белгісі           | No         | Иә        | No         | Белгі атауларын өзгертуге болады. Бұл мүмкіндік тек Web for Project үшін қол жетімді                                                                                                                                                                                                                                                                      |
| Белгілеуге арналған жоба тапсырмасы   | Иә        | No         | Иә        | Бұл мүмкіндік тек Web for Project үшін қол жетімді                                                                                                                                                                                                                                                                                                  |
| Жоба спринті          | Иә        | Иә        | Иә        | The **Бастау** өрісінде күннен ертерек күн болуы керек **Аяқтау** өріс. Бір жобаға арналған спринттер бір-бірімен қабаттаса алмайды. Бұл мүмкіндік тек Web for Project үшін қол жетімді                                                                                                                                                                    |




ID сипаты міндетті емес. Егер ол қарастырылған болса, жүйе оны қолдануға әрекет жасайды және оны пайдалану мүмкін болмаса, ерекше жағдай жасайды. Егер ол қарастырылмаған болса, жүйе оны жасайды.

**Шектеулер мен белгілі қателер**

Төменде шектеулер мен белгілі мәселелер тізімі берілген:

-   Project Schedule API интерфейстерін тек пайдаланушылар пайдалана алады **Microsoft Project лицензиясы бар пайдаланушылар**. Оларды пайдалана алмайды:
    -   Бағдарлама пайдаланушылары
    -   Жүйе пайдаланушылары
    -   Интеграция пайдаланушылары
    -   Қажетті лицензиясы жоқ басқа пайдаланушылар
-   Әр **OperationSet** ең көбі 100 операция жасай алады.
-   Әрбір пайдаланушыда ең көбі 10 ашық **OperationSets** бола алады.
-   Қазіргі уақытта Project Operations жобадағы ең көбі 500 тапсырманы қолдайды.
-   Әрбір жаңарту ресурсын тағайындау контуры әрекеті бір әрекет ретінде есептеледі.
-   Жаңартылған контурлардың әрбір тізімі ең көбі 100 уақыт кесіндісін қамтуы мүмкін.
-   **OperationSet** ақаулық күйі және сәтсіздік журналдары қазіргі уақытта қолжетімді емес.
-   Бір жобада ең көбі 400 спринт бар.
-   [Жобалар мен тапсырмалардағы шектеулер мен шекаралар](/project-for-the-web/project-for-the-web-limits-and-boundaries).
-   Белгілер қазір тек Web for Project үшін қолжетімді.

**Қатені өңдеу**

-   Операциялық жиындардан туындаған қателерді қарап шығу үшін **Параметрлер** \> **Кесте интеграциясы** \> **Операциялар жиындары** бөліміне өтіңіз.
-   Жоба кестесіндегі қызметтен туындаған қателерді қарап шығу үшін **Параметрлер** \> **Кестені біріктіру** \> **PSS қателер журналдары** тармағына өтіңіз.

**Ресурстарды тағайындау контурларын өңдеу**

Нысанды жаңартатын барлық басқа жобаны жоспарлау API интерфейстерінен айырмашылығы, ресурс тағайындау контуры API бір ғана өріске, msdyn_plannedwork, бір нысандағы msydn_resourceassignment жаңартуларына жауапты.

Берілген кесте режимі:

-   **тұрақты бірліктер**
-   жоба күнтізбесі 9-5p 9-5p, дүйсенбі, сейсенбі, бейсенбі, жұма (СӘРСЕНБІ КҮНІ ЖҰМЫС ЖОҚ)
-   және ресурс күнтізбесі 9-1p PST дүйсенбіден жұмаға дейін

Бұл тапсырма бір аптаға, күніне төрт сағатқа арналған. Себебі ресурс күнтізбесі 9-1 PST немесе күніне төрт сағат.

| &nbsp;     | Тапсырма | Басталу күні | Аяқталған күні  | Шама | 13.06.2022 | 14.06.2022 | 15.06.2022 | 16.06.2022 | 17.06.2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 жұмысшы |  T1  | 13.06.2022  | 17.06.2022 | 20       | 4         | 4         | 4         | 4         | 4         |

Мысалы, жұмысшының осы аптада күніне үш сағат жұмыс істегенін және басқа тапсырмалар үшін бір сағат уақытын беруін қаласаңыз.

#### <a name="updatedcontours-sample-payload"></a>UpdatedContours үлгі пайдалы жүктемесі:

```json
[{

"minutes":900.0,

"start":"2022-06-13T00:00:00-07:00",

"end":"2022-06-18T00:00:00-07:00"

}]
```

Бұл контур кестесін жаңарту API іске қосылғаннан кейінгі тағайындау.

| &nbsp;     | Тапсырма | Басталу күні | Аяқталған күні  | Шама | 13.06.2022 | 14.06.2022 | 15.06.2022 | 16.06.2022 | 17.06.2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 жұмысшы | T1   | 13.06.2022  | 17.06.2022 | 15       | 3-көше         | 3-көше         | 3-көше         | 3-көше         | 3-көше         |


**Үлгі сценарий**

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

** Қосымша үлгілер

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
