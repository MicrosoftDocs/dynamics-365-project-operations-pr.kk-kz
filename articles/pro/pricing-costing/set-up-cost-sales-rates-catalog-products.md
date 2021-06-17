---
title: Каталог өнімдері үшін құн мен сатылым мөлшерлемелерін орнату - жеңілдетілген
description: Бұл тақырыпта өнім каталогындағы элементтің өзіндік құны мен сатылым мөлшерлерін орнату әдісі туралы ақпарат берілген.
author: rumant
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4995859696c844e99593139f63dffbf86a52f2f0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004335"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="b846b-103">Каталог өнімдері үшін құн мен сатылым мөлшерлемелерін орнату - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="b846b-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="b846b-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="b846b-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="b846b-105">Dynamics 365 Project Operations бағдарламасында өнім каталогындағы элементтерге баға белгілеу Dynamics 365 Sales бағдарламасымен бірдей.</span><span class="sxs-lookup"><span data-stu-id="b846b-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="b846b-106">Project Operations бағдарламасында өнімдерді бағалау немесе жобаларда пайдалану мүмкін емес, сондықтан өнім каталогының бағалары баға ұсыныстары мен келісім-шарттарға арналған жоба бағатізбесінде белгілеудің қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="b846b-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="b846b-107">Өнім каталогының бағаларын белгілеу үшін баға ұсынысы, келісім-шарт немесе тіркелгінің **Өнім бағасы** өрісін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="b846b-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="b846b-108">Жоба бағатізбелерінде өнім каталогының бағаларын белгілеуге болмайды.</span><span class="sxs-lookup"><span data-stu-id="b846b-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="b846b-109">Жоба бағатізбелері тек Project Operations бағдарламасына ғана қатысты.</span><span class="sxs-lookup"><span data-stu-id="b846b-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="b846b-110">Бағдарламаға арналған бизнес логикасы бағатізбені баға ұсынысынан келісім-шартқа көшіреді.</span><span class="sxs-lookup"><span data-stu-id="b846b-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="b846b-111">Нәтиже келісім-шарттың арнайы жоба бағатізбесі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="b846b-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="b846b-112">Баға ұсынысындағы жоба бағатізбесі өте үлкен болса, көшіру әрекеті баға ұсыныстарын жеңіп алу процесін кешіктіруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="b846b-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="b846b-113">Өнім бағатізбелері келісім-шарттар бойынша реттелетін бағатізбелер жасау үшін көшірілмейді.</span><span class="sxs-lookup"><span data-stu-id="b846b-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="b846b-114">Көшіру болмағандықтан, баға ұсыну процесінің өнімділігіне әсер етпейді.</span><span class="sxs-lookup"><span data-stu-id="b846b-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]