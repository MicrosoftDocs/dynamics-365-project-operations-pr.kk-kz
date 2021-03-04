---
title: Демо нұсқа параметрлері мен конфигурация деректерін қолдану - жеңілдетілген
description: Бұл тақырып Project Operations жүйесі үшін демонстрацияны және конфигурация деректерін қолдану туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 762b0cf317d442565a033f56033a53a5b5cc435c
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089126"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>Project Operations жүйесіне арналған демо нұсқа параметрлерін және конфигурация деректерін қолдану - жеңілдетілген 

_**Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a>Алғышарттар

Конфигурацияны бастамас бұрын, Dynamics 365 Project Operations бағдарламасы үшін Common Data Service (CDS) ортасы дайындалған болуы қажет.


## <a name="instructions"></a>Нұсқаулар

1. [Негізгі деректер бумасын](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip) жүктеп алыңыз. 
2. *ProjOpsDemoDataSetupAndMaster - біріктірілген CMT* өтіп, орындалатын файлды *DataMigrationUtility* орындалатын файлды іске қосыңыз.
3. Common Data Service конфигурацияны тасымалдау (CMT) шеберінің 1-бетінде **Деректерді импорттау**, содан кейін **Жалғастыру** опцияларын таңдаңыз.

    ![Конфигурацияны тасымалдау](./media/1ConfigurationMigration.png)

4. CMT шеберінің 2-бетінде **Орналастыру түрі** ретінде **Microsoft 365** қызметін таңдаңыз.
5. **Қолжетімді ұйымдар тізімін көрсету** және **Кеңейтілген түрде көрсету** өрістеріне құсбелгі қойыңыз.
6. Қатысушы аймағын таңдап, тіркелу деректеріңізді енгізіп, содан кейін **Жүйеге кіру** опциясын таңдаңыз.

   ![Конфигурацияға кіру](./media/2ConfigurationSignin.png)

7. 3-бетте, қатысушыдағы ұйымдар тізімінен демо деректерді импорттау ұйымын таңдап, содан соң **Жүйеге кіру** опциясын таңдаңыз.
8. 4-бетте бумадан шығарылған қалтадан *MasterAndSetupData* zip файлын, *ProjOpsDemoDataSetupAndMaster - біріктірілген CMT* таңдаңыз.

   ![Zip файлы](./media/3ZipFile.png)

   ![Файлды таңдаңыз](./media/4SelectAFile.png)

9. Zip файлы таңдалғаннан кейін **Деректерді импорттау** опциясын таңдаңыз.

   ![Деректерді импорттау](./media/5ImportData.png)

10. Импорттау желі жылдамдығына байланысты шамамен екі-он минутқа созылады. Аяқтағаннан кейін CMT шеберінен шығыңыз. 
11. Ұйымыңыздан келесі 20 ұйымның деректерін тексеріңіз:

    -   Валюта
    -   Тіркелгі
    -   Ұйымдық бірлік
    -   КОНТАКТ 
    -   Бірлік
    -   Бірлік тобы
    -   Бағатізбе
    -   Жоба параметрі бағатізбесі 
    -   Есеп-шот жиілігі
    -   Тапсырыс беруге болатын ресурс санаты
    -   Транзакция санаты
    -   Шығыс санаты
    -   Рөл бағасы
    -   Транзакция санаты бағасы
    -   Сипаттама
    -   Резервтелетін ресурс
    -   Тапсырыс беруге болатын ресурс санатының байланысы
    -   Тапсырыс беруге болатын ресурс сипаттамасы

    ![Импорттауды аяқтау](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]