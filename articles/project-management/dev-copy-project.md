---
title: Copy Project көмегімен жоба үлгілерін жасау
description: Бұл мақалада Жобаны көшіру теңшелетін әрекетін пайдаланып жоба үлгілерін жасау жолы туралы ақпарат берілген.
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

msdyn\_ CopyProjectV3

### <a name="input-parameters"></a>Кіріс параметрлер

Үш кіріс параметрі берілген:

- **ReplaceNamedResources** немесе **Топтарды және тапсырмаларды тазалау** – Опциялардың біреуін ғана орнатыңыз. Екеуін де орнатпаңыз.

    - **\{"ReplaceNamedResources":шын\}** – Жоба операцияларының әдепкі әрекеті. Кез келген атаулы ресурстар жалпы ресурстармен ауыстырылады.
    - **\{«Таза командалар мен тапсырмалар»:шын\}** – Web for Project үшін әдепкі әрекет. Барлық тапсырмалар мен топ мүшелері жойылады.

- **SourceProject** – Көшірілетін бастапқы жобаның нысан сілтемесі. Бұл параметр нөл болуы мүмкін емес.
- **Мақсат** – Көшірілетін мақсатты жобаның нысан сілтемесі. Бұл параметр нөл болуы мүмкін емес.

Келесі кестеде үш параметрдің қысқаша мазмұны берілген.

| Параметр                | Түр             | Value                 |
|--------------------------|------------------|-----------------------|
| ReplaceNamedResources    | Boolean          | **Рас** немесе **Жалған** |
| Топтарды және тапсырмаларды тазалау | Boolean          | **Рас** немесе **Жалған** |
| SourceProject            | Нысан анықтамасы | Бастапқы жоба    |
| Межелі орын                   | Нысан анықтамасы | Мақсатты жоба    |

Әрекеттердің қосымша әдепкі параметрлерін қараңыз [Web API әрекеттерін пайдаланыңыз](/powerapps/developer/common-data-service/webapi/use-web-api-actions).

### <a name="validations"></a>Тексерулер

Келесі тексерулер орындалады.

1. Нөл ұйымдағы екі жобаның да бар екенін растау үшін бастапқы және мақсатты жобаларды тексереді және шығарып алады.
2. Жүйе келесі шарттарды тексеру арқылы мақсатты жобаның көшіру үшін жарамды екенін растайды:

    - Жобада бұрынғы әрекет жоқ (соның ішінде **Тапсырмалар** қойындысы) және жоба жаңадан жасалған.
    - Бұл жобада алдыңғы көшірме жоқ, импорттау сұралмаған және жобада жоқ **Сәтсіз** күй.

3. Операция HTTP арқылы шақырылмайды.

## <a name="specify-fields-to-copy"></a>Көшіру үшін өрістерді көрсетіңіз

Әрекет шақырылған кезде, **Copy Project** жоба көшірілгенде қандай өрістер көшірілетінін анықтау үшін **Жоба бағандарын көшіру** жоба көрінісін қарастырады.

### <a name="example"></a>Мысал

Келесі мысалда қоңырау шалу жолы көрсетілген **CopyProjectV3** көмегімен реттелетін әрекет **RemoveNamedResources** параметр жинағы.

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
