---
title: Project Service Automation бағдарламасын конфигурациялау
description: Project Service жүйесін теңшеу қадамдары
author: ruhercul
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
ms.openlocfilehash: fd02611b5b3133e097b2818a725b6c5d667e5ac0
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079769"
---
# <a name="configure-project-service"></a><span data-ttu-id="d5283-103">Project Service жүйесін теңшеу</span><span class="sxs-lookup"><span data-stu-id="d5283-103">Configure Project Service</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="d5283-104">Тіркелгілерді, жобаларды және ресурстарды басқаруға [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] ішіндегі [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] автоматтандыру мүмкіндіктерін пайдалану алдында ұйым қажеттіліктеріне сәйкес [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] шешімін сәйкестендіру үшін бірнеше конфигурация қадамын орындау қажет.</span><span class="sxs-lookup"><span data-stu-id="d5283-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="d5283-105">Осы қадамдарға келесілер кіреді:</span><span class="sxs-lookup"><span data-stu-id="d5283-105">These steps include:</span></span>  
  
-   <span data-ttu-id="d5283-106">[Уақыт бірліктерін реттеу](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="d5283-107">Жобаларды жоспарлау және шот ұсыну негізі ретінде пайдаланылатын өнім каталогындағы уақыт бірліктерін теңшеңіз.</span><span class="sxs-lookup"><span data-stu-id="d5283-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="d5283-108">[Валюталарды және айырбас бағамдарын реттеу](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="d5283-109">Жобаларға пайдаланылатын валюталарды орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5283-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="d5283-110">[Бөлімшелер жасау](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="d5283-111">Географиясы бойынша бизнесті, бизнес функциясын немесе басқа логикалық бөлімді бөлуге пайдаланылатын компания топтарын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5283-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="d5283-112">[Есеп-шот жиіліктерін реттеу](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="d5283-113">Клиенттерге шот ұсынуға пайдалану керек уақыт кезеңдерін орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5283-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="d5283-114">[Транзакция санаттарын конфигурациялау](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="d5283-115">Кеңесшілер шот ұсынылатын және шот ұсынылмайтын шығыстарын ала алатын транзакция санаттарын орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5283-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="d5283-116">[Шығыс санаттарын конфигурациялау](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="d5283-117">Кеңесшілер шот ұсынылатын және шот ұсынылмайтын шығыстарын ала алатын санаттарды орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5283-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="d5283-118">[Өнім каталогының элементтерін жасау](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="d5283-119">Бағдарламалық жасақтама лицензиялары сияқты сатылатын өнімдерді өнім каталогына қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5283-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="d5283-120">[Бағатізбе жасау](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="d5283-121">Жоба талап ететін әрбір рөлге арналған клиенттерден алу керек сомаға байланысты әр түрлі бағатізбелерді теңшеңіз.</span><span class="sxs-lookup"><span data-stu-id="d5283-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="d5283-122">[Ресурстарды реттеу](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="d5283-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="d5283-123">Жобаларға керек біліктіліктерді, тиімділіктерді, ресурс рөлдерін басқа ресурс ақпаратын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="d5283-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="d5283-124">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="d5283-124">See Also</span></span>  
 <span data-ttu-id="d5283-125">[Project Service Automation бағдарламасына шолу](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="d5283-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="d5283-126">[Project Service Automation бағдарламасын конфигурациялау](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="d5283-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="d5283-127">[Тіркелгі менеджерінің нұсқаулығы](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="d5283-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="d5283-128">[Жоба менеджерінің нұсқаулығы](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="d5283-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="d5283-129">[Ресурстар менеджерінің нұсқаулығы](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="d5283-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="d5283-130">Уақыт, шығындар және бірлескен жұмыс нұсқаулығы</span><span class="sxs-lookup"><span data-stu-id="d5283-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)