---
title: Нысан, басқару элементі және пайдаланушы интерфейсіндегі өзгерістер (Project Service Automation 3.x)
description: Бұл тақырыпта Microsoft Dynamics Project Service Automation 3.x нұсқасы үшін шешім өзгерістері сипатталған.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 03/15/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: e3d6f515cec51cb30f83ff22a14ecb125dc81214
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6007958"
---
# <a name="entity-control-and-user-interface-changes-project-service-automation-3x"></a>Нысан, басқару элементі және пайдаланушы интерфейсіндегі өзгерістер (Project Service Automation 3.x)

[!include [banner](../../includes/psa-now-project-operations.md)]


Microsoft Dynamics Project Service Automation (PSA) 3.x нұсқасының шығарылымымен, нысандарға, басқару элементтеріне, көріністерге және пайдаланушы интерфейсіне көптеген өзгерістер енгізілді. Бұл тақырыпта осы маңызды өзгерістер туралы ақпарат берілген.

## <a name="parent-child-relationships-for-sales-document-sales-document-line-sales-document-line-detail-entities"></a>Сатылым құжаты, сатылым құжатының жолы және сатылым құжаты жолы мәліметінің нысандарына арналған басты-еншілес қарым-қатынастар
Dynamics 365 Project Service Automation (PSA) бағдарламасының 3.0 нұсқасына дейін шығарылған нұсқаларында, сатылым құжаты, сатылым құжатының жолы және сатылым құжаты жолы мәліметінің нысандары арасындағы кейбір қарым-қатынастар қатысты нысанның GUID идентификаторын жол көрсетіліміне орнататын жолдық өрістер арқылы жүзеге асырылды. Бұл осы қарым-қатынастардың Dynamics CRM нысандар қатынасы сияқты бірдей жұмыс істеуі және жолдық өрістердің іздеу өрістері сияқты қызмет етуі үшін серверде және шешімнің клиенттік жақтарында маңызды реттелетін кодты қажет ететін платформаның шектеулеріне байланысты болды.

PSA 3.0 нұсқасы сатылым құжаты мен сатылым құжаты жолының нысандары арасында жаңа нысандар қатынастарын пайдалану үшін жаңартылды.

Іздеу өрістерін енді нысандарға сілтемелерді көрсету үшін пайдалануға болатындықтан, алдыңғы нұсқалардағы қатысты нысанның GUID идентификаторының жол мәні бар өрістер енді қажет емес және сол себепті ұсынылмайды. Бұрынғы жолдық өрістермен анықталатын қарым-қатынастарды өңдейтін реттелетін клиенттік және серверлік код та ұсынылмайды.

### <a name="entity-schema-changes"></a>Нысан схемасының өзгерістері
Төмендегі кестеде ұсынылмайтын жолдық өрістер мен нысандарға арналған жаңа іздеу өрістерінің бірге-бір тізімі берілген. 

 Нысан |   Ұсынылмайтын өріс (Жол) | Жаңа өріс (Іздеу)
--- | --- | ---
Есеп-шот туралы мәлімет (Есеп-шот жолы) |  msdyn_contractline |    msdyn_contractlineid
msdyn_actual (Нақты) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_contractlineinvoiceschedule (Жоба келісім-шарты жолының есеп-шот ұсыну кестесі) |    msdyn_contractline |    msdyn_contractlineid
msdyn_contractlinescheduleofvalue (Жоба келісім-шарты жолының кезеңі) |   msdyn_contractline |    msdyn_contractlineid
msdyn_fact (Факт) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_invoicelinetransaction (Есеп-шот жолы мәліметі) | msdyn_invoiceline <br> msdyn_salescontractline | msdyn_invoicelineid <br> msdyn_salescontractlineid
msdyn_journalline (Журнал жолы) |  msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlineresourcecategory (Жоба келісім-шарты жолы ресурсының санаты) | msdyn_salescontractline |   msdyn_contractlineid
msdyn_orderlinetransaction (Жоба келісім-шартының жолы туралы мәлімет) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlinetransactioncategory (Жоба келісім-шарт жолының транзакция санаты) |   msdyn_contractline |    msdyn_contractlineid
msdyn_orderlinetransactionclassification (Жоба келісім-шарты жолының транзакция жіктеуі) |   msdyn_contractline |    msdyn_contractlineid
msdyn_quotelineinvoiceschedule (Баға ұсыну жолы есеп-шоты кестесі) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelineresourcecategory (Баға ұсыну жолы ресурсы санаты) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinescheduleofvalue (Баға ұсыну жолы кезеңі) | msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransaction (Баға ұсыну жолы мәліметі) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactioncategory (Баға ұсыну жолы транзакциясы санаты) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactionclassification (Баға ұсыну транзакциясы жіктеуі) |  msdyn_quoteline |   msdyn_quotelineid
SalesOrderDetail (Тапсырыс жолы) | msdyn_quotelineid | msdyn_quoteline 

### <a name="deprecated-custom-views-and-controls"></a>Ұсынылмайтын реттелетін көріністер мен басқару элементтері
Келесі реттелетін көріністер мен басқару элементтері және олармен байланысты артефактілер ұсынылмайды.

- Жауапкершілік көрінісі.
- Баға ұсыну жолының **Жоба туралы ақпарат** бетінде баға ұсыну жолы мәліметтерін көрсетуге арналған тордың басқару элементтері.
- Сату тапсырысы жолының **Жоба туралы ақпарат** бетінде жоба келісім-шартының жолы туралы мәліметтерді көрсетуге арналған тордың басқару элементтері.

> [!NOTE]
> Ұсынылмайтын ресурстардың толық тізімі үшін, [Project Service Automation 3.x нұсқасындағы ұсынылмайтын веб-ресурстар](../developer-guides/web-resources-deprecated-v3.x.md) бөлімін қараңыз

## <a name="unified-client-interface-app-module"></a>Бірыңғай клиенттік интерфейс бағдарламасының модулі
Бірыңғай клиенттік интерфейс (UCI) бағдарламасының модульдерінің енгізілуімен, жүйеден PSA сайт картасының жазбалары алынып тасталды.  
Мүмкіндікке, баға ұсынуға, тапсырысқа және есеп-шотқа арналған пішінді ауыстыруға байланысты функционалдылық ұсынылмайды, себебі UCI бағдарламасының модулі пішіндердің PSA нұсқаларын ғана қамтиды.  

Келесі веб-ресурстар ұсынылмайды:

- msdyn_\SalesDocument\SalesDocumentFormLoader.js
- msdyn_\SalesDocument\PSSalesDocumentCustomFormIds.js

> [!NOTE]
> Ұсынылмайтын ресурстардың толық тізімі үшін, [Project Service Automation 3.x нұсқасындағы ұсынылмайтын веб-ресурстар](../developer-guides/web-resources-deprecated-v3.x.md) бөлімін қараңыз.




[!INCLUDE[footer-include](../../includes/footer-banner.md)]