---
title: Microsoft Project бағдарламасында жұмысты Project Service қондырмасы көмегімен жоспарлаңыз
description: Бұл тақырыпта Microsoft Project Service үшін Microsoft Project қондырмасын пайдалану жолы туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 01/07/2021
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
ms.openlocfilehash: 87387ff870a7ef3ed0689f4ae38daad8cf220b46
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145950"
---
# <a name="plan-your-work-in-microsoft-project-with-the-project-service-add-in"></a>Microsoft Project бағдарламасында жұмысты Project Service қондырмасы көмегімен жоспарлаңыз

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3x](../includes/cc-applies-to-psa-app-3x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесі болжамдарды қоса жоба жоспарлауын орындауды жеңілдетеді. Соңғы ұсыныс жіберілген кезде құн, әрекет және сатылым мәндерінің анық болуы үшін жұмысты анықтауға болады.  

[!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] жүйесін орнатуға және жоспарлау жұмысын [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасының таныс ортасында орындауға болады. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасының күшті жоспарлау мен басқару мүмкіндіктерін пайдаланып, жоба жоспарын Project Service Automation қызметінде жаңартыңыз.  

> [!IMPORTANT]
> - [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобалары үшін [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлдарын сақтау мақсатында SharePoint құжаттарды басқару мүмкіндігін пайдалану үшін, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] әкімшісі құжаттарды басқару мүмкіндігін іске қосуы керек. 
> - [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] тек [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition нұсқасымен үйлесімді.  

## <a name="download-and-install-the-add-in"></a>Қосылатын модульді жүктеп алу және орнату  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне кіру ақпаратын дайындап қойыңыз. Осы ақпарат [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасынан [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне қосылу үшін қажет.  

1.  Жүктеп алу орталығынан Project Service бағдарламасының [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) немесе [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956) қолдау көрсетілетін нұсқасы үшін қондырманы жүктеп алыңыз.  

2.  Жүктеп алу сілтемесін таңдаңыз.  

3.  Жүктеп алу аяқталған кезде қондырманы орнату үшін **Иә** параметрін таңдаңыз.  

## <a name="configure-the-add-in"></a>Қосылатын модульді конфигурациялау  

1. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын ашыңыз және **Project Service** қойыншасын таңдаңыз.  

2. **Қосылу** опциясын таңдаңыз.  

3. Жүйеге кіру ақпаратын енгізіп, **Кіру** пәрменін таңдаңыз.  

   Енді қосылатын модуль пайдалануын бастауға болады.  

## <a name="read-from-a-template"></a>Үлгіден оқу  
 Жобаны жоспарлауды бастау үшін [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішінде жасалған және [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасына көшірілген үлгіден оқыңыз. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Жоба үлгісін жасау (Project Service Automation)](../psa/create-project-template.md)  

1.  **Project Service** қойыншасынан **Оқу** > **Project Service Automation жоба үлгісі** тармағын таңдаңыз.  

2.  Тізімнен жоба үлгісін таңдап, **Ашу** пәрменін таңдаңыз.  

    > [!NOTE]
    >  Әдепкі бойынша, үлгіден Project бағдарламасына көшірілген тапсырмалар қолмен жоспарланған ретінде орнатылады.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>Жоба ресурстарына [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] рөлдерін белгілеу  

1.  Жобаны ашыңыз және **Тапсырма** таспасын таңдаңыз.  

2. **Гант диаграммасы** мәзірін таңдап, **Ресурс парағы** параметрін таңдаңыз.  

3. Ресурс парағында **Project Service ресурс рөлі** ашылмалы мәзірін таңдап, Project Service Automation рөлін таңдаңыз.  

## <a name="staff-your-project-with-resources"></a>Жобаны ресурстармен жабдықтау  

1.  Project Service қойыншасынан жолды таңдаңыз және **Ресурстар табу** пәрменін таңдаңыз.  

2.  **Ресурсты тіркеу** экранында жобаға пайдалану қажет ресурсты таңдаңыз.  

3.  **Тапсырыс беру** пәрменін таңдаңыз, содан кейін **OK** пәрменін таңдаңыз.  

## <a name="publish-your-project"></a>Жобаны жариялау  
Жоба жоспарлауы аяқталған кезде келесі қадам жобаны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне импорттау және жариялау болады.  

Жоба [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне импортталады. Бағалар және топ жасау процесі қолданылады. Топтың, жоба болжамдарының және жұмыс декомпозициясы құрылымының жасалғанын көру үшін жобаны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесінде ашыңыз. Төмендегі кестеде нәтижелерді табатын жер көрсетілген.


|              Microsoft Project                                                           |                      Project Service Automation                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Гант диаграммасы**   | [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жұмыс декомпозициясының құрылымы** экранына импорттайды. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Ресурс парағы** |   [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жоба тобы мүшелері** экранына импорттайды.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Пайдалану пайдалану**    |    [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Жоба болжамдары** экранына импорттайды.     |

**Жобаны импорттау және жариялау үшін**  
1. **Project Service** қойыншасынан **Жариялау** > **Жаңа Project Service Automation жобасы** тармағына өтіңіз.  

2. **Project Service қызметіндегі жаңа жобаға жариялау** диалогтік терезесінде **Жоба атауы** мәнін енгізіңіз және **Тұтынушы** параметрін таңдаңыз.  

3. Сонымен қатар жоспардың жоба файлын Project Service Automation қызметіне байланыстыру үшін **Жоба жоспарын Project Service Automation қызметіне байланыстыру** пәрменін таңдаңыз.  

4. **Жариялау** пәрменін таңдаңыз.  

   Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне байланыстыру Project файлын басты етеді және [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіндегі жұмыс декомпозициясының құрылымын тек оқуға арналған етіп орнатады.  Жоба жоспарына өзгерістер енгізу үшін оларды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасау және жаңартулар ретінде [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіне жариялау қажет.  

## <a name="edit-a-project-thats-been-imported"></a>Импортталған жобаны өңдеу  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметіне импортталған жоба жоспарына өзгерістер енгізу үшін екі таңдау бар:  

- Басты файлды ашып, оны [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында өңдеңіз.  

- Файлды ажыратыңыз және оны тікелей Project Service қызметінде өңдеңіз. Әдепкі бойынша, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ішінен жүктеп салынған жоба құлыпталады және оны тек Project бағдарламасында өңдеуге болады. Файлды [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішінде өңдеу үшін файл ажыратылу болуы керек.  

### <a name="edit-in-pn_microsoft_project"></a>[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында өңдеу  

1. Негізгі мәзірден **Project Service** > **Жобалар** тармағына өтіңіз.  

2. Жобалар тізімінен [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасаған жобаны ашыңыз.  

3. Таспадан **MS Project бағдарламасында ашу** пәрменін таңдаңыз. Бұл байланысқан басты файлды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашады.  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>Файлды ажырату және [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] қызметінде өңдеу  

1. Негізгі мәзірден **Project Service** > **Жобалар** тармағына өтіңіз.  

2. Жобалар тізімінен [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасаған жобаны ашыңыз.  

3. Таспадан **MS Project бағдарламасынан ажырату** пәрменін таңдаңыз.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>SharePoint немесе Office топтарына жоба файлын жүктеп салу  
 Жоба файлын SharePoint бағдарламасына жүктеп салып, оны [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасына арналған "Қатысты құжаттар" аймағынан табуға болады.  Әкімші SharePoint құжаттарды басқару мүмкіндігін конфигурациялауы және оны жоба нысаны үшін қосуы қажет. 

 Әрі Office Groups орнатылған болса, Project файлын [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] ішіне жүктеп салуға болады.

### <a name="upload-a-file-for-sharepoint"></a>SharePoint бағдарламасы үшін файлды жүктеп салу  

1. Негізгі мәзірден **Project Service** > **Жүктеп салу** тармағына өтіңіз.  

2. **Project Service Automation жоба құжаттарына** параметрін таңдаңыз.  

3. **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашуды қосу** диалогтік терезесінде **Иә** немесе **Жоқ** параметрін таңдаңыз.  

   - **Иә** параметрін таңдасаңыз, Project Service Automation қызметінде **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** параметрін таңдауға [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын іске қосып, SharePoint құжат кітапханасынан жоба файлын жүктеуге болады.  

   - **Жоқ** параметрін таңдасаңыз, **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** параметрі жұмыс істемейді.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметінде **Құжаттар** астында нақты [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасы үшін табуға болады.  

### <a name="upload-a-file-for-office-groups"></a>Файлды Office Groups үшін жүктеп салу  

1. Негізгі мәзірден **Project Service** > **Жүктеп салу** тармағына өтіңіз.  

2. **Project Service Automation жоба құжаттарына** параметрін таңдаңыз.  

3. **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашуды қосу** диалогтік терезесінде **Иә** немесе **Жоқ** параметрін таңдаңыз.  

   - **Иә** параметрін таңдасаңыз, Project Service Automation қызметінде **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** параметрін таңдауға, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасын іске қосып, SharePoint құжат кітапханасынан жоба файлын жүктеуге болады.  

   - **Жоқ** параметрін таңдасаңыз, **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында ашу** параметрі жұмыс істемейді.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметінде **Құжаттар** астында нақты [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жобасы үшін табуға болады.  

## <a name="publish--your-project-as-a-template"></a>Жобаны үлгі ретінде жариялау  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіндегі жоба үлгісі ретінде сақтап, жобаны сақтауға және қайта пайдалануға болады. Жоба үлгілері [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіндегі қайта пайдаланылатын жоба жоспарлары болып табылады. Қосымша ақпарат алу үшін [Жоба үлгісін жасау (Project Service Automation)](../psa/create-project-template.md) тармағын қараңыз. 

1. **Project Service** қойыншасынан **Жариялау** > **Жаңа Project Service Automation жоба үлгісі** тармағына өтіңіз.  

2. **Project Service үлгісінде жаңа жобаны жариялау** диалогтік терезесінде **Жоба үлгісінің атауы** параметрін енгізіңіз.  

3. Сонымен қатар жоспардың Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] қызметіне байланыстыру үшін **Жоба жоспарын Project Service Automation қызметіне байланыстыру** пәрменін таңдаңыз.  

4. **Жариялау** пәрменін таңдаңыз.  

Project файлын [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесіне байланыстыру Project файлын басты етеді және [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] үлгісіндегі жұмыс декомпозициясының құрылымын тек оқуға арналған етіп орнатады.  Жоба жоспарына өзгерістер енгізу үшін оларды [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] бағдарламасында жасау және жаңартулар ретінде [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ішіне жариялау қажет.

## <a name="read-a-resource-loaded-schedule"></a>Ресурс жүктелген кестені оқу

Project Service Automation бағдарламасының жобасын оқығанда, ресурс күнтізбесі жұмыс үстелі клиентімен синхрондалмайды. Егер тапсырма ұзақтықтарында, үлгерімінде немесе аяқталуында айырмашылықтар болса, бұл ресурстарға және жұмыс үстелі клиентіне жобаға қолданылатын жұмыс сағаты үлгісі күнтізбесінің бірдей болмауынан болуы мүмкін.


## <a name="data-synchronization"></a>Деректерді синхрондау
Осы бөлімдегі кестелерде Project Service Automation қызметі мен Microsoft Project жұмыс үстелі қондырмасы арасында нысан деректерін синхрондау туралы ақпарат берілген.

### <a name="project-task-entity-table"></a>Жоба тапсырмасының нысан кестесі
Келесі кестеде жоба тапсырмасының нысан деректерінің Project Service Automation қызметі мен Microsoft Project жұмыс үстелі қондырмасы арасында синхрондалу жолы көрсетілген.

| **Нысан** | **Өріс** | **Project Service Automation бағдарламасына арналған Microsoft Project** | **Microsoft Project бағдарламасына арналған Project Service Automation** |
| --- | --- | --- | --- |
| Жоба тапсырмасы | Ақырғы күн | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | Жоспарланған күш | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | MS Project клиентінің идентификаторы | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | Негізгі тапсырма | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | Project | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | Жоба тапсырмасы | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | Жоба тапсырмасы атауы | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | Ресурс бірлігі (v3.0 ішінде ұсынылмайды) | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | Жоспарланған ұзақтық | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | Басталу күні | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы | WBS ИД | Синхрондалған | Синхрондалмаған |

### <a name="team-member-entity-table"></a>Топ мүшесінің нысан кестесі
Келесі кестеде топ мүшесінің нысан деректерінің Project Service Automation қызметі мен Microsoft Project жұмыс үстелі қондырмасы арасында синхрондалу жолы көрсетілген

| **Нысан** | **Өріс** | **Project Service Automation бағдарламасына арналған Microsoft Project** | **Microsoft Project бағдарламасына арналған Project Service Automation** |
| --- | --- | --- | --- |
| Топ мүшесі | MS Project клиентінің идентификаторы | Синхрондалған | Синхрондалмаған |
| Топ мүшесі | Орын атауы | Синхрондалған | Синхрондалмаған |
| Топ мүшесі | жоба | Синхрондалған | Синхрондалған |
| Топ мүшесі | Жоба тобы | Синхрондалған | Синхрондалған |
| Топ мүшесі | Ресурс бірлігі | Синхрондалмаған | Синхрондалған |
| Топ мүшесі | Рөл | Синхрондалмаған | Синхрондалған |
| Топ мүшесі | Жұмыс сағаттары | Синхрондалмаған | Синхрондалмаған |

### <a name="resource-assignment-entity-table"></a>Ресурс тағайындауының нысан кестесі
Келесі кестеде ресурс тағайындауының нысан деректерінің Project Service Automation қызметі мен Microsoft Project жұмыс үстелі қондырмасы арасында синхрондалу жолы көрсетілген

| **Нысан** | **Өріс** | **Project Service Automation бағдарламасына арналған Microsoft Project** | **Microsoft Project бағдарламасына арналған Project Service Automation** |
| --- | --- | --- | --- |
| Ресурс тағайындауы | Басталу күні | Синхрондалған | Синхрондалмаған |
| Ресурс тағайындауы | сағат | Синхрондалған | Синхрондалмаған |
| Ресурс тағайындауы | MS Project клиентінің идентификаторы | Синхрондалған | Синхрондалмаған |
| Ресурс тағайындауы | Жоспарланған жұмыс | Синхрондалған | Синхрондалмаған |
| Ресурс тағайындауы | Project | Синхрондалған | Синхрондалмаған |
| Ресурс тағайындауы | Жоба тобы | Синхрондалған | Синхрондалмаған |
| Ресурс тағайындауы | Ресурс тағайындауы | Синхрондалған | Синхрондалмаған |
| Ресурс тағайындауы | Тапсырма | Синхрондалған | Синхрондалмаған |
| Ресурс тағайындауы | Аяқталу күні | Синхрондалған | Синхрондалмаған |

### <a name="project-task-dependencies-entity-table"></a>Жоба тапсырмасы тәуелділіктерінің нысан кестесі
Келесі кестеде жоба тапсырмасы тәуелдіктерінің нысан деректерінің Project Service Automation қызметі мен Microsoft Project жұмыс үстелі қондырмасы арасында синхрондалу жолы көрсетілген

| **Нысан** | **Өріс** | **Project Service Automation бағдарламасына арналған Microsoft Project** | **Microsoft Project бағдарламасына арналған Project Service Automation** |
| --- | --- | --- | --- |
| Жоба тапсырмасы тәуелділіктері | Жоба тапсырмасы тәуелділігі | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы тәуелділіктері | Сілтеме түрі | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы тәуелділіктері | Бастапқы тапсырма | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы тәуелділіктері | Project | Синхрондалған | Синхрондалмаған |
| Жоба тапсырмасы тәуелділіктері | Кейінгі тапсырма | Синхрондалған | Синхрондалмаған |

### <a name="additional-resources"></a>Қосымша ресурстар
 [Жоба менеджерінің нұсқаулығы](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]