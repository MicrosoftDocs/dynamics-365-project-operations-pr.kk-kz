---
title: Microsoft Project бағдарламасында жұмысты жоспарлау үшін Project Service қондырмасын пайдалану | MicrosoftDocs
description: Бұл тақырыпта Microsoft Project Service үшін Microsoft Project қондырмасын қосу, конфигурациялау және пайдалану жолы туралы ақпарат берілген.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
ms.topic: article
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
ms.openlocfilehash: e85b3e0e13bb48aeb9eeb111c2f782f4d62505a7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014528"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a>Microsoft Project бағдарламасында жұмысты жоспарлау үшін Project Service Automation қосылатын модулін пайдалану

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесі болжамдарды қоса жоба жоспарлауын орындауды жеңілдетеді. Соңғы ұсыныс жіберілген кезде құн, әрекет және сатылым мәндерінің анық болуы үшін жұмысты анықтауға болады.  

 Енді [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] жүйесін орнатуға және жоспарлау жұмысын [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасының таныс ортасында орындауға болады. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасының күшті жоспарлау мен басқару мүмкіндіктерін пайдаланып, жоба жоспарын Project Service Automation қызметінде жаңартыңыз.  

> [!IMPORTANT]
> - [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобалары үшін [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлдарын сақтау мақсатында SharePoint құжаттарды басқару мүмкіндігін пайдалану үшін, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] әкімшісі құжаттарды басқару мүмкіндігін іске қосуы керек. 
> - [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] тек [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition нұсқасымен үйлесімді.  

## <a name="download-and-install-the-add-in"></a>Қосылатын модульді жүктеп алу және орнату  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне кіру ақпаратын дайындап қойыңыз. Осы ақпарат [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасынан [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне қосылу үшін қажет.  

1.  Жүктеп алу орталығынан Project Service бағдарламасының [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) немесе [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956) қолдау көрсетілетін нұсқасы үшін қондырманы жүктеп алыңыз.  

2.  Жүктеп алу сілтемесін басыңыз.  

3.  Жүктеп алу аяқталған кезде қондырманы орнату үшін **Иә** параметрін таңдаңыз.  

## <a name="configure-the-add-in"></a>Қосылатын модульді конфигурациялау  

1. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын ашыңыз және **Project Service** қойыншасын басыңыз.  

2. **Қосылу** пәрменін таңдаңыз.  

3. Жүйеге кіру ақпаратын енгізіп, **Кіру** пәрменін таңдаңыз.  

   Енді қосылатын модуль пайдалануын бастауға болады.  

## <a name="read-from-a-template"></a>Үлгіден оқу  
 Жобаны жоспарлауды бастау үшін [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішінде жасалған және [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасына көшірілген үлгіден оқыңыз. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Жоба үлгісін жасау (Project Service Automation)](../psa/create-project-template.md)  

1.  **Project Service** қойыншасынан **Оқу** > **Project Service Automation жоба үлгісі** тармағын басыңыз.  

2.  Тізімнен жоба үлгісін таңдап, **Ашу** пәрменін таңдаңыз.  

    > [!NOTE]
    >  Әдепкі бойынша, үлгіден Project бағдарламасына көшірілген тапсырмалар қолмен жоспарланған ретінде орнатылады.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>Жоба ресурстарына [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] рөлдерін белгілеу  

1.  Жобаны ашыңыз және **Тапсырма** таспасын басыңыз.  

2.  **Гант диаграммасы** мәзірін басып, **Ресурс парағы** параметрін таңдаңыз.  

3.  Ресурс парағында **Project Service ресурс рөлі** ашылмалы мәзірін басыңыз және Project Service Automation рөлін таңдаңыз.  

## <a name="staff-your-project-with-resources"></a>Жобаны ресурстармен жабдықтау  

1.  Project Service қойыншасынан жолды таңдаңыз және **Ресурстар табу** пәрменін таңдаңыз.  

2.  **Ресурсты тіркеу** экранында жобаға пайдалану қажет ресурсты таңдаңыз.  

3.  **Тіркеу** пәрменін таңдап, **OK** түймешігін басыңыз.  

## <a name="publish-your-project"></a>Жобаны жариялау  
Жоба жоспарлауы аяқталған кезде келесі қадам жобаны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне импорттау және жариялау болады.  

Жоба [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне импортталады. Бағалар және топ жасау процесі қолданылады. Топтың, жоба болжамдарының және жұмыс декомпозициясы құрылымының жасалғанын көру үшін жобаны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесінде ашыңыз. Төмендегі кестеде нәтижелерді табатын жер көрсетілген:


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Гант диаграммасы**   | [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жұмыс декомпозициясының құрылымы** экранына импорттайды. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Ресурс парағы** |   [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жоба тобы мүшелері** экранына импорттайды.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Пайдалану пайдалану**    |    [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жоба болжамдары** экранына импорттайды.     |

**Жобаны импорттау және жариялау үшін**  
1. **Project Service** қойыншасынан **Жариялау** > **Жаңа Project Service Automation жобасы** тармағын басыңыз.  

2. **Project Service қызметіндегі жаңа жобаға жариялау** диалогтық терезесінде **Жоба атауы** мәнін енгізіңіз және **Тұтынушы** параметрін таңдаңыз.  

3. Сонымен қатар жоспардың Project файлын Project Service Automation қызметіне байланыстыру үшін **Жоба жоспарын Project Service Automation қызметіне байланыстыру** пәрменін белгілеңіз.  

4. **Жариялау** түймешігін басыңыз.  

   Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне байланыстыру Project файлын басты етеді және [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіндегі жұмыс декомпозициясының құрылымын тек оқуға арналған етіп орнатады.  Жоба жоспарына өзгерістер енгізу үшін оларды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасау және жаңартулар ретінде [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіне жариялау қажет.  

## <a name="edit-a-project-thats-been-imported"></a>Импортталған жобаны өңдеу  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметіне импортталған жоба жоспарына өзгерістер енгізу үшін екі таңдау бар:  

- Басты файлды ашып, оны [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында өңдеңіз.  

- Файлды ажыратыңыз және оны тікелей Project Service қызметінде өңдеңіз. Әдепкі бойынша, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ішінен жүктеп салынған жоба құлыпталады және оны тек Project бағдарламасында өңдеуге болады. Файлды [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішінде өңдеу үшін файл ажыратылу болуы керек.  

### <a name="edit-in-pn_microsoft_project"></a>[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында өңдеу  

1. Негізгі мәзірден **Project Service** > **Жобалар** тармағын басыңыз.  

2. Жобалар тізімінен [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасалған жобаны ашыңыз.  

3. Таспадан **MS Project бағдарламасында ашу** пәрменін таңдаңыз. Бұл байланысқан басты файлды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашады.  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>Файлды ажырату және [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] қызметінде өңдеу  

1. Негізгі мәзірден **Project Service** > **Жобалар** тармағын басыңыз.  

2. Жобалар тізімінен [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасалған жобаны ашыңыз.  

3. Таспадан **MS Project бағдарламасынан ажырату** пәрменін таңдаңыз.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>SharePoint немесе Office топтарына жоба файлын жүктеп салу  
 Жоба файлын SharePoint бағдарламасына жүктеп салып, оны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасына арналған "Қатысты құжаттар" аймағынан табуға болады.  Әкімші SharePoint құжаттарды басқару мүмкіндігін конфигурациялауы және оны жоба нысаны үшін қосуы қажет. 

 Әрі Office Groups орнатылған болса, Project файлын [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] ішіне жүктеп салуға болады.

### <a name="upload-a-file-for-sharepoint"></a>SharePoint бағдарламасы үшін файлды жүктеп салу  

1. Негізгі мәзірден **Project Service** > **Жүктеп салу** тармағын басыңыз.  

2. **Project Service Automation жоба құжаттарына** параметрін таңдаңыз.  

3. **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашуды қосу** диалогтық терезесінде **Иә** немесе **Жоқ** параметрін таңдаңыз.  

   - **Иә** параметрін таңдасаңыз, Project Service Automation қызметінде **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** түймешігін басып, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын іске қосып, SharePoint құжаттар кітапханасынан жоба файлын жүктеуге болады.  

   - **Жоқ** параметрін таңдасаңыз, **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** түймешігінің сілтемесі істемейді.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметінде **Құжаттар** астында нақты [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасы үшін табуға болады.  

### <a name="upload-a-file-for-office-groups"></a>Файлды Office Groups үшін жүктеп салу  

1. Негізгі мәзірден **Project Service** > **Жүктеп салу** тармағын басыңыз.  

2. **Project Service Automation жоба құжаттарына** параметрін таңдаңыз.  

3. **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашуды қосу** диалогтық терезесінде **Иә** немесе **Жоқ** параметрін таңдаңыз.  

   - **Иә** параметрін таңдасаңыз, Project Service Automation қызметінде **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** түймешігін басып, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын іске қосып, SharePoint құжаттар кітапханасынан жоба файлын жүктеуге болады.  

   - **Жоқ** параметрін таңдасаңыз, **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** түймешігінің сілтемесі істемейді.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметінде **Құжаттар** астында нақты [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасы үшін табуға болады.  

## <a name="publish--your-project-as-a-template"></a>Жобаны үлгі ретінде жариялау  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіндегі жоба үлгісі ретінде сақтап, жобаны сақтауға және қайта пайдалануға болады.  Жоба үлгілері [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіндегі қайта пайдаланылатын жоба жоспарлары болып табылады. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Жоба үлгісін жасау (Project Service Automation)](../psa/create-project-template.md)  

1. **Project Service** қойыншасынан **Жариялау** > **Жаңа Project Service Automation жоба үлгісі** тармағын басыңыз.  

2. **Project Service үлгісінде жаңа жобаны жариялау** диалогтық терезесінде **Жоба үлгісінің атауы** параметрін енгізіңіз.  

3. Сонымен қатар Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметіне байланыстыру үшін **Жоба жоспарын Project Service Automation қызметіне байланыстыру** пәрменін белгілеңіз.  

4. **Жариялау** түймешігін басыңыз.  

Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне байланыстыру Project файлын басты етеді және [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] үлгісіндегі жұмыс декомпозициясының құрылымын тек оқуға арналған етіп орнатады.  Жоба жоспарына өзгерістер енгізу үшін оларды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасау және жаңартулар ретінде [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіне жариялау қажет.

## <a name="read-a-resource-loaded-schedule"></a>Ресурс жүктелген кестені оқу

Project Service Automation бағдарламасының жобасын оқығанда, ресурс күнтізбесі жұмыс үстелі клиентімен синхрондалмайды. Егер тапсырма ұзақтықтарында, үлгерімінде немесе аяқталуында айырмашылықтар болса, бұл ресурстарға және жұмыс үстелі клиентіне жобаға қолданылатын жұмыс сағаты үлгісі күнтізбесінің бірдей болмауынан болуы мүмкін.


## <a name="data-synchronization"></a>Деректерді синхрондау

Келесі кестеде деректер Project Service Automation және Microsoft Project жұмыс үстелі қондырмасы арасында синхрондалу жолы көрсетілген.

| **Нысан** | **Өріс** | **Project Service Automation бағдарламасына арналған Microsoft Project** | **Microsoft Project бағдарламасына арналған Project Service Automation** |
| --- | --- | --- | --- |
| Жоба тапсырмасы | Ақырғы күн | ● | - |
| Жоба тапсырмасы | Жоспарланған күш | ● | - |
| Жоба тапсырмасы | MS Project клиентінің идентификаторы | ● | - |
| Жоба тапсырмасы | Негізгі тапсырма | ● | - |
| Жоба тапсырмасы | Project | ● | - |
| Жоба тапсырмасы | Жоба тапсырмасы | ● | - |
| Жоба тапсырмасы | Жоба тапсырмасы атауы | ● | - |
| Жоба тапсырмасы | Ресурс бірлігі (v3.0 ішінде ұсынылмайды) | ● | - |
| Жоба тапсырмасы | Жоспарланған ұзақтық | ● | - |
| Жоба тапсырмасы | Басталу күні | ● | - |
| Жоба тапсырмасы | WBS ИД | ● | - |

| **Нысан** | **Өріс** | **Project Service Automation бағдарламасына арналған Microsoft Project** | **Microsoft Project бағдарламасына арналған Project Service Automation** |
| --- | --- | --- | --- |
| Топ мүшесі | MS Project клиентінің идентификаторы | ● | - |
| Топ мүшесі | Орын атауы | ● | - |
| Топ мүшесі | жоба | ● | ● |
| Топ мүшесі | Жоба тобы | ● | ● |
| Топ мүшесі | Ресурс бірлігі | - | ● |
| Топ мүшесі | Рөл | - | ● |
| Топ мүшесі | Жұмыс сағаттары | Синхрондалмайды | Синхрондалмайды |

| **Нысан** | **Өріс** | **Project Service Automation бағдарламасына арналған Microsoft Project** | **Microsoft Project бағдарламасына арналған Project Service Automation** |
| --- | --- | --- | --- |
| Ресурс тағайындауы | Басталу күні | ● | - |
| Ресурс тағайындауы | сағат | ● | - |
| Ресурс тағайындауы | MS Project клиентінің идентификаторы | ● | - |
| Ресурс тағайындауы | Жоспарланған жұмыс | ● | - |
| Ресурс тағайындауы | Project | ● | - |
| Ресурс тағайындауы | Жоба тобы | ● | - |
| Ресурс тағайындауы | Ресурс тағайындауы | ● | - |
| Ресурс тағайындауы | Тапсырма | ● | - |
| Ресурс тағайындауы | Аяқталу күні | ● | - |

| **Нысан** | **Өріс** | **Project Service Automation бағдарламасына арналған Microsoft Project** | **Microsoft Project бағдарламасына арналған Project Service Automation** |
| --- | --- | --- | --- |
| Жоба тапсырмасы тәуелділіктері | Жоба тапсырмасы тәуелділігі | ● | - |
| Жоба тапсырмасы тәуелділіктері | Сілтеме түрі | ● | - |
| Жоба тапсырмасы тәуелділіктері | Бастапқы тапсырма | ● | - |
| Жоба тапсырмасы тәуелділіктері | Project | ● | - |
| Жоба тапсырмасы тәуелділіктері | Кейінгі тапсырма | ● | - |

### <a name="see-also"></a>Сонымен қатар келесіні қараңыз:  
 [Жоба менеджерінің нұсқаулығы](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]