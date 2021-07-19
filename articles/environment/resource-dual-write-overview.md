---
title: Project Operations қос жазу интеграциясы
description: Бұл тақырыпта Project Operations қос жазу интеграциясына шолу ұсынылады.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: 540b6f74d8e79116e5fdb2ceffaa4bbb487ff08f
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368438"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="d5068-103">Project Operations қос жазу интеграциясына шолу</span><span class="sxs-lookup"><span data-stu-id="d5068-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="d5068-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="d5068-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d5068-105">Project Operations бағдарламасы Microsoft Dataverse және Dynamics 365 Finance бағдарламаларында деректерді синхрондау үшін [қос жазу мүмкіндіктерін](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="d5068-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="d5068-106">Келесі суретте деректердің Dataverse және Finance бағдарламалары арасында интеграция бөлігі ретінде синхрондалу жолы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="d5068-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![Project Operations деректер ағындарына шолу](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="d5068-108">Dataverse жүйесіндегі Project Operations бағдарламасы Power Platform мүмкіндіктерін пайдалана отырып, қазіргі пайдаланушы интерфейсі (UI) мен кодсыз/жеңіл кодты қарапайым кеңейту мүмкіндігін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="d5068-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="d5068-109">Жоба менеджерлері, ресурстар менеджерлері, жобалық топ мүшелері және басқа да клиенттермен жұмыс істеу бөлімінің тұлғалары өз әрекеттерін Dataverse жүйесіндегі Project Operations бағдарламасында орындайды.</span><span class="sxs-lookup"><span data-stu-id="d5068-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="d5068-110">Finance жүйесіндегі Project Operations бағдарламасы жоба есебі және табысты тануды қолдау әрекетін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="d5068-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="d5068-111">Project Operations бағдарламасы сату салығын есептеу, валюта айырбастау бағамдары, қаржылық өлшем бойынша есеп және тағы басқалары үшін Finance платформасындағы қаржы құрылымына қосылады.</span><span class="sxs-lookup"><span data-stu-id="d5068-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="d5068-112">Жоба бухгалтерлерінің тәжірибесі негізінен Finance жүйесіне негізделген.</span><span class="sxs-lookup"><span data-stu-id="d5068-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="d5068-113">Project Operations интеграциясы келесі құрамдас интеграциясынан тұрады:</span><span class="sxs-lookup"><span data-stu-id="d5068-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="d5068-114">Project Operations бағдарламасын орнату және конфигурация деректерінің интеграциясы</span><span class="sxs-lookup"><span data-stu-id="d5068-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="d5068-115">Жоба болжамдары мен нақты көрсеткіштері</span><span class="sxs-lookup"><span data-stu-id="d5068-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="d5068-116">Жоба есеп-шоттары</span><span class="sxs-lookup"><span data-stu-id="d5068-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="d5068-117">Шығысты басқару</span><span class="sxs-lookup"><span data-stu-id="d5068-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="d5068-118">Жеткізуші есеп-шоты</span><span class="sxs-lookup"><span data-stu-id="d5068-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
