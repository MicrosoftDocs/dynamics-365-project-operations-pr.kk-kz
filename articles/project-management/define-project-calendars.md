---
title: Жоба күнтізбелерін анықтау
description: Бұл тақырып жоба кестесін бақылау үшін күнтізбелік үлгіні жобаға қолдану жолы туралы ақпарат береді.
author: ruhercul
manager: AnnBe
ms.date: 02/05/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1d5642d7a2246dc878b2bc4f504f138b71d29a69
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981307"
---
# <a name="define-project-calendars"></a><span data-ttu-id="27f18-103">Жоба күнтізбелерін анықтау</span><span class="sxs-lookup"><span data-stu-id="27f18-103">Define project calendars</span></span>

<span data-ttu-id="27f18-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="27f18-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="27f18-105">Жобаны жасап, басқару үшін жобаға күнтізбелік үлгіні қолдану қажет.</span><span class="sxs-lookup"><span data-stu-id="27f18-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="27f18-106">Күнтізбе үлгісі келесі жоба төлсипаттарын анықтайды:</span><span class="sxs-lookup"><span data-stu-id="27f18-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="27f18-107">Жұмыс сағаттары, оның ішінде басталу және аяқталу уақыты</span><span class="sxs-lookup"><span data-stu-id="27f18-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="27f18-108">Жұмыс күндері</span><span class="sxs-lookup"><span data-stu-id="27f18-108">Working days</span></span>
- <span data-ttu-id="27f18-109">Жұмыс емес күндер секілді күнтізбелік ерекшеліктер</span><span class="sxs-lookup"><span data-stu-id="27f18-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="27f18-110">Жобаға қолданылатын күнтізбе үлгісі - бұл сіздің ұйымыңыздың параметрлерінде анықталған күнтізбе үлгісінің көшірмесі.</span><span class="sxs-lookup"><span data-stu-id="27f18-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="27f18-111">Егер күнтізбе үлгісін өзгертсеңіз, онда бұл өзгерістер жобаның жұмыс уақытына қолданылмайды.</span><span class="sxs-lookup"><span data-stu-id="27f18-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="27f18-112">Жобаның жұмыс сағаттарын өзгерту үшін жаңа үлгі қолданылуы қажет.</span><span class="sxs-lookup"><span data-stu-id="27f18-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="27f18-113">Ұйымыңыз үшін күнтізбелік үлгіні жасау үшін екі негізгі талап қойылады:</span><span class="sxs-lookup"><span data-stu-id="27f18-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="27f18-114">Жаңа немесе қолданыстағы тапсырыс беру ресурсын пайдаланып үлгінің қажетті жұмыс сағаттарын анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="27f18-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="27f18-115">Жаңа күнтізбелік үлгі жасап, үлгіні тапсырыс беруге болатын ресурспен байланыстырыңыз.</span><span class="sxs-lookup"><span data-stu-id="27f18-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="27f18-116">**Үлгінің жұмыс сағаттарын анықтау**</span><span class="sxs-lookup"><span data-stu-id="27f18-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="27f18-117">**Ресурстар** \> **Ресурстар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="27f18-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="27f18-118">Күнтізбе үлгісінде сілтеме үшін жаңа ресурс жасаңыз немесе бар ресурсты таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="27f18-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="27f18-119">Ресурстың **Жұмыс сағаттары** қойыншасын таңдап, күнтізбе ережелерін конфигурациялау үшін [Ресурс үшін жұмыс сағаттарын орнату](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) бөліміндегі нұсқауларды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="27f18-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="27f18-120">**Жаңа күнтізбе үлгісін жасау**</span><span class="sxs-lookup"><span data-stu-id="27f18-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="27f18-121">**Параметрлер** \> **Күнтізбе үлгісі** бөліміне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="27f18-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="27f18-122">**Жаңа** опциясын таңдап, атауын, сипаттамасын және үлгі ресурсын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="27f18-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="27f18-123">Күнтізбе үлгісінде ресурсқа сілтеме жасалған кезде, ресурс күнтізбесінің көшірмесі күнтізбе үлгісімен байланысты болады.</span><span class="sxs-lookup"><span data-stu-id="27f18-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="27f18-124">Егер көшірілген үлгінің жұмыс сағаттары өзгерсе, бұл өзгерістер күнтізбе үлгісіне қолданылмайды.</span><span class="sxs-lookup"><span data-stu-id="27f18-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="27f18-125">Енді жұмыс үлгісін жобаның күнтізбелік үлгісімен байланыстыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="27f18-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

