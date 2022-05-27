---
title: Project Operations бағдарламасын орнату және конфигурация деректерінің интеграциясы
description: Бұл тақырып Project Operations қос жазу карталарын орнату және конфигурациялау туралы ақпарат береді.
author: sigitac
ms.date: 4/23/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6d263f7c5ef0d562edde6a603340a3b8746195df190fdb527bfa40297f68eed2
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986543"
---
# <a name="project-operations-setup-and-configuration-data-integration"></a>Project Operations бағдарламасын орнату және конфигурация деректерінің интеграциясы

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Бұл тақырып орнату және конфигурация нысандарына арналған Project Operations қос жазу интеграциясы туралы ақпарат береді.

## <a name="project-contracts-contract-lines-and-projects"></a>Жобалық келісімшарттар, келісімшарт жолдары және жобалар

Жобалық келісімшарттар, келісімшарт жолдары және жобалар Dataverse платформасында жасалып, қосымша есеп үшін Finance and Operations бағдарламаларына синхрондалады. Осы нысандардағы жазбаларды тек Dataverse платформасында жасауға және жоюға болады. Дегенмен сатылым салығының тобы секілді есеп төлсипаттары әдепкі бойынша жасалып, Finance and Operations бағдарламаларындағы осы жазбаларға қаржылық өлшемдер қосылуы мүмкін.

  ![Жоба келісімшарты интеграциясының тұжырымдамалары.](./media/1ProjectContract.jpg)

Сатылым әрекетінің ықтимал тұтынушылары және баға ұсыныстары Dataverse платформасында бақыланып. Finance and Operations бағдарламаларына синхрондалмайды, себебі осы әрекетпен байланысты төменгі есеп жоқ.

Dataverse платформасындағы келісімшарт функциялары **Жобалық келісім-шарт тақырыптары (сатылым тапсырысы)** кесте картасы арқылы Finance and Operations бағдарламаларында жобалық келісімшарт жазбасын жасайды. Dataverse бағдарламасында жобалық келісімшартты сақтау жобалық келісімшарттың тұтынушы нысаны жазбасының жасалуын іске қосады. Бұл жазба Finance and Operations бағдарламаларына **Жобаның қаржыландыру көзі (msdyn\_projectcontractssplitbillingrules)** кесте нысаны арқылы синхрондалады. Бұл карта сонымен қатар жобалық келісімшарт бойынша тұтынушың қосу, жаңарту және жою әрекеттерін синхрондайды. Жобалық келісімшарт тұтынушылары арасындағы бөлінген шот ұсыну пайызы тек Dataverse платформасында өңделеді және Finance and Operations бағдарламаларына синхрондалады.

Dataverse платформасында жобалық келісімшарт жасалғаннан кейін жоба бухгалтері **Жобаларды басқару және есеп** > **Жобалық келісімшарттар** > **Орнату** > **Әдепкі есепті көрсету** бөліміне өту арқылы Finance and Operations бағдарламаларында осы жоба келісімшарты үшін есеп төлсипаттарын жаңарта алады. Бухгалтер Dataverse бағдарламасында қатысты жобалық келісімшарт жазбасын ашатын Finance and Operations бағдарламаларында жобалық келісімшарт идентификаторын таңдау арқылы сұралған жеткізу күні және келісімшарт сомасы секілді операциялық жобалық келісімшарт төлсипаттарын қарап шыға алады.

Жоба нысаны **V2 жобалары (msdyn\_projects)** кесте нысаны арқылы Finance and Operations бағдарламаларына синхрондалады. Жоба бухгалтері келесі әрекеттерді орындай алады:

  - **Жобаларды басқару және есеп** > **Барлық жобалар** терезесіне өту арқылы Finance and Operations бағдарламаларындағы жобаларды қарап шығыңыз. 
  - **Жобаларды басқару және есеп** > **Барлық жобалар** > **Орнату** > **Әдепкі есепті көрсету** терезесіне өту арқылы Finance and Operations бағдарламаларында жобаның есеп төлсипаттарын жаңартыңыз.  
  - Dataverse бағдарламасында қатысты жоба жазбасын ашатын Finance and Operations бағдарламаларында жоба идентификаторын таңдау арқылы болжалды басталу және аяқталу күндері секілді операциялық жоба төлсипаттарын қарап шығыңыз.

Жоба **Жобалық келісімшарт жолы** нысаны арқылы жоба келісімшартымен байланыстырылады.

Dataverse платформасындағы жобалық келісімшарт жолдары **Жобалық келісімшарт жолдары (сатылым тапсырысы туралы мәліметтер)** кесте картасы арқылы Finance and Operations бағдарламаларында жобалық келісімшарт бойынша шот ұсыну ережесін жасайды. Шот ұсыну әдісі Finance and Operations бағдарламаларында жобалық келісімшарт бойынша шот ұсыну ереже түрін анықтайды:

  - Уақыт және материал бойынша шот ұсыну әдісі бар жобалық келісімшарт жолдары уақыт және материал түріндегі шот ұсыну ережесін жасайды.
  - Белгіленген баға бойынша шот ұсыну әдісінің келісімшарт жолдары аралық кезеңдегі шот ұсыну ережесін жасайды.

Жобалық келісімшарт жолдарын **Жобаларды басқару және есеп** > **Жоба келісімшарты** > **Орнату** > **Әдепкі есепті көрсету** бөліміне өтіп, **Келісімшарт жолдары** қойыншасындағы мәліметтерді қарап шығу арқылы Finance and Operations бағдарламасындағы жоба бухгалтері қарап шыға алады.

## <a name="billing-milestones"></a>Шот ұсыну кезеңдері

Белгіленген баға бойынша шот ұсыну әдісін пайдаланатын жобалық келісімшарт жолдарына шот ұсыну кезеңдері арқылы есеп-шот ұсынылады. Шот ұсыну кезеңдері Finance and Operations бағдарламаларындағы жоба шотындағы транзакцияларға **Project Operations интеграциясының келісімшарт жолының кезеңдері (msdyn\_contractlinescheduleofvalues)** кесте нысаны арқылы синхрондалады.

  ![Шот ұсыну кезеңдерінің интеграциясы.](./media/2Milestones.jpg)

Бухгалтер **Жобаларды басқару және есеп** > **Жобалық келісімшарттар** > **Сақтау** > **Шоттағы транзакциялар** немесе **Жобаларды басқару және есеп** > **Барлық жобалар** > **Сақтау** > **Шоттағы транзакциялар** терезесіне өту арқылы шоттағы транзакцияларды қарап шығып, есеп төлсипаттарын қарап шыға алады.

Жобаның берілген келісімшарт жолы үшін шот ұсыну кезеңін алғаш жасаған кезде жүйе осы келісімшарт жолымен байланыстырылған жоба үшін белгіленген баға кірісін бағалау жобасын автоматты түрде жасайды. Белгіленген баға кірісін бағалау жобаларын **Жобаларды басқару және есеп** > **Белгіленген баға кірісін бағалау жобалары** параметріне өту арқылы қарап шығуға болады.

### <a name="project-tasks"></a>Жоба тапсырмалары

Жобалық тапсырмалар Finance and Operations бағдарламаларына **Жобалық тапсырмалар (msdyn\_projecttasks)** кесте картасы арқылы тек анықтамалық мақсаттар үшін синхрондалады. Finance and Operations бағдарламалары арқылы жасау, жаңарту және жою операцияларына қолдау көрсетілмейді.

  ![Жобалық тапсырмалар интеграциясы.](./media/3Tasks.jpg)

## <a name="project-resources"></a>Жоба ресурстары

**Жоба ресурстары рөлдері** нысаны Finance and Operations бағдарламаларына **Барлық компанияларға арналған жобалық ресурстық рөлдер (bookableresourcecategories)** кесте нысаны арқылы тек анықтамалық мақсаттар үшін синхрондалады. Dataverse платформасындағы ресурстық рөлдер компанияға қатысты болмағандықтан, жүйе автоматты түрде қос жазу интеграциясы ауқымына кіретін барлық заңды нысандар үшін Finance and Operations бағдарламаларында автоматты түрде компанияға арналған тиісті ресурстық рөлдер жазбаларын жасайды.

![Ресурс рөлдерін біріктіру.](./media/5Resources.jpg)

Project Operations бағдарламасындағы жобалық ресурстар Dataverse жүйесінде сақталып, Finance and Operations бағдарламаларына синхрондалмайды.

### <a name="transaction-categories"></a>Транзакция санаттары

Транзакция санаттары Dataverse платформасында сақталып, **Жобалық транзакция санаттары (msdyn\_transactioncategories)** кесте нысаны арқылы Finance and Operations бағдарламаларына синхрондалады. Транзакция санатының жазбасы синхрондалғаннан кейін жүйе автоматты түрде төрт ортақ санат жазбасын жасайды. Әрбір жазба Finance and Operations бағдарламаларындағы транзакция түріне сәйкестендіріліп, оларды транзакция санаты жазбасына байланыстырады.

![Транзакция санаттарын біріктіру.](./media/4TransactionCategories.jpg)

Бағалаулар мен нақты көрсеткіштер үшін транзакция санаттарын пайдалану жоба бухгалтері немесе жүйе әкімшісінің әрбір заңды нысанда тиісті жоба санаттарын жасауын қажет етеді. Қосымша ақпарат алу үшін [Жоба санаттарын конфигурациялау](../project-accounting/configure-project-categories.md) бөлімін қараңыз.