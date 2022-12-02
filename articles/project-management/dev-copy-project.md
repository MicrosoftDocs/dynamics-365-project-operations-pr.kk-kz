---
title: Copy Project көмегімен жоба үлгілерін жасау
description: Бұл мақалада Copy Project реттелетін әрекеті көмегімен жоба үлгілерін жасау жолы туралы ақпарат берілген.
author: stsporen
ms.date: 03/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 47c1023bbc4c21e3571bffbf3670bf0f7854f81d
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923839"
---
# <a name="develop-project-templates-with-copy-project"></a>Copy Project көмегімен жоба үлгілерін жасау

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Dynamics 365 Project Operations бағдарламасы жобаны көшіру және кез келген тапсырманы рөлді көрсететін жалпы ресурстарға қайтару мүмкіндігін қолдайды. Тұтынушылар бұл функцияны жобаның негізгі үлгілерін құру үшін пайдалана алады.

**Copy Project** таңдалған кезде, мақсатты жобаның күйі жаңартылады. Көшіру әрекеті қашан аяқталғанын анықтау **Күй себебі** пәрменін пайдаланыңыз. **Copy Project** таңдау мақсатты жоба нысанында ешқандай мақсатты күн анықталмаса, жобаның басталу күнін ағымдағы басталу күніне дейін жаңартады.

## <a name="copy-project-custom-action"></a>Copy Project реттелетін әрекеті

### <a name="name"></a>Аты 

msdyn\_CopyProjectV3

### <a name="input-parameters"></a>Кіріс параметрлер

Үш кіріс параметрі берілген:

- **ReplaceNamedResources** немесе **ClearTeamsAndAssignments** – опциялардың тек біреуін орнатыңыз. Екеуін де орнатуға болмайды.

    - **\{"ReplaceNamedResources":true\}** – Project Operations бағдарламасының әдепкі әрекеті. Барлық аталған ресурстар жалпы ресурстармен алмастырылады.
    - **\{"ClearTeamsAndAssignments":true\}** – Project for the Web бағдарламасы үшін әдепкі әрекет. Барлық тағайындаулар мен топ мүшелері жойылады.

- **SourceProject** – көшірілетін бастапқы жобаның нысан сілтемесі. Бұл параметр бос мәнді болмауы керек.
- **Target** – көшірілетін мақсатты жобаның нысан сілтемесі. Бұл параметр бос мәнді болмауы керек.

Келесі кестеде үш параметр бойынша жиынтық мәлімет берілген.

| Параметр                | Түр             | Value                 |
|--------------------------|------------------|-----------------------|
| ReplaceNamedResources    | Boolean          | **True** немесе **False** |
| ClearTeamsAndAssignments | Boolean          | **True** немесе **False** |
| SourceProject            | Нысан анықтамасы | Бастапқы жоба    |
| Межелі орын                   | Нысан анықтамасы | Мақсатты жоба    |

Әрекеттердегі әдепкі параметрлер туралы ақпарат алу үшін [Веб API әрекеттерін пайдалану](/powerapps/developer/common-data-service/webapi/use-web-api-actions) бөлімін қараңыз.

### <a name="validations"></a>Тексерімдер

Келесі тексерімдер жасалады.

1. Ұйымдағы екі жобаның да бар екенін растау үшін нөлдік мәндер тексеріледі және бастапқы және мақсатты жобалар шығарып алынады.
2. Жүйе келесі шарттарды тексеру арқылы мақсатты жобаның көшіру үшін жарамды екенін тексереді:

    - Жобада бұрынғы әрекеттер (соның ішінде **Тапсырмалар** қойыншасын таңдау) жоқ және жоба жаңадан жасалған.
    - Бұл жобада алдыңғы көшірме жоқ, импорттау сұралмаған және **Сәтсіз** күйі болмаған.

3. Операция HTTP арқылы шақырылмайды.

## <a name="specify-fields-to-copy"></a>Көшіру үшін өрістерді көрсетіңіз

Әрекет шақырылған кезде, **Copy Project** жоба көшірілгенде қандай өрістер көшірілетінін анықтау үшін **Жоба бағандарын көшіру** жоба көрінісін қарастырады.

### <a name="example"></a>Мысал

Келеcі мысалда **removeNamedResources** параметрлер жинағы көмегімен **CopyProjectV3** реттелетін әрекетін шақыру әдісі көрсетілген.

```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

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
            targetProject["msdyn_subject"] = "Example Project - Copy";
            targetProject.Id = organizationService.Create(targetProject);

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption, true, false);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, bool replaceNamedResources = true, bool clearTeamsAndAssignments = false)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;

            if (replaceNamedResources)
            {
                req["ReplaceNamedResources"] = true;
            }
            else
            {
                req["ClearTeamsAndAssignments"] = true;
            }

            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```

[!INCLUDE[footer-include](../includes/footer-banner.md)]
