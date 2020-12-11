---
title: Ресурсты пайдалануға шолу
description: Бұл тақырыпта ресурсты Project Operations бағдарламасында пайдалану туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8b85464dbb68523b122116225a604f67e7236f3e
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401383"
---
# <a name="resource-utilization-overview"></a>Ресурсты пайдалануға шолу

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Ресурстардың мақсатты шот ұсынылған қолданысы болуы мүмкін. Осы мақсатты пайдалану ресурстың әдепкі рөліндегі атрибут ретінде анықталады немесе жеке тіркелетін ресурстың жазбасында орнатылады. Пайдалану есептеулері ресурстар бекітілген уақыт жазбаларын пайдалану арқылы есеп берген нақты сағат санына негізделген.

Пайдалануды есептеу үшін келесі формулалар пайдаланылады:

  - Шот ұсынылған қолданыс = ақылы нақты сағаттар ÷ ресурс сыйымдылығы
  - Шот ұсынылмайтын қолданыс = шот ұсыну түрінің идентификаторы бар нақты уақыт = ақысыз, қосымша немесе қолжетімді емес ÷ ресурс сыйымдылығы
  - Ішкі = сатылым келісім-шарты жоқ нақты уақыт ÷ ресурс сыйымдылығы
  - Ресурс сыйымдылығы = ресурстың жұмыс сағаттары – кеңседен тыс – жұмыс істемейтін күндер

**Ресурсты пайдалану** көрінісін **Ресурстар** тақтасынан табуға болады.

Тордағы әрбір ұяшық ресурстың күн, апта немесе ай сияқты кезеңдегі шот ұсынылған қолданысының пайыздық мөлшерін көрсетеді. Ұяшықтарды бояу үшін келесі формулалар пайдаланылады:

  - **Жасыл**: шот ұсынылған қолданыс >= ресурстың мақсатты қолданысы
  - **Сары**: мақсатты қолданыс – 20 <= шот ұсынылған қолданыс < мақсатты қолданыс
  - **Қызыл**: шот ұсынылған қолданыс < мақсатты қолданыс – 20

**Ресурсты пайдалану** көрінісі кесте тақтасына негізделгендіктен, нәтижелерді сүзгілеу үшін кесте тақтасының сүзгілеу мүмкіндіктерін пайдалануға болады.

Тор рөлге немесе жеке ресурсқа мақсатты қолданысты орнатуды талап етеді. Бұл орнатуды орындау үші, **Ресурстар** > **Ресурс рөлдері** тармағына өтіңіз.

Сонымен қатар әрбір тіркелетін ресурсқа әдепкі рөлді тағайындау керек. **Ресурстар** > **Ресурстар** тармағына өтіңіз. **Project Service** қойыншасында ресурс рөлінің анықталғанын және оның **Әдепкі** өрісі **Иә** параметріне орнатылғанын тексеріңіз. **Әдепкі** = **жоқ** параметріне орнатылған қосымша рөлдерді қосуға болады. **Әдепкі** = **иә** параметріне орнатылған рөл ресурсты сол рөлдің мақсаты бойынша пайдалануды бағалау үшін пайдаланылады.

**Project Service** қойыншасында, ресурс үшін жеке мақсатты қолданысты орнатуға болады. Сонда пайдалануды есептеу ресурстың әдепкі рөлінің орнына ресурстың мақсатын бағалау үшін мақсатты қолданысты пайдаланады.

Қолдану ресурсқа егер оның торда көрсетілген уақыт кезеңінде бекітілген, ақылы уақыты болса ғана көрсетіледі.