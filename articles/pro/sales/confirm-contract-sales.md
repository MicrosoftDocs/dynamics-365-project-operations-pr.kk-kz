---
title: Жоба келісім-шартын растау
description: Бұл тақырып Project Operations жүйесінде келісім-шартты растау жолы туралы ақпарат береді.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 24da0887c0266d51bddcbbf8efd6f2644b6d0f4f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128290"
---
# <a name="confirm-a-project-contract"></a><span data-ttu-id="dfad6-103">Жоба келісім-шартын растау</span><span class="sxs-lookup"><span data-stu-id="dfad6-103">Confirm a project contract</span></span>

<span data-ttu-id="dfad6-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="dfad6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="dfad6-105">Dynamics 365 Project Operations ішіндегі жоба келісім-шарты **Расталған** себебінен белсенді немесе **Жоғалған** себебінен жабық болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="dfad6-105">A project contract in Dynamics 365 Project Operations can be active with a reason of **Confirmed**, or closed with a reason of **Lost**.</span></span> <span data-ttu-id="dfad6-106">Жоба келісім-шартын растаған кезде, күй **Жоба** деңгейінен **Белсенді** деңгейіне жаңартылады және күй себебі – **Расталған**.</span><span class="sxs-lookup"><span data-stu-id="dfad6-106">When you confirm a project contract, the status updates from **Draft** to **Active** and the status reason is **Confirmed**.</span></span> <span data-ttu-id="dfad6-107">Белсенді немесе жабық келісім-шартты өзгерту немесе қайта ашу мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="dfad6-107">An active or closed contract can't be edited or reopened.</span></span> 

### <a name="financial-impact-of-confirming-a-project-contract"></a><span data-ttu-id="dfad6-108">Жоба келісім-шартын растаудың қаржылық әсері</span><span class="sxs-lookup"><span data-stu-id="dfad6-108">Financial impact of confirming a project contract</span></span>

<span data-ttu-id="dfad6-109">Жоба келісім-шарты расталғаннан кейін, бағдарлама ескі құнның нақты көсеткіштерін қайта қалпына келтіру және жаңа құнның нақты көрсеткіштерін қайта жасау арқылы құндарды қайта есептейді.</span><span class="sxs-lookup"><span data-stu-id="dfad6-109">After a project contract is confirmed, the application recalculates the costs by reversing the older cost actuals and creating new cost actuals.</span></span> <span data-ttu-id="dfad6-110">Құнның жаңа нақты көрсеткіштері жобаның келісім-шарт жолының шот ұсыну әдісі негізінде өңделеді.</span><span class="sxs-lookup"><span data-stu-id="dfad6-110">The new cost actuals are then processed based on the billing method of the associated project contract line.</span></span> <span data-ttu-id="dfad6-111">Егер құнның нақты шығындары уақыт пен материалдық келісімшарт жолына сілтеме жасаса, бағдарлама автоматты түрде сатылымның тиісті нақты көрсеткіштерін қайта жасайды.</span><span class="sxs-lookup"><span data-stu-id="dfad6-111">If the cost actuals reference a Time and Material contract line, the application automatically re-creates corresponding unbilled sales actuals.</span></span> <span data-ttu-id="dfad6-112">Егер құнның нақты көрсеткіштері белгіленген бағаның келісім-шарт жолына сілтеме жасаса, бағдарлама құнның нақты шығындарын қайта өңдеуді тоқтатады.</span><span class="sxs-lookup"><span data-stu-id="dfad6-112">If the cost actuals reference a Fixed Price contract line, the application stops reprocessing the cost actuals.</span></span>

<span data-ttu-id="dfad6-113">Шектерден аспау, төлем қабілеттілігін орнату және нақты бағалар бойынша баға мен шығындар бағаланады, содан кейін растау процесінің бір бөлігі ретінде жаңартылады.</span><span class="sxs-lookup"><span data-stu-id="dfad6-113">Not-to-exceed limits, chargeability setup, and pricing and costing on the actuals is evaluated and then updated as part of the confirmations process.</span></span>

## <a name="close-a-project-contract-as-lost"></a><span data-ttu-id="dfad6-114">Жоба келісім-шартын жоғалған ретінде жабу</span><span class="sxs-lookup"><span data-stu-id="dfad6-114">Close a project contract as lost</span></span>

<span data-ttu-id="dfad6-115">Жоба келісім-шартын жоғалған ретінде жабу кезінде келісім-шарт күйі **Жабық** күйге жаңартылып, күй себебі **Жоғалған** болады.</span><span class="sxs-lookup"><span data-stu-id="dfad6-115">When you close a project contract as lost, the contract status is updated to **Closed** and the status reason is **Lost**.</span></span> <span data-ttu-id="dfad6-116">Жоба келісім-шарты тек оқуға арналған болады.</span><span class="sxs-lookup"><span data-stu-id="dfad6-116">The project contract becomes read-only.</span></span> <span data-ttu-id="dfad6-117">Жабық жоба келісімшартын қайта аша алмайтындықтан, өзгерістер аяқталғанға дейін растау диалогы беріледі.</span><span class="sxs-lookup"><span data-stu-id="dfad6-117">A confirmation dialog is provided before the changes are complete because you can't reopen a closed project contract.</span></span>

<span data-ttu-id="dfad6-118">Егер жоғалған ретінде жабылған жоба келісім-шартында оның жолдары көрсетілген болса, онда ол да жабық деп белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="dfad6-118">If the project contract that is closed as lost references a project on its lines, that project is also marked as closed.</span></span> <span data-ttu-id="dfad6-119">Сол күннен бастап кез келген ресурстарға тапсырыс жойылады.</span><span class="sxs-lookup"><span data-stu-id="dfad6-119">Any resource bookings from that day forward are canceled.</span></span> <span data-ttu-id="dfad6-120">Жоба келісім+шарты бойынша есеп-шотта жоқ кез келген сатылым нақты көрсеткіштері қайтарылады.</span><span class="sxs-lookup"><span data-stu-id="dfad6-120">Any unbilled sales actuals on the project contract that aren't already on an invoice, will be reversed.</span></span>

> [!NOTE]
> <span data-ttu-id="dfad6-121">Dynamics 365 Project Operations ішінде жоба келісім-шартын жоғалған деп жабу байланысты мүмкіндіктің күйіне әсер етпейді.</span><span class="sxs-lookup"><span data-stu-id="dfad6-121">In Dynamics 365 Project Operations, closing a project contract as lost will not impact that status of the associated opportunity.</span></span> <span data-ttu-id="dfad6-122">Мүмкіндік ашық болып қалады және қолмен жабық болуы керек.</span><span class="sxs-lookup"><span data-stu-id="dfad6-122">The opportunity will remain open and must be manually closed.</span></span>
