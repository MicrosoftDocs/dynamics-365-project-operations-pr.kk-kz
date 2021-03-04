---
title: Жұмыс декомпозициясының құрылымы бойынша пікірлерді жаңарту
description: Бұл тақырыпта Project Service Automation 2.x және 3.x аралығындағы нұсқадағы жұмыс декомпозициясының құрылымын жаңарту туралы ақпарат берілген.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: cea8ce7f61fbc0f0c8c8deb522bc332be102238d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149550"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a>Жұмыс декомпозициясының құрылымы бойынша пікірлерді жаңарту

[!include [banner](../includes/psa-now-project-operations.md)]

Бұл тақырыпта Project Service Automation 2.x және 3.x аралығындағы нұсқадағы жұмыс декомпозициясының құрылымын жаңарту туралы ақпарат берілген. Бұл тақырыпта сәтті жаңарту үшін қажет Project Service Automation (PSA) жобасындағы дұрыс күйді анықтайды. Сондай-ақ жаңартудың сәтсіз болуына әкелетін блоктаудың жалпы шарттары туралы ақпарат бар. Жоба кестесінде жоба тапсырмалары мен функцияларын анықтау туралы қосымша ақпаратты [Жоба кестелері](project-creating.md) бөлімінен қараңыз.

## <a name="key-entities"></a>Негізгі нысандар
Ресурстармен жүктеліп қойған жұмыс декомпозициясының нақты құрылымы үшін келесі нысандар қажет:

- [Жоба](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [Жоба тобы](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [Жоба тапсырмасы](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [Ресурс тапсырмалары](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [Жоба тапсырмасы тәуелділігі](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [Тапсырыс беруге болатын ресурстар](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

Жұмыс декомпозициясының құрылымын жүктеген ресурсты анықтау үшін келесі қадамдарды орындау керек:

1. Жаңа жоба жасаңыз. Жаңа жоба жасау жолы туралы ақпарат алу үшін [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project) бөлімін қараңыз.
2. Бір немесе бірнеше тапсырма жасаңыз. Тапсырма жасау жолы туралы ақпарат алу үшін [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask) бөлімін қараңыз.
3. Тапсырма тәуелділіктерін анықтаңыз. Қосымша ақпарат алу үшін [Жоба тапсырмасы тәуелділігі](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency) мақаласын қараңыз.
4. Жобаға жоба тобының мүшелерін тағайындаңыз. Қосымша ақпарат алу үшін [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam) бөлімін қараңыз.
5. Тапсырмаларға жоба тобының мүшелерін тағайындаңыз. Қосымша ақпарат алу үшін [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment) бөлімін қараңыз.

## <a name="project-team-relationships"></a>Жоба тобының қатынастары

Жаңартуды сәтті орындау үшін келесі қатынастарды дұрыс сақтау керек:
- Жоба тобының барлық мүшелері тапсырыс беруге болатын ресурспен байланыстырылуы керек.
- Жоба тобының барлық мүшелері бірдей жобамен байланыстырылуы керек. 

## <a name="project-task-relationships"></a>Жоба тапсырмасының қатынастары
Жаңартуды сәтті орындау үшін келесі қатынастарды дұрыс сақтау керек:

- Кез келген қатысты тапсырмалар бір жобамен байланысты болуы керек.
- Әр жол тапсырмасында негізгі тапсырма болуы керек.
- Әр тапсырмада негізгі жоба болуы керек.

### <a name="valid-conditions"></a>Жарамды шарттар

- Барлық тапсырма ұзақтықтары бір сағаттан үлкен немесе оған тең болуы (> =) және 1 800 000 минуттан (1250 күн) аспауы керек.*
- Барлық тапсырмалардың басталу күні 2000/01/01 күнінен кейін болуы керек.*
- Барлық тапсырмалардың басталу күні осы күннен бастап ең көбі 17 жыл бұрын болуы керек.*
- Барлық тапсырмалардың басталу күні аяқталу күнінен ертерек немесе оған тең болуы керек.
- Классификациялар бойынша транзакцияның барлық түрлерінде (шығыс, материал, салық және уақыт) **Әдепкі бірлік** және **Бірлік тобы** мәндері болуы керек.
- Күн пішімдерінде әріптер болмауы керек.

### <a name="potential-mitigation-steps"></a>Ықтимал жеңілдету қадамдары
- Жоба идентификаторы жоқ жоба тапсырмаларын анықтау үшін "Кеңейтілген іздеу" құралын қолданыңыз.
- Жоспарланған ұзақтығы> 1,800,000-ден үлкен жоба тапсырмаларын анықтау үшін "Кеңейтілген іздеу" құралын қолданыңыз.
- Деректерді өзгертуден бұрын, деректердің нашар күйге келуіне әкелуі мүмкін кез келген реттеулерді зерттеуіңіз керек. Бұл реттеулер деректерге қатысты жаңартуларды жасамас бұрын қарастырылуы керек.
- Жоғып кеткен анықталған тапсырмалар үшін, егер олар қажет болмаса немесе дұрыс негізгі жобамен байланысты болуы керек болса, оларды жою туралы ойланыңыз.
- Ұзақтығы 1250 күннен асатын кез келген тапсырмалар үшін, егер мүмкін болса, жалпы ұзақтығын көрсететін бірнеше тапсырма қосуды ойлаңыз.

> [!NOTE]
> Жұлдызшамен (\*) белгіленген элементтер тұтынушымен қарым-қатынасты басқару (CRM) қызметінің тек 7320 қайталанатын кеңейтуді қолдайтынына байланысты шектеулерге ие. Бұл шектен аспау керек.

## <a name="resource-assignment-relationships"></a>Ресурсты тағайындау қатынастары
Жаңартуды сәтті орындау үшін келесі қатынастарды дұрыс сақтау керек:

- Жұмыс декомпозициясының құрылымындағы барлық ресурс тапсырмалары бірдей жобамен байланысты болуы керек.
- Жұмыс декомпозициясының құрылымындағы барлық ресурс тапсырмалары бірдей жобаның топ мүшелерімен байланысты болуы керек.

### <a name="potential-mitigation-steps"></a>Ықтимал жеңілдету қадамдары
- Жоғарыда сипатталған жағдайлардан тыс барлық тапсырмаларды анықтаңыз.  
- Жарамсыз болып табылатын кез келген ресурс тапсырмалары жойылуы керек.

## <a name="project-task-dependency-relationships"></a>Жоба тапсырмасы тәуелділігінің қатынастары
Жаңартуды сәтті орындау үшін келесі қатынастарды дұрыс сақтау керек:

- Жоба тапсырмасының барлық тәуелділіктері бір жобамен байланысты болуы керек.
- Тапсырмада бірнеше рет сілтеме жасалған бірдей тәуелділік болмауы керек.
