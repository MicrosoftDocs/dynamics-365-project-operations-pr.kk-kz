---
title: Жоба тапсырмаларын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына синхрондаңыз
description: Бұл тақырыпта жоба тапсырмаларын тікелей Microsoft Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance бағдарламасына синхрондау үшін пайдаланылатын үлгі және негізгі тапсырма сипатталған.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 0383607a07def6c21562bf4b0893fe3ce3db6a04
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079642"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>Жоба тапсырмаларын тікелей Project Service Automation бағдарламасынан Finance and Operations бағдарламасына синхрондаңыз

[!include[banner](../includes/banner.md)]

Бұл тақырыпта жоба тапсырмаларын тікелей Dynamics 365 Project Service Automation бағдарламасынан Dynamics 365 Finance бағдарламасына синхрондау үшін пайдаланылатын үлгі және негізгі тапсырма сипатталған.

> [!NOTE]
> - Жоба тапсырмаларын біріктіру, шығындар транзакциясының санаттары, сағаттық болжамдар, шығын болжамдары және функционалды құлыптау 8.0 нұсқасында қолжетімді.
> - Егер Enterprise Edition 7.3.0 нұсқасын пайдалансаңыз, 4132657 білім қоры мен 4132660 білім қорын орнатқаннан кейін, үлгілерді жоба тапсырмаларын, шығыс транзакция санаттарын, сағаттық болжамдарды, шығын болжамдарын және нақты көрсеткіштерді біріктіру және функционалды құлыптауды конфигурациялау үшін пайдалана аласыз. Бухгалтерлік шоттар бойынша таратуды қалпына келтіру керек болса, онда сізге 4131710 білім қорын орнатуды ұсынамыз.
> - Нақты көрсеткіштерді біріктіру 8.0.1 немесе одан кейінгі нұсқада қолжетімді.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Project Service Automation және Finance бағдарламасындағы деректер ағыны

Project Service Automation және Finance бағдарламасын біріктіру шешімі деректерді біріктіру мүмкіндігін Project Service Automation және Finance мысалдары бойынша деректерді синхрондау үшін пайдаланады. Деректерді біріктіру мүмкіндігімен бірге қолжетімді біріктіру үлгісі Project Service Automation бағдарламасынан Finance бағдарламасына жоба тапсырмалары туралы деректер ағынына мүмкіндік береді.

Келесі суретте деректердің Project Service Automation және Finance арасында синхрондалу жолы көрсетілген.

[![Project Service Automation бағдарламасын Finance бағдарламасымен біріктіруге арналған деректер ағыны](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>Үлгі және тапсырма

Үлгіге қатынасу мақсатында, жалпы үлгілерді таңдау үшін Microsoft Power Apps басқару орталығында **Жобалар**, содан кейін оң жақ жоғарғы бұрышта **Жаңа жоба** пәрменін таңдаңыз.

Жоба тапсырмаларын Project Service Automation бағдарламасынан Finance бағдарламасына синхрондау үшін келесі үлгі және негізгі тапсырма пайдаланылады.

- **Деректерді біріктірудегі үлгі атауы:** Жоба тапсырмалары (Fin және Ops арналған PSA)
- **Жобадағы тапсырманың атауы:** Жоба тапсырмалары

Жоба тапсырмаларын синхрондау орын алмас бұрын, жоба келісім-шарттары мен жобаларды синхрондау қажет.

## <a name="entity-set"></a>Нысан жиынтығы

| Project Service Automation | Қаржы                             |
|----------------------------|-------------------------------------|
| Жоба тапсырмалары              | Жоба тапсырмасы үшін нысанды біріктіру |

## <a name="entity-flow"></a>Нысан ағыны

Жоба тапсырмалары Project Service Automation бағдарламасында басқарылады және олар жоба әрекеттері ретінде Finance бағдарламасына синхрондалады.

## <a name="prerequisites-and-mapping-setup"></a>Алғышарттар және салыстыру параметрі

Жоба тапсырмаларын синхрондау орын алмас бұрын, жоба келісім-шарттары мен жобаларды синхрондау қажет.

## <a name="power-query"></a>Power Query

Егер бұл шарт орындалса, деректерді сүзгілеу үшін Microsoft Power Query for Excel бағдарламасын пайдалану қажет:

- Жоба тапсырмасында ресурстарға қатысты жазбалар бар.

Егер Power Query қолдану қажет болса, келесі нұсқаулықты орындаңыз:

- Жоба тапсырмаларының (Fin және Ops арналған PSA) үлгісінде **IsLineTask** сүзгісін **Жалған** мәніне орнату арқылы жоба тапсырмасынан ресурстарға қатысты жазбаларды шығаратын әдепкі сүзгі бар. Егер өз үлгіңізді жасасаңыз, онда осы сүзгіні қосу қажет.

## <a name="template-mapping-in-data-integration"></a>Деректерді біріктіруде үлгіні салыстыру

Келесі суретте деректерді біріктіру кезіндегі үлгі тапсырмаларын салыстыру әрекеттерінің мысалы келтірілген. Картада Project Service Automation бағдарламасынан Finance бағдарламасына синхрондалатын өріс туралы ақпарат көрсетілген.

[![Үлгіні салыстыру](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)
