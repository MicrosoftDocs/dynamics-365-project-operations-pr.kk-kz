---
title: Project Service Automation бағдарламасына шолу
description: Бұл тақырыпта Dynamics 365 Project Service Automation бағдарламасын Dynamics 365 Finance бағдарламасына біріктіру шешімі туралы ақпарат көрсетілген.
author: KimANelson
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 897e1a1c-d31c-42b8-bb59-6b67202d8d61
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 080a545d8713e52d9778367aec1969b815d683e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753088"
---
# <a name="project-service-automation-overview"></a>Project Service Automation бағдарламасына шолу

[!include[banner](../includes/banner.md)]

Project Service Automation және Finance біріктіру шешімі Common Data Service арқылы Dynamics 365 Finance және Dynamics 365 Project Service Automation даналары бойынша деректерді синхрондау үшін деректерді біріктіру мүмкіндігін пайдаланады. Деректерді біріктіру мүмкіндігімен бірге қолжетімді біріктіру үлгілері Project Service Automation бағдарламасынан Finance бағдарламасына жоба, жоба келісім-шарттары, жоба келісім-шарты жолдары, жоба келісім-шарты жолының кезеңдері, жоба тапсырмалары, шығыс транзакция санаттары, сағаттық болжамдар және шығын болжамдары ағынына мүмкіндік береді.

> [!NOTE]
> - Егер 7.3.0 нұсқасын пайдалансаңыз, 4074835 білім қорын орнату қажет. Содан кейін белгіленген баға жобаларын біріктіре аласыз.
> - Егер 7.3.0 нұсқасын пайдалансаңыз және төлем транзакцияларын Project Service Automation бағдарламасынан алып тастасаңыз, онда ол төлемдерді жоба есеп-шотына қосу үшін 4345320 білім қорын орындау қажет.
> - 8.0 нұсқасын пайдалансаңыз, жоба тапсырмаларын біріктіру, шығындар транзакциясының санаттары, сағаттық болжамдар, шығын болжамдары және функционалды құлыптау мүмкіндіктерін пайдалана аласыз.
> - 8.0.1 немесе одан кейінгі нұсқаны пайдалансаңыз, нақты көрсеткіштерді синхрондау мүмкіндігіне ие боласыз.

Project Service Automation Finance бағдарламасын біріктірмес бұрын, Project Service Automation біріктіру параметрлерін конфигурациялау қажет. Қосымша ақпаратты [Project Service Automation біріктіру параметрлері](PSA-parameters.md) бөлімінен қараңыз.

Бұл біріктіру шешімі келесі сценарийлерде тікелей синхрондауға мүмкіндік береді:

- Project Service Automation бағдарламасында жоба келісім-шарттарын орындаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.
- Project Service Automation бағдарламасында жобалар жасаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.
- Project Service Automation бағдарламасында жоба келісім-шарты жолдарын сақтаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.
- Project Service Automation бағдарламасында жоба келісім-шарты жолының кезеңдерін сақтаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.
- Project Service Automation бағдарламасында жоба тапсырмаларын орындаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.
- Finance бағдарламасында шығыс транзакция санаттарын сақтаңыз және оларды Finance бағдарламасынан Project Service Automation бағдарламасына тікелей синхрондаңыз.
- Project Service Automation бағдарламасында жобаның сағаттық болжамдарын жасаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.
- Project Service Automation бағдарламасында жобаның шығын болжамдарын жасаңыз және оларды Project Service Automation бағдарламасынан Finance бағдарламасына тікелей синхрондаңыз.
- Project Service Automation бағдарламасында жоба уақыты, шығын және төлемнің нақты көрсеткіштерін жасаңыз және оларды Finance бағдарламасында жариялай алу үшін Project Service Automation біріктіру журналында жоба транзакцияларын жасаңыз.

## <a name="data-synchronization"></a>Деректерді синхрондау

Келесі суретте деректердің Project Service Automation және Finance арасында біріктіру бөлігі ретінде синхрондалу жолы көрсетілген.

> [!NOTE]
> Ағымдағы уақытта барлық үлгілер қолжетімді емес. Үлгілер аяқталғаннан кейін шығарылады.

[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіру](./media/PSA-integration.png)](./media/PSA-integration.png)

## <a name="system-requirements-for-finance"></a>Finance бағдарламасына қойылатын жүйе талаптары

Project Service Automation және Finance біріктіру шешімін пайдалану үшін Platform 12 немесе одан кейінгі жаңартуы бар Enterprise Edition 7.3 нұсқасын орнату қажет.

## <a name="system-requirements-for-project-service-automation"></a>Project Service Automation бағдарламасы үшін қойылатын жүйе талаптары

Project Service Automation және Finance біріктіру шешімін пайдалану үшін келесі компоненттерді орнату қажет:

- Dynamics 365 Project Service Automation 9.0.0.0 нұсқасы не одан жоғары
- Dynamics 365 Sales, 1.14.0.0 (v14) нұсқасы немесе одан кейінгі нұсқасына арналған қаражат шешімінің әлеуетті тұтынушысы
- Dynamics 365 Project Service Automation 1.0.0.0 нұсқасы немесе одан кейінгі нұсқасына арналған Project Service Automation және Finance шешімі

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a>Project Service Automation данасында Project Service Automation және Finance біріктіру шешімін орнатыңыз

[Microsoft жүктеу орталығынан](https://www.microsoft.com/download/details.aspx?id=57016) Project Service Automation және Finance біріктіру шешімін жүктеп алыңыз және шешіммен бірге берілген нұсқауларды орындаңыз.
