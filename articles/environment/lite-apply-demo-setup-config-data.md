---
title: Демо нұсқа параметрлері мен конфигурация деректерін қолдану - жеңілдетілген
description: Бұл тақырып Project Operations жүйесі үшін демонстрацияны және конфигурация деректерін қолдану туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 421c9d28088c92617687641d93b3ad5d6bfea73c
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642100"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="5f1a1-103">Project Operations жүйесіне арналған демо нұсқа параметрлерін және конфигурация деректерін қолдану - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="5f1a1-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="5f1a1-104">_\*\*Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="5f1a1-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="5f1a1-105">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="5f1a1-105">Prerequisites</span></span>

<span data-ttu-id="5f1a1-106">Конфигурацияны бастамас бұрын, Dynamics 365 Project Operations бағдарламасы үшін Common Data Service (CDS) ортасы дайындалған болуы қажет.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="5f1a1-107">Нұсқаулар</span><span class="sxs-lookup"><span data-stu-id="5f1a1-107">Instructions</span></span>

1. <span data-ttu-id="5f1a1-108">[Негізгі деректер бумасын](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip) жүктеп алыңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="5f1a1-109">*ProjOpsDemoDataSetupAndMaster - біріктірілген CMT* өтіп, орындалатын файлды *DataMigrationUtility* орындалатын файлды іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="5f1a1-110">Common Data Service конфигурацияны тасымалдау (CMT) шеберінің 1-бетінде **Деректерді импорттау**, содан кейін **Жалғастыру** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Конфигурацияны тасымалдау](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="5f1a1-112">CMT шеберінің 2-бетінде **Орналастыру түрі** ретінде **Microsoft 365** қызметін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="5f1a1-113">**Қолжетімді ұйымдар тізімін көрсету** және **Кеңейтілген түрде көрсету** өрістеріне құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="5f1a1-114">Қатысушы аймағын таңдап, тіркелу деректеріңізді енгізіп, содан кейін **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Конфигурацияға кіру](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="5f1a1-116">3-бетте, қатысушыдағы ұйымдар тізімінен демо деректерді импорттау ұйымын таңдап, содан соң **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="5f1a1-117">4-бетте бумадан шығарылған қалтадан *MasterAndSetupData* zip файлын, *ProjOpsDemoDataSetupAndMaster - біріктірілген CMT* таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Zip файлы](./media/3ZipFile.png)

![Файлды таңдаңыз](./media/4SelectAFile.png)

9. <span data-ttu-id="5f1a1-120">Zip файлы таңдалғаннан кейін **Деректерді импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-120">After the zip file is selected, select **Import Data**.</span></span>

![Деректерді импорттау](./media/5ImportData.png)

10. <span data-ttu-id="5f1a1-122">Импорттау желі жылдамдығына байланысты шамамен екі-он минутқа созылады.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="5f1a1-123">Аяқтағаннан кейін CMT шеберінен шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="5f1a1-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="5f1a1-124">Ұйымыңыздан келесі 20 ұйымның деректерін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="5f1a1-124">Check your organization for data in the following 20 entities:</span></span>

-   <span data-ttu-id="5f1a1-125">Валюта</span><span class="sxs-lookup"><span data-stu-id="5f1a1-125">Currency</span></span>
-   <span data-ttu-id="5f1a1-126">Тіркелгі</span><span class="sxs-lookup"><span data-stu-id="5f1a1-126">Account</span></span>
-   <span data-ttu-id="5f1a1-127">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="5f1a1-127">Organizational Unit</span></span>
-   <span data-ttu-id="5f1a1-128">Істес кісі</span><span class="sxs-lookup"><span data-stu-id="5f1a1-128">Contact</span></span>
-   <span data-ttu-id="5f1a1-129">Салық тобы</span><span class="sxs-lookup"><span data-stu-id="5f1a1-129">Tax Group</span></span>
-   <span data-ttu-id="5f1a1-130">Тұтынушы тобы</span><span class="sxs-lookup"><span data-stu-id="5f1a1-130">Customer Group</span></span>
-   <span data-ttu-id="5f1a1-131">Бірлік</span><span class="sxs-lookup"><span data-stu-id="5f1a1-131">Unit</span></span>
-   <span data-ttu-id="5f1a1-132">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="5f1a1-132">Unit Group</span></span>
-   <span data-ttu-id="5f1a1-133">Бағатізбе</span><span class="sxs-lookup"><span data-stu-id="5f1a1-133">Price List</span></span>
-   <span data-ttu-id="5f1a1-134">Жоба параметрі бағатізбесі</span><span class="sxs-lookup"><span data-stu-id="5f1a1-134">Project Parameter Price List</span></span> 
-   <span data-ttu-id="5f1a1-135">Есеп-шот жиілігі</span><span class="sxs-lookup"><span data-stu-id="5f1a1-135">Invoice Frequency</span></span>
-   <span data-ttu-id="5f1a1-136">Тапсырыс беруге болатын ресурс санаты</span><span class="sxs-lookup"><span data-stu-id="5f1a1-136">Bookable Resource Category</span></span>
-   <span data-ttu-id="5f1a1-137">Транзакция санаты</span><span class="sxs-lookup"><span data-stu-id="5f1a1-137">Transaction Category</span></span>
-   <span data-ttu-id="5f1a1-138">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="5f1a1-138">Expense Category</span></span>
-   <span data-ttu-id="5f1a1-139">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="5f1a1-139">Role Price</span></span>
-   <span data-ttu-id="5f1a1-140">Транзакция санаты бағасы</span><span class="sxs-lookup"><span data-stu-id="5f1a1-140">Transaction Category Price</span></span>
-   <span data-ttu-id="5f1a1-141">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="5f1a1-141">Characteristic</span></span>
-   <span data-ttu-id="5f1a1-142">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="5f1a1-142">Bookable Resource</span></span>
-   <span data-ttu-id="5f1a1-143">Тапсырыс беруге болатын ресурс санатының байланысы</span><span class="sxs-lookup"><span data-stu-id="5f1a1-143">Bookable resource category Assn</span></span>
-   <span data-ttu-id="5f1a1-144">Тапсырыс беруге болатын ресурс сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="5f1a1-144">Bookable Resource Characteristic</span></span>

![Импорттауды аяқтау](./media/6CompleteImport.png)
