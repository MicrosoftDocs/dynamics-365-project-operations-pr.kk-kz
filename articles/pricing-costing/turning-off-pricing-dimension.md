---
title: Бағалау өлшемін өшіру
description: Осы тақырып бағалау өлшемдерін өшіру әдісі туралы ақпаратты ұсынады.
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
ms.openlocfilehash: 54e02726138f7306481ca50d5204ee29a3b68549
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896513"
---
# <a name="turning-off-a-pricing-dimension"></a>Бағалау өлшемін өшіру

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Баға стратегиясын бірнеше жылда бір рет қарап, жаңартып отыру қажет болуы мүмкін. Сіз жасаған кез келген жаңартулар қолданыстағы бағалар өлшемін өшіруді және жаңасын жасауды талап етуі мүмкін. Мысалы, сіз бұрын **Рөл** арқылы бағалаған болуыңыз мүмкін, бірақ қазір **Жұмыс тәжірибесі** арқылы бағалау туралы шешім қабылдадыңыз. Бұл **Рөл** опциясын бағалау өлшемі ретінде өшіруді және **Жұмыс тәжірибесі** опциясын жаңа бағалау өлшемі ретінде жасауды қажет етуі мүмкін. 

Бағалар өлшемін кірістірілгеніне немесе реттелетініне қарамастан өшіру бағалар өлшемінің **Құнға қолданылатын** және **Сатылымға қолданылатын** өрістерін **Жоқ** параметріне орнату арқылы жүзеге асырылуы мүмкін.

Алайда бұлай жасаған кезде, **Байланыстырылған баға жазбалары болса, бағалау өлшемін жаңарту немесе жою мүмкін емес** қате туралы хабарын алуыңыз мүмкін.

Бұл қате туралы хабар өшірілетін өлшем үшін алдын ала орнатылған баға жазбалары бар екенін көрсетеді. Барлық өлшемге қатысты **Рөл бағасы** және **Рөлдің үстеме бағасы** жазбалары өлшем қолданысын **Жоқ** параметріне орнату алдында жойылуы керек. Бұл ереже сіз жасаған кірістірілген бағалар өлшемдеріне де, кез келген реттелетін бағалар өлшемдеріне де қолданылады. Бұл тексерудің себебі - әрбір **Рөл бағасы** жазбасы өлшемдердің бірегей тіркесімін қамтуы керек. Мысалы, **АҚШ құн мөлшерлемелері, 2018** деп аталатын бағатізбеде келесідей **Рөл бағасы** жолдары бар. 

| Стандартты тақырып         | Ұйымдық бөлімше    |Бірлік   |Баға  |Валюта  |
| -----------------------|-------------|-------|-------|----------|
| Жүйелер инженері|Contoso АҚШ|Hour| 100|USD|
| Жоғарғы жүйелер инженері|Contoso АҚШ|Hour| 150| USD|


**Стандартты тақырып** нысанын бағалау өлшемі ретінде өшірсеңіз және бағалау механизмі бағаны іздейтін болса, ол енгізу контекстіндегі **Ұйымдық бірлік** мәнін ғана пайдаланатын болады. Егер енгізу мәтінмәнінің **Ұйымдық бөлімшесі** "Contoso US" болса, нәтиже анық болмайды, себебі екі жол да сәйкес келеді. Бұл сценарийді болдырмау үшін **Рөл бағасы** жазбаларын жасаған кезде жүйе өлшемдер тіркесімінің бірегей екендігін тексереді. Өлшем **Рөл бағасы** жазбалары жасалғаннан кейін өшірілсе, бұл шектеуді бұзуға болады. Сондықтан өлшемді өшірмес бұрын, осы өлшем мәні толтырылған барлық **Рөл бағасы** және **Рөлдің үстеме бағасы** жолдарын жою керек.
