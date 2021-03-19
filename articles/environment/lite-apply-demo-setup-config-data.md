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
ms.openlocfilehash: 694dbc74591de74895095a9da6e590069711fc83
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290141"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="b976e-103">Project Operations жүйесіне арналған демо нұсқа параметрлерін және конфигурация деректерін қолдану - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="b976e-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="b976e-104">_\*\*Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="b976e-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="b976e-105">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="b976e-105">Prerequisites</span></span>

<span data-ttu-id="b976e-106">Конфигурацияны бастамас бұрын, Dynamics 365 Project Operations бағдарламасы үшін Common Data Service (CDS) ортасы дайындалған болуы қажет.</span><span class="sxs-lookup"><span data-stu-id="b976e-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="b976e-107">Нұсқаулар</span><span class="sxs-lookup"><span data-stu-id="b976e-107">Instructions</span></span>

1. <span data-ttu-id="b976e-108">[Негізгі деректер бумасын](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip) жүктеп алыңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="b976e-109">*ProjOpsDemoDataSetupAndMaster - біріктірілген CMT* өтіп, орындалатын файлды *DataMigrationUtility* орындалатын файлды іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="b976e-110">Common Data Service конфигурацияны тасымалдау (CMT) шеберінің 1-бетінде **Деректерді импорттау**, содан кейін **Жалғастыру** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![Конфигурацияны тасымалдау](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="b976e-112">CMT шеберінің 2-бетінде **Орналастыру түрі** ретінде **Microsoft 365** қызметін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="b976e-113">**Қолжетімді ұйымдар тізімін көрсету** және **Кеңейтілген түрде көрсету** өрістеріне құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="b976e-114">Қатысушы аймағын таңдап, тіркелу деректеріңізді енгізіп, содан кейін **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![Конфигурацияға кіру](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="b976e-116">3-бетте, қатысушыдағы ұйымдар тізімінен демо деректерді импорттау ұйымын таңдап, содан соң **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="b976e-117">4-бетте бумадан шығарылған қалтадан *MasterAndSetupData* zip файлын, *ProjOpsDemoDataSetupAndMaster - біріктірілген CMT* таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

   ![Zip файлы](./media/3ZipFile.png)

   ![Файлды таңдаңыз](./media/4SelectAFile.png)

9. <span data-ttu-id="b976e-120">Zip файлы таңдалғаннан кейін **Деректерді импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-120">After the zip file is selected, select **Import Data**.</span></span>

   ![Деректерді импорттау](./media/5ImportData.png)

10. <span data-ttu-id="b976e-122">Импорттау желі жылдамдығына байланысты шамамен екі-он минутқа созылады.</span><span class="sxs-lookup"><span data-stu-id="b976e-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="b976e-123">Аяқтағаннан кейін CMT шеберінен шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="b976e-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="b976e-124">Ұйымыңыздан келесі 20 ұйымның деректерін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="b976e-124">Check your organization for data in the following 20 entities:</span></span>

    -   <span data-ttu-id="b976e-125">Валюта</span><span class="sxs-lookup"><span data-stu-id="b976e-125">Currency</span></span>
    -   <span data-ttu-id="b976e-126">Тіркелгі</span><span class="sxs-lookup"><span data-stu-id="b976e-126">Account</span></span>
    -   <span data-ttu-id="b976e-127">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="b976e-127">Organizational Unit</span></span>
    -   <span data-ttu-id="b976e-128">КОНТАКТ </span><span class="sxs-lookup"><span data-stu-id="b976e-128">Contact</span></span>
    -   <span data-ttu-id="b976e-129">Бірлік</span><span class="sxs-lookup"><span data-stu-id="b976e-129">Unit</span></span>
    -   <span data-ttu-id="b976e-130">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="b976e-130">Unit Group</span></span>
    -   <span data-ttu-id="b976e-131">Бағатізбе</span><span class="sxs-lookup"><span data-stu-id="b976e-131">Price List</span></span>
    -   <span data-ttu-id="b976e-132">Жоба параметрі бағатізбесі</span><span class="sxs-lookup"><span data-stu-id="b976e-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="b976e-133">Есеп-шот жиілігі</span><span class="sxs-lookup"><span data-stu-id="b976e-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="b976e-134">Тапсырыс беруге болатын ресурс санаты</span><span class="sxs-lookup"><span data-stu-id="b976e-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="b976e-135">Транзакция санаты</span><span class="sxs-lookup"><span data-stu-id="b976e-135">Transaction Category</span></span>
    -   <span data-ttu-id="b976e-136">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="b976e-136">Expense Category</span></span>
    -   <span data-ttu-id="b976e-137">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="b976e-137">Role Price</span></span>
    -   <span data-ttu-id="b976e-138">Транзакция санаты бағасы</span><span class="sxs-lookup"><span data-stu-id="b976e-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="b976e-139">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="b976e-139">Characteristic</span></span>
    -   <span data-ttu-id="b976e-140">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="b976e-140">Bookable Resource</span></span>
    -   <span data-ttu-id="b976e-141">Тапсырыс беруге болатын ресурс санатының байланысы</span><span class="sxs-lookup"><span data-stu-id="b976e-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="b976e-142">Тапсырыс беруге болатын ресурс сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="b976e-142">Bookable Resource Characteristic</span></span>

    ![Импорттауды аяқтау](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]