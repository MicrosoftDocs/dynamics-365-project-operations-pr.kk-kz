---
title: Project Operations жүйесіндегі жеткізуші және сатып алу бойынша бағатізбені басқару
description: Бұл мақалада жеткізуші деректерін және қосалқы мердігерлердің сатып алу бағасы тізімдерін жасауға және қолдауға көмектесетін ақпарат берілген.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 3cd883fed8a59f1c54c39e2d051b9748833ba692
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261894"
---
# <a name="vendor-and-purchase-price-list-management-in-project-operations"></a>Project Operations жүйесіндегі жеткізуші және сатып алу бойынша бағатізбені басқару


_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_

## <a name="vendors-in-project-operations"></a>Project Operations жүйесіндегі жеткізушілер

Microsoft Dynamics 365 Project Operations жүйесінде сатып алушы тіркелгілерінде **Сатушы** немесе **Жеткізуші** түріндегі қатынас болады. Қосалқы келісімшарт бойынша сатушы ретінде осы қатынас түрлерінің бірі бар тіркелгі жазбасын ғана таңдауға болады.

Бір немесе бірнеше сатып алу бағатізбелерін сатушы жазбасымен байланыстыруға болады. Дегенмен, жеткізуші жазбаларымен байланысты әрбір сатып алу бағатізбесі нақты күндік тиімділікке ие болуы керек. Project Operations жүйесі сатып алу бағатізбелеріне сәйкес келетін күндердің тиімділігін қолдамайды.

Әдепкі бойынша, жеткізуші жазбасындағы келесі өрістер мен түсініктер жеткізуші үшін жасалған кез келген қосалқы келісім үшін қолданылады:

- Төлем шарттары
- Есепшот ұсынылатын контакт
- Негізгі контакт

    > [!NOTE]
    > Әдепкі бойынша, жеткізушінің негізгі байланысы қосалқы келісімшарттың жеткізуші шотының менеджері ретінде пайдаланылады.

- Валюта
- Ағымдағы сатып алу бағатізбелері

## <a name="purchase-price-lists-in-project-operations"></a>Project Operations жүйесіндегі сатып алу бағатізбелері

**Контекст** өрісі **Сатып алу** өрісіне орнатылатын бағатізбе сатып алу бағатізбесі ретінде қарастырылады. Сатып алу бағатізбесін уақыт, шығындар мен материалдар бойынша сатып алу бағаларының каталогын көрсету үшін анықтауға болады. Сатып алу бағатізбелері Project Operations бағдарламасындағы шығындар мен сатылым бағатізбелеріне ұқсайды. Келесі түсініктер сатып алу бағатізбесіне шығындар мен сатылым бағатізбелеріне қолданылатын әдіспен қолданылады:

- **Күн тиімділігі** - сатып алу бағатізбелерінде күн тиімділігі бар. Күн тиімділігі әр бағатізбедегі басталу және аяқталу күндері өрістерімен көрсетіледі. Басталу мен аяқталу күндерінің арасындағы уақыт — күшіне енетін күн мерзімі.
- **Валюта** — бағатізбедегі валюта сатып алу бағатізбелері еңбек, шығын санаттары мен каталогтағы өнімдер үшін көрсетілген валюта ретінде пайдаланылады.
- **Әдепкі уақыт бірлігі** — әдепкі уақыт бірлігі сатып алудағы еңбек бағасын көрсетеді. Бағатізбедегі уақыт бірлігі өрісі тек әдепкі мәнді беру үшін пайдаланылады. Бұл мәнді жеке рөлдік баға жолдарында өзгертуге болады.

Сатып алу бағатізбелері жеткізушілердің жазбаларына жобалық бағатізбе ретінде белгілі байланыстар ретінде қосылуы мүмкін. Бұл бағатізбелер қосалқы келісімшарт жолдарындағы әдепкі бағаларды енгізу үшін пайдаланылады. Әдепкі бойынша, сатушы жазбасына бірнеше сатып алу бағатізбелері тіркелген кезде, ең соңғы бағатізбе сатушы үшін жасалған қосалқы келісімшарттар үшін пайдаланылады. Сатушы жазбаларына **Контекст** өрісі **Сатып алу** күйіне орнатылатын бағатізбелер ғана тіркеледі.

### <a name="subcontract-specific-purchase-price-lists"></a>Қосалқы келісімшартқа сәйкес сатып алу бағатізбелері

Сатып алу бағатізбелері қосалқы келісімшарттарға жобалық бағатізбе ретінде белгілі байланыстар ретінде қосылуы мүмкін. Бұл бағатізбелер қосалқы келісімшарт жолдарындағы әдепкі бағаларды енгізу үшін пайдаланылады. Әдепкі бойынша, қосалқы келісімшартқа бірнеше сатып алу бағатізбесі қосылған кезде, олардың әрқайсысының нақты күндік тиімділігі болуы керек. Project Operations жүйесі қабаттасатын күн тиімділігі бар сатып алу бағатізбелеріне қолдау көрсетпейді. Қосалқы келісімшарттарға **Контекст** өрісі **Сатып алу** күйіне орнатылатын бағатізбелер ғана тіркеледі.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]