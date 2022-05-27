---
title: Бірнеше тұтынушыны жоба келісім-шарттары бойынша басқару
description: Бұл тақырыпта жоба келісім-шарты бойынша бірнеше тұтынушыны басқару жолдары туралы ақпарат берілген.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1adb786c36d43a148e8c5a8b25ded5a997557119f7e6e9e2248935ad4ed211d5
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "6992078"
---
# <a name="manage-multiple-customers-on-project-contracts"></a>Бірнеше тұтынушыны жоба келісім-шарттары бойынша басқару

Бұл тақырыпта жоба келісім-шарты бойынша бірнеше тұтынушыны басқару жолдары туралы ақпарат берілген. Мәмілені қаржыландыру үшін бірнеше тұтынушыға арналған келісім-шарт қажет болған кезде жоба келісім-шартын пайдалана аласыз. **Жоба келісім-шарты** бетінде, **Қорытынды** қойыншасы мәміле жасасу үшін алғашқы тұтынушы туралы ақпаратты қамтиды. Мәмілеге қатысатын басқа тұтынушыларды **Тұтынушылар** қойыншасына қосуға болады.

Жоба келісім-шартының **Тұтынушылар** қойыншасындағы барлық келісім-шарт жолы тұтынушылары әдепкі бойынша жоба келісім-шарты үшін жасалған кез келген жаңа жобаға негізделген келісім-шарт жолы тұтынушылары болып табылады. Бұрыннан бар кез келген жобаға негізделген келісім-шарт жолдары кейіннен жасалған жаңа келісім-шарт тұтынушылар жазбаларына иелік етпейді.

Келісім-шарт пен келісім-шарт жолы тұтынушыларын келісім-шарт жеңіп алынғанға дейін кез келген уақытта қосуға, жаңартуға немесе жоюға болады. Жоба келісім-шартындағы тұтынушы иеленуші компаниясының немесе заңды тұлғаның **Тұтынушылар** бетінде тұтынушы ретінде орнатылуы керек. Dynamics 365 Project Operations бағдарламасының **Жобаларды басқару және бухгалтерлік есеп** модулінде орнатылған заңды тұлғалар және Project Operations бағдарламасының **Жоба сатылымы** және **Жеткізу** модульдерінде компаниялар ретінде қолжетімді.

## <a name="primary-customers"></a>Бастапқы тұтынушылар

Жоба келісім-шартының **Қысқаша мазмұны** қойыншасындағы тізімде көрсетілген тұтынушы алғашқы тұтынушы ретінде келісім-шарттың ықтимал тұтынушысы болып табылады. Алғашқы тұтынушыны келісім-шарт тұтынушысы тізімінен жаңарту мүмкін емес. Алғашқы тұтынушыны келісім-шарттағы тұтынушылар тізімінен өшіруге тырыссаңыз, сіз келісім-шарттағы алғашқы тұтынушының жазбасын жою мүмкін емес деген қате орын алады. Оның орнына, жоба келісім-шартындағы **Қорытынды** қойыншасының **Ықтимал тұтынушы** өрісіндегі тұтынушыны өзгертіңіз. Бұл өрісті жаңартқан кезде келісім-шарттың қысқаша мазмұны бетінде жаңартылған кезде, жаңадан таңдалған тұтынушы жаңа келісім-шарт тұтынушысы ретінде қосылады және **Алғашқы** жалаушасы **Иә** мәніне орнатылады. Бұрынғы алғашқы тұтынушы әлі де келісім-шарт бойынша тұтынушы болып табылады, алайда олар енді негізгі тапсырыс беруші болып табылмайды.

## <a name="create-update-or-delete-a-contract-customer-record"></a>Келісім-шарт тұтынушысының жазбасын жасау, жаңарту немесе жою

Келісім-шарт тұтынушысын **Келісім-шарт** бетіндегі **Келісім-шарт тұтынушылары** қойыншасынан жасауға, жаңартуға немесе жоюға болады. Келесі өрістер жоба келісім-шартының келісім-шарт тұтынушысының жазбасында қамтылады.

| **Өріс** | **Орны** | **Сипаттамасы** | 
| --- | --- | --- | 
| Тіркелгі | **Келісім-шарт тұтынушылары** қойыншасындағы өңдеуге болатын тор және келісім-шарт тұтынушысына арналған негізгі және жылдам жасау беттері. | Барлық белсенді тіркелгілердің тізімін көрсетеді. Бұл өріс жазба жасалғаннан кейін бұғатталады. Жазбаны жаңарту үшін оны жойып, содан кейін қайта жасаңыз. Егер сіз қандай да бір нақты көрсеткіштерді тіркеген болсаңыз немесе келісім-шарт тұтынушысы жазбасы алғашқы тұтынушы болса, сіз жазбаны жоя алмайсыз. Келісім-шарт жолы жасалған кезде, келісім-шарт тұтынушылары келісім-шарт жолы тұтынушылары ретінде көшіріледі. |
| Есеп айырысу бөліну пайызы | **Келісім-шарт тұтынушылары** қойыншасындағы өңдеуге болатын тор және келісім-шарт тұтынушысына арналған негізгі және жылдам жасау беттері. | Келісім-шарт жолы тұтынушысына жатқызылатын әрбір төлем жасалмаған сатылым транзакциясының пайызын білдіреді. Жаңа жоба бойынша келісім-шарт жолдары жасалған кезде, төлемнің бөліну пайызы жасалған жаңа кез келген келісім-шарт жолдарына және жобаның келісім-шарт жолы тұтынушыларына көшіріледі. |
| Есеп-шот шығарылатын істес кісі | **Келісім-шарт тұтынушылары** қойыншасындағы өңдеуге болатын тор және келісім-шарт тұтынушысына арналған негізгі және жылдам жасау беттері. | Бұл мәтін өрісі тұтынушы үшін есеп-шоттағы байланыс тұлғасын анықтау үшін пайдаланылуы керек. Әдепкі мән қатысты тіркелгі жазбасынан алынады. Байланыс тұлғасы осы тұтынушы үшін жасалған есеп-шоттағы **Шот жіберілетін байланыс тұлғасы** өрісіне көшіріледі. |
| Есеп-шот шығару мекенжайындағы аты | **Келісім-шарт тұтынушылары** қойыншасындағы өңдеуге болатын тор және келісім-шарт тұтынушысына арналған негізгі және жылдам жасау беттері. | Бұл өрісті тұтынушы үшін есеп-шоттағы байланыс тұлғасын анықтау үшін пайдалану керек. Әдепкі мән қатысты тіркелгі жазбасынан алынады. Есім осы тұтынушы үшін жасалған есеп-шоттағы **Шот жіберілетін байланыс тұлғасы** өрісіне көшіріледі. |
| Төлем шарттары | **Келісім-шарт тұтынушылары** қойыншасындағы өңдеуге болатын тор және келісім-шарт тұтынушысына арналған негізгі және жылдам жасау беттері. | Әдепкі мән қатысты тіркелгі жазбасынан алынады. Шарттар осы тұтынушы үшін жасалған есеп-шоттағы **Шот жіберілетін байланыс тұлғасы** өрісіне көшіріледі. |
| Иеленуші компания | **Жоба келісім-шарт тұтынушылары** қойыншасындағы өңдеуге болатын тор және жоба келісім-шарт тұтынушысына арналған негізгі және жылдам жасау беттері. | Тұтынушы **Жобаны басқару және бухгалтерлік есеп** модулінде орнатылған заңды тұлға. Бұл өріс тек оқуға арналған және жоба келісім-шартының иеленуші компаниясы үшін орнатылған.</br>**Тіркелгі** өрісіне қосылатын тұтынушылар тізімі Project Operations **Жобаларды басқару және есепке алу** модуліндегі меншік иесінің тізіміне сүзгіленеді. Иеленуші компания заңды тұлғаға тең Project Operations бағдарламасының **Жобаларды басқару және бухгалтерлік есеп** модулі. Жобадан түскен барлық шығыстар мен кірістер иеленуші компанияның бас кітабында есепке алынады. |
| Дөңгелектеу | **Келісім-шарт тұтынушылары** қойыншасындағы өңдеуге болатын тор және келісім-шарт тұтынушысына арналған негізгі және жылдам жасау беттері. | Тұтынушы мәміле бойынша әдепкі дөңгелектеу тұтынушысы болып табылатындығын көрсетеді. Жоба келісім-шарты бойынша тек бір дөңгелектеу тұтынушысы болуы мүмкін. Шығындар мен төленбеген сатылымдарды саны бойынша бөлініп, дөңгелектеу айырмашылығына әкелсе, бұл айырмашылық тұтынушымен салыстырылатын нақты мәнге қолданылады. |
| Асырмау шегі | **Келісім-шарт тұтынушылары** қойыншасындағы өңдеуге болатын тор және келісім-шарт тұтынушысына арналған негізгі және жылдам жасау беттері. | Тұтынушыға өзара әрекеттесу үшін есеп-шот жасалатын жалпы соманың келісілген шегі немесе ең жоғарғы шегін көрсетеді. Келісім-шарт тұтынушысы деңгейінде белгіленген асырмау шегі осы келісім-шарт тұтынушысына сілтеме жасайтын шот ұсынылмаған сатылымның нақты көрсеткіштері бойынша бағаланады. |

## <a name="edit-billing-split-percentages"></a>Төлемнің бөліну пайызын өңдеу

Есеп айырысудың пайыздық мөлшерлемесін торды өңдеу арқылы өңдеуге болады. Есеп айырысудың пайыздық мөлшерлемесі 100 пайызды құрамаған жағдайда, қате пайда болады. Есеп айырысудың пайыздық мөлшерлемесін өңдегеннен кейін, қатені жою үшін **Жоба келісім-шарты** бетін жаңартыңыз.

Сондай-ақ жоба келісім-шарты тұтынушылары қосалқы торында **Біркелкі тарату** пәрменін таңдай аласыз. Есеп айырысу жоба келісім-шарты бойынша барлық тұтынушыларға біркелкі бөлінеді. Дөңгелектеу коэффициенті бар болса, коэффициент дөңгелектеу тұтынушысына қосылады. Келісім-шарт бойынша тұтынушылардың әрқайсысында **Дөңгелектеу** жалаушасы **Иә** мәніне орнатылды. Бұл тұтынушы — дөңгелектеу тұтынушысы. Әдетте дөңгелектеу тұтынушысы келісім-шарттың негізгі тұтынушысы болып табылады, бірақ бұл талап етілмейді.


[!INCLUDE[footer-include](../includes/footer-banner.md)]