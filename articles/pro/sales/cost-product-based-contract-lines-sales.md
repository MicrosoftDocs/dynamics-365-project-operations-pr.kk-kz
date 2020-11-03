---
title: Өнімге негізделген келісім-шарт жолдарын есептеу
description: Бұл тақырыпта жасау туралы ақпарат берілген
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7dfb9425174dddee52f9ee64f7a963e48a6bca70
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/20/2020
ms.locfileid: "4079891"
---
# <a name="costing-product-based-contract-lines"></a><span data-ttu-id="e9836-103">Өнімге негізделген келісім-шарт жолдарын есептеу</span><span class="sxs-lookup"><span data-stu-id="e9836-103">Costing product-based contract lines</span></span>

<span data-ttu-id="e9836-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="e9836-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="e9836-105">Dynamics 365 Project Operations бағдарламасындағы өнімге негізделген келісім-шарт жолдары **Шығын** өрісін қамтиды, ол өнім шығынын төменгі табыстылықты есептеу үшін сақтайды.</span><span class="sxs-lookup"><span data-stu-id="e9836-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="e9836-106">Каталог өнімі үшін өнімге негізделген келісім-шарт жолы жасалған кезде, өнімге негізделген келісім-шарт жолының құны өнім каталогындағы **Стандартты құн** өрісіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="e9836-106">When a product-based contract line is created for a catalog product, the cost of the product-based contract line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="e9836-107">Өнім каталогындағы **Стандартты құн** өрісі ұйымның негізгі валютасымен белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="e9836-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="e9836-108">Бірлік құны келісім-шарт жолындағы әдепкі мәнге келтірілген кезде, ол келісім-шарттағы сатылым валютасына ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="e9836-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="e9836-109">Өнімге негізделген келісім-шарт жолындағы бірлік құны</span><span class="sxs-lookup"><span data-stu-id="e9836-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="e9836-110">Өнімге негізделген келісім-шарт жолындағы бірлік құнына ие болу әр сатылым үшін өнімге әртүрлі құн беруге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="e9836-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="e9836-111">Әрдайым қажет бола бермегенімен, жеткізуші тарапынан тұтынушыға өнімнің өзіндік құнын төмендетуге болатын сценарийлер бар.</span><span class="sxs-lookup"><span data-stu-id="e9836-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="e9836-112">Төмендегі сценарийді қарастырыңыз:</span><span class="sxs-lookup"><span data-stu-id="e9836-112">Consider the following scenario:</span></span>

<span data-ttu-id="e9836-113">Fabrikam Robotics компаниясы Adatum корпорациясының құрастыру жолдарына робот қаруын орнатуда.</span><span class="sxs-lookup"><span data-stu-id="e9836-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="e9836-114">Fabrikam орнату қызметін ұсынады, бірақ роботты қару Trey Research компаниясынан сатып алынады.</span><span class="sxs-lookup"><span data-stu-id="e9836-114">Fabrikam provides installation services but the robotic arms are procured from Trey Research.</span></span> <span data-ttu-id="e9836-115">Егер Adatum корпорациясында робот қаруының орнатылуы Trey Research компаниясы үшін жаңа индустрияны ашса, Trey бұл келісім үшін Fabrikam компаниясына арнайы жеңілдік ұсына алады.</span><span class="sxs-lookup"><span data-stu-id="e9836-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="e9836-116">Бұл жағдайда Fabrikam компаниясы роботтық қару үшін өнімге негізделген келісім-шарттар желісін жасайды және осы келісім-шарттың бірлігі үшін шығындарды енгізеді, бұл Trey Research компаниясының роботтық қарудың стандартты құнынан өзгеше.</span><span class="sxs-lookup"><span data-stu-id="e9836-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms and inputs a per unit cost for this contract that is different from the standard cost of robotic arms from Trey Research.</span></span>
