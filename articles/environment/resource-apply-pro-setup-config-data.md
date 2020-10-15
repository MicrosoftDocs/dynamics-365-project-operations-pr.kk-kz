---
title: Project Operations жүйесіне арналған Common Data Service бағдарламасында конфигурация деректерін орнату және қолдану
description: Бұл тақырып Project Operations жүйесінде конфигурация деректерін қолдану туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d99ab4c7b2ebf6ba56b86a3e0151036c6247e484
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948950"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a><span data-ttu-id="19392-103">Project Operations жүйесіне арналған Common Data Service бағдарламасында конфигурация деректерін орнату және қолдану</span><span class="sxs-lookup"><span data-stu-id="19392-103">Set up and apply configuration data in the Common Data Service for Project Operations</span></span>

<span data-ttu-id="19392-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="19392-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="19392-105">Орнату және конфигурация деректерін орнату</span><span class="sxs-lookup"><span data-stu-id="19392-105">Install setup and configuration data</span></span>

1. <span data-ttu-id="19392-106">[Орнату және конфигурация деректер бумасын](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip) жүктеңіз, құлыптан шығарыңыз және мұрағаттан шығарыңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-106">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="19392-107">Мұрағаттан шығарылмаған қалтаға өтіп, *DataMigrationUtility* орындалатын файлды іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-107">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="19392-108">Common Data Service конфигурацияны тасымалдау (CMT) шеберінің 1-бетінде**Деректерді импорттау**, содан кейін **Жалғастыру** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-108">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Конфигурацияны тасымалдау](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="19392-110">CMT шеберінің 2-бетінде **Орналастыру түрі** ретінде **Office 365** қызметін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-110">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="19392-111">**Қолжетімді ұйымдар тізімін көрсету** және **Кеңейтілген түрде көрсету** өрістеріне құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-111">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="19392-112">Қатысушы аймағын таңдап, тіркелу деректеріңізді енгізіп, **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-112">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Конфигурацияға кіру](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="19392-114">3-бетте, қатысушыдағы ұйымдар тізімінен демо деректерді импорттау ұйымын таңдап, содан соң **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-114">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="19392-115">4-бетте бумадан шығарылған қалтадан *SampleSetupAndConfigData* zip файлын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-115">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Zip файлын таңдау](./media/3ZipFile.png)

![Файлды таңдаңыз](./media/4SelectAFile.png)

9. <span data-ttu-id="19392-118">Zip файлы таңдалғаннан кейін **Деректерді импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-118">After the zip file is selected, select **Import Data**.</span></span>

![Деректерді импорттау](./media/5ImportData.png)

10. <span data-ttu-id="19392-120">Импорттау желі жылдамдығына байланысты шамамен екі-он минутқа созылады.</span><span class="sxs-lookup"><span data-stu-id="19392-120">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="19392-121">Импорттау аяқталғаннан кейін CMT шеберінен шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-121">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="19392-122">Ұйымыңыздан келесі 19 ұйымның деректерін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="19392-122">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="19392-123">Валюта</span><span class="sxs-lookup"><span data-stu-id="19392-123">Currency</span></span>
  - <span data-ttu-id="19392-124">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="19392-124">Organizational Unit</span></span>
  - <span data-ttu-id="19392-125">Істес кісі</span><span class="sxs-lookup"><span data-stu-id="19392-125">Contact</span></span>
  - <span data-ttu-id="19392-126">Салық тобы</span><span class="sxs-lookup"><span data-stu-id="19392-126">Tax Group</span></span>
  - <span data-ttu-id="19392-127">Тұтынушы тобы</span><span class="sxs-lookup"><span data-stu-id="19392-127">Customer Group</span></span>
  - <span data-ttu-id="19392-128">Бірлік</span><span class="sxs-lookup"><span data-stu-id="19392-128">Unit</span></span>
  - <span data-ttu-id="19392-129">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="19392-129">Unit Group</span></span>
  - <span data-ttu-id="19392-130">Бағатізбе</span><span class="sxs-lookup"><span data-stu-id="19392-130">Price List</span></span>
  - <span data-ttu-id="19392-131">Жоба параметрі бағатізбесі</span><span class="sxs-lookup"><span data-stu-id="19392-131">Project Parameter Price List</span></span>
  - <span data-ttu-id="19392-132">Есеп-шот жиілігі</span><span class="sxs-lookup"><span data-stu-id="19392-132">Invoice Frequency</span></span>
  - <span data-ttu-id="19392-133">Тапсырыс беруге болатын ресурс санаты</span><span class="sxs-lookup"><span data-stu-id="19392-133">Bookable Resource Category</span></span>
  - <span data-ttu-id="19392-134">Транзакция санаты</span><span class="sxs-lookup"><span data-stu-id="19392-134">Transaction Category</span></span>
  - <span data-ttu-id="19392-135">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="19392-135">Expense Category</span></span>
  - <span data-ttu-id="19392-136">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="19392-136">Role Price</span></span>
  - <span data-ttu-id="19392-137">Транзакция санаты бағасы</span><span class="sxs-lookup"><span data-stu-id="19392-137">Transaction Category Price</span></span>
  - <span data-ttu-id="19392-138">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="19392-138">Characteristic</span></span>
  - <span data-ttu-id="19392-139">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="19392-139">Bookable Resource</span></span>
  - <span data-ttu-id="19392-140">Тапсырыс беруге болатын ресурс санатының байланысы</span><span class="sxs-lookup"><span data-stu-id="19392-140">Bookable resource category Assn</span></span>
  - <span data-ttu-id="19392-141">Тапсырыс беруге болатын ресурс сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="19392-141">Bookable Resource Characteristic</span></span>

![Импорттауды аяқтау](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="19392-143">Project Operations конфигурацияларын жаңарту</span><span class="sxs-lookup"><span data-stu-id="19392-143">Update Project Operations configurations</span></span>

1. <span data-ttu-id="19392-144">CE ортасына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="19392-144">Navigate to the CE environment.</span></span> <span data-ttu-id="19392-145">Оны [Power Platform басқару орталығын](https://admin.powerplatform.microsoft.com/environments) ашып, ортаны таңдап, содан кейін **Ортаны ашу** опциясын таңдау арқылы табуға болады.</span><span class="sxs-lookup"><span data-stu-id="19392-145">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Ортаны ашу](./media/7OpenEnvironment.png)

2. <span data-ttu-id="19392-147">Пайдаланушыға арналған тапсырыс беруге болатын ресурсты жасау үшін **Жобалар** > **Ресурс**, содан кейін **Жаңа** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="19392-147">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Тапсырыс беруге болатын ресурстар](./media/8BookableResources.png)

3. <span data-ttu-id="19392-149">**Жалпы мәліметтер** қойыншасында әкімші пайдаланушыны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-149">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="19392-150">Уақыт белдеуі сіз тұрған аймаққа сәйкес келетіндігін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="19392-150">Verify that the time zone matches the one you are in.</span></span> 

![Жаңа тапсырыс беруге болатын ресурс](./media/9NewBookableResource.png)

4. <span data-ttu-id="19392-152">**Жоспарлау** қойыншасындағы **Компания** өрісінде **USPM** компаниясын таңдап, содан соң **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-152">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Жоспарлау қойыншасы](./media/10SchedulingTab.png)

5. <span data-ttu-id="19392-154">**Жұмыс сағаттары** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-154">Select the **Work hours** tab.</span></span>  

![Жұмыс сағаттары](./media/11WorkHours.png)

6. <span data-ttu-id="19392-156">Күнтізбедегі кез келген мәнді екі рет шертіп, **Өңдеу** > **Сериядағы барлық оқиғалар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-156">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Іскери күнтізбе](./media/12WorkCalendar.png)

7. <span data-ttu-id="19392-158">Жұмыс уақытын сегіз (8) сағаттық жұмыс күніне ауыстырыңыз, демалыс күндерін жұмыс емес күн ретінде белгілеңіз және уақыт белдеуі сіздікімен сәйкес келетініне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="19392-158">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="19392-159">**Сақтау және жабу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-159">Select **Save and close**.</span></span>

![Күнтізбені жаңарту](./media/13UpdateCalendar.png)

9. <span data-ttu-id="19392-161">**Параметрлер** > **Күнтізбелік үлгілер** тармағына өтіп, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-161">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Күнтізбе үлгілері](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="19392-163">Атын енгізіп, жасаған үлгі ресурсын таңдап, содан кейін **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-163">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Күнтізбе үлгісін сақтау](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="19392-165">**Параметрлер** тармағына өтіп, жазбаны екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-165">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Жоба параметрлері](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="19392-167">Келесі өрістерді жаңартыңыз:</span><span class="sxs-lookup"><span data-stu-id="19392-167">Update the following fields:</span></span>

 - <span data-ttu-id="19392-168">**Әдепкі компания**: USPM</span><span class="sxs-lookup"><span data-stu-id="19392-168">**Default company**: USPM</span></span>
 - <span data-ttu-id="19392-169">**Әдепкі ұйымдық бөлім**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="19392-169">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="19392-170">**Шот-фактураның жиілігі**: Жетінші және соңғы күн</span><span class="sxs-lookup"><span data-stu-id="19392-170">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="19392-171">**Жұмыс уақытының үлгісі**: Сіз жасаған үлгі өзгерісі.</span><span class="sxs-lookup"><span data-stu-id="19392-171">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="19392-172">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="19392-172">Select **Save**.</span></span> 

![Жаңартылған жоба параметрлері](./media/17UpdatedProjectParameters.png)
