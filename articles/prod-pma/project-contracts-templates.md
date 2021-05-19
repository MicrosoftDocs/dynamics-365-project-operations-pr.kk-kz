---
title: Жоба келісім-шарттары мен жобаларын тікелей Project Service Automation жүйесінен Finance бағдарламасына синхрондау
description: Бұл тақырыпта үлгі мен жобаның келісім-шарттары мен жобаларын Microsoft Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance жүйесіне синхрондау үшін пайдаланылатын негізгі тапсырмалар сипатталады.
author: Yowelle
manager: AnnBe
ms.date: 12/17/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 319000e6a826580049e8575def5790ab595a3165
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289601"
---
# <a name="synchronize-project-contracts-and-projects-directly-from-project-service-automation-to-finance"></a>Жоба келісім-шарттары мен жобаларын тікелей Project Service Automation жүйесінен Finance бағдарламасына синхрондау 

[!include[banner](../includes/banner.md)]

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Бұл тақырыпта үлгі мен жобаның келісім-шарттары мен жобаларын Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance жүйесіне синхрондау үшін пайдаланылатын негізгі тапсырмалар сипатталады.

> [!NOTE] 
> Enterprise Edition 7.3.0 бағдарламасын пайдаланатын болсаңыз 4074835 білім қорын орнату қажет.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Project Service Automation және Finance бағдарламасындағы деректер ағыны

> [!NOTE]
> Project Service Automation бағдарламасын Finance біріктіру шешіміне пайдаланудан бұрын, Dynamics 365 деректерді біріктіру мүмкіндігімен таныс болуыңыз қажет.

Project Service Automation және Finance бағдарламасын біріктіру шешімі деректерді біріктіру мүмкіндігін Project Service Automation және Finance мысалдары бойынша деректерді синхрондау үшін пайдаланады. Деректерді біріктіру мүмкіндігімен қолжетімді біріктіру үлгісі жобаның келісім-шарттары, жобалар, жобаның келісім-шарт жолдары және жобаның келісім-шарт жолының кезеңдері туралы деректер ағынын Project Service Automation бағдарламасынан Finance бағдарламасына қосады.

Келесі суретте деректердің Project Service Automation және Finance арасында синхрондалу жолы көрсетілген.

[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіруге арналған деректер ағыны](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)

## <a name="templates-and-tasks"></a>Үлгілер және тапсырмалар

Қолжетімді үлгілерге қатынасу үшін Microsoft Power Apps басқару орталығында **Жобалар** опциясын таңдап, содан соң жоғарғы оң жақтағы бұрышта жалпы үлгілерді таңдау үшін **Жаңа жоба** опциясын таңдаңыз.

Келесі үлгілер және негізгі тапсырмалар жобаның келісім-шарттарын және жобаларын Project Service Automation бағдарламасынан Finance бағдарламасына синхрондау үшін пайдаланылады.

### <a name="integrating-with-dynamics-365-project-service-automation-v2x"></a>Dynamics 365 Project Service Automation v2.x қызметімен біріктіру
- **Деректерді біріктірудегі үлгі атауы:** Жобалар мен келісім-шарттар (Project Service Automation - Finance)
- **Жобадағы тапсырмалардың атауы**

    - Project Service Automation - Finance жобалық келісім-шарттары
    - Project Service Automation - Finance жобалары
    - Project Service Automation - Finance жобалық келісім-шарт жолдары
    - Project Service Automation - Finance жобалық келісім-шарт жолының кезеңдері
  
### <a name="integrating-with-dynamics-365-project-service-automation-v3x"></a>Dynamics 365 Project Service Automation v3.x қызметімен біріктіру
Жобаның келісім-шарттық жолы кезеңінің үлгісіне әсер ететін Project Service Automation бағдарламасындағы схема өзгерісі бар, сондай-ақ v2 нұсқасын пайдалану Dynamics 365 бағдарламасымен Project Service Automation v3.x біріктіру үшін қажет.

- **Деректерді біріктірудегі үлгі атауы:** Жобалар мен келісім-шарттар (Project Service Automation 3.x - Finance) - v2
- **Жобадағы тапсырмалардың атауы**

    - Project Service Automation - Finance жобалық келісім-шарттары
    - Project Service Automation - Finance жобалары
    - Project Service Automation - Finance жобалық келісім-шарт жолдары
    - Project Service Automation - Finance жобалық келісім-шарт жолының кезеңдері

Жобаның келісім-шарттары мен жобаларын синхрондау орындалмас бұрын, тіркелгілерді синхрондау қажет.

## <a name="entity-set"></a>Нысан жиынтығы

| Project Service Automation       | Қаржы                                                |
|----------------------------------|--------------------------------------------------------|
| Тапсырыстар                           | Жобаның келісім-шартына арналған біріктіру нысаны                |
| Жобалар                         | Жобаға арналған біріктіру нысаны                         |
| Тапсырыс жолдары                      | Жобаның келісім-шарт жолына арналған біріктіру нысаны           |
| Жобаның келісім-шарт жолының кезеңдері | Жобаның келісім-шарт жолының кезеңіне арналған біріктіру нысаны |

## <a name="entity-flow"></a>Нысан ағыны

Жобаның келісім-шарттары Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жобаның келісім-шарттары ретінде синхрондалады. Біріктіру үлгісінің бөлігі ретінде жобаның келісім-шартына арналған Finance жүйесіндегі бастапқы біріктіруді орнатуға болады.

Уақыт пен материал және бекітілген баға жобалары Project Service Automation бағдарламасында басқарылады және жобалар ретінде Finance бағдарламасына синхрондалады. Үлгіні біріктіру бөлігі ретінде сіз Finance бағдарламасында жобаны біріктіру көзін орната аласыз. Қазіргі уақытта тек уақыт және материал және бекітілген баға жобаларына қолдау көрсетіледі.


Жобаның келісім-шарт жолдары Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жоба келісім-шартының шот ұсыну ережелері ретінде синхрондалады. Егер шот ұсыну әдісі әдепкі жобасы түрінен өзгеше болса, синхрондау келісім-шарт жолының жобасы мен жоба тобына арналған жоба түрін жаңартады.

Жобаның келісім-шарт жолының кезеңдері Project Service Automation бағдарламасында басқарылады және олар Finance бағдарламасында жоба келісім-шартының шот ұсыну ережесінің кезеңдері ретінде синхрондалады.

## <a name="project-service-automation-to-finance-integration-solution"></a>Project Service Automation бағдарламасынан Finance бағдарламасына біріктіру шешімі

**Жоба келісім-шартының идентификаторы** өрісі **Жоба келісім-шарттары** бетінде қолжетімді. Бұл өріс біріктіруге қолдау көрсету үшін қалыпты және бірегей кілт ретінде жасалған.

Жаңа жобалық келісім-шарт жасалған кезде, егер **Жоба келісім-шартының идентификаторы** мәні әлі де болмаса, ол нөмір реттілігін пайдалану арқылы автоматты түрде құрылады. Мән өсу нөмірі реттілігінің алдында келетін **ORD** мәнінен, содан соң алты таңбалық жұрнақтан тұрады. Мұнда мысал берілген: **ORD-01022-Z4M9Q0**.

**Жоба нөмірі** өрісі **Жобалар** бетінде қолжетімді. Бұл өріс біріктіруге қолдау көрсету үшін қалыпты және бірегей кілт ретінде жасалған.

Жаңа жобалық келісім-шарт жасалған кезде, егер **Жоба нөмірі** мәні әлі де болмаса, ол нөмір реттілігін пайдалану арқылы автоматты түрде құрылады. Мән өсу нөмірі реттілігінің алдында келетін **PRJ** мәнінен, содан соң алты таңбалық жұрнақтан тұрады. Мұнда мысал берілген: **PRJ-01049-CCNID0**.

Project Service Automation бағдарламасынан Finance бағдарламасына біріктіру шешімі қолданылған кезде жаңарту сценарийін **Жобаның келісім-шарт идентификаторы** өрісін қолданыстағы жобалық келісім-шарттарына, ал **Жоба нөмірі** өрісін Project Service Automation бағдарламасындағы қолданыстағы жобаларға орнатады.

## <a name="prerequisites-and-mapping-setup"></a>Алғышарттар және салыстыру параметрі

- Жобаның келісім-шарттары мен жобаларын синхрондау орындалмас бұрын, тіркелгілерді синхрондау қажет.
- Байланыс жинағында **msdyn\_organizationalunits** - **msdyn\_name \[Name\]** үшін біріктіру кілтінің өрісін салыстыруды қосыңыз. Алдымен байланыс жинағына жобаны қосу қажет болуы мүмкін. Қосымша ақпаратты [Деректерді бағдарламаларға арналған Common Data Service қызметіне біріктіру](https://docs.microsoft.com/powerapps/administrator/data-integrator) тақырыбынан қараңыз.
- Байланыс жинағында **msdyn\_projects** - **msdynce\_projectnumber \[Project Number\]** үшін біріктіру кілтінің өрісін салыстыруды қосыңыз. Алдымен байланыс жинағына жобаны қосу қажет болуы мүмкін. Қосымша ақпаратты [Деректерді бағдарламаларға арналған Common Data Service қызметіне біріктіру](https://docs.microsoft.com/powerapps/administrator/data-integrator) тақырыбынан қараңыз.
- Жобалық келісім-шарттарға арналған **SourceDataID** және жобалар басқа мәнге жаңартылуы мүмкін немесе салыстырудан алынып тасталынуы мүмкін. Әдепкі үлгі мәні – **Project Service Automation**.
- **PaymentTerms** салыстырылуы ол Finance жүйесіндегі жарамды төлем шарттарын көрсететіндей жаңартылуы тиіс. Жоба тапсырмасынан салыстыруды алып тастауға болады. Әдепкі мәнді салыстырудың демо-деректер үшін әдепкі мәндері бар. Келесі кестеде Project Service Automation бағдарламасындағы мәндер көрсетіледі.

    | Мәні | Сипаттамасы   |
    |-------|---------------|
    | 1-көше     | Есеп-шотты алған соң 30 күннен кейін төлеу        |
    | 2-көше     | 2% 10, Нетто 30 |
    | 3     | Есеп-шотты алған соң 45 күннен кейін төлеу        |
    | 4     | Есеп-шотты алған соң 60 күннен кейін төлеу        |

## <a name="power-query"></a>Power Query

Келесі шарттар орындалған жағдайда деректерді сүзгілеу үшін Excel бағдарламасына арналған Microsoft Power Query жүйесін пайдаланыңыз:

- Dynamics 365 Sales бағдарламасында сатылым тапсырыстарыңыз бар.
- Project Service Automation бағдарламасында бірнеше ұйым бөлімшелері бар, сондай-ақ ұйым бөлімшелері Finance жүйесіндегі бірнеше заңды тұлғаларға салыстырылады.

Power Query бағдарламасын пайдалану қажет болса, мына нұсқауларды орындаңыз:

- Жобалар және келісім-шарттар (PSA бағдарламасынан Fin және Ops бағдарламаларына) үлгісінің **Жұмыс элементі (msdyn\_ordertype = 192350001)** түрінің тек сатылым тапсырыстарын қамтитын әдепкі сүзгілері бар. Бұл сүзгі жоба келісім-шарттарының Finance жүйесіндегі сатылым тапсырыстары үшін жасалмайтынына кепілдік береді. Егер өз үлгіңізді жасасаңыз, онда осы сүзгіні қосу қажет.
- Интеграциялық байланыс жиынтығының заңды нысанымен синхрондалуы тиіс келісім-шарттық ұйымдарды ғана қамтитын Power Query сүзгісін жасаңыз. Мысалы, Contoso US келісім-шартының ұйым бөлімшесімен болатын жобалық келісім-шарттар USSI заңды нысаны үшін синхрондалуы қажет, бірақ Contoso US келісім-шартының ұйым бөлімшесімен болатын жобалық келісім-шарттар USMF заңды нысаны үшін синхрондалуы қажет. Егер сіз бұл сүзгіні тапсырманы салыстыруға қоспасаңыз, барлық жобалық келісім-шарттар келісім-шарттың ұйым бөлімшесіне тәуелсіз түрде байланыс жинағы үшін анықталған заңды нысанға синхрондалады.

## <a name="template-mapping-in-data-integration"></a>Деректерді біріктіруде үлгіні салыстыру

> [!NOTE] 
> **CustomerReference**, **AddressCity**, **AddressCountryRegionID**, **AddressDescription**, **AddressLine1**, **AddressLine2**, **AddressState** және **AddressZipCode** өрістері жобалық келісім-шарттарға арналған әдепкі салыстыруда қамтылмаған. Осы деректердің жобалық келісім-шарттар үшін синхрондалуы қажет болса, салыстыруларды қосуға болады.
>
> **Description**, **ParentID**, **ProjectGroup**, **ProjectManagerPersonnelNumber** және **ProjectType** өрістері жобаларға арналған әдепкі салыстыруда қамтылмайды. Осы деректердің жобалар үшін синхрондалуы қажет болса, салыстыруларды қосуға болады.

Келесі суреттер деректерді біріктіру қызметіндегі үлгі тапсырмасын салыстырулар мысалдарын көрсетеді. Картада Project Service Automation бағдарламасынан Finance бағдарламасына синхрондалатын өріс туралы ақпарат көрсетілген.

[![Жоба келісім-шартының үлгісін салыстыру](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)

[![Жоба үлгісін салыстыру](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)

[![Жоба келісім-шарт жолдары үлгісін салыстыру](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)

[![Жоба келісім-шарт жолы кезеңінің үлгісін салыстыру](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)

#### <a name="project-contract-line-milestone-mapping-in-the-projects-and-contracts-psa-3x-to-dynamics---v2-template"></a>Жобалар және келісім-шарттар (Dynamics PSA 3.x) - v2 үлгісіндегі жобалық келісім-шарты жолы кезеңін салыстыруы:

[![Екінші нұсқа үлгісі бар жоба келісім-шарт жолы кезеңін салыстыру](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]