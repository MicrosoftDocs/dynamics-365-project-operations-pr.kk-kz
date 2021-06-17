---
title: Жұмыс уақыты үлгілерін жасау
description: Бұл тақырыпта Project Service қызметінде жұмыс сағаттарының үлгісін жасау жолдары сипатталады.
author: ruhercul
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
ms.openlocfilehash: 105e3cb2ef7b904e96dc21013906e0b7444e3b88
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997203"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="c981b-103">Жұмыс сағаттары үлгісін жасау (Project Service)</span><span class="sxs-lookup"><span data-stu-id="c981b-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="c981b-104">Жобаны жасап, басқару үшін жобаға күнтізбелік үлгіні қолдану қажет.</span><span class="sxs-lookup"><span data-stu-id="c981b-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="c981b-105">Күнтізбе үлгісі келесі жоба төлсипаттарын анықтайды:</span><span class="sxs-lookup"><span data-stu-id="c981b-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="c981b-106">Жұмыс сағаттары, оның ішінде басталу және аяқталу уақыты</span><span class="sxs-lookup"><span data-stu-id="c981b-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="c981b-107">Жұмыс күндері</span><span class="sxs-lookup"><span data-stu-id="c981b-107">Working days</span></span>
- <span data-ttu-id="c981b-108">Жұмыс емес күндер секілді күнтізбелік ерекшеліктер</span><span class="sxs-lookup"><span data-stu-id="c981b-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="c981b-109">Жобаға қолданылатын күнтізбе үлгісі - бұл сіздің ұйымыңыздың параметрлерінде анықталған күнтізбе үлгісінің көшірмесі.</span><span class="sxs-lookup"><span data-stu-id="c981b-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="c981b-110">Егер күнтізбе үлгісін өзгертсеңіз, онда бұл өзгерістер жобаның жұмыс уақытына қолданылмайды.</span><span class="sxs-lookup"><span data-stu-id="c981b-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="c981b-111">Жобаның жұмыс сағаттарын өзгерту үшін жаңа үлгі қолданылуы қажет.</span><span class="sxs-lookup"><span data-stu-id="c981b-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="c981b-112">Ұйымыңыз үшін күнтізбелік үлгіні жасау үшін екі негізгі талап қойылады:</span><span class="sxs-lookup"><span data-stu-id="c981b-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="c981b-113">Жаңа немесе қолданыстағы тапсырыс беру ресурсын пайдаланып үлгінің қажетті жұмыс сағаттарын анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="c981b-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="c981b-114">Жаңа күнтізбелік үлгі жасап, үлгіні тапсырыс беруге болатын ресурспен байланыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="c981b-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="c981b-115">**Үлгінің жұмыс сағаттарын анықтау**</span><span class="sxs-lookup"><span data-stu-id="c981b-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="c981b-116">**Ресурстар** \> **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="c981b-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="c981b-117">Күнтізбе үлгісінде сілтеме үшін жаңа ресурс жасаңыз немесе бар ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="c981b-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="c981b-118">Ресурстың **Жұмыс сағаттары** қойыншасын таңдап, күнтізбе ережелерін конфигурациялау үшін [Ресурс үшін жұмыс сағаттарын орнату](/dynamics365/field-service/set-work-hours-resource.md) бөліміндегі нұсқауларды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="c981b-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="c981b-119">**Жаңа күнтізбе үлгісін жасау**</span><span class="sxs-lookup"><span data-stu-id="c981b-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="c981b-120">**Параметрлер** \> **Күнтізбе үлгісі** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="c981b-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="c981b-121">**Жаңа** опциясын таңдап, атауын, сипаттамасын және үлгі ресурсын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="c981b-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="c981b-122">Күнтізбе үлгісінде ресурсқа сілтеме жасалған кезде, ресурс күнтізбесінің көшірмесі күнтізбе үлгісімен байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="c981b-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="c981b-123">Егер көшірілген үлгінің жұмыс сағаттары өзгерсе, бұл өзгерістер күнтізбе үлгісіне қолданылмайды.</span><span class="sxs-lookup"><span data-stu-id="c981b-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="c981b-124">Сонымен қатар, келесіні қараңыз:</span><span class="sxs-lookup"><span data-stu-id="c981b-124">See Also</span></span>  
 [<span data-ttu-id="c981b-125">Ресурстарды орнату</span><span class="sxs-lookup"><span data-stu-id="c981b-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
