---
title: Жоба менеджерінің нұсқаулығы
description: Project Service жүйесімен жобаны басқару нұсқаулығы
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0e8ffb5c-b1ee-4b37-b4f0-3888c1d4e199
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: a3d28bcbdf7209a4c5b6042591e23220ec24c21f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753151"
---
# <a name="project-manager-guide-project-service"></a>Жобаны басқару нұсқаулығы (Project Service)

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] жүйесіндегі [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] мүмкіндіктері жобаның баға ұсыныстарын және келісім-шарттарын жасауға және келісім-шартты жеңіп алғаннан кейін клиенттердің жобаларын жасауға және басқаруға көмектеседі. Сонымен қатар, олар аналитиктерге жобалар ықтимал және табысты екендігін көрсетеді. Жобаларды, материалдарды немесе бекітілген бағалы негізде орнатуға болады.  
  
 Жобаны басқару құралдары мыналар бойынша көмектеседі:  
  
-   Жұмысты тиімді бағалау  
  
-   Жобалар үдерістер тізбегінде болған кездегі болжалды ресурс талаптары  
  
-   Топ мүшелерінің жобаларда бірлесіп жұмыс істеуіне және ағымдағы әрі дәл жоба күйін барлық уақытта сақтауға мүмкіндік беру  
  
-   Әрбір істі сәтті ету үшін ықтимал қауіптерді пробелсенді түрде анықтап, шешіңіз.  
  
Бұл нұсқаулық жобаларды жасау және басқару үшін қажетті ақпаратты қамтамасыз етеді:  
  
-   [Сатылым процесі барысында жоба үшін жұмыс болжамдарын қамтамасыз ету](../project-service/provide-estimates-project-during-sales-process.md)  
  
-   [Жоба жасау](../project-service/create-project.md)  
  
-   [Microsoft Project бағдарламасында жұмысты жоспарлау үшін Project Service Automation қондырмасын пайдалану](../project-service/add-plan-work-microsoft-project.md)  
  
-   [Жұмыс декомпозициясының құрылымымен жобаны жоспарлау](../project-service/schedule-project-work-breakdown-structure.md)  
  
-   [Жоба құнын және табыс болжамдарын анықтау](../project-service/determine-project-cost-revenue-estimates.md)  
  
-   [Жобаның орындалу барысын және құнын бақылау](../project-service/track-project-progress-cost.md)  
  
-   [Жоба үлгісін жасау](../project-service/create-project-template.md)  
  
-   [Ресурс сұрауларын жіберу](../project-service/submit-resource-requests.md)  
  
-   [Жоба үшін Office 365 тобын жасау](../project-service/create-office-365-group-project.md)  
  
-   [Жобаға құжаттар қосу](../project-service/add-documents-project.md)  
  
-   [Жоба күйін бақылау](../project-service/track-project-status.md)  
  
-   [Жоба тобы мүшелерін көру және тапсырыстарды басқару](../project-service/view-project-team-members-manage-bookings.md)  
  
-   [Жоба болжамдарын көру және өңдеу](../project-service/view-edit-project-estimates.md)  
  
-   [Уақытты және шығыстарды бекіту](../project-service/approve-time-expenses.md)  
  
-   [Жобаның нақты мәндерін қарап шығу](../project-service/review-project-actuals.md)  
  
-   [Есеп-шоттарды көру және жіберу](../project-service/view-send-invoices.md)  
  
-   [Бақылау тақталары мен есептерді көру](../project-service/view-dashboards-reports.md)  
  
## <a name="prerequisites"></a>Алғышарттар  
 Егер әлдеқашан болмасаңыз, жобаларды жасауды бастау алдында келесі элементтерді орындау керек:  
  
-   [Жұмыс сағаттары үлгісін жасау](../project-service/create-work-hours-template.md). Кестедегі әр күн бойынша жұмыс сағаттары санын анықтайтын жоба күнтізбесін және қызмет есептейтін күндерді орнатыңыз.  
  
-   [Бағатізбе жасау](../project-service/create-price-list.md). Ұйымдағы ресурс рөлдерінің құн және сатылым бағаларын шығыстар мен өнімдер сияқты басқа санаттар үшін орнатыңыз.  
  
-   [Ресурс рөлдерін қосу](../project-service/add-resource-roles.md). Ресурс талаптарын және жоба құндарын анықтауға көмектесетін рөлдерді анықтаңыз.  
  
### <a name="see-also"></a>Сонымен қатар, келесіні қараңыз:  
 [Project Service бағдарламасына шолу](../project-service/overview.md)   
 [Әкімші нұсқаулығы](../project-service/admin-guide.md)   
 [Тіркелгі менеджерінің нұсқаулығы](../project-service/account-manager-guide.md)   
 [Ресурстар менеджерінің нұсқаулығы](../project-service/resource-manager-guide.md)   
 [Уақыт, шығындар және бірлескен жұмыс нұсқаулығы](../project-service/time-expense-collaboration-guide.md)

