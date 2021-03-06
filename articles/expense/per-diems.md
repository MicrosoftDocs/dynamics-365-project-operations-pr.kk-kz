---
title: Тәуліктік
description: Бұл тақырыпта шығысты басқаруда пайдаланылатын тәуліктік ережелер туралы ақпарат берілген.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 7d1c4ac7781cb711e2cc0d09606d422b4dd554f3
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908322"
---
# <a name="per-diems"></a>Тәуліктік

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_


Тәулік - бұл жұмыс орнына бара жатқан жұмысшыға төленетін жәрдемақы. Шығысты басқаруда әр түрлі сапар жағдайлары үшін тәуліктік ережелерді жасауға болады. Тәуліктік тарифтер жылдың уақытына, сапар орнына немесе екеуіне де байланысты болуы мүмкін. Тәуліктік ережені жасаған кезде, жұмысшы тегін тамақтанса немесе қызмет алса, тәуліктік тарифтің пайыздық мөлшерінің ұсталатынын көрсетуге болады. Сонымен қатар жұмысшылардың сапарына қолданылатын тәуліктік тарифтің минималды және максималды сағаттарын орнатуға болады.

## <a name="configuration"></a>Теңшелім 

1. Тәуліктік орындарды қосу үшін **Орнату** > **Есептеулер мен кодтар** > **Тәуліктік орындар** тармағына өтіңіз.
2. Жоғарыда қосылған орындардың әрқайсысы үшін белгілі бір басталу мен аяқталу күні арасында қонақ үйге, тамақтануға және басқа шығындарға жарамды тәуліктік тариф мен валютаны таңдаңыз. Тәуліктік тарифтер мен валюталарды **Орнату** > **Есептеулер мен кодтар** > **Тәуліктік** тармағында конфигурациялауға болады.
3. **Тәуліктік орындар** бетінде тәуліктік тариф деңгейлерін конфигурациялаңыз. Тәуліктік тариф деңгейлері қонақ үйге, тамақтануға және басқа шығыстарға күнделікті жәрдемақының пайыздық бөлінуін анықтауға мүмкіндік береді. 
4. Таңертеңгілік, түскі немесе кешкі ас кезінде тамақтану пайызының төмендеуін көрсету үшін **Шығысты басқару параметрлері** бетіндегі **Тәуліктік** қойыншасында өрістерді жаңартыңыз. 
    
## <a name="submit-expenses-using-per-diem"></a>Тәуліктік тарифті пайдаланып шығыстарды жіберу
Бір тәуліктік шығыстарды жіберу үшін шығыс туралы есепті жасаған кезде **Тәуліктік** шығыс санатын пайдаланыңыз. **Күнінен бастап алынған тәуліктік тариф**, **Бүгінгі күнге дейінгі тәуліктік тариф** және **Тәуліктік орын** енгізіңіз. Бұл сома таңдалған орын үшін тәуліктік тарифтер негізінде есептеледі, ал тамақтануды төмендету тәуліктік тариф деңгейлері бойынша есептеледі.
