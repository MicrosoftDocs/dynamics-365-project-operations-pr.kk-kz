---
title: Өнімге негізделген мүмкіндік жолдары - жеңілдетілген
description: Бұл тақырыпта Project Operations бағдарламасындағы өнімге негізделген мүмкіндік жолдарының элементтері туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f7dfabd068e180c7122ede0f79aaebfe220250a1
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949551"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="db53a-103">Өнімге негізделген мүмкіндік жолдары - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="db53a-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="db53a-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="db53a-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="db53a-105">Өнімге негізделген мүмкіндіктер жолдары - бұл Мүмкіндіктегі жол элементтері.</span><span class="sxs-lookup"><span data-stu-id="db53a-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="db53a-106">Бұл нақты жол элементтері тұтынушыға ұсынылатын ықтимал есеп-шотта орналасқан.</span><span class="sxs-lookup"><span data-stu-id="db53a-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="db53a-107">Есеп-шотта басқа қосымша қызметтер жоқ.</span><span class="sxs-lookup"><span data-stu-id="db53a-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="db53a-108">Байланысқан шығындар мен тұтынулар байланысты жобалардың тапсырмалары бойынша бақыланбайды.</span><span class="sxs-lookup"><span data-stu-id="db53a-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="db53a-109">Өнімге негізделген жолдар каталог элементтері немесе енгізілген өнімдер болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="db53a-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="db53a-110">Мүмкіндік өніміне негізделген жолдардағы функционалды мүмкіндіктердің көпшілігі Dynamics 365 Sales бағдарламасы ұсынған функционалды мүмкіндіктерге сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="db53a-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="db53a-111">Өнімге негізделген мүмкіндік жолдары туралы қосымша ақпаратты келесі бөлімнен қараңыз: [Мүмкіндікке өнімдер қосу](/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="db53a-111">For more information about product-based opportunity lines, see [Add products to an opportunity](/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="db53a-112">**Тұтынушы бюджеті** – бұл жобаға негізделген мүмкіндік жолдарына арналған тұжырымдама.</span><span class="sxs-lookup"><span data-stu-id="db53a-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="db53a-113">**Тұтынушы бюджеті** өрісінде тұтынушы элемент үшін төлеуге дайын болатын сома бақыланады.</span><span class="sxs-lookup"><span data-stu-id="db53a-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="db53a-114">Мүмкіндіктер жиынтығының кіріс әдісі **Жүйе арқылы есептелген** күйінде болған кезде, болжамды кірісті есептеу үшін мүмкіндік сызықтары бойынша тұтынушы бюджетінің мәндері жинақталады.</span><span class="sxs-lookup"><span data-stu-id="db53a-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 



[!INCLUDE[footer-include](../../includes/footer-banner.md)]