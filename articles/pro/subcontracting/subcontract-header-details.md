---
title: Қосалқы мердігерлерге арналған тақырып мәліметтері
description: Бұл мақалада Project Operations ішіндегі қосалқы мердігер тақырыбындағы мүмкіндіктер түсіндіріледі.
author: rumant
ms.date: 09/14/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 00b7c08235654d4bed0bcb4053d2044a3d092b54
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522567"
---
# <a name="header-details-for-subcontracts"></a>Қосалқы мердігерлерге арналған тақырып мәліметтері

_**Келесіге қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Бұл мақалада қосалқы мердігер тақырыбындағы функционалдылық түсіндіріледі Dynamics 365 Project Operations.

Жоба менеджері жобаларды жоспарлайтын және орындайтын болғандықтан, олар қосалқы мердігерлерді жалдап, сатушылардан өнімдер мен қызметтерді сатып ала алады. Жоба менеджеріне өнімдерді немесе қызметтерді сатып алу қажет болғанда, олар Project Operations бағдарламасында қосалқы мердігерлік келісім-шарт жасай алады.

Қосалқы мердігерлік келісім-шарт жасау үшін келесі қадамдарды орындаңыз.

1. Навигация тақтасында **Қосалқы мердігерлер** опциясын таңдап, **Қосалқы мердігерлік келісім-шарт** бетінде **Жаңа** опциясын таңдаңыз.
2. Қажет ақпаратты енгізіп, **Сақтау** пәрменін таңдаңыз.

    Келесі кестеде **Қосалқы келісім-шарт тақырыбы** бетіндегі өрістер туралы ақпарат берілген.

    | Өріс | Сипаттамасы |Функциялық әсер |
    |---|------|---| 
    | Атауы | Қосалқы мердігерлік келісім-шарттың атауы. | Барлық қосалқы келісім-шарттық ашылмалы тізімдерде қосалқы келісім-шарттың атауы қосалқы келісім-шартты анықтауға көмектесу үшін бірінші бағанда көрсетілген. | 
    | Сипаттамасы | Қосалқы мердігерлік келісім-шарт бойынша сатып алынатын қызметтер мен өнімдердің қысқаша сипаттамасы. | Ешқайсысы |
    | Жеткізуші | Өнімдер мен қызметтер сатып алынатын компанияның атауы. Осы тіркелгі жазбасында **Сатушы** немесе **Жеткізуші** қатынас түрі бар. | Таңдалған жеткізуші негізінде келесі өрістер үшін әдепкі мәндер автоматты түрде енгізіледі:<br/> **• Валюта** </br> **• Бағатізбелер** </br> **• Төлем шарттары**</br> **• Төлем мекенжайы**</br> **• Шот ұсыну мекенжайы**</br> **• Есеп-шот шығару мекенжайындағы аты** </br>**• Сатушы шот менеджері**|
    | Қосалқы келісім-шарт күні | Қосалқы келісім-шарт жасалған күн. | Қосалқы келісім-шарт күні тиісті жеткізушіге бекітілген бағатізбелерден немесе жоба параметрлерінен сатып алудың дұрыс бағасын таңдау үшін қолданылады. |
    | Күй себебіі | Қосалқы мердігерлік келісім-шарт күйі. | Күй қосалқы келісім-шарттың бизнес процесінің қай бөлігінде екенін және оны өңдеуге болатынын анықтайды. <br/>Мәндерге мыналар жатады:<br>• **Жоба**: қосалқы келісім-шартты өңдеуге болады. Қосалқы келісім-шарттарды **Жоба** күйімен өңдеуге болады.<br/>• **Расталған**: жеткізушімен келіссөз аяқталды және жеткізілімге қосалқы келісім-шарт мақұлданды. <br/>• **Жабық**: қосалқы келісім-шарт бойынша жеткізу аяқталды.<br/>• **Бас тартылды**: қосалқы келісім-шарт жойылды және жеткізілім жоспарланбаған.  | 
    | Валюта | Өнімдер мен қызметтерді сатып алатын валюта. Әдепкі мән жеткізуші шотынан автоматты түрде енгізіледі, бірақ оны өзгертуге болады. | Қосалқы келісім-шарт валютасы тиісті жеткізушіге бекітілген бағатізбелерден немесе жоба параметрлерінен сатып алудың бағасын таңдау үшін пайдаланылады. Басқа валютадағы бағатізбелерді қосалқы келісім-шартпен байланыстыру мүмкін емес, Осы қосалқы келісім-шарттан жеткізуші ресурстар жеткізетін уақыт, шығындар мен материалдардың құны жоба бойынша осы валютада жазылады. Қосалқы келісім-шарт жазбасы сақталғаннан кейін қосалқы келісім-шарттағы валютаны өзгерту мүмкін емес.|
    | Келісім-шарт бірлігі | Сатып алу келісім-шартын немесе сатушымен қосалқы мердігерлік келісім-шарт жасайтын компания бөлімі. | Ешқайсысы |
    | Төлем шарттары | Осы қосалқы келісім-шарт бойынша ұсынылатын жеткізуші шот-фактуралары бойынша төлем шарттары. Әдепкі мән жеткізуші шотының жазбасынан автоматты түрде енгізіледі. | Қосалқы келісім-шарт бойынша төлем шарттары осы қосалқы келісім-шартқа байланысты барлық жеткізушілердің шот-фактураларына көшіріледі. Егер қосалқы келісім-шарттың **Жоба** күйі болса, төлем шарттарын жаңартуға болады. | 
    | Төлем мекенжайы | Төлемдер жіберілуі керек жеткізуші мекенжайы. Әдепкі мән жеткізуші шотының жазбасынан автоматты түрде енгізіледі. | Қосалқы келісім-шарттағы төлем мекенжайы осы қосалқы келісім-шарт үшін жасалған барлық жеткізуші шот-фактураларына төлем мекенжайы ретінде көшіріледі. Егер қосалқы келісім-шарттың **Жоба** күйі болса, төлем мекенжайын жаңартуға болады.|
    | Есеп-шот шығару мекенжайындағы аты | Шот-фактураны жіберетін сатушының компаниясындағы адамның немесе бөлімнің аты. Әдепкі мән жеткізуші шотының жазбасынан автоматты түрде енгізіледі. | Қосалқы келісім-шарт бойынша **Есеп-шот шығару мекенжайындағы аты** мәні осы қосалқы келісім-шартқа байланысты барлық жеткізушілердің шот-фактураларына көшіріледі. Егер қосалқы келісім-шарттың **Жоба** күйі болса, осы өрісті жаңартуға болады.|
    | Шот ұсыну мекенжайы | Жеткізушінің шот-фактураларында пайдаланылатын мекенжай. Әдепкі мән жеткізуші шотының жазбасынан автоматты түрде енгізіледі. | Бұл мекенжай — осы қосалқы келісім-шарт үшін жасалған жеткізуші есеп-шоттарындағы "есеп-шот" мекенжайы. |
    | Аралық қорытынды | Егер қосалқы келісім-шартта жолдар болмаса, салықтардың алдында тапсырыстың қосалқы жиынтығын енгізіңіз. Егер қосалқы мердігерлік келісім-шартта жолдар болса, бұл өріс тек оқуға арналған. Көрсетілген сома қосалқы келісім-шарттағы барлық жолдардың жиынтық сомасы болып табылады. | Ешқайсысы |
    | Жиынтық табыс салығы | Егер қосалқы келісім-шартта жолдар болмаса, осы қосалқы келісім-шарттағы жалпы салықтарды енгізіңіз. Егер қосалқы мердігерлік келісім-шартта жолдар болса, бұл өріс тек оқуға арналған. Көрсетілген сома қосалқы келісім-шарттағы барлық жолдардың салық сомасының қосындысы болып табылады. | Ешқайсысы |
    | Жалпы сома | Бұл есептелген өріс салықтар қосылғаннан кейін қосалқы мердігерлік келісім-шарттың жалпы сомасын көрсетеді. | Ешқайсысы |
    | Расталған күн | Қосалқы келісім-шарт расталған күн. | Ешқайсысы |
    | Сұраған | Әдепкі бойынша бұл өріс қосалқы келісім-шарт жасайтын пайдаланушының атына орнатылады. Алайда қосалқы келісім-шартты жасаушы оның атынан қосалқы келісім-шарт жасайтын адамды көрсету үшін мәнді өзгерте алады. | Ешқайсысы |
    | Сатушы шот менеджері | Сатушы тіркелгісінің негізгі контактісінің атауы. Әдепкі мән жеткізуші шотының жазбасынан автоматты түрде енгізіледі. Қосалқы келісім-шарттың жеткізуші шотының менеджері ретінде басқа контактіні таңдай аласыз. | Баға келіссөздерінің нәтижесі ретінде қосалқы келісім-шартқа өзгерістер енгізілгенде контактіге хабарлау үшін электрондық пошта ескертулерін орнатуға болады. |