---
title: Тапсырмалар торында жұмыс істеу кезінде ақаулықтарды жою
description: Бұл тақырып тапсырмалар торында жұмыс істеу кезінде ақаулықтарды жою туралы қажетті ақпаратты ұсынады.
author: ruhercul
ms.date: 01/19/2021
ms.topic: article
ms.product: ''
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: a15a4752de7537b3f60d5ee3269c846257a1fe4a
ms.sourcegitcommit: 72fa1f09fe406805f7009fc68e2f3eeeb9b7d5fc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 06/09/2021
ms.locfileid: "6213407"
---
# <a name="troubleshoot-working-in-the-task-grid"></a><span data-ttu-id="9b977-103">Тапсырмалар торында жұмыс істеу кезінде ақаулықтарды жою</span><span class="sxs-lookup"><span data-stu-id="9b977-103">Troubleshoot working in the Task grid</span></span> 

<span data-ttu-id="9b977-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="9b977-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9b977-105">Бұл бөлімде шығындарды басқарумен жұмыс жасау кезінде туындауы мүмкін мәселелерді қалай түзетуге болатындығы сипатталған.</span><span class="sxs-lookup"><span data-stu-id="9b977-105">This topic describes how to fix issues that you might encounter while working with cost management.</span></span>

## <a name="enable-cookies"></a><span data-ttu-id="9b977-106">"Cookies" файлдарын қосу</span><span class="sxs-lookup"><span data-stu-id="9b977-106">Enable cookies</span></span>

<span data-ttu-id="9b977-107">Project Operations бағдарламасы жұмыс декомпозициясының құрылымын көрсету үшін үшінші тарап cookies файлдарының қосылуын қажет етеді.</span><span class="sxs-lookup"><span data-stu-id="9b977-107">Project Operations requires that third-party cookies be enabled in order to render the work breakdown structure.</span></span> <span data-ttu-id="9b977-108">Үшінші тарап cookies файлдары қосылмаған кезде, тапсырмаларды көрудің орнына, **Жоба** бетіндегі **Тапсырмалар** қойыншасын таңдағанда, бос бетті көресіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-108">When third-party cookies aren't enabled, instead of seeing tasks, you will see a blank page when you select the **Tasks** tab on the **Project** page.</span></span>

![Үшінші тарап cookies файлдары қосылмаған кездегі бос қойынша](media/blankschedule.png)


### <a name="workaround"></a><span data-ttu-id="9b977-110">Жұмыс шешімі</span><span class="sxs-lookup"><span data-stu-id="9b977-110">Workaround</span></span>
<span data-ttu-id="9b977-111">Microsoft Edge немесе Google Chrome шолғыштарында келесі процедуралар үшінші тарап cookies файлдарын қосу үшін шолғыш параметрін жаңарту жолдарын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="9b977-111">For Microsoft Edge or Google Chrome browsers, the following procedures outline how to update your browser setting to enable third-party cookies.</span></span>

#### <a name="microsoft-edge"></a><span data-ttu-id="9b977-112">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9b977-112">Microsoft Edge</span></span>

1. <span data-ttu-id="9b977-113">Edge шолғышын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-113">Open your Edge browser.</span></span>
2. <span data-ttu-id="9b977-114">Үстіңгі оң жақ бұрыштан **көп нүкте** (…) белгішесін таңдап, **Параметрлер** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-114">In the upper-right corner, select the **ellipsis** (...), and then select **Settings**.</span></span>
3. <span data-ttu-id="9b977-115">**Cookie файлдары және сайт рұқсаттары** бөлімінде **Cookie файлдары және сайт туралы деректер** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-115">Under **Cookies and site permissions**, select **Cookies and site data**.</span></span>
4. <span data-ttu-id="9b977-116">**Үшінші тарап cookie файлдарын бұғаттау** функциясын өшіріңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-116">Turn off **Block third-party cookies**.</span></span>

#### <a name="google-chrome"></a><span data-ttu-id="9b977-117">Google Chrome</span><span class="sxs-lookup"><span data-stu-id="9b977-117">Google Chrome</span></span>

1. <span data-ttu-id="9b977-118">Chrome шолғышын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-118">Open your Chrome browser.</span></span>
2. <span data-ttu-id="9b977-119">Үстіңгі оң жақ бұрыштан үш тік нүктені таңдап, содан кейін **Параметрлер** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-119">In the upper-right corner, select the three vertical dots, and then select **Settings**.</span></span>
3. <span data-ttu-id="9b977-120">**Құпиялылық және қауіпсіздік** бөлімінде **Cookie файлдары және басқа сайт туралы деректер** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-120">Under **Privacy and security**, select **Cookies and other site data**.</span></span>
4. <span data-ttu-id="9b977-121">**Барлық cookie файлдарына рұқсат беру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-121">Select **Allow all cookies**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9b977-122">Егер үшінші тарапты cookie файлдарын бұғаттасаңыз, тіпті, ерекшеліктер тізімінде сайтқа рұқсат берілсе де басқа сайттардағы барлық cookie деректері мен сайт деректері бұғатталады.</span><span class="sxs-lookup"><span data-stu-id="9b977-122">If you block third-party cookies, all cookies and site data from other sites will be blocked, even if the site is allowed on your exceptions list.</span></span>

## <a name="pex-endpoint"></a><span data-ttu-id="9b977-123">PEX соңғы нүктесі</span><span class="sxs-lookup"><span data-stu-id="9b977-123">PEX Endpoint</span></span>

<span data-ttu-id="9b977-124">Project Operations бағдарламасы жоба параметрінің PEX соңғы нүктесіне сілтемесін талап етеді.</span><span class="sxs-lookup"><span data-stu-id="9b977-124">Project Operations requires that a project parameter reference the PEX Endpoint.</span></span> <span data-ttu-id="9b977-125">Бұл соңғы нүкте жұмыс декомпозициясының құрылымын көрсету үшін пайдаланылатын қызметпен байланыс орнату үшін қажет.</span><span class="sxs-lookup"><span data-stu-id="9b977-125">This endpoint is required to communicate with the service used to render the work breakdown structure.</span></span> <span data-ttu-id="9b977-126">Егер параметр қосылмаған болса, сізге "Жоба параметрі жарамды емес" деген қате жіберіледі.</span><span class="sxs-lookup"><span data-stu-id="9b977-126">If the parameter isn't enabled, you will receive the error, "The project parameter is not valid".</span></span> 

### <a name="workaround"></a><span data-ttu-id="9b977-127">Жұмыс шешімі</span><span class="sxs-lookup"><span data-stu-id="9b977-127">Workaround</span></span>
 ![Жоба параметріндегі PEX соңғы нүктесінің өрісі](media/projectparameter.png)

1. <span data-ttu-id="9b977-129">**Жоба параметрлері** бетіне **PEX соңғы нүктесі** өрісін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-129">Add the **PEX Endpoint** field to the **Project Parameters** page.</span></span>
2. <span data-ttu-id="9b977-130">Өрісті келесі мәнмен жаңартыңыз: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=/<id>&type=2`</span><span class="sxs-lookup"><span data-stu-id="9b977-130">Update the field with the following value: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=/<id>&type=2`</span></span>
3. <span data-ttu-id="9b977-131">**Жоба параметрлері** бетінен өрісті жойыңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-131">Remove the field from the **Project Parameters** page.</span></span>

## <a name="privileges-for-project-for-the-web"></a><span data-ttu-id="9b977-132">Вебке арналған жобаның артықшылықтары</span><span class="sxs-lookup"><span data-stu-id="9b977-132">Privileges for Project for the Web</span></span>

<span data-ttu-id="9b977-133">Project Operations бағдарламасы сыртқы жоспарлау қызметіне негізделген.</span><span class="sxs-lookup"><span data-stu-id="9b977-133">Project Operations relies on an external scheduling service.</span></span> <span data-ttu-id="9b977-134">Қызмет пайдаланушыдан жұмыс декомпозициясының құрылымымен байланысты нысандарды оқу және жазу үшін тағайындалған бірнеше рөлдерді талап етеді.</span><span class="sxs-lookup"><span data-stu-id="9b977-134">The service requires that a user have several roles assigned to read and write to entities related to the work breakdown structure.</span></span> <span data-ttu-id="9b977-135">Бұл нысандар жобалық тапсырмаларды, ресурстарды тағайындауды және тапсырма тәуелділіктерін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="9b977-135">These entities include project tasks, resource assignments, and task dependencies.</span></span> <span data-ttu-id="9b977-136">Егер пайдаланушы **Тапсырмалар** қойыншасына өткенде жұмыс декомпозициясының құрылымын көрсете алмаса, ол Project Operations жобасының қосылмауынан болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="9b977-136">If a user can't render the work breakdown structure when they go to the **Tasks** tab, it's probably because Project for Project Operations hasn't been enabled.</span></span> <span data-ttu-id="9b977-137">Пайдаланушыға қауіпсіздік рөлі қатесі немесе кіруден бас тартуға байланысты қате жіберілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="9b977-137">A user might receive either a security role error, or an error related to a denial of access.</span></span>


## <a name="workaround"></a><span data-ttu-id="9b977-138">Жұмыс шешімі</span><span class="sxs-lookup"><span data-stu-id="9b977-138">Workaround</span></span>

1. <span data-ttu-id="9b977-139">**Параметр > Қауіпсіздік > Пайдаланушылар > Бағдарлама пайдаланушылары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-139">Go to **Setting > Security > Users > Application Users**.</span></span>  

   ![Бағдарламаны оқу құралы](media/applicationuser.jpg)
   
2. <span data-ttu-id="9b977-141">Төмендегілерді тексеру үшін бағдарлама пайдаланушысы жазбасын екі рет басыңыз:</span><span class="sxs-lookup"><span data-stu-id="9b977-141">Double-click the application user record to verify the following:</span></span>

 - <span data-ttu-id="9b977-142">Пайдаланушы жобаға қол жеткізе алады.</span><span class="sxs-lookup"><span data-stu-id="9b977-142">The user has access to the project.</span></span> <span data-ttu-id="9b977-143">Әдетте бұл тексеру пайдаланушыда **Жоба менеджері** қауіпсіздік рөлінің бар екенін тексеру үшін жасалады.</span><span class="sxs-lookup"><span data-stu-id="9b977-143">This verification is typically done by ensuring that the user has **Project Manager** security role.</span></span>
 - <span data-ttu-id="9b977-144">Microsoft Project бағдарламасы пайдаланушысы бар және дұрыс конфигурацияланған.</span><span class="sxs-lookup"><span data-stu-id="9b977-144">The Microsoft Project application user exists and is configured correctly.</span></span>
 
3. <span data-ttu-id="9b977-145">Егер бұл пайдаланушы болмаса, жаңа пайдаланушы жазбасын жасай аласыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-145">If this user doesn't exist, you can create a new user record.</span></span> <span data-ttu-id="9b977-146">**Жаңа пайдаланушылар** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-146">Select **New Users**.</span></span> <span data-ttu-id="9b977-147">Нысан пішінін **Бағдарлама пайдаланушысы** күйіне өзгертіп, содан кейін **Бағдарлама идентификаторы** опциясын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="9b977-147">Change the entry form to **Application User**, and then add the **Application ID**.</span></span>

   ![Бағдарлама пайдаланушысы туралы мәліметтер](media/applicationuserdetails.jpg)

4. <span data-ttu-id="9b977-149">Пайдаланушыға дұрыс лицензия берілгенін және қызметтің лицензия туралы егжей-тегжейлі жоспарлау қызметінде қосылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-149">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
5. <span data-ttu-id="9b977-150">Пайдаланушының project.microsoft.com сайтын аша алатынын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-150">Verify that the user can open project.microsoft.com.</span></span>
6. <span data-ttu-id="9b977-151">Жоба параметрлері арқылы жүйенің жобаның соңғы нүктесін көрсетіп тұрғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-151">Verify through the project parameters that the system is pointing to the correct project endpoint.</span></span>
7. <span data-ttu-id="9b977-152">Жоба бағдарламасының пайдаланушысы құрылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-152">Verify that the project application user is created.</span></span>
8. <span data-ttu-id="9b977-153">Пайдаланушыға келесі қауіпсіздік рөлдерін қолданыңыз:</span><span class="sxs-lookup"><span data-stu-id="9b977-153">Apply the following security roles to the user:</span></span>

  - <span data-ttu-id="9b977-154">Dataverse пайдаланушысы</span><span class="sxs-lookup"><span data-stu-id="9b977-154">Dataverse User</span></span>
  - <span data-ttu-id="9b977-155">Project Operations жүйесі</span><span class="sxs-lookup"><span data-stu-id="9b977-155">Project Operations System</span></span>
  - <span data-ttu-id="9b977-156">Жоба жүйесі</span><span class="sxs-lookup"><span data-stu-id="9b977-156">Project System</span></span>

## <a name="error-when-updating-the-work-breakdown-structure"></a><span data-ttu-id="9b977-157">Жұмыс декомпозициясының құрылымын жаңарту кезінде қате пайда болды</span><span class="sxs-lookup"><span data-stu-id="9b977-157">Error when updating the work breakdown structure</span></span>

<span data-ttu-id="9b977-158">Жұмыс декомпозициясының құрылымына бір немесе бірнеше жаңарту жасалғанда, өзгерістер соңында сәтсіздікке ұшырайды және сақталмайды.</span><span class="sxs-lookup"><span data-stu-id="9b977-158">When one or more updates are made to the work breakdown structure, the changes eventually fail and aren't saved.</span></span> <span data-ttu-id="9b977-159">Кесте торында "Сіз жасаған соңғы өзгеріс сақталмады" деген қате пайда болды.</span><span class="sxs-lookup"><span data-stu-id="9b977-159">An error occurs in the schedule grid noting that “Recent change you’ve made couldn’t be saved.”</span></span>

### <a name="workaround"></a><span data-ttu-id="9b977-160">Жұмыс шешімі</span><span class="sxs-lookup"><span data-stu-id="9b977-160">Workaround</span></span>

1. <span data-ttu-id="9b977-161">Пайдаланушыға дұрыс лицензия берілгенін және қызметтің лицензия туралы егжей-тегжейлі жоспарлау қызметінде қосылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-161">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
2. <span data-ttu-id="9b977-162">Пайдаланушының project.microsoft.com сайтын аша алатынын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-162">Verify that the user can open project.microsoft.com.</span></span>
3. <span data-ttu-id="9b977-163">Жүйенің жобаның соңғы нүктесін көрсетіп тұрғанын тексеріңіз,.</span><span class="sxs-lookup"><span data-stu-id="9b977-163">Verify that the system is pointing to the correct project endpoint,.</span></span>
4. <span data-ttu-id="9b977-164">Жоба бағдарламасының пайдаланушысы құрылғанын тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="9b977-164">Verify that the Project Application user has been created.</span></span>
5. <span data-ttu-id="9b977-165">Пайдаланушыға келесі қауіпсіздік рөлдерін қолданыңыз:</span><span class="sxs-lookup"><span data-stu-id="9b977-165">Apply the following security roles to the user:</span></span>
  
  - <span data-ttu-id="9b977-166">Dataverse пайдаланушысы немесе негізгі пайдаланушы</span><span class="sxs-lookup"><span data-stu-id="9b977-166">Dataverse user or Base user</span></span>
  - <span data-ttu-id="9b977-167">Project Operations жүйесі</span><span class="sxs-lookup"><span data-stu-id="9b977-167">Project Operations System</span></span>
  - <span data-ttu-id="9b977-168">Жоба жүйесі</span><span class="sxs-lookup"><span data-stu-id="9b977-168">Project System</span></span>
  - <span data-ttu-id="9b977-169">Project Operations қос жазу жүйесі (бұл рөл, егер сіз Project Operations жүйесінің ресурс/биржадан тыс негіздегі сценарийлерін қолданатын болсаңыз қажет.)</span><span class="sxs-lookup"><span data-stu-id="9b977-169">Project Operations Dual Write System (This role is required if you are deploying the resource/non-stocked based scenario of Project Operations.)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
