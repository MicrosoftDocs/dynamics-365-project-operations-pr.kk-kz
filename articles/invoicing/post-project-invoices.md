---
title: Шот жіберу процесіне шолу
description: Бұл тақырып ресурс/биржадан тыс негіздегі сценарийлер үшін Project Operations жүйесіндегі есеп-шот ұсынудың процестік шолуын ұсынады.
author: sigitac
ms.date: 01/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: 804d42f7e8bfd103b9143dc0f5c7ddecdee9e66e6072c3e7bf76b2a8c549cf55
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "7003778"
---
# <a name="invoicing-process-overview"></a>Шот жіберу процесіне шолу

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations жоба менеджерінің, сондай-ақ дебиторлық қарыздар қызметкерінің/жоба бухгалтерінің қажеттіліктеріне сай кешенді мүмкіндіктерді ұсынады. Есеп-шот ұсыну процесі үшін жоба менеджері жоба бойынша төлемдердің артта қалуын басқарады, ал дебиторлық қарыздар бойынша қызметкер/жоба бухгалтері тұтынушыларға сәйкес келетін және нақты есеп-шот ұсыну құжатын жасайды.

![Шот-фактура бойынша схема.](./media/invoicing-flow.png)

Жоба келісімшартының желісі байланысты жобалық операциялар үшін төлем әдісін анықтайды. Жоба менеджері уақыт пен шығындар бойынша операцияларды бекіткен кезде, жүйе **Жобаның нақты көрсеткіштері** нысанында операцияларды есепке алып, Dynamics 365 Finance бағдарламасындағы **Жобаларды басқару және есепке шолу** модуліне ақпарат жібереді. Содан кейін жоба бухгалтері [Project Operations Integration журналы](../project-accounting/project-operations-integration-journal.md) арқылы жазбаларды қарап, орналастырады. Бұл журналда есеп айырысу, сатуға салынатын салық тобы, есеп айырысу элементінің сатуға салынатын салық тобы және қаржылық өлшемдер сияқты жобаның нақты көрсеткіштері үшін маңызды бухгалтерлік есеп туралы мәліметтер бар.

Жобаның менеджері [Уақыт және материалдық шоттың орындалмаған әрекеттері](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) бөліміндегі уақыт пен материалдарды есепке алу әдісін және [Бекітілген баға кезеңдері](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones) бөліміндегі бекітілген бағаны есептеу жүйелерін пайдалану арқылы шот ұсынылмаған сатылым транзакцияларын қарап шыға алады. Бұл көріністер келесі шот жіберу цикліне қосылуы қажет транзакцияларды сүзгілеуге және таңдауға, содан кейін оларды **Шот-фактураға дайын** ретінде белгілеуге мүмкіндік береді.

[Қолмен проформа-шотын жасауға](../proforma-invoicing/create-manual-proforma-invoice.md) немесе [кезеңдік процесті](../proforma-invoicing/configure-automated-invoice-creation.md) пайдалануға болады. Жоба менеджері [жоба профома-шотын қажетінше реттеп](../proforma-invoicing/manage-proforma-invoice.md), содан кейін растай алады.

Расталған шот-фактура Finance жүйесіндегі **Жобаларды басқару және есеп** модуліне жіберіледі. Жоба бухгалтері жоба шот-фактурасын ұсынады және жаңартады, содан кейін құжатты орналастырып, басып шығарады. Жарияланған шот-фактуралар бас кітапта, сондай-ақ тұтынушы мен жобаның қосалқы кітаптарында тіркеледі.


[!INCLUDE[footer-include](../includes/footer-banner.md)]