---
title: Демо нұсқа параметрлері мен конфигурация деректерін қолдану
description: Бұл тақырып Project Operations жүйесі үшін демонстрацияны және конфигурация деректерін қолдану туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42e02f393e89d20b2a462645f519a3792bee8f2f
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948947"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="a9b18-103">Project Operations қарапайым орналастыруы үшін демо баптау және конфигурация деректерін қолдану - проформа-шотын ұсыну мәмілесі</span><span class="sxs-lookup"><span data-stu-id="a9b18-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="a9b18-104">_\*\*Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="a9b18-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="a9b18-105">[Негізгі деректер бумасын](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip) жүктеп алыңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="a9b18-106">*ProjOpsDemoDataSetupAndMaster - біріктірілген CMT* өтіп, орындалатын файлды *DataMigrationUtility* орындалатын файлды іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="a9b18-107">Common Data Service конфигурацияны тасымалдау (CMT) шеберінің 1-бетінде**Деректерді импорттау**, содан кейін **Жалғастыру** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Конфигурацияны тасымалдау](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="a9b18-109">CMT шеберінің 2-бетінде **Орналастыру түрі** ретінде **Office 365** қызметін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-109">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="a9b18-110">**Қолжетімді ұйымдар тізімін көрсету** және **Кеңейтілген түрде көрсету** өрістеріне құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="a9b18-111">Қатысушы аймағын таңдап, тіркелу деректеріңізді енгізіп, содан кейін **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Конфигурацияға кіру](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="a9b18-113">3-бетте, қатысушыдағы ұйымдар тізімінен демо деректерді импорттау ұйымын таңдап, содан соң **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="a9b18-114">4-бетте бумадан шығарылған қалтадан *MasterAndSetupData* zip файлын, *ProjOpsDemoDataSetupAndMaster - біріктірілген CMT* таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Zip файлы](./media/3ZipFile.png)

![Файлды таңдаңыз](./media/4SelectAFile.png)

9. <span data-ttu-id="a9b18-117">Zip файлы таңдалғаннан кейін **Деректерді импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-117">After the zip file is selected, select **Import Data**.</span></span>

![Деректерді импорттау](./media/5ImportData.png)

10. <span data-ttu-id="a9b18-119">Импорттау желі жылдамдығына байланысты шамамен екі-он минутқа созылады.</span><span class="sxs-lookup"><span data-stu-id="a9b18-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="a9b18-120">Аяқтағаннан кейін CMT шеберінен шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="a9b18-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="a9b18-121">Ұйымыңыздан келесі 20 ұйымның деректерін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="a9b18-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="a9b18-122">Валюта</span><span class="sxs-lookup"><span data-stu-id="a9b18-122">Currency</span></span>
- <span data-ttu-id="a9b18-123">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="a9b18-123">Organizational Unit</span></span>
- <span data-ttu-id="a9b18-124">Істес кісі</span><span class="sxs-lookup"><span data-stu-id="a9b18-124">Contact</span></span>
- <span data-ttu-id="a9b18-125">Салық тобы</span><span class="sxs-lookup"><span data-stu-id="a9b18-125">Tax Group</span></span>
- <span data-ttu-id="a9b18-126">Тұтынушы тобы</span><span class="sxs-lookup"><span data-stu-id="a9b18-126">Customer Group</span></span>
- <span data-ttu-id="a9b18-127">Бірлік</span><span class="sxs-lookup"><span data-stu-id="a9b18-127">Unit</span></span>
- <span data-ttu-id="a9b18-128">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="a9b18-128">Unit Group</span></span>
- <span data-ttu-id="a9b18-129">Бағатізбе</span><span class="sxs-lookup"><span data-stu-id="a9b18-129">Price List</span></span>
- <span data-ttu-id="a9b18-130">Жоба параметрі бағатізбесі</span><span class="sxs-lookup"><span data-stu-id="a9b18-130">Project Parameter Price List</span></span>
- <span data-ttu-id="a9b18-131">Есеп-шот жиілігі</span><span class="sxs-lookup"><span data-stu-id="a9b18-131">Invoice Frequency</span></span>
- <span data-ttu-id="a9b18-132">Есеп-шот жиілігі мәліметі</span><span class="sxs-lookup"><span data-stu-id="a9b18-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="a9b18-133">Тапсырыс беруге болатын ресурс санаты</span><span class="sxs-lookup"><span data-stu-id="a9b18-133">Bookable Resource Category</span></span>
- <span data-ttu-id="a9b18-134">Транзакция санаты</span><span class="sxs-lookup"><span data-stu-id="a9b18-134">Transaction Category</span></span>
- <span data-ttu-id="a9b18-135">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="a9b18-135">Expense Category</span></span>
- <span data-ttu-id="a9b18-136">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="a9b18-136">Role Price</span></span>
- <span data-ttu-id="a9b18-137">Транзакция санаты бағасы</span><span class="sxs-lookup"><span data-stu-id="a9b18-137">Transaction Category Price</span></span>
- <span data-ttu-id="a9b18-138">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="a9b18-138">Characteristic</span></span>
- <span data-ttu-id="a9b18-139">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="a9b18-139">Bookable Resource</span></span>
- <span data-ttu-id="a9b18-140">Тапсырыс беруге болатын ресурс санатының байланысы</span><span class="sxs-lookup"><span data-stu-id="a9b18-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="a9b18-141">Тапсырыс беруге болатын ресурс сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="a9b18-141">Bookable Resource Characteristic</span></span>

![Импорттауды аяқтау](./media/6CompleteImport.png)
