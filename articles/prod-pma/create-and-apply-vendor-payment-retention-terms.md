---
title: Жеткізушінің төлемін сақтау шарттарын жасау және қолдану
description: Бұл тақырыпта жеткізушілердің төлемдерін сақтау шарттарын белгілеу және сақтау жолдары туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: e6f6424b983f76a96825d76e1b4b81b54dc84b84
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270955"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a>Жеткізушінің төлемін сақтау шарттарын жасау және қолдану

[!include [banner](../includes/banner.md)] 

Жоба үшін сатушының төлемін сақтау мерзімдерін белгілеу сіздің ұйымыңыз жеткізушіге төленген төлемдердің бір бөлігін сақтап қалғысы келгенде пайдалы. Мысалы, жеткізушіге жеткізілген өнім сіздің күткеніңізге дейін төлем жасау керек болғанда. Сатушы төлемін сақтау шарттары сатушы келісім-шартымен келісілген кезде анықталуы мүмкін.

## <a name="create-vendor-payment-retention-terms"></a>Сатушы төлемін сақтау шарттарын жасау

Сіз сатушының сақтау үшін төлем пайызын және шығарылатын бұрын сақталған сомалардың пайызын енгізе аласыз. Сомалар сатушы есеп-шоттарында келісім-шарт белгіленген аяқталу кезеңіне жеткенге дейін сақталады. Сақтау шарттарын орнатқаннан кейін, оларды сатушыға арналған кез келген жобаға қолдануға болады.

Сатушы төлемдерін сақтау шарттарын орнату және сақтау үшін келесі қадамдарды пайдаланыңыз. 

1. **Жобаларды басқару және есепке алу** > **Сақтау** > **Сатушының төлемін сақтау шарттары** тармағына өтіңіз.
2. Сатушының жаңа сақтау шартын қосу үшін **Жаңа** пәрменін таңдаңыз. Жаңа шартқа арналған **Ереже идентификаторы** мәні автоматты түрде енгізіледі. 
3. **Сипаттама** өрісіне қысқаша сипаттама енгізіп, **Шарттар** FastTab қойыншасында келесі үшін шарт мәндерін енгізу үшін **Жол қосу** пәрменін таңдаңыз.

   - **Жеткізілген бірліктер пайызы**: шарттың аяқталу пайызын енгізіңіз. Сомалар сатушы есеп-шоттарында жобаның аяқталу кезеңі белгіленген пайызға тең болғанға дейін сақталады. Мысалы, егер сіз 50,00 енгізсеңіз, онда жоба 50 пайыз аяқталғанға дейін сақталады.
   - **Сақтау пайызы**: сақталатын сатушы есеп-шотының сома пайызын енгізіңіз. Мысалы, егер сіз 10,00 енгізсеңіз, онда сатушы есеп-шоты сомасының 10 пайызы жоба **Өріске жеткізілген бірлік пайызы** мәнінде белгіленгендей аяқтау пайызына жеткенге дейін сақталады.
   - **Шығару пайызы**: жоба аяқталуының таңдалған деңгейіне шығарылатын бұрын сақталған кез келген соманың пайызын енгізу үшін **Жол қосу** пәрменін таңдаңыз.

> [!NOTE]
> Егер сізде жоба аяқталуының әртүрлі деңгейлері үшін бірнеше кезеңдер болса, әр сақтау ережелері үшін жеке сатушының сақтау шарты жолын енгізіңіз. Әрбір жолда жоба аяқталуының әр белгіленген деңгейі үшін әртүрлі сақтау пайызы және әртүрлі шығару пайызы көрсетілуі мүмкін.

Сатушыға арналған сақтау шарттарын жасағаннан кейін, шарттарды жобаға қолдануға болады.

## <a name="apply-vendor-retention-terms-to-a-project"></a>Жобаға сатушының сақтау шарттарын қолдану

1. **Жобаларды басқару және есепке алу** > **Жобалар** > **Барлық жобалар** тармағына өтіп, жоба тізімі бетінен жобаны ашыңыз.
2. **Сатушы келісімдері** FastTab қойыншасында **Жол қосу** пәрменін таңдаңыз.
3. **Тіркелгі кодының өрісі** параметрінде, келесі параметрлердің бірін таңдаңыз: 

   - **Кесте**: сатушының сақтау шарттары бір сатушыға қолданылады.
   - **Топ**: сатушының сақтау шарттары сатушылар тобындағы барлық сатушыларға қолданылады.
   - **Барлығы**: сатушының сақтау шарттары барлық сатушыға қолданылады.

4. **Сатушы/сатушы топ өрісі** параметрінде, сатушының сақтау шарттары қолданылатын сатушыны немесе сатушы тобын таңдаңыз. Алдыңғы қадамда **Барлық** параметрін таңдаған болсаңыз, бұл өріс қолжетімді болмайды.
5. **Сатушының сақтау шарттары** өрісінде, алдыңғы процедурада жасалған сақтау шарттарын таңдаңыз.
6. Егер де жобада сатушыға арналған төленген кезде төлеу (PWP) шарттары бар болса, жобаға **PWP шекті пайызы** өрісінде шекті пайызды енгізіңіз.

Сатушының сақтау шарттары сіздің сатушы үшін жасаған сатып алу тапсырыстарында да көрсетіледі.


[!INCLUDE[footer-include](../includes/footer-banner.md)]