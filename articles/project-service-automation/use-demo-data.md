---
title: Көрсетілім деректерімен эксперимент жасау
description: Project Service Automation бағдарламасының демо деректерін жүктеп алу және пайдалану әдісі
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: b195e5c8-63bc-4e90-914c-f29b8d565942
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 76dd5ff14cbafbfc5341885f0469a6e3e71dd66f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753099"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="35ef5-103">Демо деректермен эксперимент өткізу (Project Service)</span><span class="sxs-lookup"><span data-stu-id="35ef5-103">Experiment with demo data (Project Service)</span></span>

<span data-ttu-id="35ef5-104">Dynamics 365 Project Service Automation бағдарламасымен танысу үшін, алдын ала конфигурацияланған ортаны зерттеу пайдалы болып табылады.</span><span class="sxs-lookup"><span data-stu-id="35ef5-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="35ef5-105">Бұл мақсатта біз осы шешімдер туралы білуді жеңілдететін бөлек үлгі деректерді орнату бумасын (қазіргі уақытта тек ағылшын тілінде) жасадық.</span><span class="sxs-lookup"><span data-stu-id="35ef5-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="35ef5-106">Орнату бумасы [Microsoft Қотару Орталығы](https://go.microsoft.com/fwlink/?linkid=859966) сайтында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="35ef5-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="35ef5-107">Package Deployer құралын орнатуды орындау мына әрекеттерді орындайды:</span><span class="sxs-lookup"><span data-stu-id="35ef5-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="35ef5-108">Project Service әрекетін анықтайтын әдепкі параметрлерді жасайды немесе орнатады</span><span class="sxs-lookup"><span data-stu-id="35ef5-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="35ef5-109">Тапсырыс беруге болатын ресурстар, рөлдер, сатылым және құн бағатізбелері, ұйымдық бірліктер, қатысты сату процесінің жазбалары, жұмысқа тапсырыстар және жобалар сияқты үлгі деректерді импорттайды</span><span class="sxs-lookup"><span data-stu-id="35ef5-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="35ef5-110">**Демо деректерді жоюдың жолы жоқ.**</span><span class="sxs-lookup"><span data-stu-id="35ef5-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="35ef5-111">Сондықтан бұл буманы тек көрсетілім, бағалау, оқыту және сынақ жүйелерінде пайдалану керек.</span><span class="sxs-lookup"><span data-stu-id="35ef5-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="35ef5-112">Қосымша ақпаратты мына [блогта](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data) қараңыз.</span><span class="sxs-lookup"><span data-stu-id="35ef5-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="35ef5-113">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="35ef5-113">See Also</span></span>  
 <span data-ttu-id="35ef5-114">[Әкімші нұсқаулығы](../project-service/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="35ef5-114">[Administrator Guide](../project-service/admin-guide.md) </span></span>  
 <span data-ttu-id="35ef5-115">[Тіркелгі менеджерінің нұсқаулығы](../project-service/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="35ef5-115">[Account Manager Guide](../project-service/account-manager-guide.md) </span></span>  
 <span data-ttu-id="35ef5-116">[Жоба менеджерінің нұсқаулығы](../project-service/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="35ef5-116">[Project Manager Guide](../project-service/project-manager-guide.md) </span></span>  
 <span data-ttu-id="35ef5-117">[Ресурстар менеджерінің нұсқаулығы](../project-service/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="35ef5-117">[Resource Manager Guide](../project-service/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="35ef5-118">Уақыт, шығындар және бірлескен жұмыс нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="35ef5-118">Time, Expense, and Collaboration Guide</span></span>](../project-service/time-expense-collaboration-guide.md)
