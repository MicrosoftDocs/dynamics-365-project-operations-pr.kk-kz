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
ms.openlocfilehash: d0bc6d171f2f3080b7b1c34222de49e93415a139
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079739"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="f27ff-103">Демо деректермен эксперимент өткізу (Project Service)</span><span class="sxs-lookup"><span data-stu-id="f27ff-103">Experiment with demo data (Project Service)</span></span>

<span data-ttu-id="f27ff-104">Dynamics 365 Project Service Automation бағдарламасымен танысу үшін, алдын ала конфигурацияланған ортаны зерттеу пайдалы болып табылады.</span><span class="sxs-lookup"><span data-stu-id="f27ff-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="f27ff-105">Бұл мақсатта біз осы шешімдер туралы білуді жеңілдететін бөлек үлгі деректерді орнату бумасын (қазіргі уақытта тек ағылшын тілінде) жасадық.</span><span class="sxs-lookup"><span data-stu-id="f27ff-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="f27ff-106">Орнату бумасы [Microsoft Қотару Орталығы](https://go.microsoft.com/fwlink/?linkid=859966) сайтында қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="f27ff-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="f27ff-107">Package Deployer құралын орнатуды орындау мына әрекеттерді орындайды:</span><span class="sxs-lookup"><span data-stu-id="f27ff-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="f27ff-108">Project Service әрекетін анықтайтын әдепкі параметрлерді жасайды немесе орнатады</span><span class="sxs-lookup"><span data-stu-id="f27ff-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="f27ff-109">Тапсырыс беруге болатын ресурстар, рөлдер, сатылым және құн бағатізбелері, ұйымдық бірліктер, қатысты сату процесінің жазбалары, жұмысқа тапсырыстар және жобалар сияқты үлгі деректерді импорттайды</span><span class="sxs-lookup"><span data-stu-id="f27ff-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="f27ff-110">**Демо деректерді жоюдың жолы жоқ.**</span><span class="sxs-lookup"><span data-stu-id="f27ff-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="f27ff-111">Сондықтан бұл буманы тек көрсетілім, бағалау, оқыту және сынақ жүйелерінде пайдалану керек.</span><span class="sxs-lookup"><span data-stu-id="f27ff-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="f27ff-112">Қосымша ақпаратты мына [блогта](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data) қараңыз.</span><span class="sxs-lookup"><span data-stu-id="f27ff-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="f27ff-113">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="f27ff-113">See Also</span></span>  
 <span data-ttu-id="f27ff-114">[Әкімші нұсқаулығы](../psa/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="f27ff-114">[Administrator Guide](../psa/admin-guide.md) </span></span>  
 <span data-ttu-id="f27ff-115">[Тіркелгі менеджерінің нұсқаулығы](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="f27ff-115">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="f27ff-116">[Жоба менеджерінің нұсқаулығы](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="f27ff-116">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="f27ff-117">[Ресурстар менеджерінің нұсқаулығы](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="f27ff-117">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="f27ff-118">Уақыт, шығындар және бірлескен жұмыс нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="f27ff-118">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)