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
ms.openlocfilehash: 1df4864ca8dbf6948ca88a7c82a6c0a676e3bd53
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5275050"
---
# <a name="manage-projects-and-bookings-in-your-calendar-project-service"></a><span data-ttu-id="83f83-103">Күнтізбедегі жобалар мен тапсырыстарды басқару (Project Service)</span><span class="sxs-lookup"><span data-stu-id="83f83-103">Manage projects and bookings in your calendar (Project Service)</span></span>

> [!Note]
> <span data-ttu-id="83f83-104">ҰСЫНЫЛМАҒАН: бұл мүмкіндік ұсынылмады және енді қолжетімсіз.</span><span class="sxs-lookup"><span data-stu-id="83f83-104">DEPRECATED: This feature has been deprecated and is no longer available.</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] 

<span data-ttu-id="83f83-105">[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесі арқылы жеке кездесулерді, жоба жұмысының тапсырыстарын және Field Service жұмысқа тапсырыс белгілеулерін көріңіз.</span><span class="sxs-lookup"><span data-stu-id="83f83-105">View personal appointments, project-work bookings, and field service work order assignments using the [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span>  
  
 <span data-ttu-id="83f83-106">Барлығы бір жерде болған кезде күніңізді басқару оңай болады.</span><span class="sxs-lookup"><span data-stu-id="83f83-106">With everything in one place, it’s easy to manage your day.</span></span> <span data-ttu-id="83f83-107">Жиналыстар, кездесулер, тапсырыстар мен тапсырмалардың барлығы [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="83f83-107">Your meetings, appointments, bookings, and tasks are all available in your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span>  
  
 <span data-ttu-id="83f83-108">Егер [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] жүйесін пайдалансаңыз, әрі Project Service қызметінің уақытты енгізу көрінісінде жеке кездесулерді енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="83f83-108">If you’re using [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you can also enter your personal appointments in the Project Service time entry view.</span></span> <span data-ttu-id="83f83-109">Бұл жоба және ресурс реттеушілеріне жобаға қолжетімділігіңізді білуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="83f83-109">This lets project and resource managers know your availability for projects.</span></span> <span data-ttu-id="83f83-110">Әрі ол уақытыңызды үнемдейді, себебі жеке кездесулер туралы ақпаратты екі рет енгізу қажет емес.</span><span class="sxs-lookup"><span data-stu-id="83f83-110">It also saves you time, because you don’t have to enter info about your personal appointments twice.</span></span> <span data-ttu-id="83f83-111">Жеке кездесулерді күнтізбеден Project Service қызметінің уақытты енгізу көрінісіне импорттауға болады.</span><span class="sxs-lookup"><span data-stu-id="83f83-111">You can simply import your personal appointments from your calendar to Project Service time entry view.</span></span>  
  
 <span data-ttu-id="83f83-112">Күнтізбе бүгіннен бастап алдағы төрт аптаға дейінгі жоба және жұмыс тапсырыстарын синхрондайды.</span><span class="sxs-lookup"><span data-stu-id="83f83-112">Your calendar will sync project and work order bookings from today to upcoming four weeks.</span></span> <span data-ttu-id="83f83-113">Осы параметрді өзгерту мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="83f83-113">This setting can’t be changed.</span></span>  
  
 <span data-ttu-id="83f83-114">Синхрондауға тек бір жолмен қолдау көрсетіледі, ол [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесіндегі PSA автоматтандыру мүмкіндігімен.</span><span class="sxs-lookup"><span data-stu-id="83f83-114">Syncing is only supported one way, from PSA to your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span> <span data-ttu-id="83f83-115">Кері тәртіпте синхрондауға болады.</span><span class="sxs-lookup"><span data-stu-id="83f83-115">You can sync in the reverse order.</span></span> 
  
 <span data-ttu-id="83f83-116">[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесін пайдалану әдісін үйрену үшін [Бизнеске арналған вебтегі Outlook күнтізбесі](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936) бөлімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-116">To learn how to use your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar, see [Calendar in Outlook on the web for business](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936).</span></span>  
  
## <a name="setup"></a><span data-ttu-id="83f83-117">Орнату</span><span class="sxs-lookup"><span data-stu-id="83f83-117">Setup</span></span>  
 <span data-ttu-id="83f83-118">[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесіндегі тапсырыстарды қарау және басқару алдында бірнеше нәрсені орнату қажет.</span><span class="sxs-lookup"><span data-stu-id="83f83-118">Before you can see and manage your bookings on your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar, you need to set a few things up.</span></span>  
  
- <span data-ttu-id="83f83-119">Сізде [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] глобалдық әкімшісінің немесе жүйе әкімшісінің тіркелгі деректері болуы керек.</span><span class="sxs-lookup"><span data-stu-id="83f83-119">You will need to have [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] Global Administrator or System Administrator credentials.</span></span>  
  
- <span data-ttu-id="83f83-120">Әкімшіңіз электрондық пошта серверінің профилін конфигурациялауы және әрбір пайдаланушы өз пошта жәшігін конфигурациялауы қажет.</span><span class="sxs-lookup"><span data-stu-id="83f83-120">Your Admin will need to configure the email server profile and each user will need to configure their mailbox.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="83f83-121">[Сервер тарапында синхрондау арқылы электрондық поштаның өңделуін орнату](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)</span><span class="sxs-lookup"><span data-stu-id="83f83-121">[Set up email processing through server-side synchronization](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)</span></span>  
  
## <a name="turn-on-synchronization-for-your-organization-admin-task"></a><span data-ttu-id="83f83-122">Ұйымыңыз үшін синхрондауды қосу (әкімші тапсырмасы)</span><span class="sxs-lookup"><span data-stu-id="83f83-122">Turn on synchronization for your organization (admin task)</span></span>  
  
1.  <span data-ttu-id="83f83-123">Негізгі мәзірден **Параметрлер** > **Басқару** тармағын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-123">From the main menu, click **Settings** > **Administration**.</span></span>  
  
2.  <span data-ttu-id="83f83-124">**Жүйелік параметрлер** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-124">Click **System Settings**.</span></span>  
  
3.  <span data-ttu-id="83f83-125">**Синхрондау** қойыншасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-125">Click the **Synchronization** tab.</span></span>  
  
4.  <span data-ttu-id="83f83-126">**Ресурс тапсырысының синхрондауын қосуды таңдау** астында **Ресурс тапсырысын Outlook бағдарламасымен синхрондау** пәрменін белгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="83f83-126">Under **Select whether to enable syncing of resource booking with**, check the **Synchronize resource booking with Outlook**.</span></span>  
  
## <a name="turn-on-synchronization-for-your-user-profile-user-task"></a><span data-ttu-id="83f83-127">Пайдаланушы профилі үшін синхрондауды қосу (пайдаланушы тапсырмасы)</span><span class="sxs-lookup"><span data-stu-id="83f83-127">Turn on synchronization for your user profile (user task)</span></span>  
  
1.  <span data-ttu-id="83f83-128">Экранның жоғарғы оң жақ бұрышындағы **Параметрлер** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-128">Click the **Settings** button in the upper-right corner of the screen.</span></span>  
  
2.  <span data-ttu-id="83f83-129">**Опциялар** түймесін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-129">Click **Options**.</span></span>  
  
3.  <span data-ttu-id="83f83-130">**Синхрондау** қойыншасын басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-130">Click the **Synchronization** tab.</span></span>  
  
4.  <span data-ttu-id="83f83-131">**Outlook арқылы ресурс тапсырысын синхрондау** астында **Outlook арқылы ресурс тапсырысын синхрондау** пәрменін белгілеңіз.</span><span class="sxs-lookup"><span data-stu-id="83f83-131">Under **Resource booking sync with Outlook**, check the **Synchronization resource booking with Outlook**.</span></span>  
  
## <a name="import-your-personal-appointments-user-task"></a><span data-ttu-id="83f83-132">Жеке кездесулерді импорттау (пайдаланушы тапсырмасы)</span><span class="sxs-lookup"><span data-stu-id="83f83-132">Import your personal appointments (user task)</span></span>  
 <span data-ttu-id="83f83-133">Жеке кездесулерді күнтізбеден Project Service Automation қызметінің уақытты енгізу көрінісіне импорттауға болады.</span><span class="sxs-lookup"><span data-stu-id="83f83-133">You can import your personal appointments from your calendar to Project Service Automation time entry view.</span></span>  
  
1. <span data-ttu-id="83f83-134">[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] күнтізбесін ашыңыз және **Деректерді импорттау** пәрменін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-134">Open [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar and click **Import Data**.</span></span>  
  
2. <span data-ttu-id="83f83-135">Сүзгілер экранында **Exchange кездесулері** параметрін таңдап, **Қолдану** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-135">On the Filters screen, select **Appointments from Exchange** and then click **Apply**.</span></span>  
  
3. <span data-ttu-id="83f83-136">Жүйе кездесулерді ағымдағы аптадан ұсынылған жазбалар ретінде уақыт жазбасы көрісіне жеткізеді.</span><span class="sxs-lookup"><span data-stu-id="83f83-136">The system will pull appointments into time entry view as suggested entries from the current week.</span></span> <span data-ttu-id="83f83-137">Басқа апта үшін жазбаларды қосу үшін **Алдыңғы** немесе **Келесі** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-137">To add entries for another week, click **Previous** or **Next**.</span></span>  
  
4. <span data-ttu-id="83f83-138">Project Service Automation қызметінің уақытты енгізу көрінісіне қосу қажет кездесуді таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-138">Select the appointment that you want to add to Project Service Automation time entry view.</span></span>  
  
5. <span data-ttu-id="83f83-139">**Уақытты енгізу** қалқылмалы жолағында кездесуді Project Service Automation қызметінің уақытты енгізу көрінісіне түрлендірудің тиісті параметрлерін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-139">On the **Time Entry** popup box, select the appropriate options to convert the appointment to a Project Service Automation time entry view.</span></span>  
  
6. <span data-ttu-id="83f83-140">**Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83f83-140">Click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="83f83-141">Сонымен қатар келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="83f83-141">See Also</span></span>  
 [<span data-ttu-id="83f83-142">Уақыт, шығындар және бірлескен жұмыс нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="83f83-142">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]