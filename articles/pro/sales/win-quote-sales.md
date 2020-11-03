---
title: Баға ұсыныстарын жабу
description: Бұл тақырыпта Project Operations бағдарламасындағы баға ұсынысын жабу туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cc3b2cdeb1ac46b7d927c1f96e94e9154d3eebf8
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079581"
---
# <a name="close-quotes"></a><span data-ttu-id="cc4a7-103">Баға ұсыныстарын жабу</span><span class="sxs-lookup"><span data-stu-id="cc4a7-103">Close quotes</span></span> 

<span data-ttu-id="cc4a7-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="cc4a7-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cc4a7-105">Жобаның баға ұсынысын Ұтқан немесе Ұтылған ретінде жабуға болады.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="cc4a7-106">Баға ұсыныстарындағы белсендіру және түзету операцияларына Microsoft Dynamics 365 Project Operations бағдарламасында қолдау көрсетілмейді, сондықтан баға ұсынысының жобасы жабылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-106">The Activate and Revise operations on quotes is not supported in Microsoft Dynamics 365 Project Operations, so a draft quote can be closed.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="cc4a7-107">Баға ұсынысын Ұтқан ретінде жабу</span><span class="sxs-lookup"><span data-stu-id="cc4a7-107">Close a quote as Won</span></span>

<span data-ttu-id="cc4a7-108">Жобаның баға ұсынысын Ұтқан ретінде жабу күйі Жабық және күй себебі Ұтқан күйінде қойылған баға ұсынысын жабады.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-108">Closing a project quote as Won will close the quote with the status set to Closed and the status reason set to Won.</span></span> <span data-ttu-id="cc4a7-109">Баға ұсынысын жабу жобаның баға ұсынысын тек оқу үшін қолжетімді етеді және баға ұсынысы туралы ақпаратты қамтитын жобалық келісім-шартты жасайды.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="cc4a7-110">Жабық баға ұсынысын қайта ашуға болмайтындықтан, өзгертулер енгізілмес бұрын растау диалогтық терезесі пайда болады, өйткені жабық баға ұсынысын қайта ашу мүмкін емес және өзгертулер қайтымсыз.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-110">Because a closed quote can't be reopened, a confirmation dialog There is a confirmation dialog before the changes are done since a closed quote cannot be re-opened and the changes are irreversible.</span></span>

<span data-ttu-id="cc4a7-111">Егер баға ұсынысы мүмкіндікке тіркелген болса, кез келген басқа жобаның баға ұсыныстары автоматты түрде Ұтылған ретінде жабылады.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="cc4a7-112">Ұтқан ретінде баға ұсынысын жабудың қаржылық әсері</span><span class="sxs-lookup"><span data-stu-id="cc4a7-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="cc4a7-113">Егер жобада, ол әлі де жобалық баға ұсынысына тіркелген кезде, жазылған уақыт үшін қандай да бір нақты көрсеткіштер болған болса, онда уақыт немесе шығыс құны ғана жазылады.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-113">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="cc4a7-114">Баға ұсынысы Ұтқан ретінде жабылғаннан кейін, бағдарлама ескі құнның нақты көсеткіштерін қайта қалпына келтіру және жаңа құнның нақты көрсеткіштерін қайта жасау арқылы құндарда рефакторинг жасайды.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="cc4a7-115">Бағдарлама құнның осы нақты көрсеткіштерін жобаның келісім-шарт жолының шот ұсыну әдісі негізінде өңдейді.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="cc4a7-116">Егер құнның нақты көрсеткіштері уақыт пен материалдық келісім-шарт жолына сілтеме жасаса, жүйе автоматты түрде баға ұсынысы жабылған кезде және жоба бойынша келісім-шарт жасалынған кезде есеп-шот ұсынылмаған сатудың тиісті нақты көрсеткіштерін жасайды.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-116">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="cc4a7-117">Егер құнның нақты көрсеткіштері келісім-шарт жолының белгіленген бағасына сілтеме жасаса, бағдарлама жоба келісім-шартының тұтынушыларына бөлінген төлем ережелері негізінде құнның нақты көрсеткіштерін қайта өңдеуді тоқтатады.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="cc4a7-118">Баға ұсынысын ұтылған ретінде жабу:</span><span class="sxs-lookup"><span data-stu-id="cc4a7-118">Closing a quote as lost:</span></span>

<span data-ttu-id="cc4a7-119">Жобаның баға ұсынысын Ұтылған деп жабу күйді Жабық, ал күй себебін Ұтылған деп орнатады.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-119">Closing a project quote as Lost will set the status to Closed and status reason to Lost.</span></span> <span data-ttu-id="cc4a7-120">Баға ұсынысын жабу жобаның баға ұсынысын тек оқу үшін қолжетімді етеді.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="cc4a7-121">Жабық баға ұсынысын қайта ашу мүмкін болмағандықтан, оны жаппас бұрын растау диалогтік терезесі өзгертулерді растайды.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="cc4a7-122">Егер Ұтылған ретінде жабылған жобаның баға ұсынысы оның кез келген жолында сілтеме жасаған болса, онда ол сондай-ақ Жабық деп белгіленеді және сол күннен бастап кез келген ресурстардың тапсырыстары жойылады.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-122">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="cc4a7-123">Project Operations бағдарламасында баға ұсынысын Ұтқан немесе Ұтылған деп жабу қолмен жабылғанға дейін ашық болатын Мүмкіндік күйіне әсер етпейді.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-123">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
