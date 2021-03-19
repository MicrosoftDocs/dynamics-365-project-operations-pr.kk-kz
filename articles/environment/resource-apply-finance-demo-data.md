---
title: Демо деректерді Finance бұлт қызметтеріне орналастырылған ортаға қолдану
description: Бұл тақырып Project Operations демо деректерін Dynamics 365 Finance бұлт қызметтеріне орналастырылған ортаға қалай қолдануға болатындығын түсіндіреді.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a7239301dc8b775dc4a53a1cf6c0bcba3956125a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289871"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a><span data-ttu-id="cfed6-103">Демо деректерді Finance бұлт қызметтеріне орналастырылған ортаға қолдану</span><span class="sxs-lookup"><span data-stu-id="cfed6-103">Apply demo data to a Finance Cloud-hosted environment</span></span>

<span data-ttu-id="cfed6-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="cfed6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cfed6-105">Бұл тақырып тек Microsoft Dynamics 365 Finance 10.0.13 нұсқасына ғана қатысты және тек бұлт қызметтеріне орналастырылған ортада орындалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="cfed6-105">This topic is only applicable only Microsoft Dynamics 365 Finance version 10.0.13 and can be performed only on a Cloud-hosted environment.</span></span> <span data-ttu-id="cfed6-106">Ортағаның сапа жаңартуларын қолданар **АЛДЫНДА** осы тақырыптағы қадамдарды аяқтаңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-106">Complete the steps in this topic **BEFORE** you apply quality updates to the environment.</span></span>

1. <span data-ttu-id="cfed6-107">LCS жобасында **Орта туралы мәліметтер** бетін ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-107">In your LCS project, open the **Environment details** page.</span></span> <span data-ttu-id="cfed6-108">Оның Remote Desktop Protocol (RDP) бағдарламалық жасақтамасы арқылы ортаға қосылуға қажетті мәліметтерді қамтитынына назар аударыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-108">Notice that it includes the details needed to connect to the environment by using Remote Desktop Protocol (RDP).</span></span>

![ ортасының мәліметтері](./media/1EnvironmentDetails.png)

<span data-ttu-id="cfed6-110">Ерекшеленген тіркелгі деректерінің бірінші жиынтығы жергілікті тіркелгі деректері болып табылады және жұмыс үстелінің қашықтан қосылуына сілтеме жасайды.</span><span class="sxs-lookup"><span data-stu-id="cfed6-110">The first set of highlighted credentials are the local account credentials and contain a hyperlink to the remote desktop connection.</span></span> <span data-ttu-id="cfed6-111">Тіркелгі деректері орта әкімшісінің пайдаланушы аты мен құпиясөзін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="cfed6-111">The credentials include the environment admin username and password.</span></span> <span data-ttu-id="cfed6-112">Тіркелгі деректерінің екінші жиынтығы осы ортада SQL Server басқару жүйесіне кіру үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="cfed6-112">The second set of credentials are used to log in to SQL Server in this environment.</span></span>

2. <span data-ttu-id="cfed6-113">**Жергілікті тіркелгілер** ішіндегі сілтеме арқылы ортаға қашықтан қосылыңыз және **Жергілікті тіркелгінің деректері** арқылы аутентификациялаңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-113">Remote to the environment by the hyperlink in **Local Accounts**, and use the **Local Account credentials** to authenticate.</span></span>
3. <span data-ttu-id="cfed6-114">**Интернет ақпараттық қызметтері** > **Бағдарлама қорлары** > **AOSService** тармағына өтіп, қызметті тоқтатыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-114">Go to **Internet Information Services** > **Application Pools** > **AOSService** and stop the service.</span></span> <span data-ttu-id="cfed6-115">SQL дерекқорын ауыстыруды жалғастыру үшін сіз осы уақытта қызметті тоқтатасыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-115">You are stopping the service at this point so that you can continue to replace the SQL database.</span></span>

![AOS қызметін тоқтату](./media/2StopAOS.png)

4. <span data-ttu-id="cfed6-117">**Қызметтер** бөліміне өтіп, келесі екі элементті тоқтатыңыз:</span><span class="sxs-lookup"><span data-stu-id="cfed6-117">Go to **Services** and stop the following two items:</span></span>

- <span data-ttu-id="cfed6-118">Microsoft Dynamics 365 Unified Operations Batch Management Service қызметі</span><span class="sxs-lookup"><span data-stu-id="cfed6-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span></span>
- <span data-ttu-id="cfed6-119">Microsoft Dynamics 365 Unified Operations: деректерді импорттау экспорттау құрылымы</span><span class="sxs-lookup"><span data-stu-id="cfed6-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span></span>

![Қызметтерді тоқтату](./media/3StopServices.png)

5. <span data-ttu-id="cfed6-121">Microsoft SQL Server Management Studio ортасын ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-121">Open Microsoft SQL Server Management Studio.</span></span> <span data-ttu-id="cfed6-122">SQL серверінің тіркелгі деректерімен кіріп, LCS **Орталардың мәліметтері** бетінен axdbadmin пайдаланушысы мен құпиясөзін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-122">Log in with SQL server credentials and use the axdbadmin user and password from the LCS **Environments details** page.</span></span>

![SQL Server Management Studio](./media/4SSMS.png)

6. <span data-ttu-id="cfed6-124">**Дерекқорлар** мен Object Explorer объектілерді шолушысында **AXDB** орналасқан жерін анықтаңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-124">In Object Explorer, **Databases** and locate **AXDB**.</span></span> <span data-ttu-id="cfed6-125">[Жүктеу орталығы](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip) орналасқан дерекқорды жаңа дерекқормен алмастырасыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-125">You will replace database with a new database that is located in the [Download Center](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span></span> 
7. <span data-ttu-id="cfed6-126">Сіз zip файлын қашықтан басқарылатын VM жүйесіне көшіріңіз және оның zip мазмұнын шығарып алыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-126">Copy the zip file to the VM you are remoted into and extract zip contents.</span></span>
8. <span data-ttu-id="cfed6-127">SQL Server Management Studio утилитасында **AxDB** пәрменінде тінтуірдің оң жағын басыңыз, содан кейін **Тапсырмалар** > **Қалпына келтіру** > **Дерекқор** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-127">In SQL Server Management Studio, right-click **AxDB**, and then select **Tasks** > **Restore** > **Database**.</span></span>

![Дерекқорды қалпына келтіру](./media/5RestoreDatabase.png)

9. <span data-ttu-id="cfed6-129">**Бастапқы құрылғы** опциясын таңдап, көшірген zip файлынан алынған файлға өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-129">Select **Source Device** and navigate to the file extracted from zip you copied.</span></span>

![Бастапқы құрылғылар](./media/6SourceDevice.png)

10. <span data-ttu-id="cfed6-131">**Опциялар**, содан кейін **Қолданыстағы дерекқорды қайта жазу** мен **Мақсатты дерекқорға қолданыстағы байланыстарды жабу** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-131">Select **Options**, and then select **Overwrite the existing database** and **Close existing connections to destination database**.</span></span> 
11. <span data-ttu-id="cfed6-132">**OK** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-132">Select **OK**.</span></span>

![Параметрлерді қалпына келтіру](./media/7RestoreSetting.png)

<span data-ttu-id="cfed6-134">Сіз AXDB қалпына келтірудің сәтті өткендігі туралы растау аласыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-134">You will receive confirmation that the AXDB restore was successful.</span></span> <span data-ttu-id="cfed6-135">Осы растауды алғаннан кейін SQL Services Management Studio ортасын жабуға болады.</span><span class="sxs-lookup"><span data-stu-id="cfed6-135">After you receive this confirmation, you can close SQL Services Management Studio.</span></span>

12. <span data-ttu-id="cfed6-136">**Интернет ақпараттық қызметтері** > **Бағдарлама қорлары** > **AOSService** тармағына қайта оралып, AOSService қызметін іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-136">Go back to **Internet Information Services** > **Application Pools** > **AOSService** and start the AOSService.</span></span>
13. <span data-ttu-id="cfed6-137">**Қызметтер** бөліміне өтіп, алдында тоқтатқан екі қызметті іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-137">Go to **Services** and start the two services you stopped earlier.</span></span>

14. <span data-ttu-id="cfed6-138">Осы VM жүйесінде AdminUserProvisioning құралын табыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-138">Locate the AdminUserProvisioning tool on this VM.</span></span> <span data-ttu-id="cfed6-139">K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe жолынан қараңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-139">Look under, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span></span>
15. <span data-ttu-id="cfed6-140">**Электрондық пошта** өрісіндегі пайдаланушы мекенжайыңызды қолданып, .ext файлын іске қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-140">Run the .ext file using your user address in the **Email Address** field.</span></span> 
16. <span data-ttu-id="cfed6-141">**Жіберу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-141">Select **Submit**.</span></span>

![Әкімші пайдаланушысы дайындалуда](./media/8AdminUserProvisioning.png)

<span data-ttu-id="cfed6-143">Мұны аяқтауға бірнеше минут кетеді.</span><span class="sxs-lookup"><span data-stu-id="cfed6-143">This takes a couple of minutes to complete.</span></span> <span data-ttu-id="cfed6-144">Сіз әкімші пайдаланушысы сәтті жаңартылғандығы туралы растау хабарламасын алуыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="cfed6-144">You should receive a confirmation message that the Admin user was successfully updated.</span></span>

17. <span data-ttu-id="cfed6-145">Соңында, пәрмендік жолды әкімші ретінде іске қосып, iisreset пәрменін орындаңыз</span><span class="sxs-lookup"><span data-stu-id="cfed6-145">Lastly, run Command Prompt as Administrator and perform iisreset</span></span>

![IIS Reset пәрмені](./media/9IISReset.png)

18. <span data-ttu-id="cfed6-147">Қашықтағы жұмыс үстелінің сессиясын жауып, оның күтілгендей жұмыс істеп тұрғанын растау үшін ортаға кіру мақсатында LCS **Орта туралы мәліметтер** бетін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="cfed6-147">Close the remote desktop session and use the LCS **Environment details** page to log in to the environment to confirm it is working as expected.</span></span>

![Finance and Operations](./media/10FinanceAndOperations.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]