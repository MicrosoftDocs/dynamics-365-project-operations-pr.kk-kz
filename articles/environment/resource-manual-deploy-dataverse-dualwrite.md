---
title: Қос жазу мүмкіндігіне ие Project Operations Dataverse бағдарламасын қолмен орналастыру
description: Бұл тақырып қос жазу мүмкіндігіне қолдау көрсетуі үшін Project Operations Dataverse бағдарламасын қолмен орналастыру жолын түсіндіреді.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 06325a9a9f9084d1f506f2493c32565fe7b7c52ae6fe22c81339b9c1d632e688
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986453"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a>Қос жазу мүмкіндігіне ие Project Operations Dataverse бағдарламасын қолмен орналастыру

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

Бұл тақырып қос жазу мүмкіндігіне қолдау көрсетуі үшін Microsoft Dynamics 365 Project Operations бағдарламасын Microsoft Dataverse жүйесіне қолмен орналастыру жолын түсіндіреді. Project Operations бағдарламасы ортаның конфигурациясын анықтайды және алғышарттар орындалған жағдайда қос жазу мүмкіндігіне қосымша қолдау көрсетеді.

Microsoft Dynamics Lifecycle Services (LCS) арқылы орналастыру кезінде егер сіз осы тақырыптағы нұсқауларды орындаған болсаңыз, Microsoft Power Platform біріктіруін (бұрын Common Data Service ортасы деп аталған) орналастыруды өткізіп жіберсеңіз болады.

Қос жазу мүмкіндігіне қолдау көрсетуі үшін Project Operations бағдарламасын Dataverse жүйесіне орналастырудың төрт негізгі қадамы бар:

1. [Dataverse жүйесінде қос жазу мүмкіндігіне қолдау көрсететін жаңа орта жасау](#create).
2. [Ортаға қос жазу алғышарттарын қосу](#prerequisites).
3. [Project Operations Dataverse бағдарламасын қосу](#dataverse).
4. [Орталарды байланыстыру](#link).

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a>Dataverse жүйесінде қос жазу мүмкіндігіне қолдау көрсететін жаңа орта жасау

Бұл процедураны орындау үшін әкімші ретінде кіру керек.

1. [Power Platform басқару орталығын](https://admin.powerplatform.com) ашыңыз және әкімші ретінде кіріңіз.
2. Жаңа орта жасаңыз және оған атау беріңіз.
3. Орта түрін таңдаңыз. Егер сіз сынақ нұсқасы ұсынысына жазылсаңыз, **Сынақ нұсқасы (жазылымға негізделген)** түрін таңдаңыз.
4. Орналастыру аймағын растаңыз.
5. **Осы орта үшін дерекқор жасау** опциясын қосыңыз. 
6. Тілді растаңыз және содан кейін валютаның Finance and Operations бағдарламаларының валютасына сәйкес келетінін растаңыз.
7. **Dynamics 365 бағдарламалары** опциясын қосыңыз және **Осы бағдарламаларды автоматты түрде орналастыру** өрісінің **Жоқ** мәніне орнатылғанын растаңыз.
8. Қауіпсіздік тобы қажет болса, қауіпсіздік тобын қосыңыз.
9. Орта жасау үшін **Сақтау** пәрменін таңдаңыз.
10. Орналастыру аяқталғанын және ортаның **Дайын** күйіне жетуін күтіңіз.

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a>Ортаға қос жазу алғышарттарын қосу

Қос жазу қолдауы **Компания** нысаны сияқты негізгі нысандарға қосылатын қосымша өрістерді қамтиды. Егер сіз бұрыннан бар ортаға қос жазу қолдауын қоссаңыз, қолдауды қосу үшін деректерді жаңартуыңыз керек болуы мүмкін. Деректерді бастапқы жүктеу әдісі туралы ақпарат алу үшін [Компания деректерін бастапқы жүктеу](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data) бөлімін қараңыз. Қос жазу мүмкіндігін туралы қосымша ақпарат алу үшін [Қос жазу жүйесінің талаптары](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req) бөлімін қараңыз.

Ортаға қос жазу алғышарттарын қосу үшін осы процедураны аяқтаңыз.

1. Жаңа ғана жасаған ортаны ашыңыз және содан кейін **Ресурс** \> **Dynamics 365 бағдарламалары** тармағына өтіңіз.
2. Бағдарлама тізімінде **Қос жазу негізгі шешімі** параметрін таңдаңыз және оны орнатыңыз.
3. Орнату аяқталғанша күтіңіз. Содан кейін бағдарлама тізімінде **Қос жазу бағдарламасы өзара қатынасының шешімі** параметрін таңдаңыз және оны орнатыңыз.

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a>Project Operations Dataverse бағдарламасын қосу

Сіз бұл процедураны тек Project Operations бағдарламасын орнатпас бұрын алдыңғы процедураларды орындаған жағдайда ғана орындай аласыз. Орнату кезінде жүйе орта конфигурациясын талдайды және қажет болған жағдайда қос жазу мүмкіндігіне қолдау қосады.

1. Бұрын жасаған ортаны ашыңыз және содан кейін **Ресурс** \> **Dynamics 365 бағдарламалары** тармағына өтіңіз.
2. Бағдарлама тізімінен **Microsoft Dynamics 365 Project Operations** бағдарламасын таңдаңыз және оны орнатыңыз.

## <a name="link-your-environments"></a><a name="link"></a>Орталарды байланыстыру

Dataverse ортасы орналастырылғаннан кейін, Finance and Operations бағдарламаларындағы сілтемені реттеуге болады. [Орталарды байланыстыру үшін қос жазу шеберін пайдалану](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment) бөліміндегі қадамдарды орындаңыз.