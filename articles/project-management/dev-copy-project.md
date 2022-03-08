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
# <a name="develop-project-templates-with-copy-project"></a>Copy Project көмегімен жоба үлгілерін жасау

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations бағдарламасы жобаны көшіру және кез келген тапсырманы рөлді көрсететін жалпы ресурстарға қайтару мүмкіндігін қолдайды. Тұтынушылар бұл функцияны жобаның негізгі үлгілерін құру үшін пайдалана алады.

**Copy Project** таңдалған кезде, мақсатты жобаның күйі жаңартылады. Көшіру әрекеті қашан аяқталғанын анықтау **Күй себебі** пәрменін пайдаланыңыз. **Copy Project** таңдау мақсатты жоба нысанында ешқандай мақсатты күн анықталмаса, жобаның басталу күнін ағымдағы басталу күніне дейін жаңартады.

## <a name="copy-project-custom-action"></a>Copy Project реттелетін әрекеті 

### <a name="name"></a>Атауы 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>Кіріс параметрлер
Үш кіріс параметрі берілген:

| Параметр          | Түр   | Мәндер                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** немесе **{"clearTeamsAndAssignments":true}** |
| SourceProject      | Нысан анықтамасы | Бастапқы жоба |
| Мақсатты мән             | Нысан анықтамасы | Мақсатты жоба |


- **{"clearTeamsAndAssignments":true}**: интернетке арналған жобаның әдепкі әрекеті және барлық тапсырмалар мен топ мүшелерін жояды.
- **{"removeNamedResources":true}** Project Operation бағдарламасына арналған әдепкі әрекет және тағайындауларды жалпы ресурстарға қайтарады.

Әрекеттердегі әдепкі параметрлер туралы ақпарат алу үшін [Веб API әрекеттерін пайдалану](/powerapps/developer/common-data-service/webapi/use-web-api-actions) бөлімін қараңыз

## <a name="specify-fields-to-copy"></a>Көшіру үшін өрістерді көрсетіңіз 
Әрекет шақырылған кезде, **Copy Project** жоба көшірілгенде қандай өрістер көшірілетінін анықтау үшін **Жоба бағандарын көшіру** жоба көрінісін қарастырады.


### <a name="example"></a>Мысал
Келеcі мысалда **removeNamedResources** параметрлер жинағы көмегімен **CopyProject** пайдаланушы әрекетін шақыру әдісі көрсетілген.
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