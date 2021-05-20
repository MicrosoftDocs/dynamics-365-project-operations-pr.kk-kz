---
title: Жұмыс уақыты үлгілерін жасау
description: Бұл тақырыпта Project Service қызметінде жұмыс сағаттарының үлгісін жасау жолдары сипатталады.
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
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 525f601ad6fee902cb6d5c128b596cc2d33f30c4
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981262"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="5af99-103">Жұмыс сағаттары үлгісін жасау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="5af99-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="5af99-104">Жобаны жасап, басқару үшін жобаға күнтізбелік үлгіні қолдану қажет.</span><span class="sxs-lookup"><span data-stu-id="5af99-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="5af99-105">Күнтізбе үлгісі келесі жоба төлсипаттарын анықтайды:</span><span class="sxs-lookup"><span data-stu-id="5af99-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="5af99-106">Жұмыс сағаттары, оның ішінде басталу және аяқталу уақыты</span><span class="sxs-lookup"><span data-stu-id="5af99-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="5af99-107">Жұмыс күндері</span><span class="sxs-lookup"><span data-stu-id="5af99-107">Working days</span></span>
- <span data-ttu-id="5af99-108">Жұмыс емес күндер секілді күнтізбелік ерекшеліктер</span><span class="sxs-lookup"><span data-stu-id="5af99-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="5af99-109">Жобаға қолданылатын күнтізбе үлгісі - бұл сіздің ұйымыңыздың параметрлерінде анықталған күнтізбе үлгісінің көшірмесі.</span><span class="sxs-lookup"><span data-stu-id="5af99-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="5af99-110">Егер күнтізбе үлгісін өзгертсеңіз, онда бұл өзгерістер жобаның жұмыс уақытына қолданылмайды.</span><span class="sxs-lookup"><span data-stu-id="5af99-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="5af99-111">Жобаның жұмыс сағаттарын өзгерту үшін жаңа үлгі қолданылуы қажет.</span><span class="sxs-lookup"><span data-stu-id="5af99-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="5af99-112">Ұйымыңыз үшін күнтізбелік үлгіні жасау үшін екі негізгі талап қойылады:</span><span class="sxs-lookup"><span data-stu-id="5af99-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="5af99-113">Жаңа немесе қолданыстағы тапсырыс беру ресурсын пайдаланып үлгінің қажетті жұмыс сағаттарын анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="5af99-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="5af99-114">Жаңа күнтізбелік үлгі жасап, үлгіні тапсырыс беруге болатын ресурспен байланыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="5af99-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="5af99-115">**Үлгінің жұмыс сағаттарын анықтау**</span><span class="sxs-lookup"><span data-stu-id="5af99-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="5af99-116">**Ресурстар** \> **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="5af99-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="5af99-117">Күнтізбе үлгісінде сілтеме үшін жаңа ресурс жасаңыз немесе бар ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5af99-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="5af99-118">Ресурстың **Жұмыс сағаттары** қойыншасын таңдап, күнтізбе ережелерін конфигурациялау үшін [Ресурс үшін жұмыс сағаттарын орнату](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) бөліміндегі нұсқауларды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="5af99-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="5af99-119">**Жаңа күнтізбе үлгісін жасау**</span><span class="sxs-lookup"><span data-stu-id="5af99-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="5af99-120">**Параметрлер** \> **Күнтізбе үлгісі** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="5af99-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="5af99-121">**Жаңа** опциясын таңдап, атауын, сипаттамасын және үлгі ресурсын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="5af99-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="5af99-122">Күнтізбе үлгісінде ресурсқа сілтеме жасалған кезде, ресурс күнтізбесінің көшірмесі күнтізбе үлгісімен байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="5af99-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="5af99-123">Егер көшірілген үлгінің жұмыс сағаттары өзгерсе, бұл өзгерістер күнтізбе үлгісіне қолданылмайды.</span><span class="sxs-lookup"><span data-stu-id="5af99-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="5af99-124">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="5af99-124">See Also</span></span>  
 [<span data-ttu-id="5af99-125">Ресурстарды орнату</span><span class="sxs-lookup"><span data-stu-id="5af99-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
