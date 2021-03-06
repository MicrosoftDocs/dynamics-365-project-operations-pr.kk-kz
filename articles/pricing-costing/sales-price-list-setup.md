---
title: Сатылым прайс-листін орнату
description: Осы тақырып жоба бағасын белгілеу үшін сатылым прайс-листтері туралы ақпаратты ұсынады.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2a66802adfcadab7b4d34149b146ca3cb27c903e
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896468"
---
# <a name="sales-price-list-setup"></a>Сатылым прайс-листін орнату

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Жобаның баға ұсыныстары мен келісім-шарттары үшін, жобаның бағатізбесінде өнімнің бағатізбесінен өзгеше бағаны алдын ала анықтау үлгісі бар. Өнім каталогына негізделген баға ұсыну жолы үшін, рөлдер мен санаттарға бағаны тікелей баға ұсыну жолында алдын ала анықтауға болады, себебі әрбір баға ұсыну жолы нақты бір каталог элементіне нұсқайды. Дегенмен жобаға негізделген баға ұсыну жолында рөлдер мен санаттарға бағаны тікелей баға ұсыну жолында алдын ала анықтау мүмкін емес. Жоба прайс-листін анықталған екі үлгімен жұмыс істеу үшін пайдалануға болады.

> [!NOTE]
> Бағаны алдын ала анықтау кезінде екеуінің арасындағы әрекеттер айырмашылығының себебінен, жоба ресурстары мен каталог элементтері үшін бөлек бағатізбенің болғаны жөн.

Жобаның бағасын белгілеу үшін, келесі нысандардың әрқайсысы бір немесе бірнеше байланыстырылған сатылым бағатізбесіне ие бола алады:

- Тұтынушы (тіркелгі) 
- Мүмкіндік 
- Баға ұсыну 
- Жоба келісім-шарты

Бұл нысандардың бағатізбемен байланысы жоба бағатізбелерімен анықталады. Тұтынушы, мүмкіндік, баға ұсыну және жоба келісім-шарты бойынша сатылымдар нысандарымен бір немесе бірнеше бағатізбені байланыстыруға болады.

Жобаның әдепкі бағатізбесі тұтынушы жазбасына автоматты түрде енгізілмейді. Дегенмен жобаның бағатізбесін тұтынушы жазбасына қолмен тіркеуге болады. Бұған қарамастан, жобаның бағатізбесін тұтынушымен реттелетін баға келісімі болған кезде ғана қолмен тіркеуіңіз керек. 

Жоба прайс-листі сатылым нысанына бекітілген кезде, келесі ақпарат тексеріледі:

- Прайс-листте **Сатылым** контексті бар. 
- Бағатізбенің валютасы тұтынушы валютасына сәйкес келеді. 

Жоба келісім-шартында, жобаның қатысты прайс-листтерін автоматты түрде орнату үшін келесі кезектілік тәртібі пайдаланылады:

1. Баға ұсыну
2. Мүмкіндік
3. Тұтынушы 
4. Глобалдық параметрлер 

Жоба прайс-листі әдепкі бойынша енгізіледі, жүйе валютаның тұтынушы валютасына сәйкестігін және енгізілген әдепкі прайс-листтерде **Сатылым** контексті бар-жоғын тексереді.

Тұтынушы, мүмкіндік, баға ұсыну және жоба келісім-шартының нысандарымен бірнеше бағатізбені байланыстыруға болады. Бұл мүмкіндік құнсыздану себебінен орын алатын баға жаңартулары үшін тіркелгіге бірнеше бағатізбені қажет етуіңіз мүмкін ұзақ мерзімді жоба келісім-шарты үшін күн бойынша әдепкі бағаларды қолдайды. Дегенмен тұтынушы, мүмкіндік, баға ұсыну немесе жоба келісім-шартының нысанымен байланыстырылған бағатізбелердің жарамдылық мерзімі қабаттасқан болса, әдепкі бағалардың дұрыс болмауы мүмкін. Сондықтан жарамдылық мерзімі қабаттасқан жоба бағатізбелерінің осы нысандармен байланыстырылмағанына көз жеткізу қажет.
