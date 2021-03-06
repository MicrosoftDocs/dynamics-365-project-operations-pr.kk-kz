---
title: Жобаға негізделген мүмкіндік жолдары
description: Бұл тақырыпта жобаға негізделген мүмкіндік жолдарымен жұмыс істеу туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7b255d607ac8180c249a9b9831db6f8d0cd3937b
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898403"
---
# <a name="project-based-opportunity-lines"></a>Жобаға негізделген мүмкіндік жолдары

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_


Жобаға негізделген мүмкіндік жолдары тек жобаға негізделген мүмкіндіктерде қолжетімді. Жобаға негізделген мүмкіндік жазбалары **Түрі** өрісінің мәнін **Жұмысқа негізделген** мәніне орнатты.

Жобаға негізделген мүмкіндік жолдары - тұтынушыға жобаның көмегімен жеткізілетін жол элементтері. Алайда жобаны жобаға негізделген мүмкіндік жолына байланыстыру мүмкін емес. Жобаларды жол элементтеріне **Баға ұсынысы** кезеңінен бастап байланыстыруға болады, өйткені әдетте мүмкіндік мәміленің алғашқы кезеңінде пайда болады. Тұтынушыға жұмысты жеткізу үшін пайдаланылатын жоба санын анықтау сатылым кезеңінде кейінірек қабылданатын шешім болып табылады. Тұтынушыға жеке жеткізу компоненттерін анықтау үшін мүмкіндік кезеңін пайдаланыңыз. Осы компоненттерді жеткізу үшін пайдаланылатын жобалардың нақты санына қатысты шешімдер жұмыс туралы көбірек ақпарат пайда болғанға дейін көбейтілуі мүмкін.

Төменде жобаға негізделген мүмкіндік жолындағы өрістер берілген:

| **Өріс** | **Орны** | **Маңыздылық, мақсаты және нұсқаулығы** | **Төменгі әсер** |
| --- | --- | --- | --- |
| Өнім түрі | Жалпы қойынды (жасырын) | Бұл параметрлер жиыны өрісі. Егер Dynamics 365 Operations бағдарламасы орнатылған болса, қолжетімді нұсқалардың бірі **Жобаға негізделген қызмет** болып табылады.  | Жобаға негізделген мүмкіндік жолын мүмкіндіктегі жобаға негізделген жолдар торынан жасаған кезде, бұл өрістің мәні **Жобаға негізделген қызмет** мәніне орнатылады.  <br> Егер сіз бұл мәнді өзгертсеңіз немесе алдын ала анықтасаңыз, жобаның функционалды мүмкіндігі жобаға негізделген жол элементтерінде қосылмайды. |
| Мүмкіндік | «Жалпы мәліметтер» қойыншасы | Бұл өріс тек оқуға арналған және осы жол элементіне жататын негізгі мүмкіндік жазбасына сілтеме жасайды. | Бұл өрістің төменгі әсері жоқ. |
| Атауы | «Жалпы мәліметтер» қойыншасы | Бұл осы жол элементіне қысқаша сәйкестілік беру үшін пайдалануға болатын өңделетін мәтіндік өріс | Бұл мән осы мүмкіндіктен баға ұсынысын жасаған кезде баға ұсыну жолына көшіріледі |
| Тұтынушы бюджеті | «Жалпы мәліметтер» қойыншасы | Бұл өзгертілетін валюта өрісін ұтынушының осы жол үшін жұмсауға дайын сомасын бақылау үшін пайдалануға болады. | Бұл мән осы мүмкіндіктен баға ұсынысын жасаған кезде баға ұсыну жолындағы тиісті өріске көшіріледі |
| Есепшот ұсыну әдісі | «Жалпы мәліметтер» қойыншасы | Бұл өңделетін өріс келесі мәндерге ие:</br>- Уақыт және материал</br>- Бекітілген баға | Бұл мән осы мүмкіндіктен баға ұсынысын жасаған кезде баға ұсыну жолындағы тиісті өріске көшіріледі. Баға ұсыну жолы жасалғаннан кейін, өріс құлыпталады және оны өзгерту мүмкін емес болады. Бұл өріс мәнін мүмкіндігінше дәл тағайындаңыз. Осы өрістің баға ұсыну жолындағы мәнін өзгерту қажет болса, баға ұсыну жолын жойып, қайта жасаңыз. |
