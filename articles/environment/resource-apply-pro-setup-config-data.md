---
title: Common Data Service қызметінде конфигурация деректерін орнатып, қолдану
description: Бұл тақырып Project Operations жүйесінде конфигурация деректерін қолдану туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7742e81316b217066f9f3b8d5c23aa64f1a7efc4
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642235"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="83d15-103">Common Data Service қызметінде конфигурация деректерін орнатып, қолдану</span><span class="sxs-lookup"><span data-stu-id="83d15-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="83d15-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="83d15-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="83d15-105">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="83d15-105">Prerequisites</span></span>

<span data-ttu-id="83d15-106">Common Data Service (CDS) қызметінде деректерді конфигурациялауды бастамас бұрын келесі алғышарттар орындалулары керек:</span><span class="sxs-lookup"><span data-stu-id="83d15-106">Before you beging to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="83d15-107">Project Operations бағдарламасы үшін CDS ортасымен және Dynamics 365 Finance ортасымен қамтамасыз ету.</span><span class="sxs-lookup"><span data-stu-id="83d15-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="83d15-108">Dynamics 365 Finance жүйесінен алынған заңды тұлға туралы ақпарат CDS ортасымен ортақ пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="83d15-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="83d15-109">Бұл CDS қызметіндегі **Компания** нысанында келесі компаниялық жазбалардың бар екендігін білдіреді:</span><span class="sxs-lookup"><span data-stu-id="83d15-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="83d15-110">THPM</span><span class="sxs-lookup"><span data-stu-id="83d15-110">THPM</span></span>
  - <span data-ttu-id="83d15-111">USPM</span><span class="sxs-lookup"><span data-stu-id="83d15-111">USPM</span></span>
  - <span data-ttu-id="83d15-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="83d15-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="83d15-113">Орнату және конфигурация деректерін орнату</span><span class="sxs-lookup"><span data-stu-id="83d15-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="83d15-114">[Орнату және конфигурация деректер бумасын](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip) жүктеңіз, құлыптан шығарыңыз және мұрағаттан шығарыңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="83d15-115">Мұрағаттан шығарылмаған қалтаға өтіп, *DataMigrationUtility* орындалатын файлды іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="83d15-116">Common Data Service конфигурацияны тасымалдау (CMT) шеберінің 1-бетінде **Деректерді импорттау**, содан кейін **Жалғастыру** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Конфигурацияны тасымалдау](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="83d15-118">CMT шеберінің 2-бетінде **Орналастыру түрі** ретінде **Microsoft 365** қызметін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="83d15-119">**Қолжетімді ұйымдар тізімін көрсету** және **Кеңейтілген түрде көрсету** өрістеріне құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="83d15-120">Қатысушы аймағын таңдап, тіркелу деректеріңізді енгізіп, **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Конфигурацияға кіру](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="83d15-122">3-бетте, қатысушыдағы ұйымдар тізімінен демо деректерді импорттау ұйымын таңдап, содан соң **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="83d15-123">4-бетте бумадан шығарылған қалтадан *SampleSetupAndConfigData* zip файлын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Zip файлын таңдау](./media/3ZipFile.png)

![Файлды таңдаңыз](./media/4SelectAFile.png)

9. <span data-ttu-id="83d15-126">Zip файлы таңдалғаннан кейін **Деректерді импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-126">After the zip file is selected, select **Import Data**.</span></span>

![Деректерді импорттау](./media/5ImportData.png)

10. <span data-ttu-id="83d15-128">Импорттау желі жылдамдығына байланысты шамамен екі-он минутқа созылады.</span><span class="sxs-lookup"><span data-stu-id="83d15-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="83d15-129">Импорттау аяқталғаннан кейін CMT шеберінен шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="83d15-130">Ұйымыңыздан келесі 19 ұйымның деректерін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="83d15-130">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="83d15-131">Валюта</span><span class="sxs-lookup"><span data-stu-id="83d15-131">Currency</span></span>
  - <span data-ttu-id="83d15-132">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="83d15-132">Organizational Unit</span></span>
  - <span data-ttu-id="83d15-133">Істес кісі</span><span class="sxs-lookup"><span data-stu-id="83d15-133">Contact</span></span>
  - <span data-ttu-id="83d15-134">Салық тобы</span><span class="sxs-lookup"><span data-stu-id="83d15-134">Tax Group</span></span>
  - <span data-ttu-id="83d15-135">Тұтынушы тобы</span><span class="sxs-lookup"><span data-stu-id="83d15-135">Customer Group</span></span>
  - <span data-ttu-id="83d15-136">Бірлік</span><span class="sxs-lookup"><span data-stu-id="83d15-136">Unit</span></span>
  - <span data-ttu-id="83d15-137">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="83d15-137">Unit Group</span></span>
  - <span data-ttu-id="83d15-138">Бағатізбе</span><span class="sxs-lookup"><span data-stu-id="83d15-138">Price List</span></span>
  - <span data-ttu-id="83d15-139">Жоба параметрі бағатізбесі</span><span class="sxs-lookup"><span data-stu-id="83d15-139">Project Parameter Price List</span></span>
  - <span data-ttu-id="83d15-140">Есеп-шот жиілігі</span><span class="sxs-lookup"><span data-stu-id="83d15-140">Invoice Frequency</span></span>
  - <span data-ttu-id="83d15-141">Тапсырыс беруге болатын ресурс санаты</span><span class="sxs-lookup"><span data-stu-id="83d15-141">Bookable Resource Category</span></span>
  - <span data-ttu-id="83d15-142">Транзакция санаты</span><span class="sxs-lookup"><span data-stu-id="83d15-142">Transaction Category</span></span>
  - <span data-ttu-id="83d15-143">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="83d15-143">Expense Category</span></span>
  - <span data-ttu-id="83d15-144">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="83d15-144">Role Price</span></span>
  - <span data-ttu-id="83d15-145">Транзакция санаты бағасы</span><span class="sxs-lookup"><span data-stu-id="83d15-145">Transaction Category Price</span></span>
  - <span data-ttu-id="83d15-146">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="83d15-146">Characteristic</span></span>
  - <span data-ttu-id="83d15-147">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="83d15-147">Bookable Resource</span></span>
  - <span data-ttu-id="83d15-148">Тапсырыс беруге болатын ресурс санатының байланысы</span><span class="sxs-lookup"><span data-stu-id="83d15-148">Bookable resource category Assn</span></span>
  - <span data-ttu-id="83d15-149">Тапсырыс беруге болатын ресурс сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="83d15-149">Bookable Resource Characteristic</span></span>

![Импорттауды аяқтау](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="83d15-151">Project Operations конфигурацияларын жаңарту</span><span class="sxs-lookup"><span data-stu-id="83d15-151">Update Project Operations configurations</span></span>

1. <span data-ttu-id="83d15-152">CE ортасына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="83d15-152">Navigate to the CE environment.</span></span> <span data-ttu-id="83d15-153">Оны [Power Platform басқару орталығын](https://admin.powerplatform.microsoft.com/environments) ашып, ортаны таңдап, содан кейін **Ортаны ашу** опциясын таңдау арқылы табуға болады.</span><span class="sxs-lookup"><span data-stu-id="83d15-153">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Ортаны ашу](./media/7OpenEnvironment.png)

2. <span data-ttu-id="83d15-155">Пайдаланушыға арналған тапсырыс беруге болатын ресурсты жасау үшін **Жобалар** > **Ресурс**, содан кейін **Жаңа** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="83d15-155">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Тапсырыс беруге болатын ресурстар](./media/8BookableResources.png)

3. <span data-ttu-id="83d15-157">**Жалпы мәліметтер** қойыншасында әкімші пайдаланушыны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-157">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="83d15-158">Уақыт белдеуі сіз тұрған аймаққа сәйкес келетіндігін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="83d15-158">Verify that the time zone matches the one you are in.</span></span> 

![Жаңа тапсырыс беруге болатын ресурс](./media/9NewBookableResource.png)

4. <span data-ttu-id="83d15-160">**Жоспарлау** қойыншасындағы **Компания** өрісінде **USPM** компаниясын таңдап, содан соң **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-160">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Жоспарлау қойыншасы](./media/10SchedulingTab.png)

5. <span data-ttu-id="83d15-162">**Жұмыс сағаттары** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-162">Select the **Work hours** tab.</span></span>  

![Жұмыс сағаттары](./media/11WorkHours.png)

6. <span data-ttu-id="83d15-164">Күнтізбедегі кез келген мәнді екі рет шертіп, **Өңдеу** > **Сериядағы барлық оқиғалар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-164">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Іскери күнтізбе](./media/12WorkCalendar.png)

7. <span data-ttu-id="83d15-166">Жұмыс уақытын сегіз (8) сағаттық жұмыс күніне ауыстырыңыз, демалыс күндерін жұмыс емес күн ретінде белгілеңіз және уақыт белдеуі сіздікімен сәйкес келетініне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="83d15-166">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="83d15-167">**Сақтау және жабу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-167">Select **Save and close**.</span></span>

![Күнтізбені жаңарту](./media/13UpdateCalendar.png)

9. <span data-ttu-id="83d15-169">**Параметрлер** > **Күнтізбелік үлгілер** тармағына өтіп, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-169">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Күнтізбе үлгілері](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="83d15-171">Атын енгізіп, жасаған үлгі ресурсын таңдап, содан кейін **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-171">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Күнтізбе үлгісін сақтау](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="83d15-173">**Параметрлер** тармағына өтіп, жазбаны екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-173">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Жоба параметрлері](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="83d15-175">Келесі өрістерді жаңартыңыз:</span><span class="sxs-lookup"><span data-stu-id="83d15-175">Update the following fields:</span></span>

 - <span data-ttu-id="83d15-176">**Әдепкі компания**: USPM</span><span class="sxs-lookup"><span data-stu-id="83d15-176">**Default company**: USPM</span></span>
 - <span data-ttu-id="83d15-177">**Әдепкі ұйымдық бөлім**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="83d15-177">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="83d15-178">**Шот-фактураның жиілігі**: Жетінші және соңғы күн</span><span class="sxs-lookup"><span data-stu-id="83d15-178">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="83d15-179">**Жұмыс уақытының үлгісі**: Сіз жасаған үлгі өзгерісі.</span><span class="sxs-lookup"><span data-stu-id="83d15-179">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="83d15-180">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="83d15-180">Select **Save**.</span></span> 

![Жаңартылған жоба параметрлері](./media/17UpdatedProjectParameters.png)
