---
title: Project Operations қос жазу интеграциясы
description: Бұл тақырыпта Project Operations қос жазу интеграциясына шолу ұсынылады.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ce4f7bf8185e6f3f942df14d30d7b8d0a3e4444a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998688"
---
# <a name="project-operations-dual-write-integration-overview"></a>Project Operations қос жазу интеграциясына шолу

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Project Operations бағдарламасы Microsoft Dataverse және Dynamics 365 Finance бағдарламаларында деректерді синхрондау үшін [қос жазу мүмкіндіктерін](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) пайдаланады.

Келесі суретте деректердің Dataverse және Finance бағдарламалары арасында интеграция бөлігі ретінде синхрондалу жолы көрсетіледі.

![Project Operations деректер ағындарына шолу](./media/ProjectOperationsFlows.jpg)

Dataverse жүйесіндегі Project Operations бағдарламасы Power Platform мүмкіндіктерін пайдалана отырып, қазіргі пайдаланушы интерфейсі (UI) мен кодсыз/жеңіл кодты қарапайым кеңейту мүмкіндігін ұсынады. Жоба менеджерлері, ресурстар менеджерлері, жобалық топ мүшелері және басқа да клиенттермен жұмыс істеу бөлімінің тұлғалары өз әрекеттерін Dataverse жүйесіндегі Project Operations бағдарламасында орындайды.

Finance жүйесіндегі Project Operations бағдарламасы жоба есебі және табысты тануды қолдау әрекетін ұсынады. Project Operations бағдарламасы сату салығын есептеу, валюта айырбастау бағамдары, қаржылық өлшем бойынша есеп және тағы басқалары үшін Finance платформасындағы қаржы құрылымына қосылады. Жоба бухгалтерлерінің тәжірибесі негізінен Finance жүйесіне негізделген.

Project Operations интеграциясы келесі құрамдас интеграциясынан тұрады:


- [Project Operations бағдарламасын орнату және конфигурация деректерінің интеграциясы](resource-dual-write-setup-integration.md) 
- [Жоба болжамдары мен нақты көрсеткіштері](resource-dual-write-estimates-actuals.md)
- [Жоба есеп-шоттары](resource-dual-write-project-invoice.md)
- [Шығысты басқару](resource-dual-write-expense.md)
- [Жеткізуші есеп-шоты](resource-dual-write-vendor-invoice.md)
