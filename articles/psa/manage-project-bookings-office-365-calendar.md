---
title: Office 365 күнтізбесіндегі жобаларды және тапсырыстарды басқару
description: Office 365 күнтізбесіндегі жобаларды және тапсырыстарды басқару жолы
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: f9ebfadf8a331fd6a8a86a9cc040dc8957db3b82
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950316"
---
# <a name="manage-projects-and-bookings-in-your-calendar-project-service"></a>Күнтізбедегі жобалар мен тапсырыстарды басқару (Project Service)

> [!Note]
> ҰСЫНЫЛМАҒАН: бұл мүмкіндік ұсынылмады және енді қолжетімсіз.

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] 

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесі арқылы жеке кездесулерді, жоба жұмысының тапсырыстарын және Field Service жұмысқа тапсырыс белгілеулерін көріңіз.  
  
 Барлығы бір жерде болған кезде күніңізді басқару оңай болады. Жиналыстар, кездесулер, тапсырыстар мен тапсырмалардың барлығы [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесінде қолжетімді.  
  
 Егер [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесін пайдалансаңыз, әрі Project Service қызметінің уақытты енгізу көрінісінде жеке кездесулерді енгізуге болады. Бұл жоба және ресурс реттеушілеріне жобаға қолжетімділігіңізді білуге мүмкіндік береді. Әрі ол уақытыңызды үнемдейді, себебі жеке кездесулер туралы ақпаратты екі рет енгізу қажет емес. Жеке кездесулерді күнтізбеден Project Service қызметінің уақытты енгізу көрінісіне импорттауға болады.  
  
 Күнтізбе бүгіннен бастап алдағы төрт аптаға дейінгі жоба және жұмыс тапсырыстарын синхрондайды. Осы параметрді өзгерту мүмкін емес.  
  
 Синхрондауға тек бір жолмен қолдау көрсетіледі, ол [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесіндегі PSA автоматтандыру мүмкіндігімен. Кері тәртіпте синхрондауға болады. 
  
 [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесін пайдалану әдісін үйрену үшін [Бизнеске арналған вебтегі Outlook күнтізбесі](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936) бөлімін қараңыз.  
  
## <a name="setup"></a>Орнату  
 [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесіндегі тапсырыстарды қарау және басқару алдында бірнеше нәрсені орнату қажет.  
  
- Сізде [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] глобалдық әкімшісінің немесе жүйе әкімшісінің тіркелгі деректері болуы керек.  
  
- Әкімшіңіз электрондық пошта серверінің профилін конфигурациялауы және әрбір пайдаланушы өз пошта жәшігін конфигурациялауы қажет. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Сервер тарапында синхрондау арқылы электрондық поштаның өңделуін орнату](/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)  
  
## <a name="turn-on-synchronization-for-your-organization-admin-task"></a>Ұйымыңыз үшін синхрондауды қосу (әкімші тапсырмасы)  
  
1.  Негізгі мәзірден **Параметрлер** > **Басқару** тармағын басыңыз.  
  
2.  **Жүйелік параметрлер** түймешігін басыңыз.  
  
3.  **Синхрондау** қойыншасын басыңыз.  
  
4.  **Ресурс тапсырысының синхрондауын қосуды таңдау** астында **Ресурс тапсырысын Outlook бағдарламасымен синхрондау** пәрменін белгілеңіз.  
  
## <a name="turn-on-synchronization-for-your-user-profile-user-task"></a>Пайдаланушы профилі үшін синхрондауды қосу (пайдаланушы тапсырмасы)  
  
1.  Экранның жоғарғы оң жақ бұрышындағы **Параметрлер** түймешігін басыңыз.  
  
2.  **Опциялар** түймесін басыңыз.  
  
3.  **Синхрондау** қойыншасын басыңыз.  
  
4.  **Outlook арқылы ресурс тапсырысын синхрондау** астында **Outlook арқылы ресурс тапсырысын синхрондау** пәрменін белгілеңіз.  
  
## <a name="import-your-personal-appointments-user-task"></a>Жеке кездесулерді импорттау (пайдаланушы тапсырмасы)  
 Жеке кездесулерді күнтізбеден Project Service Automation қызметінің уақытты енгізу көрінісіне импорттауға болады.  
  
1. [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесін ашыңыз және **Деректерді импорттау** пәрменін басыңыз.  
  
2. Сүзгілер экранында **Exchange кездесулері** параметрін таңдап, **Қолдану** пәрменін таңдаңыз.  
  
3. Жүйе кездесулерді ағымдағы аптадан ұсынылған жазбалар ретінде уақыт жазбасы көрісіне жеткізеді. Басқа апта үшін жазбаларды қосу үшін **Алдыңғы** немесе **Келесі** параметрін таңдаңыз.  
  
4. Project Service Automation қызметінің уақытты енгізу көрінісіне қосу қажет кездесуді таңдаңыз.  
  
5. **Уақытты енгізу** қалқылмалы жолағында кездесуді Project Service Automation қызметінің уақытты енгізу көрінісіне түрлендірудің тиісті параметрлерін таңдаңыз.  
  
6. **Сақтау** түймешігін басыңыз.  
  
### <a name="see-also"></a>Сонымен қатар келесіні қараңыз:  
 [Уақыт, шығындар және бірлескен жұмыс нұсқаулығы](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]