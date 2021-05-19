---
title: Жоба сатылымын бақылау
description: Бұл тақырыпта Project Operations жобадағы жұмыс күшінің табысын бақылау амалы туралы ақпарат берілген.
author: rumant
manager: AnnBe
ms.date: 03/24/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 438c44dcfaf9677075eb07688c1e65c6e7053755
ms.sourcegitcommit: a1f9f92546ab5d8d8e5a4710ce4c96414ea55d14
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2021
ms.locfileid: "5711063"
---
# <a name="project-sales-tracking"></a>Жоба сатылымын бақылау

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Dynamics 365 Project Operations жұмыс жоспары үшін қажетті минималды нақтылау дәрежесімен еңбек болжамдары мен табысты қадағалайды. Еңбек табыстарының болжамы жоспарланған талпынысқа және жоба жоспарындағы әрбір соңғы түйініне тағайындалған жалпы немесе атаулы ресурстарға негізделген. Жоба басталған кезде және адамдар әр түрлі жобалық тапсырмалар туралы уақытты есепке ала бастаған кезде, еңбекке кеткен нақты табыстар жинақталып, болжамдарды есептеу басталады.

## <a name="labor-revenue-tracking-view"></a>Еңбек табыстарын бақылауы көрінісі

**Бақылау** қойыншасындағы **Жобалар** бетінен **Шығынды бақылау** көрінісін ашу үшін **Бақылау** > **Шығын** тармағын таңдай аласыз. Не болмаса **Табысты бақылау** көрінісін ашу үшін **Пайдалану** > **Вексель мөлшерлемесі** тармағын таңдай аласыз, бұл жоба жоспарындағы әр тапсырма бойынша алынған табыстың барысын көрсетеді. Бұл көрініс сонымен қатар тапсырмаға жұмсалған нақты еңбек табысын тапсырманың жоспарланған еңбек табыстарымен салыстырады. Project Operations еңбек табыстарының көрсеткіштерін есептеу үшін келесі формулаларды қолданады:

- **Жоспарланған табыс**: әр соңғы түйін тапсырмасындағы барлық ресурстарды тағайындаудың жоспарланған сатылым мәндері
- **Нақты табыс**: тапсырмаға жазылған уақыттағы барлық нақты шот ұсынылмаған сатылымның қосындысы
- **Шот ұсынылатын табыс %**: нақты табыс ÷ аяқтау кезіндегі табыс болжамы
- **Қалған табыс**: аяқтау кезіндегі табыс болжамы – нақты табыс
- **Аяқтау кезіндегі болжамды табыс**: қалған табыс – нақты табыс
- **Табыс ауытқуы**: жоспарланған табыс – аяқтау кезіндегі болжамды табыс


> [!NOTE]
> Project Operations бағдарламасында еңбек табыстарын тек **Бақылау** қойыншасындағы **Жоба** бетінде көрсетіледі. Материалдар мен шығындарды тұтыну материалдары бойынша жобалауға және бақылауға болатындығына қарамастан, бұл табыстар **Бақылау** қойыншасында көрсетілген табыстарға кірмейді. Бұл қойынша тек талпынысты қайта жобалау арқылы еңбек табыстарын қайта жобалауға арналған.  
> Көрсетілген барлық табыс сомалары жобаның құн валютасына ауыстырылады. Жобаның өзіндік құны жобаның келісім-шарт бірлігінің валютасы болып табылады. Белгіленген бағалық жобалар үшін **Еңбек табысын бақылау** көрінісіндегі табыстар санының қатысы жоқ, себебі шот ұсынылмаған сатылымның нақты мәндері бойынша есептеулер уақыт бекітулері бойынша жазылмаған.
> Жобаның **Болжам** қойыншасында көрсетілген уақыт бойынша сатылымдар **Бақылау** қойыншасындағы жоспарланған табысқа сәйкес келмеуі мүмкін. Бұл сәйкессіздік көзі екі себептерге байланысты болуы мүмкін:
><ol>
   ><li> <b>Болжамдар</b> қойыншасында сату валютасымен есептелген табыс көрсетіледі, ал <b>Бақылау</b> қойыншасында жоспарланған табысты құн валютасына ауыстыру көрсетілген. </li>
   ><li> Болжамды сатылым келісім-шарт валютасына <b>Бағалаулар</b> қойыншасында көрсетілгендей ауыстырылған кезде жобаның валютасына айырбастау дәлдікті жоғалтуға әкелетін қадамдарды қамтиды: </li>
><ol>
><li> Келісім-шарт валютасындағы болжамды сату сомасы алдымен негізгі валютаға ауыстырылады (1-конверсия).</li>
><li> Негізгі валютасындағы болжамды сату сомасы жоба құнының валютасына ауыстырылады (2-конверсия). </li>
></ol>
></ol>
> Валюталық дәлдік екі кезеңде де қолданылады, нәтижесінде жоба валютасында жоспарланған кірістің келісім-шарт валютасымен жоспарланған сатылымнан ауытқуы болады.
   

## <a name="reprojecting-revenues-on-leaf-node-tasks"></a>Соңғы түйін тапсырмаларын табыстарды қайта жобалау

Соңғы түйін тапсырмасы үшін еңбек табыстарын **Жоба** бетіндегі **Бақылау** қойыншасында тікелей қайта жобалау мүмкін емес. Алайда тапсырма бойынша қалған талпынысты қайта бағалау үшін **Талпынысты бақылау** көрінісін пайдалануға болады. Бұл тапсырма бойынша қалған табысты қайта есептеуге әкеледі. Төменде мұның қалай жұмыс істейтіні сипатталған.

1. Жоба менеджері тапсырма бойынша талпынысты **Қалған талпыныс** өрісіндегі әдепкі мәнді тапсырма бойынша қалған талпыныстың жаңа болжамына жаңарту арқылы қайта жобалай алады. Бұл қайта жобалау тапсырманың аяқтау кезіндегі талпыныс болжамын (EAC) және орындалу пайызын қайта есептеуді және тапсырма бойынша талпыныстың ауытқуын тудырады. Аяқтау кезіндегі құн болжамы (EAC), аяқтау кезіндегі болжам (ETC) және жиынтық тапсырмалар бойынша орындалу пайызы да қайта есептелінеді және талпыныс ауытқуының жаңа болжамын жасайды.
2. Тапсырма бойынша қалған талпыныстың жаңа мәніне сүйене отырып, жүйе **Табыстарды қадағалау** көрінісіндегі қалған табысты есептейді. Қалған талпынысқа негізделген қалған табысты есептеу үшін жүйе алдымен жиынтық тапсырма бойынша бір сағаттық талпыныстың орташа табысты жоспарланған табыс немесе жоспарланған талпыныс ретінде есептейді. Жоспарланған табыс - бұл тапсырма бойынша барлық ресурстарды тағайындау табыстарының жиынтығы. Сағатына жұмсалатын орташа табыстар тапсырма бойынша жаңадан жобаланған қалған табыстың қалған құнын есептеу үшін қолданылады.
3. Соңғы түйінді тапсырма бойынша аяқтау кезіндегі және тұтыну пайызы бойынша жобаланған шығындар қайта есептеледі.
4. Жиынтық тапсырмалардың аяқтау кезіндегі табыс мәндері түбірлік түйінге дейін қайта есептеледі.

## <a name="reprojecting-revenues-on-summary-tasks"></a>Жиынтық тапсырмалар бойынша табыстарды қайта жобалау

Жиынтық тапсырмалар немесе контейнер тапсырмалары бойынша еңбек табыстарын қайта жобалауға болады. Дегенмен жобаның жиынтық тапсырмасы үшін **Жоба** бетіндегі **Бақылау** қойыншасындағы еңбек табыстарын тікелей қайта жобалай алмайсыз. Соңғы түйіндерінің тапсырмалары сияқты жиынтық және контейнер тапсырмаларын **Талпынысты бақылау** көрінісі арқылы қайта жобалауға болады. Бұл көріністе жиынтық тапсырма бойынша қалған табысты қайта есептеуді тудыратын жиынтық тапсырма бойынша қалған талпынысты қайта жобалай аласыз. Төменде мұның қалай жұмыс істейтіні сипатталған.

1. Жоба менеджері тапсырма бойынша талпынысты **Қалған талпыныс** өрісіндегі әдепкі мәнді тапсырма бойынша **Қалған талпыныстың** жаңа болжамына жаңарту арқылы қайта жобалай алады. Бұл қайта жобалау тапсырманың аяқтау кезіндегі болжамды (EAC) және орындалу пайызын қайта есептеуді және тапсырма бойынша талпыныстың ауытқуын тудырады. Аяқтау кезіндегі құн болжамы (EAC), ETC және жиынтық тапсырмалар бойынша орындалу пайызы да қайта есептелінеді және талпыныс ауытқуының жаңа болжамын жасайды.
2. Тапсырма бойынша **Қалған талпыныс** өрісіндегі жаңа мәнге сүйене отырып, жүйе **Табыстарды қадағалау** көрінісіндегі қалған табысты есептейді. Қалған талпынысқа негізделген қалған табысты есептеу үшін жүйе алдымен жиынтық тапсырма бойынша бір сағаттық талпыныстың орташа табысты жоспарланған табыс немесе жоспарланған талпыныс ретінде есептейді. Жоспарланған табыс - бұл тапсырма бойынша барлық ресурстарды тағайындау табыстарының жиынтығы. Сағатына жұмсалатын орташа табыстар тапсырма бойынша жаңадан жобаланған табыстың қалған құнын кейіннен есептеу үшін қолданылады.
3. Жиынтық тапсырма бойынша аяқтау кезіндегі және тұтыну пайыздары бойынша жобаланған шығындар қайта есептеледі.
4. Аяқтау кезіндегі жаңа жобаланған табыстың мәнін қосалқы тапсырмаларға тапсырмада болған бастапқы жоспарланған табыспен бірдей пропорцияда үлестірілді.
5. Жаңа болжалды табыс әрбір жеке тапсырмалардан бастап, соңғы түйін тапсырмаларына дейін есептеледі. Осы мәнге сүйене отырып, соңғы түйіндерінде әсерге ұшыраған еншілес тапсырмалар олардың толық құны бойынша табыстар негізінде қалған табыстар мен табыстар пайызын қайта есептейді. Нәтижесінде тапсырма бойынша табыс ауытқуы үшін жаңа проекция пайда болады. 
6. Жиынтық тапсырмалардың аяқтау кезіндегі табыс мәндері түбірлік түйінге дейін қайта есептеледі.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
