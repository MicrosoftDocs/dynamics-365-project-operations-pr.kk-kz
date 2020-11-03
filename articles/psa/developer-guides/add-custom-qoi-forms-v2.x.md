---
title: Жаңа реттелетін нысан пішіндерін қосу (Project Service Automation 2.x)
description: Бұл тақырыпта Dynamics 365 Project Service Automation 2.x. нұсқасында мүмкіндіктерге, баға ұсыныстарына, тапсырыстарға немесе есеп-шоттарға реттелетін нысан пішіндерін қосу жолы туралы ақпарат берілген.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 57d4b9aad433af6d3e73369c76f2793f349c6965
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079854"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a>Жаңа реттелетін нысан пішіндерін қосу (Project Service Automation 2.x)

## <a name="type-field"></a>"Түрі" өрісі 

Dynamics 365 Project Service Automation қондырмасы мүмкіндік, баға ұсынысы, тапсырыс және есеп-шот нысандарының **жұмыс негізіндегі** нұсқаларының **элемент негізіндегі** және **сервер негізіндегі** нұсқаларынан айырмашылығын көру үшін, олардың **Түрі** ( **msdyn\_ordertype** ) өрісіне сүйенеді. Осы нысандардың жұмысқа негізделген нұсқаларын PSA жүйесі өңдейді. Шешімнің көптеген клиенттік және серверлік бизнес логикасы **Түрі** өрісіне байланысты болады. Сондықтан да, нысандарды жасаған кезде өрістерді дұрыс мәнмен баптандыру маңызды. Қате мән дұрыс емес әрекеттерді тудыруы мүмкін және кейбір бизнес логика дұрыс жұмыс істемеуі мүмкін.

## <a name="automatic-form-switching"></a>Пішіндерді автоматты түрде ауыстыру

Деректердің ықтимал бүлінуін және сатылым нысандарының жазбаларын дұрыс емес баптандыру және өңдеу нәтижесінде күтпеген әрекеттерді болдырмау үшін, PSA жүйесі енді кірістірілген пішіндерді ауыстыру үшін автоматты түрде ауыстыру логикасын қамтиды. Бұл логика пайдаланушыларды жұмыс негізіндегі нұсқамен жұмыс істеуге арналған дұрыс пішінге немесе мүмкіндік, баға ұсынысы, тапсырыс немесе есеп-шот нысанының кез-келген басқа түріне өткізеді. Пайдаланушы мүмкіндік, баға ұсынысы, тапсырыс немесе есеп-шот нысанының жұмыс негізіндегі нұсқасын ашқанда, пішін **Жоба туралы ақпарат** пішініне ауысады.

Пішінді автоматты түрде ауыстыру логикасы **formId** мәні мен **msdyn\_ordertype** өрісінің арасындағы салыстыруға сүйенеді . Сол салыстыруға барлық кірістірілген пішіндер қосылды. Дегенмен ұйымның қандай нұсқасының өңделетінін көрсету үшін, реттелетін пішіндерді қолмен қосу керек. Бұл **msdyn\_ordertype** өрісіне негізделген. Егер салыстыруда пішінді ауыстыру логикасы жоқ болса, логика нысанның **msdyn\_ordertype** өрісінде сақталған мәнге негізделіп, кірістірілген пішінге ауысады.

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a>Реттелетін пішіндерді қосып, пішінді ауыстыру логикасын қосыңыз

Келесі мысалда реттелетін пішінді, **Менің жоба туралы ақпаратым** қосу әдісі көрсетілген, осылайша ол жұмысқа негізделген мүмкіндіктермен жұмыс істейді. Реттелетін пішіндерді қосу үшін дәл осы процедура пайдаланылады, осылайша олар баға ұсыныстарымен, тапсырыстармен және есеп-шоттармен жұмыс істейді.

**Жоба туралы ақпарат** пішінінің реттелетін нұсқасын жасау үшін осы қадамдарды орындаңыз.

1. Мүмкіндік нысанында **Жоба туралы ақпарат** пішінін ашып, **Менің жоба туралы ақпаратым** деп аталған көшірмені сақтаңыз.
2. Пішінді ашып, сипаттарда **Жоба туралы ақпарат** пішінінің пішінді баптандыру сценарийлерінің бар екеніне көз жеткізіңіз. 

    > [!IMPORTANT]
    > Сценарийлерді алып тастамаңыз. Әйтпесе, кейбір деректер қате баптандырылуы мүмкін.

3. Пішінде **Түрі** ( **msdyn\_ordertype** ) өрісінің бар екенін тексеріңіз. 

    > [!IMPORTANT]
    > Бұл өрісті алып тастамаңыз. Әйтпесе, баптандыру сценарийлері сәтсіз болады.

4. Жаңа пішіннің **formId** мәнін табыңыз. Бұл қадамды екі түрлі жолмен орындауға болады:

    - **Менің жоба туралы ақпаратым** пішінін басқарылмайтын шешімнің бір бөлігі ретінде экспорттап, экспортталған шешімнің реттеу .xml файлында **formId** мәнін іздеңіз.
    - Пішін өңдегішінде **Менің жоба туралы ақпаратым** пішінін ашып, келесі суретте көрсетілгендей, URL мекенжайындағы **fromId** параметрінің жанында глобалдық бірегей идентификаторды (GUID) іздеңіз.

    ![URL мекенжайындағы жаңа пішіннің formId мәні](media/how-to-add-custom-forms-in-v2.0.png)

5. msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js веб-ресурсын өңдеу арқылы **formId** мәні үшін **msdyn\_ordertype** салыстыруын жасаңыз. Ресурстан кодты алып тастап, оны келесі кодпен ауыстырыңыз.

    ```javascript
    define(["require", "exports"], function (require, exports) {
        "use strict";
        var SalesDocumentCustomFormIds = (function () {
            function SalesDocumentCustomFormIds() {
            }
            SalesDocumentCustomFormIds.overwriteFormIds = function (mappedFormIds) {
                /*
                ---- Notes ----
                mappedFormIds[SalesEntity][OrderType] => The array of forms IDs that support particular entity and order type
                Add or overwrite customized formId for the particular entity and order type by calling:
                    mappedFormIds[<EntityType>][<msdyn_ordertype>].push("<formId>");
                Allowed msdyn_ordertype values for reference:
                    ServiceBased: 690970002 (Field Service version of the entity)
                    WorkBased: 192350001 (PSA version of the entity)
                    ItemBased: 192350000 (Regular out of the box entity)
                Uncomment and update one of the following lines to register custom PSA form for required entity:
                */      
                //mappedFormIds[1][192350001].push("<formId>"); //Quote
                //mappedFormIds[5][192350001].push("<formId>"); //Quote Line
                //mappedFormIds[2][192350001].push("<formId>"); //Sales Order
                //mappedFormIds[6][192350001].push("<formId>"); //Sales Order Line
                // In this example we have added new form for Opportunity
                mappedFormIds[0][192350001].push("192EE537-DCC4-45D3-B7AF-EA694B9113D2"); //Opportunity
                //mappedFormIds[4][192350001].push("<formId>"); //Opportunity Line
            };
            return SalesDocumentCustomFormIds;
        }());
        exports.default = SalesDocumentCustomFormIds;
    });
    ```

6. Реттеулерді сақтап, жариялаңыз.
