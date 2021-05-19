---
title: Project Service Automation біріктіру параметрлері
description: Бұл тақырыпта Microsoft Dynamics 365 for Project Service Automation бағдарламасын Microsoft Dynamics 365 Finance бағдарламасы арқылы біріктіру кезінде әдепкі деректердің енгізілетін жолын конфигурациялау әдісі түсіндіріледі.
author: ruhercul
manager: AnnBe
ms.date: 03/03/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: b8faba1d799e360e58d47a02dc8b46e09fa0d393
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270910"
---
# <a name="project-service-automation-integration-parameters"></a>Project Service Automation біріктіру параметрлері

[!include[banner](../includes/banner.md)]

**Project Service Automation біріктіру параметрлері** бетінде, Dynamics 365 Project Service Automation бағдарламасын Dynamics 365 Finance бағдарламасы арқылы біріктіру кезінде әдепкі деректердің енгізілетін жолын конфигурациялауға болады. Жобаларды Project Service Automation бағдарламасынан Finance бағдарламасына сәтті синхрондау үшін, келесі өрістерді орнату қажет.

**Project Service Automation біріктіру параметрлері** бетін ашу үшін, **Жобаны басқару және есеп** \> **Орнату** \> **Dynamics 365 for Project Service Automation біріктіру параметрлері** тармағына өтіңіз. 

> [!NOTE]
> - Жоба тапсырмаларын біріктіру, шығындар транзакциясының санаттары, сағаттық болжамдар, шығын болжамдары және функционалды құлыптау 8.0 нұсқасында қолжетімді.
> - Нақты көрсеткіштерді біріктіру 8.0.1 немесе одан кейінгі нұсқада қолжетімді.


| Tab пернесі                    | Өріс                | Сипаттама |
|------------------------|----------------------|-------------|
| Жалпы                 | Әдепкі жоба түрі | Әдепкі жоба түрін орнатыңыз. Жобалар Project Service Automation бағдарламасынан синхрондалған кезде, бұл мән біріктіру үлгісінде әдепкі мәнді ұсынбаған жағдайда пайдаланылады. Синхрондау кезінде, жаңа жобалардың **Жоба түрі** өрісі осы мәнге орнатылады. Дегенмен, мән жобалық келісім-шарт жолдары Project Service Automation бағдарламасынан синхрондалған кезде жаңартылуы мүмкін. |
|                        | Уақыт санаты        | Әдепкі уақыт санатын орнатыңыз. Бұл мән сағаттық болжамдар Project Service Automation бағдарламасынан синхрондалған кезде пайдаланылады. Сағаттық болжамдар мен сағаттық нақты мәндер Project Service Automation бағдарламасынан синхрондалған кезде, Finance бағдарламасындағы жаңа жоба сағаттық болжамдарының **Санат** өрісі осы мәнге орнатылады. |
|                        | Құн санаты         | Әдепкі құн санатын орнатыңыз. Бұл мән құнның нақты мәндері Project Service Automation бағдарламасынан синхрондалған кезде пайдаланылады. Құнның нақты мәндері Project Service Automation бағдарламасынан синхрондалған кезде, Finance бағдарламасындағы жаңа құн транзакцияларының **Санат** өрісі осы мәнге орнатылады. |
| Жоба тобының әдепкі мәндері | Жоба түрі         | Әдепкі жоба тобын орнатуға қажетті жоба түрін таңдайтын жолды қосу үшін **Жаңа** түймешігін басыңыз. Арнайы жоба түрін конфигурацияда тек бір рет таңдауға болады. |
|                        | Жоба тобы        | Таңдалған жоба түріне арналған әдепкі жоба тобын таңдаңыз. Жаңа жобалар Project Service Automation бағдарламасынан синхрондалған кезде, **Жоба тобы** өрісі біріктіру үлгісінде әдепкі мәнді ұсынбаған жағдайда жоба түріне арналған әдепкі мәнге орнатылады. |
| Шот ұсыну түрінің әдепкі мәндері  | Есеп-шот ұсыну түрі         | Әдепкі жол сипатын орнатуға қажетті шот ұсыну түрін таңдайтын жолды қосу үшін **Жаңа** түймешігін басыңыз. Арнайы шот ұсыну түрін конфигурацияда тек бір рет таңдауға болады. |
|                        | Жол сипаты        | Таңдалған шот ұсыну түріне арналған әдепкі жол сипатын таңдаңыз. Жаңа сағаттық болжамдар, жаңа шығыс болжамдар немесе жаңа нақты мәндер Project Service Automation бағдарламасынан синхрондалған кезде, **Жол сипаты** өрісі шот ұсыну түріне арналған әдепкі мәнге орнатылады. |
| Функционалдықты құлыптау  | Қолданылмайды       | Project Service Automation бағдарламасынан алынған жобалар мен келісім-шарттарға арналған Finance бағдарламасын өшіру үшін функционалдықты таңдаңыз. Мысалы, келісім-шарттар мен жобаларды өңдеу, жұмыс декомпозициясының құрылымдарын жасау және уақыт кестелерін Finance бағдарламасына енгізу мүмкіндігін өшіруге болады. Есепке қатысты өрістер параметр орнатуы арқылы қолжетімді болмаған жағдайда да қосулы болады. Әдепкі бойынша, барлық функционалдық қосылады. |


[!INCLUDE[footer-include](../includes/footer-banner.md)]