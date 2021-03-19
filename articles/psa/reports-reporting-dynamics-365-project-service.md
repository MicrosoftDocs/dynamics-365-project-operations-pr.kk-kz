---
title: Есеп беру басты беті
description: Бұл тақырыпта Dynamics 365 Project Service Automation бағдарламасындағы есеп беру туралы ақпарат берілген.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: 78c62f69c6529669789a461f1ded8e3ea5f8219e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283285"
---
# <a name="reporting-home-page"></a><span data-ttu-id="19bf6-103">"Есептер" басты беті</span><span class="sxs-lookup"><span data-stu-id="19bf6-103">Reporting home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="19bf6-104">Microsoft Dynamics 365 Project Service Automation жобаға негізделген ұйымдарға жеке бизнес операцияларын тиімді басқаруға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="19bf6-104">Microsoft Dynamics 365 Project Service Automation lets project-based organizations efficiently manage the operations of their business.</span></span> <span data-ttu-id="19bf6-105">Кез келген жоба бойынша топ мүшелері мүмкіндікті басқаруы, жұмыс бағасын ұсынуы және жоспарлауы, жобаларды ресурспен қамтамасыз етуі, жұмысты жоспарға сәйкес басқаруы, жұмыс үшін есеп-шот ұсынуы, содан кейін жобаны аяқтау үшін жұмысты орындауы керек.</span><span class="sxs-lookup"><span data-stu-id="19bf6-105">On any project, team members must manage the opportunity, quote and plan the work, resource the projects, manage the work according to the plan, bill for the work, and then do the work to complete the project.</span></span> <span data-ttu-id="19bf6-106">Операциялар туралы есеп беру мүмкіндігі ұйымның күйін анықтауға және қажет болатын түзету шараларын қабылдауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="19bf6-106">The ability to report on operations is key to determining the health of the organization and taking any corrective action that's required.</span></span> <span data-ttu-id="19bf6-107">PSA бағдарламасындағы есеп беру мүмкіндігі үшін Microsoft Dynamics 365 есеп берудің әдістері мен технологиялары қолданылады.</span><span class="sxs-lookup"><span data-stu-id="19bf6-107">PSA uses Microsoft Dynamics 365 reporting methods and technologies for all its reporting.</span></span> <span data-ttu-id="19bf6-108">Есеп берудің нұсқалары туралы қосымша ақпаратты [Dynamics 365 Customer Engagement (on-premises) 9 нұсқасына арналған есепті жазу нұсқаулығы](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365) мақаласынан қараңыз.</span><span class="sxs-lookup"><span data-stu-id="19bf6-108">For more information about the options for reporting, see the [Report writing guide for Dynamics 365 Customer Engagement (on-premises), version 9](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span></span>

## <a name="report-wizard"></a><span data-ttu-id="19bf6-109">Есептер шебері</span><span class="sxs-lookup"><span data-stu-id="19bf6-109">Report Wizard</span></span>

<span data-ttu-id="19bf6-110">Есептер шебері әзірлеушілер емес пайдаланушыларға қарапайым есептерді құруға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="19bf6-110">The Report Wizard lets non-developers create simple reports.</span></span> <span data-ttu-id="19bf6-111">Бағдарлама қолданыстағы платформада жасалғандықтан, тәжірибе [Есептер шеберін пайдаланып есеп жасау немесе өңдеу](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard) бөлімінде құжатталған тәжірибемен бірдей болады.</span><span class="sxs-lookup"><span data-stu-id="19bf6-111">Because the app is built on an existing platform, the experience is the same as the experience that is documented in [Create or edit a report using the Report Wizard](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span></span> <span data-ttu-id="19bf6-112">Алайда, Project Service Automation бағдарламасына тән нысандарды қолдана алатын боласыз.</span><span class="sxs-lookup"><span data-stu-id="19bf6-112">However, you will use the Project Service Automation-specific entities.</span></span>

## <a name="custom-sql-server-reporting-services-reports"></a><span data-ttu-id="19bf6-113">SQL Server Reporting Services реттелетін есептері</span><span class="sxs-lookup"><span data-stu-id="19bf6-113">Custom SQL Server Reporting Services reports</span></span>

<span data-ttu-id="19bf6-114">Егер бизнесіңіз есептер шебері көмегімен жасау мүмкін емес нақты есепті қажет етсе, реттелетін есепті жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="19bf6-114">If your business requires a specific report that can't be created by using the Report Wizard, you can create a custom report.</span></span> <span data-ttu-id="19bf6-115">Сәйкес Microsoft SQL Server Data Tools және есептерді жасау модульдерімен бірге Microsoft Visual Studio орнатылған болуы керек.</span><span class="sxs-lookup"><span data-stu-id="19bf6-115">You must have Microsoft Visual Studio installed, together with the appropriate Microsoft SQL Server Data Tools and Report Authoring Extensions.</span></span> <span data-ttu-id="19bf6-116">Құралдар мен нұсқалар туралы қосымша ақпаратты [SQL Server Data Tools арқылы есептер жазу ортасы](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="19bf6-116">For more information about tools and versions, see [Report writing environment using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span></span> <span data-ttu-id="19bf6-117">Реттелетін есепті жасау жолы туралы ақпаратты [SQL Server Data Tools көмегімен жаңа есепті жасау](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools) бөлімінен қараңыз.</span><span class="sxs-lookup"><span data-stu-id="19bf6-117">For information about how to create a custom report, see [Create a new report using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span></span>

## <a name="power-bi-insights-apps"></a><span data-ttu-id="19bf6-118">Power BI аналитикалық деректер бағдарламалары</span><span class="sxs-lookup"><span data-stu-id="19bf6-118">Power BI insights apps</span></span>

<span data-ttu-id="19bf6-119">Microsoft Power BI және Dynamics 365 сізге деректермен аналитикалық деректер бағдарламалары түрінде жұмыс істеудің керемет әдісін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="19bf6-119">Together, Microsoft Power BI and Dynamics 365 give you a powerful way to work with your data, in the form of insights apps.</span></span> <span data-ttu-id="19bf6-120">Аналитикалық деректер бағдарламаларының қолжетімділігі туралы ақпаратты [Power BI аналитикалық деректер бағдарламалары бетінен](https://powerbi.microsoft.com/power-bi-insights-apps/) қараңыз.</span><span class="sxs-lookup"><span data-stu-id="19bf6-120">For information about the availability of insights apps, see the [Power BI insights apps page](https://powerbi.microsoft.com/power-bi-insights-apps/).</span></span>


## <a name="additional-resources"></a><span data-ttu-id="19bf6-121">Қосымша ресурстар</span><span class="sxs-lookup"><span data-stu-id="19bf6-121">Additional resources</span></span>
<span data-ttu-id="19bf6-122">PSA бағдарламасында есеп беру туралы қосымша ақпарат алу үшін келесі тақырыптарды қараңыз:</span><span class="sxs-lookup"><span data-stu-id="19bf6-122">For more information about reporting in PSA, see the following topics:</span></span>

- [<span data-ttu-id="19bf6-123">Project Service деректер үлгісімен жұмыс істеу</span><span class="sxs-lookup"><span data-stu-id="19bf6-123">Working with the Project Service data model</span></span>](reports-working-project-service-data-model.md)
- [<span data-ttu-id="19bf6-124">Бақылау тақталары</span><span class="sxs-lookup"><span data-stu-id="19bf6-124">Dashboards</span></span>](reports-dashboards.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]