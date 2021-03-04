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
ms.openlocfilehash: 31986efed81892cc5722cb8f5e292cde14d8843d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144600"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a><span data-ttu-id="9f96b-103">Жаңа реттелетін нысан пішіндерін қосу (Project Service Automation 2.x)</span><span class="sxs-lookup"><span data-stu-id="9f96b-103">Add new custom entity forms (Project Service Automation 2.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a><span data-ttu-id="9f96b-104">"Түрі" өрісі</span><span class="sxs-lookup"><span data-stu-id="9f96b-104">Type field</span></span> 

<span data-ttu-id="9f96b-105">Dynamics 365 Project Service Automation қондырмасы мүмкіндік, баға ұсынысы, тапсырыс және есеп-шот нысандарының **жұмыс негізіндегі** нұсқаларының **элемент негізіндегі** және **сервер негізіндегі** нұсқаларынан айырмашылығын көру үшін, олардың **Түрі** (**msdyn\_ordertype**) өрісіне сүйенеді.</span><span class="sxs-lookup"><span data-stu-id="9f96b-105">Dynamics 365 Project Service Automation relies on the **Type** (**msdyn\_ordertype**) field of the Opportunity, Quote, Order, and Invoice entities to distinguish **work-based** versions of these entities from **item-based** and **service-based** versions.</span></span> <span data-ttu-id="9f96b-106">Осы нысандардың жұмысқа негізделген нұсқаларын PSA жүйесі өңдейді.</span><span class="sxs-lookup"><span data-stu-id="9f96b-106">Work-based versions of these entities are handled by PSA.</span></span> <span data-ttu-id="9f96b-107">Шешімнің көптеген клиенттік және серверлік бизнес логикасы **Түрі** өрісіне байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="9f96b-107">Lots of business logic on the client side and server side of the solution depends on the **Type** field.</span></span> <span data-ttu-id="9f96b-108">Сондықтан да, нысандарды жасаған кезде өрістерді дұрыс мәнмен баптандыру маңызды.</span><span class="sxs-lookup"><span data-stu-id="9f96b-108">Therefore, it's important that the field be initialized with a correct value when the entities are created.</span></span> <span data-ttu-id="9f96b-109">Қате мән дұрыс емес әрекеттерді тудыруы мүмкін және кейбір бизнес логика дұрыс жұмыс істемеуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="9f96b-109">An incorrect value can cause incorrect behaviors, and some business logic might not run correctly.</span></span>

## <a name="automatic-form-switching"></a><span data-ttu-id="9f96b-110">Пішіндерді автоматты түрде ауыстыру</span><span class="sxs-lookup"><span data-stu-id="9f96b-110">Automatic form switching</span></span>

<span data-ttu-id="9f96b-111">Деректердің ықтимал бүлінуін және сатылым нысандарының жазбаларын дұрыс емес баптандыру және өңдеу нәтижесінде күтпеген әрекеттерді болдырмау үшін, PSA жүйесі енді кірістірілген пішіндерді ауыстыру үшін автоматты түрде ауыстыру логикасын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="9f96b-111">To avoid potential data corruption and unexpected behaviors that are caused by incorrect initialization and editing of the sales entity records, PSA now includes logic for automatic form switching in out-of-box forms.</span></span> <span data-ttu-id="9f96b-112">Бұл логика пайдаланушыларды жұмыс негізіндегі нұсқамен жұмыс істеуге арналған дұрыс пішінге немесе мүмкіндік, баға ұсынысы, тапсырыс немесе есеп-шот нысанының кез келген басқа түріне өткізеді.</span><span class="sxs-lookup"><span data-stu-id="9f96b-112">This logic takes users to the correct form for working with the work-based version or any other type of Opportunity, Quote, Order, or Invoice entity.</span></span> <span data-ttu-id="9f96b-113">Пайдаланушы мүмкіндік, баға ұсынысы, тапсырыс немесе есеп-шот нысанының жұмыс негізіндегі нұсқасын ашқанда, пішін **Жоба туралы ақпарат** пішініне ауысады.</span><span class="sxs-lookup"><span data-stu-id="9f96b-113">When a user opens the work-based version of an Opportunity, Quote, Order, or Invoice entity, the form is switched to **Project Information**.</span></span>

<span data-ttu-id="9f96b-114">Пішінді автоматты түрде ауыстыру логикасы **formId** мәні мен **msdyn\_ordertype** өрісінің арасындағы салыстыруға сүйенеді .</span><span class="sxs-lookup"><span data-stu-id="9f96b-114">The automatic form switching logic relies on the mapping between the **formId** value and the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="9f96b-115">Сол салыстыруға барлық кірістірілген пішіндер қосылды.</span><span class="sxs-lookup"><span data-stu-id="9f96b-115">All out-of-box forms have been added to that mapping.</span></span> <span data-ttu-id="9f96b-116">Дегенмен ұйымның қандай нұсқасының өңделетінін көрсету үшін, реттелетін пішіндерді қолмен қосу керек.</span><span class="sxs-lookup"><span data-stu-id="9f96b-116">However, custom forms must be manually added to indicate which version of the entity they are intended to handle.</span></span> <span data-ttu-id="9f96b-117">Бұл **msdyn\_ordertype** өрісіне негізделген.</span><span class="sxs-lookup"><span data-stu-id="9f96b-117">This is based on the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="9f96b-118">Егер салыстыруда пішінді ауыстыру логикасы жоқ болса, логика нысанның **msdyn\_ordertype** өрісінде сақталған мәнге негізделіп, кірістірілген пішінге ауысады.</span><span class="sxs-lookup"><span data-stu-id="9f96b-118">If the form switching is missing from the mapping, logic will switch to the out-of-box form, based on the value that is saved in the **msdyn\_ordertype** field of the entity.</span></span>

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a><span data-ttu-id="9f96b-119">Реттелетін пішіндерді қосып, пішінді ауыстыру логикасын қосыңыз</span><span class="sxs-lookup"><span data-stu-id="9f96b-119">Add custom forms and turn on the form switching logic</span></span>

<span data-ttu-id="9f96b-120">Келесі мысалда реттелетін пішінді, **Менің жоба туралы ақпаратым** қосу әдісі көрсетілген, осылайша ол жұмысқа негізделген мүмкіндіктермен жұмыс істейді.</span><span class="sxs-lookup"><span data-stu-id="9f96b-120">The following example shows how to add a custom form, **My Project Information**, so that it works with work-based opportunities.</span></span> <span data-ttu-id="9f96b-121">Реттелетін пішіндерді қосу үшін дәл осы процедура пайдаланылады, осылайша олар баға ұсыныстарымен, тапсырыстармен және есеп-шоттармен жұмыс істейді.</span><span class="sxs-lookup"><span data-stu-id="9f96b-121">The same process is used to add custom forms so that they work with quotes, orders, and invoices.</span></span>

<span data-ttu-id="9f96b-122">**Жоба туралы ақпарат** пішінінің реттелетін нұсқасын жасау үшін осы қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-122">Follow these steps to create a custom version of the **Project Information** form.</span></span>

1. <span data-ttu-id="9f96b-123">Мүмкіндік нысанында **Жоба туралы ақпарат** пішінін ашып, **Менің жоба туралы ақпаратым** деп аталған көшірмені сақтаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-123">In the Opportunity entity, open the **Project Information** form, and save a copy under the name **My Project Information**.</span></span>
2. <span data-ttu-id="9f96b-124">Пішінді ашып, сипаттарда **Жоба туралы ақпарат** пішінінің пішінді баптандыру сценарийлерінің бар екеніне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-124">Open the new form, and then, in the properties, make sure that the form initialization scripts from the **Project Information** form are present.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="9f96b-125">Сценарийлерді алып тастамаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-125">Don't remove the scripts.</span></span> <span data-ttu-id="9f96b-126">Әйтпесе, кейбір деректер қате баптандырылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="9f96b-126">Otherwise, some data might be initialized incorrectly.</span></span>

3. <span data-ttu-id="9f96b-127">Пішінде **Түрі** (**msdyn\_ordertype**) өрісінің бар екенін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-127">Verify that the **Type** (**msdyn\_ordertype**) field is present in the form.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="9f96b-128">Бұл өрісті алып тастамаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-128">Don't remove this field.</span></span> <span data-ttu-id="9f96b-129">Әйтпесе, баптандыру сценарийлері сәтсіз болады.</span><span class="sxs-lookup"><span data-stu-id="9f96b-129">Otherwise, the initialization scripts will fail.</span></span>

4. <span data-ttu-id="9f96b-130">Жаңа пішіннің **formId** мәнін табыңыз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-130">Find the **formId** value of the new form.</span></span> <span data-ttu-id="9f96b-131">Бұл қадамды екі түрлі жолмен орындауға болады:</span><span class="sxs-lookup"><span data-stu-id="9f96b-131">You can complete this step in two ways:</span></span>

    - <span data-ttu-id="9f96b-132">**Менің жоба туралы ақпаратым** пішінін басқарылмайтын шешімнің бір бөлігі ретінде экспорттап, экспортталған шешімнің реттеу .xml файлында **formId** мәнін іздеңіз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-132">Export the **My Project Information** form as part of an unmanaged solution, and then look up the **formId** value in the customization.xml file of the exported solution.</span></span>
    - <span data-ttu-id="9f96b-133">Пішін өңдегішінде **Менің жоба туралы ақпаратым** пішінін ашып, келесі суретте көрсетілгендей, URL мекенжайындағы **fromId** параметрінің жанында глобалдық бірегей идентификаторды (GUID) іздеңіз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-133">Open the **My Project Information** form in the form editor, and then look for the globally unique identifier (GUID) next to the **fromId** parameter in the URL, as shown in the following illustration.</span></span>

    ![URL мекенжайындағы жаңа пішіннің formId мәні](media/how-to-add-custom-forms-in-v2.0.png)

5. <span data-ttu-id="9f96b-135">msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js веб-ресурсын өңдеу арқылы **formId** мәні үшін **msdyn\_ordertype** салыстыруын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-135">Create an **msdyn\_ordertype** mapping for the **formId** value by editing the msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web resource.</span></span> <span data-ttu-id="9f96b-136">Ресурстан кодты алып тастап, оны келесі кодпен ауыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-136">Remove the code from the resource, and replace it with the following code.</span></span>

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

6. <span data-ttu-id="9f96b-137">Реттеулерді сақтап, жариялаңыз.</span><span class="sxs-lookup"><span data-stu-id="9f96b-137">Save and then publish the customizations.</span></span>
