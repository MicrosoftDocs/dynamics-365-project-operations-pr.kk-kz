---
title: Компанияаралық шығыстар
description: Бұл тақырыпта жұмысшы шығындарын жұмыс орындалған заңды нысанға белгілеу үшін компанияаралық шығындарды пайдалану туралы ақпарат берілген.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d908a1c062f5b7f01cf340dcd6f7f24714a992bf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271540"
---
# <a name="intercompany-expenses"></a>Компанияаралық шығыстар

Ұйымдағы бір заңды нысанда жұмыс істейтін қызметкер сол ұйымдағы басқа заңды нысан үшін жұмысты орындай алады. Компанияаралық шығындарды жұмысшы шығындарын жұмыс орындалған заңды нысанға белгілеу үшін пайдалануға болады. Қызметкерді жалдайтын заңды нысан несиелік заңды нысан деп аталады. Қызметкер шығындар жасайтын заңды нысан қарыз беруші заңды нысан деп аталады. 

Жұмысшы компанияаралық шығындарды жасап, ұсынбас бұрын, сізге компанияаралық шығындар желілерін қосу қажет. Қарыз беретін заңды нысанда, **Шығындарды басқару параметрлері** бетінде **Компанияаралық шығындар желілеріне рұқсат беру** опциясын таңдаңыз. 

## <a name="tax-posting-for-intercompany-expenses"></a>Компанияаралық шығыстарға салық салу

[!include [banner](../includes/banner.md)]

Шығындар туралы есепте қарыз алушы заңды нысанмен (жеткізу орны) емес, қарыз беруші заңды нысанмен (дереккөзбен) байланысты салық топтарын пайдаланбас бұрын, бұл функцияны бас кітап сатылымы салығының параметрінде қосу керек. **Компанияаралық салықтарды жүргізуге арналған заңды нысан** параметрі **Бастапқы** күйіне, ал **Сату салығына салық салу ережелерін қолдану** параметрі **Жоқ** күйіне орнатылса, қарыз беруші заңды нысан үшін салық тіркесімі пайдаланылады. Сол параметр **Межелі орын** мәніне орнатылған кезде, қарыз беруші заңды нысан үшін салық комбинациясы пайдаланылады. АҚШ-тағы заңды нысандар үшін параметр **Дереккөз** мәніне орнатылған кезде, **Дебиторлық сатылым салығы** өрісі жаңа **Бас кітапқа енгізу топтары** бетіне конфигурациялануы тиіс. Есепке алу жүйесі осы өрістегі ақпаратты есепке алу нысанына қатысты салық салу үшін пайдаланады.   
Бұл әрекет жобамен немесе жобасыз орналастырылған шығыс жолдарына сәйкес келеді.  


[!INCLUDE[footer-include](../includes/footer-banner.md)]