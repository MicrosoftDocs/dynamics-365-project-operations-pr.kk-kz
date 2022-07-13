---
title: Уақыт бойынша жеткізушінің есеп-шот желілері
description: Бұл мақалада қосалқы мердігерлер енгізген уақыт шығындары үшін жеткізушінің шот-фактура желілерін қалай жазу керектігі түсіндіріледі.
author: rumant
ms.date: 03/15/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 0b81d2884580e9054457906627c1f9101f435524
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927549"
---
# <a name="vendor-invoice-lines-for-time"></a>Уақыт бойынша жеткізушінің есеп-шот желілері

[!include [banner](../../includes/dataverse-preview.md)]

_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_

Microsoft корпорациясындағы жеткізушінің шот-фактурасы Dynamics 365 Project Operations уақыт бойынша жеткізушінің шот-фактура желілері болуы мүмкін. Жоба менеджерлері жобалар бойынша қосалқы мердігер уақытының шығындарын жазу үшін уақыт үшін жеткізушінің шот-фактура желілерін пайдалана алады.

Уақыт бойынша жеткізушінің шот-фактура желілері уақыт бойынша қосалқы мердігер сызығына сілтеме жасай алады немесе болмауы мүмкін. Уақыт бойынша жеткізушінің шот-фактура желісі қосалқы мердігерге сілтеме жасаса, жоба менеджерлері жеткізушінің шот-фактура желісі арқылы шот-фактура жазып жатқан уақытты қосалқы мердігерлер жазып алған және жоба бойынша жоба менеджерлері бекіткен уақытпен салыстырып, тексере алады.

Келесі кестеде уақыт бойынша жеткізушінің шот-фактура жолдарының өрістері туралы ақпарат берілген.

| Өріс | Сипаттама | Функциялық әсер |
| --- | --- | --- |
| Аты | Сәйкестендіруге көмектесу үшін жеткізушінің шот-фактура желісінің атауы. | Бұл атау жеткізушінің шот-фактура жолдарына негізделген барлық іздеулерде бірінші баған ретінде көрсетіледі. |
| Сипаттама | Жеткізуші шот-фактура жолында жеткізуші шот-фактурасын жасайтын қызметтердің қысқаша сипаттамасы. | Ешқандай |
| Қосалқы келісім-шарт | Қызметтерге бастапқыда тапсырыс берілген қосалқы мердігер. | Жеткізушінің шот-фактурасы үшін қосалқы мердігер таңдалғанда, жеткізушінің шот-фактурасындағы барлық жолдар сол таңдауды мұраға алады. Жеткізуші шот-фактурасында әртүрлі қосалқы мердігерлерге сілтеме жасайтын жеткізушінің шот-фактура жолдары болуы мүмкін емес. |
| Қосалқы мердігер сызығы | Қызметтерге тапсырыс берілген қосалқы мердігер сызығы. Таңдауға болатын қосалқы мердігерлік желілердің тізімі таңдалған қосалқы мердігердегі жолдармен шектеледі. | Уақыт бойынша жеткізушінің шот-фактура жолында қосалқы мердігер сызығы таңдалғанда, үшін әдепкі мәндер **Жоба**, **·**, және **Тапсыруға болатын ресурс** өрістер қосалқы мердігер жолындағы сәйкес өрістерден енгізіледі. Таңдалған қосалқы мердігер жолында мәндер болса **Жоба**, **·**, және **Брондау мүмкін** өрістерде, жеткізушінің шот-фактура жолындағы сәйкес өрістердің мәндері сол мәндерден өзгеше болмауы керек. |
| Транзакция күні | Жеткізушінің шот-фактура желісінің нақты құны жобаға жазылатын күн. | Ешқандай |
| Транзакция класы | Әдепкі мән — **Уақыт**. | Мән **Уақыт** жеткізушінің шот-фактура желісі қосалқы мердігер уақытының шот-фактура сомасын жазу үшін пайдаланылатынын көрсетеді. |
| Project | Шот-фактура жасалып жатқан қызметтер пайдаланылған жобаның атауы. | Бұл өріс міндетті және бос қалдыруға болмайды. |
| Тапсырма | Есептелетін қызметтер пайдаланылған жоба тапсырмасының атауы. Бұл өріс жоба таңдалған жағдайда ғана қолжетімді. Жоба тапсырмасын таңдау міндетті емес. | Бұл өріс бос қалдырылса, жоба менеджері жеткізушінің шот-фактура жолын жобаның кез келген тапсырмасы бойынша қосалқы мердігер ресурстарымен жазылған уақытқа сәйкестендіре алады. Егер жеткізушінің шот-фактурасы жолында қосалқы мердігер сызығына сілтеме жасалмаса және бұл өріс бос қалдырылса, жеткізушінің шот-фактура жолы арқылы жасалған нақты құн шотсыз сату фактілерімен байланыстырылмайды. Бұл жағдайда, егер тапсырмаға негізделген есепшот орнатылса, шығындар соңғы тұтынушыға шот-фактураға түспеуі мүмкін. |
| Рөл | Уақыты есептелетін қосалқы мердігер ресурстарының рөлі. | Бұл өріс жеткізушінің шот-фактурасында уақыты көрсетілген қосалқы мердігер ресурстарымен орындалатын рөлді көрсетеді. |
| Тапсырыс беруге болатын ресурс | Уақыты шот-фактура жасалып жатқан қосалқы мердігердің аты-жөні. Брондалуға болатын ресурсты таңдау міндетті емес. | Бұл өріс бос қалдырылса, жоба менеджері жеткізушінің шот-фактура жолында жеткізушіге тиесілі кез келген ресурспен жазылған уақытпен жеткізушінің шот-фактура жолын сәйкестендіре алады. |
| Шама | Шот-фактура жолында жеткізуші шот-фактура жазып жатқан уақыт санын енгізіңіз. |Ешқандай |
| Бірлік тобы | Әдепкі мән **Уақыт бірлігі тобы** және өзгерту мүмкін емес. | Ешқандай |
| Бірлік | Әдепкі мән уақыт бірлігі тобынан сағаттардың негізгі бірлігі болып табылады. Бұл мәнді күн немесе апта сияқты уақыт бірлігі тобының кез келген бірлігінде сатып алу үшін өзгертуге болады. | комбинациясы **Рөл** және **Бірлік** мәндері үшін әдепкі немесе есептелген мән ретінде пайдаланылады **Тауар өлшемінің бағасы** жеткізушінің шот-фактура жолындағы өріс. |
| Бірлік бағасы | Әдепкі бірлік бағасы комбинациясын пайдаланады **Рөл** және **Бірлік** жеткізушінің шот-фактура желісінің транзакция күніне қолданылатын жобаның прейскурантындағы мәндер. | Қолданыстағы жобаның прайс-парақшасының бағасы жеткізушінің шот-фактура жолындағы бірліктен ерекшеленетін бірлікте орнатылса, жүйе бірліктің бағасын есептеу үшін бірлікті түрлендіруді пайдаланады. |
| Аралық қорытынды | Бұл тек оқуға арналған өріс ретінде есептеледі *Саны*&times;*Тауар өлшемінің бағасы*, мәндер екеуінде де енгізілсе **Саны** өріс және **Тауар өлшемінің бағасы** өріс. Бір немесе екеуі де бос болса, осы өріске мән енгізуге болады. | Ешқандай |
| Сатылым салығы | Сату салығы сомасын енгізіңіз. | Ешқандай |
| Жалпы сома | Салықтарды қоса алғанда, жеткізуші шот-фактурасының жалпы сомасы. Бұл өріс келесідей есептеледі *Аралық жиынтық* + *Сату салығы*. | Ешқандай |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]