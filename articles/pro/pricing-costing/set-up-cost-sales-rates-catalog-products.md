---
title: Каталог өнімдерінің өзіндік құнын және сатылым мөлшерін белгілеңіз
description: Бұл тақырыпта өнім каталогындағы элементтің өзіндік құны мен сатылым мөлшерлерін орнату әдісі туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5178a9143536bf4b2573403125325017861cdd5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079727"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products"></a><span data-ttu-id="c2a02-103">Каталог өнімдерінің өзіндік құнын және сатылым мөлшерін белгілеңіз</span><span class="sxs-lookup"><span data-stu-id="c2a02-103">Set up cost and sales rates for catalog products</span></span>

<span data-ttu-id="c2a02-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="c2a02-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c2a02-105">Dynamics 365 Project Operations бағдарламасындағы өнім каталогының элементтеріне бағаны орнату Dynamics 365 Sales бағдарламасындағымен бірдей.</span><span class="sxs-lookup"><span data-stu-id="c2a02-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="c2a02-106">Өнімдерді Project Operations бағдарламасындағы жобаларда болжауға немесе пайдалануға болмайтындықтан, баға ұсыныстары мен келісім-шарттар үшін жоба бағатізбелерінде өнім каталогының бағаларын орнатудың қажеті жоқ.</span><span class="sxs-lookup"><span data-stu-id="c2a02-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="c2a02-107">Өнім каталогының бағаларын баға ұсынысының, келісім-шарттың немесе тіркелгінің **Өнімнің бағасы** өрісінде орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="c2a02-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="c2a02-108">Жоба бағатізбелерінде осы нысандар үшін өнім каталогының бағаларын орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="c2a02-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="c2a02-109">Жоба бағатізбелері тек Project Operations бағдарламасына ғана қатысты.</span><span class="sxs-lookup"><span data-stu-id="c2a02-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="c2a02-110">Бағатізбелерді баға ұсынысынан келісім-шартқа көшіретін бағдарламаға тән бизнес-логика бар.</span><span class="sxs-lookup"><span data-stu-id="c2a02-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="c2a02-111">Нәтиже келісім-шарттың арнайы жоба бағатізбесі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="c2a02-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="c2a02-112">Баға ұсынысындағы жоба бағатізбесі өте үлкен болса, көшіру әрекеті баға ұсыныстарын жеңіп алу процесін кешіктіруі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="c2a02-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="c2a02-113">Өнім бағатізбелері келісім-шарттар бойынша реттелетін бағатізбелер жасау үшін көшірілмейді.</span><span class="sxs-lookup"><span data-stu-id="c2a02-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="c2a02-114">Бұл өнімнің бағатізбелері баға ұсыныстарын жеңіп алу процесінің жұмысына әсер етпейтінін білдіреді.</span><span class="sxs-lookup"><span data-stu-id="c2a02-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
