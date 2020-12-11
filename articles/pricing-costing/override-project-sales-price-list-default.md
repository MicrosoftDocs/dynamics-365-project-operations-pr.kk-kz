---
title: Жоба сатылымдарының бағатізбелерін алдын ала анықтау
description: Бұл тақырыпта реттелетін сатылым бағатізбелерін жасау туралы ақпарат беріледі.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c97dca8685c2db7d256017cf4442416feb0e005b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130855"
---
# <a name="override-project-sales-price-lists"></a>Жоба сатылымдарының бағатізбелерін алдын ала анықтау

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

## <a name="customer-specific-project-price-lists"></a>Тұтынушыларға арналған жоба бағатізбелері

Тұтынушыларға арналған бағалық келісімдерді Dynamics 365 Project Operations жүйесіндегі шот жазбасында жобаның бағатізбесі ретінде орнатуға болады.

Тұтынушыларға арналған жоба бағатізбесін жасау үшін **Сатылым** аймағында шот жазбасына өтіңіз.

1. **Шоттар** тізім бетін ашыңыз.
2. **Шот** мәліметтер бетін ашу үшін тұтынушы жазбасын тауып, екі рет шертіңіз.
3. **Жобаның бағатізбелері** қойыншасында **+ Жаңа жобалық бағатізбе^^ опциясын таңдаңыз.
4. **Жаңа жобалық бағатізбе** бетінде ашылмалы тізімнен бағатізбені таңдаңыз. Тек контексті **Сатылым** күйіне орнатылған және валютасы шот валютасына сәйкес келетін бағатізбелер қосылады.
5. Байланыс атауын енгізіп, содан соң **Сақтау** түймешігін басыңыз. Тұтынушыларға арналған жоба бағатізбесі жасалды. Бұл бағатізбе баға ұсынысының немесе жобалық келісім-шарттың жасалған күні бағатізбенің күшіне ену күніне сәйкес келетін, тұтынушы үшін жасалған жобалық баға ұсыныстары мен келісім-шарттардағы әдепкі жобаға пайдаланылады.

## <a name="custom-pricing-on-project-quotes"></a>Жоба баға ұсыныстарындағы реттелетін баға белгілеу

Жобалық баға ұсыныстарында тұтынушыдан немесе жобалық параметрлерден әдепкі бойынша алынатын әдепкі стандартты бағатізбеден басталатын жобалық бағаға ие боласыз.

Белгілі бір баға ұсынысы бойынша жобамен байланысты жұмыс үшін реттелетін баға белгілеу қажет болғанда, сіз оны жобалық бағатізбелермен байланысты нысаннан ала аласыз.

Баға ұсынысына арналған жобалық баға белгілеуді орнату үшін келесі қадамдарды орындаңыз.

1. Жобалық баға ұсынысын ашып, **Жобаның бағатізбелері** қойыншасын таңдаңыз.
2. Ішкі торда **Реттелетін баға жасау** опциясын таңдаңыз.

Баға ұсынысына тіркелген жобаның барлық бағатізбелері жаңа бағатізбелерге көшіріледі. Жаңа бағатізбелер атаулары осы бағатізбелер жасалған кездегі күні мен уақыты көрсетілген баға ұсынысының атауын көрсетеді.

Сіз осы бағатізбелердің әрқайсысын пайдалана аласыз, сондай-ақ еңбек (рөл бағасы) және шығындар (санат бағасы) бағаларына жаңартулар енгізе аласыз. Бұл бағалар тек осы баға ұсыныстарына қолданылатын болады.

## <a name="price-lists-on-a-project-contract"></a>Жоба келісім-шартындағы бағатізбелер

Жобалық келісім-шартта жоба бағасы келісім-шарт атауы мен атауға қосылатын жасалған күн уақыты белгісімен әрдайым реттелетін бағатізбе ретінде әдепкі мән ретінде алынады. Бұл келісім-шарт баға ұсынысы ұтқан кезде жасалуына немесе келісім-шарттың нөлден жасалуына тәуелсіз түрде рас болып табылады. Қажет болса, бұл байланысты реттелетін бағатізбемен алып тастай аласыз және оның орнына стандартты бағатізбені жоба келісім-шартымен байланыстыра аласыз.

Стандартты бағатізбені баға ұсынысы немесе келісім-шарттағы жобаның бағатізбелерге байланыстырған кезде, бағатізбедегі бағалардағы кез келген өзгертулер бағатізбені пайдаланатын барлық баға ұсыныстарына және келісім-шарттарға әсер етеді.