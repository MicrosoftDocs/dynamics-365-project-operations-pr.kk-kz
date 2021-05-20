---
title: Copy Project көмегімен жоба үлгілерін жасау
description: Бұл тақырыпта Copy Project реттелетін әрекеті көмегімен жоба үлгілерін жасау жолы туралы ақпарат берілген.
author: stsporen
manager: Annbe
ms.date: 01/21/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cc17df0c73b276048f7c4b04bd9dc6644e828dc0
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949821"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="a7ed5-103">Copy Project көмегімен жоба үлгілерін жасау</span><span class="sxs-lookup"><span data-stu-id="a7ed5-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="a7ed5-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="a7ed5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="a7ed5-105">Dynamics 365 Project Operations бағдарламасы жобаны көшіру және кез келген тапсырманы рөлді көрсететін жалпы ресурстарға қайтару мүмкіндігін қолдайды.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="a7ed5-106">Тұтынушылар бұл функцияны жобаның негізгі үлгілерін құру үшін пайдалана алады.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="a7ed5-107">**Copy Project** таңдалған кезде, мақсатты жобаның күйі жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="a7ed5-108">Көшіру әрекеті қашан аяқталғанын анықтау **Күй себебі** пәрменін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="a7ed5-109">**Copy Project** таңдау мақсатты жоба нысанында ешқандай мақсатты күн анықталмаса, жобаның басталу күнін ағымдағы басталу күніне дейін жаңартады.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="a7ed5-110">Copy Project реттелетін әрекеті</span><span class="sxs-lookup"><span data-stu-id="a7ed5-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="a7ed5-111">Атауы</span><span class="sxs-lookup"><span data-stu-id="a7ed5-111">Name</span></span> 

<span data-ttu-id="a7ed5-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="a7ed5-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="a7ed5-113">Кіріс параметрлер</span><span class="sxs-lookup"><span data-stu-id="a7ed5-113">Input parameters</span></span>
<span data-ttu-id="a7ed5-114">Үш кіріс параметрі берілген:</span><span class="sxs-lookup"><span data-stu-id="a7ed5-114">There are three input parameters:</span></span>

| <span data-ttu-id="a7ed5-115">Параметр</span><span class="sxs-lookup"><span data-stu-id="a7ed5-115">Parameter</span></span>          | <span data-ttu-id="a7ed5-116">Түр</span><span class="sxs-lookup"><span data-stu-id="a7ed5-116">Type</span></span>   | <span data-ttu-id="a7ed5-117">Мәндер</span><span class="sxs-lookup"><span data-stu-id="a7ed5-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="a7ed5-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="a7ed5-118">ProjectCopyOption</span></span>  | <span data-ttu-id="a7ed5-119">String</span><span class="sxs-lookup"><span data-stu-id="a7ed5-119">String</span></span> | <span data-ttu-id="a7ed5-120">**{"removeNamedResources":true}** немесе **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="a7ed5-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="a7ed5-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="a7ed5-121">SourceProject</span></span>      | <span data-ttu-id="a7ed5-122">Нысан анықтамасы</span><span class="sxs-lookup"><span data-stu-id="a7ed5-122">Entity Reference</span></span> | <span data-ttu-id="a7ed5-123">Бастапқы жоба</span><span class="sxs-lookup"><span data-stu-id="a7ed5-123">Source Project</span></span> |
| <span data-ttu-id="a7ed5-124">Мақсатты мән</span><span class="sxs-lookup"><span data-stu-id="a7ed5-124">Target</span></span>             | <span data-ttu-id="a7ed5-125">Нысан анықтамасы</span><span class="sxs-lookup"><span data-stu-id="a7ed5-125">Entity Reference</span></span> | <span data-ttu-id="a7ed5-126">Мақсатты жоба</span><span class="sxs-lookup"><span data-stu-id="a7ed5-126">Target Project</span></span> |


- <span data-ttu-id="a7ed5-127">**{"clearTeamsAndAssignments":true}**: интернетке арналған жобаның әдепкі әрекеті және барлық тапсырмалар мен топ мүшелерін жояды.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="a7ed5-128">**{"removeNamedResources":true}** Project Operation бағдарламасына арналған әдепкі әрекет және тағайындауларды жалпы ресурстарға қайтарады.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="a7ed5-129">Әрекеттердегі әдепкі параметрлер туралы ақпарат алу үшін [Веб API әрекеттерін пайдалану](/powerapps/developer/common-data-service/webapi/use-web-api-actions) бөлімін қараңыз</span><span class="sxs-lookup"><span data-stu-id="a7ed5-129">For more defaults on actions, see [Use Web API actions](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="a7ed5-130">Көшіру үшін өрістерді көрсетіңіз</span><span class="sxs-lookup"><span data-stu-id="a7ed5-130">Specify fields to copy</span></span> 
<span data-ttu-id="a7ed5-131">Әрекет шақырылған кезде, **Copy Project** жоба көшірілгенде қандай өрістер көшірілетінін анықтау үшін **Жоба бағандарын көшіру** жоба көрінісін қарастырады.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>


### <a name="example"></a><span data-ttu-id="a7ed5-132">Мысал</span><span class="sxs-lookup"><span data-stu-id="a7ed5-132">Example</span></span>
<span data-ttu-id="a7ed5-133">Келеcі мысалда **removeNamedResources** параметрлер жинағы көмегімен **CopyProject** пайдаланушы әрекетін шақыру әдісі көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="a7ed5-133">The following example shows how to call the **CopyProject** custom action with the **removeNamedResources** parameter set.</span></span>
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]