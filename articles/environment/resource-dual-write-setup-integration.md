---
title: Project Operations бағдарламасын орнату және конфигурация деректерінің интеграциясы
description: Бұл мақалада Project Operations қос жазу карталарын орнату және теңшеу туралы ақпарат берілген.
author: sigitac
ms.date: 4/23/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d03393de893c39ceb53c06a3031395f765a26f55
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/18/2022
ms.locfileid: "9029159"
---
# <a name="project-operations-setup-and-configuration-data-integration"></a>Project Operations бағдарламасын орнату және конфигурация деректерінің интеграциясы

_**Қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Бұл мақалада орнату және конфигурация нысандары үшін Жоба операцияларының қосарлы жазу интеграциясы туралы ақпарат берілген.

## <a name="project-contracts-contract-lines-and-projects"></a>Жобалық келісімшарттар, келісімшарт жолдары және жобалар

Жобалық келісім-шарттар, келісімшарттық желілер және жобалар жылы жасалады Dataverse және қосымша есепке алу үшін қаржы және операция қолданбаларымен синхрондалады. Осы нысандардағы жазбаларды тек Dataverse платформасында жасауға және жоюға болады. Дегенмен, сату салығы тобының әдепкі мәндері және қаржылық өлшемдер сияқты есеп атрибуттарын қаржы және операциялар қолданбаларында осы жазбаларға қосуға болады.

  ![Жоба келісімшарты интеграциясының тұжырымдамалары.](./media/1ProjectContract.jpg)

Сатылым белсенділіктері, мүмкіндіктер және баға ұсыныстары бақыланады Dataverse және қаржы және операция қолданбаларымен синхрондамаңыз, себебі бұл әрекетпен байланысты төменгі ағындық есеп жоқ.

Жоба келісім-шартының функционалдығы Dataverse көмегімен қаржы және операциялық қолданбаларда жоба келісімшартының жазбасын жасайды **Жобаның келісімшарт тақырыптары (сату тапсырыстары)** кесте картасы. Dataverse бағдарламасында жобалық келісімшартты сақтау жобалық келісімшарттың тұтынушы нысаны жазбасының жасалуын іске қосады. Бұл жазба қаржы және операциялық қолданбаларға синхрондалады **Жобаны қаржыландыру көзі (msdyn\_ жобалық келісім-шарттарды бөлу ережелері)** кесте картасы. Бұл карта сонымен қатар жобалық келісімшарт бойынша тұтынушың қосу, жаңарту және жою әрекеттерін синхрондайды. Жобаның келісім-шартының тұтынушылары арасындағы есеп айырысу пайыздарын бөлу тек ішінде игеріледі Dataverse және қаржы және операциялар қолданбаларымен синхрондалмаған.

Жоба келісімшарты жасалғаннан кейін Dataverse, жоба есепшісі мына жерге өту арқылы қаржы және операциялық қолданбалардағы осы жоба келісімшартының есеп атрибуттарын жаңарта алады: **Жобаны басқару және бухгалтерлік есеп** > **Жоба келісімшарттары** > **Орнату** > **Әдепкі есепті көрсету**. Бухгалтер жоба келісімшартының тиісті жазбасын ашатын қаржы және операция қолданбаларында жоба келісімшартының идентификаторын таңдау арқылы сұралған жеткізу күні және келісімшарт сомасы сияқты операциялық жоба келісімшартының атрибуттарын қарай алады.Dataverse.

Жоба нысаны арқылы қаржы және операциялық қолданбаларға үндестіріледі **Жобалар V2 (msdyn\_ жобалар)** кесте картасы. Жоба бухгалтері келесі әрекеттерді орындай алады:

  - Келесіге өту арқылы қаржы және операциялық қолданбалардағы жобаларды қарап шығыңыз **Жобаны басқару және бухгалтерлік есеп** > **Барлық жобалар**. 
  - тармағына өту арқылы қаржы және операция қолданбаларында жобаның есеп атрибуттарын жаңартыңыз **Жобаны басқару және бухгалтерлік есеп** > **Барлық жобалар** > **Орнату** > **Әдепкі есепті көрсету**.  
  - Тиісті жоба жазбасын ашатын қаржы және операция қолданбаларында жоба идентификаторын таңдау арқылы болжалды басталу және аяқталу күндері сияқты операциялық жоба атрибуттарын қарап шығыңыз.Dataverse.

Жоба **Жобалық келісімшарт жолы** нысаны арқылы жоба келісімшартымен байланыстырылады.

Жобаның келісімшарттық желілері Dataverse көмегімен қаржы және операция қолданбаларында жоба келісім-шартының есепшот ережесін жасайды **Жобаның келісімшарт желілері (сату тапсырысының мәліметтері)** кесте картасы. Есепшот ұсыну әдісі қаржы және операциялар қолданбаларында жоба келісімшартының есепшот ережесінің түрін анықтайды:

  - Уақыт және материал бойынша шот ұсыну әдісі бар жобалық келісімшарт жолдары уақыт және материал түріндегі шот ұсыну ережесін жасайды.
  - Белгіленген баға бойынша шот ұсыну әдісінің келісімшарт жолдары аралық кезеңдегі шот ұсыну ережесін жасайды.

Жобаның келісім-шарт желілерін жобаның бухгалтері қаржы және операциялық қолданбаларға өту арқылы қарап шығуы мүмкін **Жобаны басқару және бухгалтерлік есеп** > **Жоба келісімшарттары** > **Орнату** > **Әдепкі есепті көрсету** туралы мәліметтерді қарап шығу **Келісімшарттық сызықтар** қойындысы. Бухгалтер сонымен қатар осы қойындыда тіркелген бағаны төлеу әдісінің келісім-шарт жолдары үшін әдепкі қаржылық өлшемдерді орната алады.

## <a name="billing-milestones"></a>Шот ұсыну кезеңдері

Белгіленген баға бойынша шот ұсыну әдісін пайдаланатын жобалық келісімшарт жолдарына шот ұсыну кезеңдері арқылы есеп-шот ұсынылады. Есеп айырысу кезеңдері қаржылық және операциялық қолданбалардағы есептік жазбадағы транзакцияларды жобалау үшін синхрондалады.**Жоба операцияларын біріктіру келісім-шарт сызығының кезеңдері (msdyn\_ келісім-шарттық мәндер кестесі)** кесте картасы.

  ![Шот ұсыну кезеңдерінің интеграциясы.](./media/2Milestones.jpg)

Бухгалтер **Жобаларды басқару және есеп** > **Жобалық келісімшарттар** > **Сақтау** > **Шоттағы транзакциялар** немесе **Жобаларды басқару және есеп** > **Барлық жобалар** > **Сақтау** > **Шоттағы транзакциялар** терезесіне өту арқылы шоттағы транзакцияларды қарап шығып, есеп төлсипаттарын қарап шыға алады.

Жобаның берілген келісімшарт жолы үшін шот ұсыну кезеңін алғаш жасаған кезде жүйе осы келісімшарт жолымен байланыстырылған жоба үшін белгіленген баға кірісін бағалау жобасын автоматты түрде жасайды. Белгіленген баға кірісін бағалау жобаларын **Жобаларды басқару және есеп** > **Белгіленген баға кірісін бағалау жобалары** параметріне өту арқылы қарап шығуға болады.

### <a name="project-tasks"></a>Жоба тапсырмалары

Жоба тапсырмалары арқылы қаржы және операциялық қолданбаларға үндестіріледі **Жоба тапсырмалары (msdyn\_ жобалық тапсырмалар)** кесте картасы тек анықтамалық мақсаттар үшін. Қаржы және операциялар қолданбалары арқылы операцияларды жасауға, жаңартуға және жоюға қолдау көрсетілмейді.

  ![Жобалық тапсырмалар интеграциясы.](./media/3Tasks.jpg)

## <a name="project-resources"></a>Жоба ресурстары

The **Жоба ресурстарының рөлдері** нысаны арқылы қаржы және операциялық қолданбалармен синхрондалады **Барлық компаниялар үшін жоба ресурсының рөлдері (bookableresourcecategories)** кесте картасы тек анықтамалық мақсаттар үшін. Себебі ресурстағы рөлдер Dataverse компанияға тән емес болса, жүйе қос жазуды біріктіру ауқымына кіретін барлық заңды тұлғалар үшін қаржы және операциялық қолданбалардағы сәйкес компанияға тән ресурс рөлдерінің жазбаларын автоматты түрде жасайды.

![Ресурс рөлдерін біріктіру.](./media/5Resources.jpg)

Жоба операцияларындағы жоба ресурстары ішінде сақталады Dataverse және қаржы және операциялар қолданбаларымен синхрондалмаған.

### <a name="transaction-categories"></a>Транзакция санаттары

Мәмілелер санаттары сақталады Dataverse көмегімен қаржы және операция қолданбаларымен синхрондалады **Жоба транзакция санаттары (msdyn\_ транзакция категориялары)** кесте картасы. Транзакция санатының жазбасы синхрондалғаннан кейін жүйе автоматты түрде төрт ортақ санат жазбасын жасайды. Әрбір жазба қаржы және операциялар қолданбаларындағы транзакция түріне сәйкес келеді және оларды транзакция санатының жазбасына байланыстырады.

![Транзакция санаттарын біріктіру.](./media/4TransactionCategories.jpg)

Бағалаулар мен нақты көрсеткіштер үшін транзакция санаттарын пайдалану жоба бухгалтері немесе жүйе әкімшісінің әрбір заңды нысанда тиісті жоба санаттарын жасауын қажет етеді. Қосымша ақпарат алу үшін [Жоба санаттарын конфигурациялау](../project-accounting/configure-project-categories.md) бөлімін қараңыз.