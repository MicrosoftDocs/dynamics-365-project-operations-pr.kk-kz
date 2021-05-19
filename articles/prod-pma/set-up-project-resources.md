---
title: Жоба ресурстарын орнату
description: Бұл тақырыпта жоба ресурстарына сұрау орнату туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0bf146c3bfb2fd558c471d8a9e980834cb1b87df
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288746"
---
# <a name="set-up-project-resources"></a>Жоба ресурстарын орнату

[!include [banner](../includes/banner.md)]

Күнтізбені орнатып, оны қызметкермен немесе жұмысшымен байланыстыру керек. Күнтізбе жобаны және жоба үшін сақталған ресурстардың жұмыс уақытын жоспарлау үшін қолданылады. Күнтізбені теңшеу кезінде жоба менеджерлері ресурстарды оңтайландыру шеңберінде ресурстарды теңестіре алады. Күнтізбелік кесте негізінде ресурстар шектеулер қойылуы мүмкін. Күнтізбені **Күнтізбелер** бетінде орнатуға болады.

Жұмысшыны жоба ресурсы ретінде орнатқан кезде ресурстарды орнататын компанияда жұмыс істейтін жұмысшылардың ішінен таңдауға болады. Сонымен қатар, ұйымыңыздағы басқа компаниялардың жұмысшыларын таңдай аласыз. Бұл жұмысшылар компания ішіндегі ресурстар ретінде белгілі.

Келесі процедураларда компанияңызда жұмысшыны жоба ресурсы ретінде орнату амалы және компанияаралық жоба ресурсын қалай орнату керектігі түсіндіріледі.

## <a name="set-up-a-worker-as-a-project-resource"></a>Жұмысшыны жоба ресурсы ретінде орнатыңыз

1. **Жұмысшылар** тізіміндегі **Жұмысшылар** бетінен жоба ресурсы ретінде қосатын жұмысшыны таңдап, жұмысшы жазбасын ашыңыз.
2. Әрекеттер тақтасынан **Жоба** &gt; **Орнату** &gt; **Жобаны орнату** опцияларын таңдаңыз.
3. Күнтізбені таңдап, бетті жабыңыз.

Сондай-ақ ресурс үшін әдепкі жобаларды алдын-ала тағайындау түрі ретінде көрсетуге болады. Алдын-ала тағайындауларды ресурс менеджері немесе жоба менеджері ресурстың қандай жобаларда жұмыс жасайтынын алдын-ала білген кезде пайдалануына болады. Алдын ала тағайындаулар, сондай-ақ, жоба демеушісі немесе тұтынушының сұранысына негізделуі мүмкін. Жобаны алдын ала тағайындау үшін, **Жобаларды тағайындау** бетінен, **Жобалар** қойыншасындағы, **Қалған жобалар** тізімінен лайықты жобаны таңдаңыз.

## <a name="set-up-an-intercompany-resource"></a>Компанияаралық ресурсты орнатыңыз

Жұмысшыны компанияаралық ресурс ретінде орнатқан кезде, бұл параметрді несие беруші компания мен қарыз алушы компанияда орындау керек.

### <a name="in-the-lending-company"></a>Несиелік компанияда

1. "Қаржы" бөлімінде несие беруші компанияның таңдалғанына көз жеткізіп, алдыңғы "Жұмысшыны жоба ресурсы ретінде орнату" бөліміндегі процедурасын орындаңыз.
2. **Компанияаралық шот** бетінен **Жаңа** опциясын таңдаңыз.
3. **Заңды нысан идентификаторы** өрісінен несиелік компанияны таңдаңыз. Қалған өрістерді сәйкесінше толтырып, **Сақтау** опциясын таңдаңыз.
4. **Тасымал құны** бетінен **Жаңа** опциясын таңдаңыз.
5. **Қарыз алушы заңды тұлға** өрісінен тиісті компанияны таңдаңыз.
6. Қарыз алушы компанияға осы бөлімнің басында жасалған ресурсты ғана беру үшін **Ресурс** өрісінен жасалған ресурстың атауын таңдаңыз. Несие беруші компанияның барлық ресурстарын қарыз алушы компанияға қолжетімді ету үшін **Ресурс** өрісін бос қалдырыңыз.
7. **Жобаны басқару және есеп параметрлері** бетіндегі **Компанияаралық** қойыншасынан **Компанияаралық ресурсты жоспарлауды және уақыт кестелерін іске қосу** опциясын **Иә** мәніне орнатыңыз.

### <a name="in-the-borrowing-company"></a>Қарыз алушы компанияда

- **Ресурстар тізімі** бетіндегі іздеу сүзгісіне қарыз алушы компанияның ресурстар тізіміне сол атаудың қосылуын қамтамасыз ету үшін несие беруші компания үшін жасалған ресурстың атын енгізіңіз.

## <a name="request-project-resources"></a>Жоба ресурстарын сұрау
Жоба ресурстарын жоспарлау мүмкіндігі ресурс менеджерлеріне жинақталған ресурстарды тек тапсырмаларға немесе жобаларға бөлуге мүмкіндік береді. Бұл мүмкіндікті қосу үшін келесі тапсырмаларды орындаңыз немесе оларды орындағаныңызға көз жеткізіңіз:

- Тізбектер санын орнатыңыз.
- Жобаларды басқару және есепке алу жұмыс ағындарын орнатыңыз.
- Ресурс сұрауы жұмыс ағындарын іске қосыңыз.

Алдыңғы тапсырмалар аяқталғаннан кейін қажет болған жағдайда келесі тапсырмаларды орындауға болады:

- Жұмсақ көшірмесі жасалған жинақталған ресурстан сұраныс жасаңыз.
- Ресурс сұрауларын бақылаңыз.
- Ресурс сұрауларын орындаңыз.
- WBS үлгісінен жинақталған ресурстарды сұраңыз.
- Жобаға ресурстарды жинақталған ресурсты сұратпай-ақ резервтеңіз.


[!INCLUDE[footer-include](../includes/footer-banner.md)]