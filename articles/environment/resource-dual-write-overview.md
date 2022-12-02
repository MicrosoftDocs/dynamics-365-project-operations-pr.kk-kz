---
title: Project Operations қос жазу интеграциясы
description: Бұл мақалада Project Operations қос жазу интеграциясына шолу ұсынылады.
author: sigitac
ms.date: 04/28/2021
ms.topic: overview
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d365a036f96ff4f7b14107b43e8c6b70df0b5362
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927979"
---
# <a name="project-operations-dual-write-integration-overview"></a>Project Operations қос жазу интеграциясына шолу

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Project Operations бағдарламасы [қос жазу мүмкіндіктері](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) опциясын Microsoft Dataverse және Dynamics 365 Finance бағдарламаларында деректерді синхрондау үшін пайдаланады.

Келесі суретте деректердің Dataverse және Finance бағдарламалары арасында интеграция бөлігі ретінде синхрондалу жолы көрсетіледі.

![Project Operations деректер ағындарына шолу.](./media/ProjectOperationsFlows.jpg)

Dataverse жүйесіндегі Project Operations бағдарламасы Power Platform мүмкіндіктерін пайдалана отырып, қазіргі пайдаланушы интерфейсі (UI) мен кодсыз/жеңіл кодты қарапайым кеңейту мүмкіндігін ұсынады. Жоба менеджерлері, ресурстар менеджерлері, жобалық топ мүшелері және басқа да клиенттермен жұмыс істеу бөлімінің тұлғалары өз әрекеттерін Dataverse жүйесіндегі Project Operations бағдарламасында орындайды.

Finance жүйесіндегі Project Operations бағдарламасы жоба есебі және табысты тануды қолдау әрекетін ұсынады. Project Operations бағдарламасы сату салығын есептеу, валюта айырбастау бағамдары, қаржылық өлшем бойынша есеп және тағы басқалары үшін Finance платформасындағы қаржы құрылымына қосылады. Жоба бухгалтерлерінің тәжірибесі негізінен Finance жүйесіне негізделген.

Project Operations интеграциясы келесі құрамдас интеграциясынан тұрады:


- [Project Operations бағдарламасын орнату және конфигурация деректерінің интеграциясы](resource-dual-write-setup-integration.md) 
- [Жоба болжамдары мен нақты көрсеткіштері](resource-dual-write-estimates-actuals.md)
- [Жоба есеп-шоттары](resource-dual-write-project-invoice.md)
- [Шығысты басқару](resource-dual-write-expense.md)
- [Жеткізуші есеп-шоты](resource-dual-write-vendor-invoice.md)
