---
title: ҚҚС қалпына келтіруі
description: Бұл тақырыпта қосылған құн салығы (ҚҚС) транзакциялары бойынша ақыны қалпына келтіру әдісін түсіндіреді.
author: saraschi2
manager: AnnBe
ms.date: 02/26/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 187532281f6aba3cc3fb03428d93c8ebc4cf4a3d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271926"
---
# <a name="vat-recovery"></a>ҚҚС қалпына келтіруі 

Жарамды қосылған құн салығы (ҚҚС) транзакциялары бойынша ақыны алу үшін компания немесе ұйым нақты ақпаратты анықтап, жинап, тексеріп, жіберуі керек. Бұл процесс бірнеше тапсырмаларды қамтиды және компанияңыздың көлеміне байланысты бірнеше қызметкерлерді немесе рөлдерді қамтуы мүмкін.

Шығыстарды басқару модулі арқылы ҚҚС салығын қалпына келтіру үшін келесі алғышарттарды орындау қажет:

- Салық кодтары шығыс санаттарына бекітілген елдер/аймақтар үшін жасалуы керек.
- Сатылым салығының тобы әрбір салық коды үшін жасалуы керек.
- Элементтің сатылым салығының коды әрбір сатылым салығының тобы үшін жасалуы керек.

Алғышарттар аяқталғаннан кейін, ҚҚС транзакциялары үшін ақы сұрау үшін қызметкерлер мына қадамдарды орындайды.

1. Шығыс туралы есепте жарамды ҚҚС ақысын анықтау үшін несие картасымен жүргізілген транзакциялар туралы салық ақпаратын енгізіңіз.
2. Барлық салық туралы ақпарат толық екеніне көз жеткізіңіз, содан кейін шығыс туралы есепті жариялаңыз.
3. Халықаралық ҚҚС қалпына келтіруі үшін жарамды шығыстарды өңдеңіз.
4. Халықаралық қалпына келтіру қайтарымдарын тапсыру үшін үшінші тарап жеткізушісіне ҚҚС бойынша қалпына келтіру деректерін жіберіңіз.
5. Жергілікті ҚҚС қалпына келтіруіне арналған шығыстарды өңдеңіз.

Келесі бөлімдерде Contoso қызметкерлерінің әр қадамды қалай аяқтайтындығын көрсететін мысалдар келтірілген.

## <a name="on-an-expense-report-enter-tax-information-about-credit-card-transactions-to-identify-eligible-vat-refunds"></a>Шығыс туралы есепте жарамды ҚҚС ақысын анықтау үшін несие картасымен жүргізілген транзакциялар туралы салық ақпаратын енгізіңіз

АҚШ-та орналасқан Contoso компаниясының сатылым өкілі Нэнси, жақында Ұлыбританияға сатылым сапарынан оралды. Сапары барысында, ол тамақтану үшін жеке кредиттік карта бойынша біраз шығыс жұмсады. Енді Нэнси шығыстары туралы қайта келісу үшін шығыс туралы есеп жасауы қажет.

Нэнси шығыс туралы есепке ақпаратты енгізген кезде, ол **Шығыс туралы есепті өңдеу** бетіндегі **Ел/аймақ** өрісінде орналасқан **Ұлыбритания** тармағын таңдайды. Содан кейін сатылым салығының топтар тізімі тек Ұлыбританияға қолданылатын топтарды көрсететіндей сүзгіленген. Нэнси **Ұлыбритания 001** сатылым салығының тобын таңдайды, содан кейін **Тамақтану** элементінің сатылым салығы тобын таңдайды. Ол тұратын жері үшін жаңа транзакцияны қосады. Ұлыбританияда тұруға арналған бір ғана сатылым салығының тобы мен элементтің сатылым салығының тобы бар болғандықтан, бұл ақпарат автоматты түрде Нэнсидің шығыс туралы есебіне толтырылады.

Contoso саясатына сәйкес, барлық шығыстардың сәйкес түбіртегі болуы керек. Сондықтан Нэнси шығыс туралы есепті сақтаған кезде, ол шығыс туралы есепте көрсетілген әрбір транзакция үшін түбіртекті қоса беруі керек екендігі туралы хабарлама алады. Нэнси өзінің шығыс туралы есебіне әр транзакция туралы түбіртектің цифрлық кескінін бекіткенін тексереді, содан кейін есепті бекітуге жібереді. Содан кейін ол қағаз түбіртектерін қосалқы кеңсесінің өңдеу тобына жібереді. Бұл команда ҚҚС қалпына келтіру деректерін Contoso үшін халықаралық ҚҚС қалпына келтіру қайтарымдарын тапсыратын үшінші тарап жеткізушісіне жібереді.

## <a name="make-sure-that-all-tax-information-is-complete-and-then-post-the-expense-report"></a>Барлық салық туралы ақпарат толық екеніне көз жеткізіңіз, содан кейін шығыс туралы есепті жариялаңыз

Эйприл, Contoso компаниясының несие берушілерінің үйлестірушісі шығыс туралы есеп берместен бұрын, онда жоқ салық туралы ақпаратты енгізуі керек. Ол **Шығыс туралы есеп** бетін ашып, Нэнсидің бекітілген шығыс туралы есебін көреді. Содан кейін Эйприл транзакциялардың мәліметтерін көру үшін шығыс туралы есепті ашады. Ол Нэнсидің транзакциялардың бірі үшін сатылым салығы тобына элементті енгізбегенін көреді. Бұл ақпарат берілмегендіктен, Эйприл шығыс туралы есепті жариялай алмайды. Сондықтан Эйприл шығысты басқарудағы **Салық конфигурациялары** бетін ашып, елге/аймаққа және транзакция түріне сәйкес элементтің сатылым салығының тобын табады. Енді Эйприл шығыс туралы есепті жалпы тіркелімге жариялай алады.

Эйприл шығыс туралы есепті жариялаған кезде ҚҚС бойынша өтелетін жұмыс элементі жасалады. Бұл жұмыс элементі қосалқы кеңсенің өңдеу тобының мүшесіне тағайындалған. Эйприлға жариялау сәтті өткенін растайтын хабарлама келеді. Бұл хабарламада қалпына келтіру үшін анықталған ҚҚС транзакцияларының саны да келтірілген.

## <a name="process-expenses-that-are-eligible-for-international-vat-recovery"></a>Халықаралық ҚҚС қалпына келтіруі үшін жарамды шығыстарды өңдеу

Арни, Contoso компаниясының қосалқы кеңсесінің өңдеу тобы мүшесі, ҚҚС қалпына келтіруі үшін барлық қажетті ақпарат шығыс туралы есептерге енгізілгенін растауға жауапты. Ол **Шығыстар салығын қалпына келтіру** бетін ашып, Нэнси жіберген шығыс туралы есепті таңдайды. Содан кейін Арни барлық қажетті түбіртектердің тіркелгенін және сатылым салығының дұрыс тобы мен элементтің сатылым салығының кодтары енгізілгенін тексереді.

Арни Нэнсидегі қағаз түбіртектерді алған кезде, қағаз түбіртектерді сандық түбіртектермен салыстырып тексереді, содан кейін шығыс туралы есептің күйін **Қалпына келтіруге дайын** күйіне өзгертеді.

## <a name="send-vat-recovery-data-to-the-third-party-vendor-to-file-international-recovery-returns"></a>Халықаралық қалпына келтіру қайтарымдарын тапсыру үшін үшінші тарап жеткізушісіне ҚҚС бойынша қалпына келтіру деректерін жіберіңіз

Арни шығыс туралы есеп деректерін ҚҚС бойынша қалпына келтіру қайтарымдарын тапсыратын үшінші тарап жеткізушісіне жіберуге дайын болған кезде, ол **Шығыстар салығын қалпына келтіру** бетін ашады. Ол бетті тек шығыс туралы есептерді **Қалпына келтіруге дайын** ретінде белгілеп көрсететіндей сүзеді. Арни содан кейін **Файл** &gt; **Excel бағдарламасына экспорттау** тармағын таңдайды. Шығыс туралы есептерден алынған ҚҚС туралы ақпарат Microsoft Excel жұмыс парағына экспортталады. Арни бұл жұмыс парағын үшінші тараптың сатушысына жібереді және қағаз түбіртектер курьер арқылы жіберілгені туралы хабарлама қосады.

## <a name="process-expenses-for-domestic-vat-recovery"></a>Жергілікті ҚҚС қалпына келтіруіне арналған шығыстарды өңдеу

Арни шығыс туралы есеп транзакциялары ҚҚС қалпына келтіруіне жарамды екенін және сандық түбіртектер есептерге қоса берілгендігін тексеруі керек. Жергілікті қалпына келтіруге арналған шығыстарды өңдеуге кірісу үшін Арни **Шығыстар салығын қалпына келтіру** бетін ашып, тексеруді қажет ететін шығыс туралы есепті таңдайды. Ол түбіртектің қызметкердің орнына компанияның атында екенін тексереді. ҚҚС қалпына келтіру үшін түбіртектер компанияның атында болуы керек. Арни содан кейін сатылым салығының дұрыс тобы мен сатылым салығының кодтары қолданылғанын растайды.

Арни қағаз түбіртектерді алған кезде, шығыс туралы есептің күйін **Қалпына келтіруге дайын** күйіне өзгертеді. Содан кейін ол қайтарымды тиісті салық органына тапсыра алады. Бұл жағдайда АҚШ-тағы тиісті салық органы Ішкі кірістер қызметі (IRS) болып табылады.


[!INCLUDE[footer-include](../includes/footer-banner.md)]