---
title: Бағатізбелерді өшіру
description: Бұл тақырыпта қолданылмаған немесе ескі бағатізбелерді өшіру немесе жою туралы түсіндіріледі.
author: rumant
manager: AnnBe
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Professional Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 3fa902e93815002be7d6915880cd7759dbbde5ef
ms.sourcegitcommit: 386921f44f1e9a8a828b140206d52945de07aee7
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/22/2021
ms.locfileid: "5701948"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="8caac-103">Бағатізбелерді өшіру</span><span class="sxs-lookup"><span data-stu-id="8caac-103">Deactivate price lists</span></span> 

<span data-ttu-id="8caac-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="8caac-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8caac-105">Dynamics 365 Project Operations бағдарламасынан ескі немесе пайдаланылмайтын бағатізбелерді жою үшін орындау керек екі қадам бар.</span><span class="sxs-lookup"><span data-stu-id="8caac-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="8caac-106">Белгілі бір беттерден бағатізбені алып тастаңыз немесе жойыңыз.</span><span class="sxs-lookup"><span data-stu-id="8caac-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="8caac-107">**Бағатізбелер** бетіндегі "Белсенді бағатізбелер" аймағынан бағатізбелерді өшіріңіз немесе жойыңыз.</span><span class="sxs-lookup"><span data-stu-id="8caac-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="8caac-108">Бағатізбені толығымен алып тастау үшін сіз екі қадамды да орындауыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="8caac-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="8caac-109">"Белсенді бағатізбелер" көрінісінен бағатізбелерді тікелей өшіру немесе жою үшін 2-ші қадамды ғана орындау жеткіліксіз.</span><span class="sxs-lookup"><span data-stu-id="8caac-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="8caac-110">Сіз сондай-ақ осы бағатізбенің байланысын 1-ші қадамда аталған барлық жерлерден жоюыңыз керек.</span><span class="sxs-lookup"><span data-stu-id="8caac-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="8caac-111">Белгілі бір беттерден бағатізбені жою</span><span class="sxs-lookup"><span data-stu-id="8caac-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="8caac-112">Project Operations ішінен бағатізбені жою үшін келесі беттерге өтіңіз:</span><span class="sxs-lookup"><span data-stu-id="8caac-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="8caac-113">**Жоба параметрлері** беті > **Бағатізбелер** қойыншасы</span><span class="sxs-lookup"><span data-stu-id="8caac-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="8caac-114">**Ұйымдық бірлік** беті > **Бағатізбелер** торы</span><span class="sxs-lookup"><span data-stu-id="8caac-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="8caac-115">**Шот** беті > **Жоба бағатізбелері** торы</span><span class="sxs-lookup"><span data-stu-id="8caac-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="8caac-116">**Жоба баға ұсыныстары** беті > **Жоба бағатізбелері** торы: бұл барлық белсенді жоба баға ұсыныстарына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="8caac-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="8caac-117">**Жоба келісім-шарттары** беті > **Жоба бағатізбелері** торы: бұл барлық белсенді жоба келісім-шарттарына қолданылады.</span><span class="sxs-lookup"><span data-stu-id="8caac-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="8caac-118">Әрбір бет үшін жойғыңыз келетін бағатізбені таңдап, **Жою** опциясын таңдау қажет.</span><span class="sxs-lookup"><span data-stu-id="8caac-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="8caac-119">Бағатізбелер бетінен бағатізбелерді өшіру немесе жою</span><span class="sxs-lookup"><span data-stu-id="8caac-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="8caac-120">Белсенді бағатізбелерден бағатізбені жою үшін мына жерге өтіңіз: **Сатылым** > **Тұтынушылар** > **Бағатізбелер**.</span><span class="sxs-lookup"><span data-stu-id="8caac-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="8caac-121">Жойғыңыз келетін бағатізбені таңдаңыз, содан кейін **Жою** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8caac-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="8caac-122">Егер кез келген бұрыннан бар транзакцияларда бағатізбеге сілтеме жасалса, сіз оны жоя алмайсыз.</span><span class="sxs-lookup"><span data-stu-id="8caac-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="8caac-123">Егер бұл орын алса, сіз бағатізбені ешбір көріністе көрінбейтіндей етіп өшіре аласыз.</span><span class="sxs-lookup"><span data-stu-id="8caac-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="8caac-124">Бағатізбені өшіру үшін бағатізбені қайтадан таңдап, **Өшіру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8caac-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
