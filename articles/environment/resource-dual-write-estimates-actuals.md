---
title: Жоба болжамдары мен нақты көрсеткіштерінің интеграциясы
description: Бұл мақалада жобалық бағалаулар мен нақты деректер үшін Project Operations қосарлы жазу интеграциясы туралы ақпарат берілген.
author: sigitac
ms.date: 4/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: dc8f65aec6f2328ccef5f9591a0f4d9c792b0d8f
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/18/2022
ms.locfileid: "9029087"
---
# <a name="project-estimates-and-actuals-integration"></a>Жоба болжамдары мен нақты көрсеткіштерінің интеграциясы

_**Қолданылады:** ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Бұл мақалада жобалық бағалаулар мен нақты деректер үшін Project Operations қосарлы жазу интеграциясы туралы ақпарат берілген.

## <a name="project-estimates"></a>Жоба болжамдары

Жобаның жұмыс күші, шығындары және материалдық сметалары жасалады және сақталады Microsoft Dataverse және бухгалтерлік есеп мақсаттары үшін қаржы және операциялық қолданбаларға синхрондалады. Қаржы және операциялар қолданбалары арқылы жасау, жаңарту және жою операцияларына қолдау көрсетілмейді.

Бағалауды жасау үшін жобаның жарамды есеп конфигурациясы қажет. Келісімшарт жолдарымен байланысты жобаларда жоба құны мен кіріс профилі ережелерінде анықталған жоба құны мен кіріс профилі болады. Қосымша ақпарат алу үшін [Есеп-шот ұсынылатын жобалар бойынша есепті конфигурациялау](../project-accounting/configure-accounting-billable-projects.md#configure-project-cost-and-revenue-profile-rules) бөлімін қараңыз.

## <a name="labor-estimates"></a>Еңбек бағалаулары

Еңбек бағалаулары жоба тапсырмасына жалпы немесе аталған ресурсты тағайындайтын жоба менеджері немесе ресурс менеджері арқылы жасалады. Ресурстық тағайындау жазбаларын Dataverse жүйесіндегі **Жоба туралы мәліметтер** бетіндегі **Ресурстық тағайындаулар** қойыншасында қарап шығуға болады. Ресурс тағайындау жазбалары Dataverse көмегімен қаржы және операциялық қолданбаларда сағаттық болжам жазбаларын жасаңыз **Сағаттық бағалаулар үшін жобалық операцияларды біріктіру нысаны (msdyn\_ ресурстарды тағайындау)**.

   ![Еңбек бағалауларының интеграциясы.](./Media/DW4LaborEstimates.png)

Қос жазу ресурстық тағайындау жазбаларын аралық кезең кестесіне (**ProjCDSEstimateHoursImport**) синхрондап, содан кейін сағаттық болжам жазбаларын жасап, жаңарту үшін бизнес логикасын пайдаланады (**ProjCDSEstimateHoursImport**).

Жоба есепшісі мына сілтемеге өту арқылы қаржы және операциялық қолданбаларда жасалған болжамды сағат жазбаларын қарайды **Жобаны басқару және бухгалтерлік есеп** > **Барлық жобалар** > **Жоспар** > **Сағат болжамдары**.

## <a name="expense-estimates"></a>Шығыс болжамдары

Шығын болжамдары Dataverse бағдарламасында **Жоба туралы мәліметтер** бетіндегі **Шығын болжамдары** қойыншасындағы жоба менеджері арқылы жасалады. Шығын болжамы жазбалары Dataverse бағдарламасындағы **Болжам жолы** нысанында сақталады. Бұл бағалау жазбаларында транзакция класы бар, **Шығын** пайдалана отырып, қаржы және операциялық қолданбалардағы шығындарды болжау жазбаларымен синхрондалады **Шығындар сметасына арналған жоба операцияларын біріктіру нысаны (msdyn\_ бағалаулар)**.

   ![Шығын бағалауларының интеграциясы.](./Media/DW4ExpenseEstimates.png)

Қос жазу мүмкіндігі шығын болжамының жазбаларын **ProjCDSEstimateExpenseImport** кезең кестесіне синхрондап, содан кейін шығын болжамы жазбаларын жасап, жаңарту үшін бизнес логикасын пайдаланады (**ProjForecastCost**). Бағалау жолдары сатылымды бағалау және шығындарды бағалау жазбаларын бөлек сақтайды. Қаржы және операциялар қолданбаларындағы бизнес логикасы кезең кестесіндегі осы мәліметтерді пайдалана отырып, бір шығыс болжамы жазбасын толтырады.

Жоба есепшісі келесіге өту арқылы қаржы және операциялық қолданбалардағы шығыстар болжамының жазбаларын қарай алады **Жобаны басқару және бухгалтерлік есеп** > **Барлық жобалар** > **Жоспар** > **Шығындардың болжамдары**.

## <a name="material-estimates"></a>Материал болжамдары

Материалдық болжамдар Dataverse бағдарламасында **Жоба туралы мәліметтер** бетіндегі **Материалдық болжамдар** қойыншасындағы жоба менеджері арқылы жасалады. Материалдық болжам жазбалары Dataverse бағдарламасындағы **Болжам жолы** нысанында сақталады. Бұл бағалау жазбаларында транзакция класы бар, **Материал** және қаржы және операциялық қолданбалардағы элементтерді болжау жазбаларымен синхрондалады **Материалдық бағалау үшін жобаны біріктіру кестесі (msdyn\_ бағалаулар)**.

   ![Материалдық болжамдар интеграциясы.](./Media/DW4MaterialEstimates.png)

Қос жазу мүмкіндігі материалдық болжам жазбаларын **ProjForecastSalesImpor** кезең кестесіне синхрондап, содан кейін элемент болжамы жазбаларын жасап, жаңарту үшін бизнес логикасын пайдаланады (**ForecastSales**). Бағалау жолдары сатылымды бағалау және шығындарды бағалау жазбаларын бөлек сақтайды. Қаржы және операциялар қолданбаларындағы бизнес логикасы кезең кестесіндегі осы мәліметтерді пайдаланып, бір Элемент болжамының жазбасын толтырады.

Жоба есепшісі келесіге өту арқылы қаржы және операциялық қолданбалардағы болжам жазбаларын қарай алады **Жобаны басқару және бухгалтерлік есеп** > **Барлық жобалар** > **Жоспар** > **Элементтердің болжамдары**.

## <a name="project-actuals"></a>Жобаның нақты көрсеткіштері

Жобаның нақты көрсеткіштері уақыт, шығын, материал және шот ұсыну әрекеті негізінде Dataverse бағдарламасында жасалады. Осы транзакциялардың барлық операциялық төлсипаттары, соның ішінде саны, шығыны, сатылым бағасы және жоба осы Dataverse нысанында түсіріледі. Толық ақпарат алу үшін [Нақты көрсеткіштер](../actuals/actuals-overview.md) бөлімін қараңыз. Нақты жазбалар қосарлы жазу кесте картасын пайдаланып, қаржы және операциялық қолданбалармен синхрондалады.**Жоба операцияларын біріктіру фактілері (msdyn\_ нақтылар)** төменгі ағынды есепке алу үшін.

   ![Нақты көрсеткіштерді біріктіру.](./Media/DW4Actuals.png)

**Project Operations интеграциясының нақты көрсеткіштері** кесте картасы барлық жазбаларды **Жалған** мәніне орнатылған **Синхрондауды өткізіп жіберу (тек ішкі пайдалану)** төлсипатымен Dataverse бағдарламасындағы **Нақты көрсеткіштер** нысанынан синхрондайды. Жазба жасалған кезде бұл төлсипат мәні автоматты түрде Dataverse бағдарламасында орнатылады. Бұл төлсипат **Шын** мәніне орнатылған мысалдар төмендегідей:

  - Компанияаралық операцияларға арналған жоба шығынының нақты көрсеткіштері. Қосымша ақпарат алу үшін [Компанияаралық транзакцияларды жасау](../project-accounting/create-intercompany-transactions.md) бөлімін қараңыз. Бұл жазбалар өткізіліп жіберіледі, себебі компания аралық сатушы шот-фактурасы жарияланған кезде жүйе қаржы және операциялық қолданбалардағы нақты жоба құнын қайта жасайды.
  - Проформа-шоты расталған кезде теріс шот ұсынылмаған сатылым жазбалары жасалды. Бұл жазбалар өткізіліп жіберіледі, себебі жобаның қаржы және операциялық қолданбалардағы қосалқы кітабы шот-фактура жасау кезінде шотсыз сату жазбасын қайтармайды, бірақ күйді толығымен шот-фактураға өзгертеді.

Қос жазу кесте нысаны нақты көрсеткіштер жазбаларын **ProjCDSActualsImport** аралық кезең кестесіне синхрондайды. Бұл жазбалар Project Operations интеграциясының журнал жолдары мен жобалық есеп-шот ұсынысы жолдарын жасау кезінде **Аралық кезең кестесінен импорттау** мерзімдік процесі арқылы өңделеді. Қосымша ақпарат алу үшін [Project Operations бағдарламасындағы интеграция журналы](../project-accounting/project-operations-integration-journal.md) бөлімін қараңыз.

Dataverse бағдарламасы сондай-ақ **Транзакция байланысы** нысанындағы жобаның нақты транзакциялары арасындағы байланыстарды түсіреді. Қосымша ақпарат алу үшін [Нақты көрсеткіштерді түпнұсқа жазбаларға байланыстыру](../actuals/linkingactuals.md) бөлімін қараңыз. Нақты транзакциялар арасындағы сілтемелер сонымен қатар қосарлы жазу кестесінің картасын пайдаланып, қаржы және операциялық қолданбаларға үндестіріледі, **Жобалық транзакция қатынастарына арналған интеграциялық нысан (msdyn\_ транзакциялық байланыстар)**. Бұл жазбалар Project Operations интеграциясының журнал жолдары мен жобалық есеп-шот ұсынысы жолдарын жасау кезінде **Аралық кезең кестесінен импорттау** мерзімдік процесі арқылы пайдаланылады.

Project Operations интеграция журналы мен жобаның есеп-шот ұсынысын орналастыру кезінде **ProjCDSActualsImport** аралық кезең кестесіндегі тиісті жазбалардың жаңартылуы іске қосылады. Жүйе нақты операциялар үшін келесі бухгалтерлік есеп төлсипаттарын түсіреді және жазады:

- Есеп валютасының сомасы
- Айырбастау бағамы
- Ваучер нөмірі
- Сатылым салығының сомасы

**Project Operations интеграциясының нақты көрсеткіштері** кесте нысаны осы ақпаратпен Dataverse бағдарламасындағы тиісті нақты жазбаларды жаңартады.