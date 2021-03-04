---
title: Баға ұсынуды жабу - жеңілдетілген
description: Бұл тақырыпта Project Operations бағдарламасындағы баға ұсынысын жабу туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8d387816f51f63ecd95df6534c7c012b323e6ddc
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764871"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="83163-103">Баға ұсынуды жабу - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="83163-103">Close a quote - lite</span></span>

<span data-ttu-id="83163-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="83163-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="83163-105">Жобаның баға ұсынысын Ұтқан немесе Ұтылған ретінде жабуға болады.</span><span class="sxs-lookup"><span data-stu-id="83163-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="83163-106">Жобалық баға ұсынысы жабылуы мүмкін, себебі баға ұсыныстарындағы белсенді және түзету операцияларына Microsoft Dynamics 365 Project Operations бағдарламасында қолдау көрсетілмейді.</span><span class="sxs-lookup"><span data-stu-id="83163-106">A draft quote can be closed because the Activate and Revise operations on quotes isn't supported in Microsoft Dynamics 365 Project Operations.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="83163-107">Баға ұсынысын Ұтқан ретінде жабу</span><span class="sxs-lookup"><span data-stu-id="83163-107">Close a quote as Won</span></span>

<span data-ttu-id="83163-108">Жобалық баға ұсынысын "Ұтқан" ретінде жапқанда, күй "Жабық" күйіне орнатылып, күй себебі "Ұтқан" болады.</span><span class="sxs-lookup"><span data-stu-id="83163-108">When you close a project quote as Won, the status is set to Closed and the status reason is Won.</span></span> <span data-ttu-id="83163-109">Баға ұсынысын жабу жобаның баға ұсынысын тек оқу үшін қолжетімді етеді және баға ұсынысы туралы ақпаратты қамтитын жобалық келісім-шартты жасайды.</span><span class="sxs-lookup"><span data-stu-id="83163-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="83163-110">Жабылған баға ұсынысын қайта ашу мүмкін емес, растау диалогтік терезесі өзгерістерді растайды.</span><span class="sxs-lookup"><span data-stu-id="83163-110">Because a closed quote can't be reopened, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="83163-111">Егер баға ұсынысы мүмкіндікке тіркелген болса, кез келген басқа жобаның баға ұсыныстары автоматты түрде Ұтылған ретінде жабылады.</span><span class="sxs-lookup"><span data-stu-id="83163-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="83163-112">Ұтқан ретінде баға ұсынысын жабудың қаржылық әсері</span><span class="sxs-lookup"><span data-stu-id="83163-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="83163-113">Егер жоба бойынша баға ұсыныстарына тіркелген кезде қандай да бір уақыттың нақты көрсеткіштері болса, онда уақыттың немесе шығындардың құны ғана жазылады.</span><span class="sxs-lookup"><span data-stu-id="83163-113">If there are any actuals for time on a project while is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="83163-114">Баға ұсынысы Ұтқан ретінде жабылғаннан кейін, бағдарлама ескі құнның нақты көсеткіштерін қайта қалпына келтіру және жаңа құнның нақты көрсеткіштерін қайта жасау арқылы құндарда рефакторинг жасайды.</span><span class="sxs-lookup"><span data-stu-id="83163-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="83163-115">Бағдарлама құнның осы нақты көрсеткіштерін жобаның келісім-шарт жолының шот ұсыну әдісі негізінде өңдейді.</span><span class="sxs-lookup"><span data-stu-id="83163-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="83163-116">Егер құнның нақты көрсеткіштері уақыт пен материалдық келісім-шарттың желісіне сілтеме жасаса, баға ұсынысы жабылған кезде және жоба бойынша келісім-шарт жасалған кезде сәйкесінше шот ұсынылмаған сатылымның нақты көрсеткіштері жасалады.</span><span class="sxs-lookup"><span data-stu-id="83163-116">If the cost actuals reference a time and material contract line, corresponding unbilled sales actuals are created for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="83163-117">Егер құнның нақты мәндері белгіленген бағаның келісім-шарт жолына сілтеме жасаса, бағдарлама жобаның келісім-шарт тұтынушылары үшін бөлудегі шот ұсыну ережелеріне негізделген өзіндік құнды қайта өңдеуді тоқтатады.</span><span class="sxs-lookup"><span data-stu-id="83163-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals that are based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="83163-118">Баға ұсынысын ұтылған ретінде жабу:</span><span class="sxs-lookup"><span data-stu-id="83163-118">Closing a quote as lost:</span></span>

<span data-ttu-id="83163-119">Жобалық баға ұсынысын "Ұтылған" ретінде жапқанда, күй "Жабық" күйіне орнатылып, күй себебі "Ұтылған" болады.</span><span class="sxs-lookup"><span data-stu-id="83163-119">When you close a project quote as Lost, the status is set to Closed and status reason is Lost.</span></span> <span data-ttu-id="83163-120">Баға ұсынысын жабу жобаның баға ұсынысын тек оқу үшін қолжетімді етеді.</span><span class="sxs-lookup"><span data-stu-id="83163-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="83163-121">Жабық баға ұсынысын қайта ашу мүмкін болмағандықтан, оны жаппас бұрын растау диалогтік терезесі өзгертулерді растайды.</span><span class="sxs-lookup"><span data-stu-id="83163-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="83163-122">Егер "Ұтылған" ретінде жабылған жобалық баға ұсынысы оның жолдарының кез келгеніндегі жобаға сілтеме жасаса, сол жоба да "Жабық" ретінде белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="83163-122">If the project quote that is closed as Lost references a project on any of its lines, that project is also marked as Closed.</span></span> <span data-ttu-id="83163-123">Сол күннен бастап кез келген ресурстарға тапсырыс жойылады.</span><span class="sxs-lookup"><span data-stu-id="83163-123">Any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="83163-124">Project Operations бағдарламасында баға ұсынысын Ұтқан немесе Ұтылған деп жабу қолмен жабылғанға дейін ашық болатын Мүмкіндік күйіне әсер етпейді.</span><span class="sxs-lookup"><span data-stu-id="83163-124">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
