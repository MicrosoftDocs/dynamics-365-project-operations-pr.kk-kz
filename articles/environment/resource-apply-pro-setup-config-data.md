---
title: Common Data Service қызметінде конфигурация деректерін орнатып, қолдану
description: Бұл тақырып Project Operations жүйесінде конфигурация деректерін қолдану туралы ақпарат береді.
author: sigitac
ms.date: 05/10/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2ea00df6112fb69b61f1889463424fdfee79aec9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001298"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="3956e-103">Common Data Service қызметінде конфигурация деректерін орнатып, қолдану</span><span class="sxs-lookup"><span data-stu-id="3956e-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="3956e-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="3956e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="3956e-105">Алғышарттар</span><span class="sxs-lookup"><span data-stu-id="3956e-105">Prerequisites</span></span>

<span data-ttu-id="3956e-106">Common Data Service (CDS) бағдарламасында деректерді конфигурациялауды бастамас бұрын, келесі алғышарттар орындалуы керек:</span><span class="sxs-lookup"><span data-stu-id="3956e-106">Before you begin to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="3956e-107">Project Operations бағдарламасы үшін CDS ортасымен және Dynamics 365 Finance ортасымен қамтамасыз ету.</span><span class="sxs-lookup"><span data-stu-id="3956e-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="3956e-108">Dynamics 365 Finance жүйесінен алынған заңды тұлға туралы ақпарат CDS ортасымен ортақ пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="3956e-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="3956e-109">Бұл CDS қызметіндегі **Компания** нысанында келесі компаниялық жазбалардың бар екендігін білдіреді:</span><span class="sxs-lookup"><span data-stu-id="3956e-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="3956e-110">THPM</span><span class="sxs-lookup"><span data-stu-id="3956e-110">THPM</span></span>
  - <span data-ttu-id="3956e-111">USPM</span><span class="sxs-lookup"><span data-stu-id="3956e-111">USPM</span></span>
  - <span data-ttu-id="3956e-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="3956e-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="3956e-113">Орнату және конфигурация деректерін орнату</span><span class="sxs-lookup"><span data-stu-id="3956e-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="3956e-114">[Орнату және конфигурация деректер бумасын](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip) жүктеңіз, құлыптан шығарыңыз және мұрағаттан шығарыңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span></span>
2. <span data-ttu-id="3956e-115">Мұрағаттан шығарылмаған қалтаға өтіп, *DataMigrationUtility* орындалатын файлды іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="3956e-116">Common Data Service конфигурацияны тасымалдау (CMT) шеберінің 1-бетінде **Деректерді импорттау**, содан кейін **Жалғастыру** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Конфигурацияны тасымалдау](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="3956e-118">CMT шеберінің 2-бетінде **Орналастыру түрі** ретінде **Microsoft 365** қызметін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="3956e-119">**Қолжетімді ұйымдар тізімін көрсету** және **Кеңейтілген түрде көрсету** өрістеріне құсбелгі қойыңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="3956e-120">Қатысушы аймағын таңдап, тіркелу деректеріңізді енгізіп, **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Конфигурацияға кіру](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="3956e-122">3-бетте, қатысушыдағы ұйымдар тізімінен демо деректерді импорттау ұйымын таңдап, содан соң **Жүйеге кіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="3956e-123">4-бетте бумадан шығарылған қалтадан *SampleSetupAndConfigData* zip файлын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Zip файлын таңдау](./media/3ZipFile.png)

![Файлды таңдаңыз](./media/4SelectAFile.png)

9. <span data-ttu-id="3956e-126">Zip файлы таңдалғаннан кейін **Деректерді импорттау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-126">After the zip file is selected, select **Import Data**.</span></span>

![Деректерді импорттау](./media/5ImportData.png)

10. <span data-ttu-id="3956e-128">Импорттау желі жылдамдығына байланысты шамамен екі-он минутқа созылады.</span><span class="sxs-lookup"><span data-stu-id="3956e-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="3956e-129">Импорттау аяқталғаннан кейін CMT шеберінен шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="3956e-130">Ұйымыңыздан келесі 26 ұйымның деректерін тексеріңіз:</span><span class="sxs-lookup"><span data-stu-id="3956e-130">Check your organization for data in the following 26 entities:</span></span>

  - <span data-ttu-id="3956e-131">Валюта</span><span class="sxs-lookup"><span data-stu-id="3956e-131">Currency</span></span>
  - <span data-ttu-id="3956e-132">Тіркелгілер диаграммасы</span><span class="sxs-lookup"><span data-stu-id="3956e-132">Chart of Accounts</span></span>
  - <span data-ttu-id="3956e-133">Қаржылық күнтізбе</span><span class="sxs-lookup"><span data-stu-id="3956e-133">Fiscal Calendar</span></span>
  - <span data-ttu-id="3956e-134">Валюта айырбастау бағамының түрлері</span><span class="sxs-lookup"><span data-stu-id="3956e-134">Currency Exchange Rate Types</span></span>
  - <span data-ttu-id="3956e-135">Төлем күні</span><span class="sxs-lookup"><span data-stu-id="3956e-135">Payment Day</span></span>
  - <span data-ttu-id="3956e-136">Төлем кестесі</span><span class="sxs-lookup"><span data-stu-id="3956e-136">Payment Schedule</span></span>
  - <span data-ttu-id="3956e-137">Төлем шарты</span><span class="sxs-lookup"><span data-stu-id="3956e-137">Payment Term</span></span>
  - <span data-ttu-id="3956e-138">Ұйымдық бірлік</span><span class="sxs-lookup"><span data-stu-id="3956e-138">Organizational Unit</span></span>
  - <span data-ttu-id="3956e-139">КОНТАКТ </span><span class="sxs-lookup"><span data-stu-id="3956e-139">Contact</span></span>
  - <span data-ttu-id="3956e-140">Салық тобы</span><span class="sxs-lookup"><span data-stu-id="3956e-140">Tax Group</span></span>
  - <span data-ttu-id="3956e-141">Тұтынушы тобы</span><span class="sxs-lookup"><span data-stu-id="3956e-141">Customer Group</span></span>
  - <span data-ttu-id="3956e-142">Жеткізуші тобы</span><span class="sxs-lookup"><span data-stu-id="3956e-142">Vendor Group</span></span>
  - <span data-ttu-id="3956e-143">Бірлік</span><span class="sxs-lookup"><span data-stu-id="3956e-143">Unit</span></span>
  - <span data-ttu-id="3956e-144">Бірлік тобы</span><span class="sxs-lookup"><span data-stu-id="3956e-144">Unit Group</span></span>
  - <span data-ttu-id="3956e-145">Бағатізбе</span><span class="sxs-lookup"><span data-stu-id="3956e-145">Price List</span></span>
  - <span data-ttu-id="3956e-146">Жоба параметрі бағатізбесі</span><span class="sxs-lookup"><span data-stu-id="3956e-146">Project Parameter Price List</span></span>
  - <span data-ttu-id="3956e-147">Есеп-шот жиілігі</span><span class="sxs-lookup"><span data-stu-id="3956e-147">Invoice Frequency</span></span>
  - <span data-ttu-id="3956e-148">Тапсырыс беруге болатын ресурс санаты</span><span class="sxs-lookup"><span data-stu-id="3956e-148">Bookable Resource Category</span></span>
  - <span data-ttu-id="3956e-149">Транзакция санаты</span><span class="sxs-lookup"><span data-stu-id="3956e-149">Transaction Category</span></span>
  - <span data-ttu-id="3956e-150">Шығыс санаты</span><span class="sxs-lookup"><span data-stu-id="3956e-150">Expense Category</span></span>
  - <span data-ttu-id="3956e-151">Рөл бағасы</span><span class="sxs-lookup"><span data-stu-id="3956e-151">Role Price</span></span>
  - <span data-ttu-id="3956e-152">Транзакция санаты бағасы</span><span class="sxs-lookup"><span data-stu-id="3956e-152">Transaction Category Price</span></span>
  - <span data-ttu-id="3956e-153">Сипаттама</span><span class="sxs-lookup"><span data-stu-id="3956e-153">Characteristic</span></span>
  - <span data-ttu-id="3956e-154">Резервтелетін ресурс</span><span class="sxs-lookup"><span data-stu-id="3956e-154">Bookable Resource</span></span>
  - <span data-ttu-id="3956e-155">Тапсырыс беруге болатын ресурс санатының байланысы</span><span class="sxs-lookup"><span data-stu-id="3956e-155">Bookable resource category Assn</span></span>
  - <span data-ttu-id="3956e-156">Тапсырыс беруге болатын ресурс сипаттамасы</span><span class="sxs-lookup"><span data-stu-id="3956e-156">Bookable Resource Characteristic</span></span>

![Импорттауды аяқтау](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="3956e-158">Project Operations конфигурацияларын жаңарту</span><span class="sxs-lookup"><span data-stu-id="3956e-158">Update Project Operations configurations</span></span>

1. <span data-ttu-id="3956e-159">CE ортасына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="3956e-159">Navigate to the CE environment.</span></span> <span data-ttu-id="3956e-160">Оны [Power Platform басқару орталығын](https://admin.powerplatform.microsoft.com/environments) ашып, ортаны таңдап, содан кейін **Ортаны ашу** опциясын таңдау арқылы табуға болады.</span><span class="sxs-lookup"><span data-stu-id="3956e-160">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Ортаны ашу](./media/7OpenEnvironment.png)

2. <span data-ttu-id="3956e-162">Пайдаланушыға арналған тапсырыс беруге болатын ресурсты жасау үшін **Жобалар** > **Ресурс**, содан кейін **Жаңа** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="3956e-162">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Тапсырыс беруге болатын ресурстар](./media/8BookableResources.png)

3. <span data-ttu-id="3956e-164">**Жалпы мәліметтер** қойыншасында әкімші пайдаланушыны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-164">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="3956e-165">Уақыт белдеуі сіз тұрған аймаққа сәйкес келетіндігін тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="3956e-165">Verify that the time zone matches the one you are in.</span></span> 

![Жаңа тапсырыс беруге болатын ресурс](./media/9NewBookableResource.png)

4. <span data-ttu-id="3956e-167">**Жоспарлау** қойыншасындағы **Компания** өрісінде **USPM** компаниясын таңдап, содан соң **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-167">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Жоспарлау қойыншасы](./media/10SchedulingTab.png)

5. <span data-ttu-id="3956e-169">**Жұмыс сағаттары** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-169">Select the **Work hours** tab.</span></span>  

![Жұмыс сағаттары](./media/11WorkHours.png)

6. <span data-ttu-id="3956e-171">Күнтізбедегі кез келген мәнді екі рет шертіп, **Өңдеу** > **Сериядағы барлық оқиғалар** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-171">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Іскери күнтізбе](./media/12WorkCalendar.png)

7. <span data-ttu-id="3956e-173">Жұмыс уақытын сегіз (8) сағаттық жұмыс күніне ауыстырыңыз, демалыс күндерін жұмыс емес күн ретінде белгілеңіз және уақыт белдеуі сіздікімен сәйкес келетініне көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="3956e-173">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="3956e-174">**Сақтау және жабу** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-174">Select **Save and close**.</span></span>

![Күнтізбені жаңарту](./media/13UpdateCalendar.png)

9. <span data-ttu-id="3956e-176">**Параметрлер** > **Күнтізбелік үлгілер** тармағына өтіп, **Жаңа** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-176">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Күнтізбе үлгілері](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="3956e-178">Атын енгізіп, жасаған үлгі ресурсын таңдап, содан кейін **Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-178">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Күнтізбе үлгісін сақтау](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="3956e-180">**Параметрлер** тармағына өтіп, жазбаны екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-180">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Жоба параметрлері](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="3956e-182">Келесі өрістерді жаңартыңыз:</span><span class="sxs-lookup"><span data-stu-id="3956e-182">Update the following fields:</span></span>

 - <span data-ttu-id="3956e-183">**Әдепкі компания**: USPM</span><span class="sxs-lookup"><span data-stu-id="3956e-183">**Default company**: USPM</span></span>
 - <span data-ttu-id="3956e-184">**Әдепкі бөлімше**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="3956e-184">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="3956e-185">**Шот-фактураның жиілігі**: Жетінші және соңғы күн</span><span class="sxs-lookup"><span data-stu-id="3956e-185">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="3956e-186">**Жұмыс уақытының үлгісі**: Сіз жасаған үлгі өзгерісі.</span><span class="sxs-lookup"><span data-stu-id="3956e-186">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="3956e-187">**Сақтау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3956e-187">Select **Save**.</span></span> 

![Жаңартылған жоба параметрлері](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
