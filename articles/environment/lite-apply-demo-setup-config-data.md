---
title: Демо нұсқа параметрлері мен конфигурация деректерін қолдану - жеңілдетілген
description: Бұл тақырып Project Operations жүйесі үшін демонстрацияны және конфигурация деректерін қолдану туралы ақпарат береді.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7729b4a9ef5f498b78af298f7233d7dd45434bb3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997158"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="82f23-103">Project Operations жүйесіне арналған демо нұсқа параметрлерін және конфигурация деректерін қолдану - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="82f23-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="82f23-104">_\*\*Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="82f23-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="82f23-105">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="82f23-105">Prerequisites</span></span>

<span data-ttu-id="82f23-106">Конфигурацияны бастамас бұрын, Dynamics 365 Project Operations бағдарламасы үшін Common Data Service (CDS) ортасы дайындалған болуы қажет.</span><span class="sxs-lookup"><span data-stu-id="82f23-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="82f23-107">Нұсқаулар</span><span class="sxs-lookup"><span data-stu-id="82f23-107">Instructions</span></span>

1. <span data-ttu-id="82f23-108">[Негізгі деректер бумасын](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip) жүктеп алыңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip).</span></span> 
2. <span data-ttu-id="82f23-109">*ProjOpsSampleSetupData - CE тек CMT* қалтасына өтіңіз және *DataMigrationUtility* орындалатын файлын іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-109">Navigate to the folder *ProjOpsSampleSetupData - CE only CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="82f23-110">Common Data Service конфигурацияны тасымалдау (CMT) шеберінің 1-бетінде **Деректерді импорттау**, содан кейін **Жалғастыру** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![Конфигурацияны тасымалдау](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="82f23-112">CMT шеберінің 2-бетінде **Орналастыру түрі** ретінде **Microsoft 365** қызметін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="82f23-113">**Қолжетімді ұйымдар тізімін көрсету** және **Кеңейтілген түрде көрсету** өрістеріне құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="82f23-114">Қатысушы аймағын таңдап, тіркелу деректеріңізді енгізіп, содан кейін **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![Конфигурацияға кіру](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="82f23-116">3-бетте, қатысушыдағы ұйымдар тізімінен демо деректерді импорттау ұйымын таңдап, содан соң **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="82f23-117">4-бетте *ProjOpsSampleSetupData - CE тек CMT* бумадан шығарылған қалтадан *SampleSetupAndConfigData* zip файлын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-117">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder, *ProjOpsSampleSetupData - CE only CMT*.</span></span>

   ![Zip файлы](./media/3ZipFile.png)

   ![Файл таңдау](./media/4SelectAFile.png)

9. <span data-ttu-id="82f23-120">Zip файлы таңдалғаннан кейін **Деректерді импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-120">After the zip file is selected, select **Import Data**.</span></span>

   ![Деректерді импорттау](./media/5ImportData.png)

10. <span data-ttu-id="82f23-122">Импорттау желі жылдамдығына байланысты шамамен екі-он минутқа созылады.</span><span class="sxs-lookup"><span data-stu-id="82f23-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="82f23-123">Аяқтағаннан кейін CMT шеберінен шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="82f23-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="82f23-124">Ұйымыңыздан келесі 18 ұйымның деректерін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="82f23-124">Check your organization for data in the following 18 entities:</span></span>

    -   <span data-ttu-id="82f23-125">Валюта</span><span class="sxs-lookup"><span data-stu-id="82f23-125">Currency</span></span>
    -   <span data-ttu-id="82f23-126">Тіркелгі</span><span class="sxs-lookup"><span data-stu-id="82f23-126">Account</span></span>
    -   <span data-ttu-id="82f23-127">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="82f23-127">Organizational Unit</span></span>
    -   <span data-ttu-id="82f23-128">КОНТАКТ </span><span class="sxs-lookup"><span data-stu-id="82f23-128">Contact</span></span>
    -   <span data-ttu-id="82f23-129">Бірлік</span><span class="sxs-lookup"><span data-stu-id="82f23-129">Unit</span></span>
    -   <span data-ttu-id="82f23-130">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="82f23-130">Unit Group</span></span>
    -   <span data-ttu-id="82f23-131">Бағатізбе</span><span class="sxs-lookup"><span data-stu-id="82f23-131">Price List</span></span>
    -   <span data-ttu-id="82f23-132">Жоба параметрі бағатізбесі</span><span class="sxs-lookup"><span data-stu-id="82f23-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="82f23-133">Есеп-шот жиілігі</span><span class="sxs-lookup"><span data-stu-id="82f23-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="82f23-134">Тапсырыс беруге болатын ресурс санаты</span><span class="sxs-lookup"><span data-stu-id="82f23-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="82f23-135">Транзакция санаты</span><span class="sxs-lookup"><span data-stu-id="82f23-135">Transaction Category</span></span>
    -   <span data-ttu-id="82f23-136">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="82f23-136">Expense Category</span></span>
    -   <span data-ttu-id="82f23-137">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="82f23-137">Role Price</span></span>
    -   <span data-ttu-id="82f23-138">Транзакция санаты бағасы</span><span class="sxs-lookup"><span data-stu-id="82f23-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="82f23-139">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="82f23-139">Characteristic</span></span>
    -   <span data-ttu-id="82f23-140">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="82f23-140">Bookable Resource</span></span>
    -   <span data-ttu-id="82f23-141">Тапсырыс беруге болатын ресурс санатының байланысы</span><span class="sxs-lookup"><span data-stu-id="82f23-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="82f23-142">Тапсырыс беруге болатын ресурс сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="82f23-142">Bookable Resource Characteristic</span></span>

    ![Импорттауды аяқтау](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
