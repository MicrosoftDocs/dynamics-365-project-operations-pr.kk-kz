---
title: Сіздегі орналастыру түрін анықтау
description: Бұл тақырыпта компанияңыздың жоба операцияларының тиісті орналастыру түрін анықтауға көмектесу үшін ақпарат береді.
author: stsporen
ms.date: 03/15/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ad700a84edd6c39609bc5b4f09ca74af3059a0dd
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997113"
---
# <a name="determine-your-deployment-type"></a>Сіздегі орналастыру түрін анықтау

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

> [!IMPORTANT]
> Лицензияны сатып алғаннан кейін, [Қадамдық орнату ағыны](https://aka.ms/provisionprojectoperations) арқылы Dynamics 365 Project Operations ең жақсы орналастыру үлгісін анықтау үшін осы жерден бастаңыз.
> Басқарылатын орнату ағынын аяқтағаннан кейін орнатуды аяқтау үшін тиісті басқару порталына бағытталасыз. Орнатуды аяқтау үшін орналастыру мәліметтерін қараңыз.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Dynamics 365 Project Service Automation арқылы Dynamics жүйесінің бар тұтынушылары
Project Operations жүйесі Project Service Automation көмегімен жеткізілген мүмкіндіктерді қамтиды. 2021 жылдың 1-толқынында тұтынушылар үшін жаңарту жолы шығарылады.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>Жобалық басқару және есеп бойынша Dynamics 365 Finance бар тұтынушылары 

Жобалық басқару және есеп мүмкіндіктерін пайдаланатын Finance бағдарламасының бұрыннан бар тұтынушылары оны сол күйінде пайдалана алады. [Қосалқы/өндіріс тапсырысы сценарийлеріне арналған Project Operations](#pma) қараңыз.


## <a name="deployment-regions"></a>Орналастыру аймақтары
Project Operations бағдарламасын орналастыруға қолдау көрсететін аймақтарды анықтау үшін [Dynamics 365 және Power Platform есебіне арналған географиялық қолжетімділік](https://dynamics.microsoft.com/en-us/geographic-availability/) бөлімін қараңыз. **Есепті қарау** параметрін таңдап, қолдау көрсетілетін аймақтарды көру үшін **Dynamics 365> Operations бағдарламалары > Dynamics 365 Project Operations** тармағын кеңейтіңіз.

## <a name="deployment-types"></a>Орналастыру түрлері
Project Operations сіздің қажеттіліктеріңізге сәйкес бірнеше орналастыру нұсқаларын қолдайды. Сіз Dynamics 365 жаңа немесе қолданыстағы тұтынушысы болсаңыз да, Project Operations сіздің қажеттіліктеріңізді қолдай алады.

Біздің[ Орналастыруға арналған сауалнама](https://aka.ms/provisionprojectoperations) дұрыс орналастыруды анықтауға көмектеседі. Нәтижелер сізді келесі орналастыру түрлеріне бағыттайды:

- [Жеңілдетілген орналастыру – проформа-шотын ұсыну мәмілесі](#lite)
- [Ресурс/биржадан тыс сценарийлерге арналған Project Operations](#integrated)
- [Қосалқы/өндіріс тапсырысы сценарийлеріне арналған Project Operations](#pma)

Project Operations заңды тұлға деңгейіндегі конфигурациялар арқылы бір ортада қосалқы/өндіріс тапсырыстың сценарийлерін және қосалқы емес/ресурстарға негізделген сценарийлерді қолдайды. Мысалы, Contoso қосалқы/өндірістік тапсырыстың мүмкіндіктерін АҚШ-тың өндірістік мекемесінде пайдалана алады (заңды тұлға = Contoso Америка Құрама Штаттарындағы өндірістік мекемесі). Contoso қосалқы емес/ресурстарға негізделген мүмкіндіктерді Contoso Ұлыбританиядағы Robotics Arms қызмет көрсететін мекемеде (заңды тұлға = Contoso Robotics, Ұлыбритания) пайдалана алады.

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a>Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі

Қарапайым орналастыру келесі мүмкіндіктерді қамтиды:

- Dynamics 365 Sales бағдарламасының тәжірибелерін кеңейтетін жобалардың сату үрдісі
- Вебке арналған Microsoft Project жобасын жоспарлау
- Көпөлшемді баға белгілеу
- Бірыңғай ресурстық басқару
- Уақытты бақылау
- Негізгі шығыс
- Жоба менеджерінің шолуы мен өңдеуі үшін арналған проформа шоты 

#### <a name="deployment-steps"></a>Орналастыру қадамдары
[Орналастыру бойынша сауалнама](https://aka.ms/provisionprojectoperations) көмегімен Project Operations жүйесінің ең тиімді орналастыру үлгісін анықтаңыз.

Бұл орналастыру үшін [Алдын ала қарау жазылымдарына арналған тіркелу](lite-preview-subscription-sign-up.md) және [Жаңа ортаны дайындау](lite-deployment.md) бөлімдерін қараңыз. 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a>Ресурс/биржадан тыс сценарийлерге арналған Project Operations
Ресурстық/қосалқы емес сценарийлерге арналған Project Operations жүйесі келесі мүмкіндіктерді қамтиды:
 
- Dynamics 365 Sales бағдарламасын кеңейтетін жобалардың сату үрдісі
- Вебке арналған Microsoft Project жобасын жоспарлау
- Көпөлшемді баға белгілеу
- Бірыңғай ресурстық басқару
- Уақытты бақылау
- Негізгі шығыс
- Толық шығыс
- ТҚР түбіртегі
- Проформа және тұтынушыға арналған шот-фактуралар 
- Жобалар бойынша табысты тану

#### <a name="deployment-steps"></a>Орналастыру қадамдары
[Орналастыру бойынша сауалнама](https://aka.ms/provisionprojectoperations) көмегімен Project Operations жүйесінің ең тиімді орналастыру үлгісін анықтаңыз.

Бұл орналастыру үшін [Алдын ала қарау жазылымдарына арналған тіркелу](resource-sign-up-preview-subscription.md) және [Жаңа ортаны дайындау](resource-provision-new-environment.md) бөлімдерін қараңыз. 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a>Қосалқы/өндіріс тапсырысы сценарийлеріне арналған Project Operations

- WBS бойынша жобаны жоспарлау
- Ресурстарды басқару
- Уақытты бақылау
- Толық шығыс
- ТҚР түбіртегі
- Толық шот-фактура
- Табысты тану
- Өндірістік тапсырыстар
- Қойма қамтамасыз етілген қосалқы материалдар

#### <a name="deployment-steps"></a>Орналастыру қадамдары
[Орналастыру бойынша сауалнама](https://aka.ms/provisionprojectoperations) көмегімен Project Operations жүйесінің ең тиімді орналастыру үлгісін анықтаңыз.

Бұл орналастыру үшін [Алдын ала қарау жазылымдарына арналған тіркелу](/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=%2fdynamics365%2ffinance%2ftoc.json) және [Жаңа ортаны дайындау](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=%2fdynamics365%2ffinance%2ftoc.json) бөлімдерін қараңыз. 



[!INCLUDE[footer-include](../includes/footer-banner.md)]