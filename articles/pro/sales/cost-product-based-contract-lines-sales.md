---
title: Өнімге негізделген келісім-шарт жолдарының құны - жеңілдетілген
description: Бұл тақырыпта жасау туралы ақпарат берілген
author: rumant
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 9458a57863244a68359f57185325c03a46bd6569
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003548"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="2defd-103">Өнімге негізделген келісім-шарт жолдарының құны - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="2defd-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="2defd-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="2defd-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="2defd-105">Dynamics 365 Project Operations бағдарламасындағы өнімге негізделген келісімшарт жолдары төменгі ағынның табыс есептеулері үшін өнімнің шығынын сақтайтын **Шығын** өрісін қамтиды.</span><span class="sxs-lookup"><span data-stu-id="2defd-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="2defd-106">Каталогтық өнім үшін өнімге негізделген келісімшарт жолы жасалған жағдайда, жолдың құны өнім каталогындағы **Стандартты шығын** өрісінде әдепкі бойынша көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="2defd-106">When a product-based contract line is created for a catalog product, the cost of the line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="2defd-107">Өнім каталогындағы **Стандартты құн** өрісі ұйымның негізгі валютасымен белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="2defd-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="2defd-108">Бірлік құны келісім-шарт жолындағы әдепкі мәнге келтірілген кезде, ол келісім-шарттағы сатылым валютасына ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="2defd-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="2defd-109">Өнімге негізделген келісім-шарт жолындағы бірлік құны</span><span class="sxs-lookup"><span data-stu-id="2defd-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="2defd-110">Өнімге негізделген келісім-шарт жолындағы бірлік құнына ие болу әр сатылым үшін өнімге әртүрлі құн беруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="2defd-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="2defd-111">Әрдайым қажет бола бермегенімен, жеткізуші тарапынан тұтынушыға өнімнің өзіндік құнын төмендетуге болатын сценарийлер бар.</span><span class="sxs-lookup"><span data-stu-id="2defd-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="2defd-112">Төмендегі сценарийді қарастырыңыз:</span><span class="sxs-lookup"><span data-stu-id="2defd-112">Consider the following scenario:</span></span>

<span data-ttu-id="2defd-113">Fabrikam Robotics компаниясы Adatum корпорациясының құрастыру жолдарына робот қаруын орнатуда.</span><span class="sxs-lookup"><span data-stu-id="2defd-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="2defd-114">Fabrikam орнату қызметтерін ұсынады, бірақ роботтандырылған қолдар Trey Research компаниясынан шығарылады.</span><span class="sxs-lookup"><span data-stu-id="2defd-114">Fabrikam provides installation services but the robotic arms are from Trey Research.</span></span> <span data-ttu-id="2defd-115">Егер Adatum корпорациясында робот қаруының орнатылуы Trey Research компаниясы үшін жаңа индустрияны ашса, Trey бұл келісім үшін Fabrikam компаниясына арнайы жеңілдік ұсына алады.</span><span class="sxs-lookup"><span data-stu-id="2defd-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="2defd-116">Бұл жағдайда Fabrikam компаниясы роботтандырылған қолдар үшін өнімге негізделген келісімшарттар жолын жасайды.</span><span class="sxs-lookup"><span data-stu-id="2defd-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms.</span></span> <span data-ttu-id="2defd-117">Осы келісімшарт үшін бірлік құны енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="2defd-117">A per unit cost is entered for this contract.</span></span> <span data-ttu-id="2defd-118">Құны Trey Research компаниясының роботтандырылған қолдарының құнынан өзгеше.</span><span class="sxs-lookup"><span data-stu-id="2defd-118">The cost is different from the cost of robotic arms from Trey Research.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]