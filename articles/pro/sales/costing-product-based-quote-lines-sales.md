---
title: Өнімге негізделген баға ұсыну жолдарын есептеу
description: Бұл тақырыпта өнімге негізделген баға ұсыну жолына шығынды қолдану туралы ақпарат берілген.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1fa7896e249abfefd3e93cba4bad789e67e14f31
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003458"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="929d8-103">Өнімге негізделген баға ұсыну жолдарын есептеу</span><span class="sxs-lookup"><span data-stu-id="929d8-103">Costing product-based quote lines</span></span>

<span data-ttu-id="929d8-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="929d8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="929d8-105">Dynamics 365 Project Operations бағдарламасындағы өнімге негізделген баға ұсыну жолдарында сондай-ақ **Шығын** өрісі бар.</span><span class="sxs-lookup"><span data-stu-id="929d8-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="929d8-106">Бұл өріс баға ұсыну жолындағы өнім шығынын бақылау үшін және төменгі табыстылығын есептеу үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="929d8-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="929d8-107">Каталог өнімі үшін өнімге негізделген баға ұсыну жолы жасалған кезде, өнімге негізделген баға ұсыну жолының құны өнім каталогындағы **Стандартты құн** өрісіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="929d8-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="929d8-108">Өнім каталогындағы стандартты құн өрісі ұйымның негізгі валютасымен белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="929d8-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="929d8-109">Өнімге негізделген баға ұсыну жолындағы әдепкі бірлік құны баға ұсынысындағы сату валютасына ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="929d8-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="929d8-110">Өнімге негізделген баға ұсыну жолындағы бірлік құны</span><span class="sxs-lookup"><span data-stu-id="929d8-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="929d8-111">Өнімге негізделген баға ұсыну жолындағы бірлік құнының мақсаты - әр сатылым үшін өнімге әртүрлі құн беру.</span><span class="sxs-lookup"><span data-stu-id="929d8-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="929d8-112">Бұл әдеттегі сценарий емес, бірақ кейде өнімнің өзіндік құнын жеткізуші соңғы сатылымның тұтынушысына байланысты төмендетуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="929d8-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="929d8-113">Мысалы:</span><span class="sxs-lookup"><span data-stu-id="929d8-113">For example:</span></span>

<span data-ttu-id="929d8-114">Fabrikam Robotics компаниясы A Datum корпорациясының құрастыру жолдарына робот қаруын орнатуда.</span><span class="sxs-lookup"><span data-stu-id="929d8-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="929d8-115">Fabrikam орнату қызметін ұсынады, бірақ роботты қару Trey робототехникасынан сатып алынады.</span><span class="sxs-lookup"><span data-stu-id="929d8-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="929d8-116">Егер А Datum корпорациясында робот қаруының орнатылуы Trey робот қаруы үшін жаңа индустрияны ашса, Trey бұл келісім үшін Fabrikam компаниясына арнайы жеңілдік бере алады.</span><span class="sxs-lookup"><span data-stu-id="929d8-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="929d8-117">Бұл жағдайда, Fabrikam роботты қару үшін өнімге негізделген баға ұсыну жолдарын жасайды және осы баға ұсынысы үшін бір дананың өзіндік құнын арнайы енгізеді.</span><span class="sxs-lookup"><span data-stu-id="929d8-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="929d8-118">Бұл шығын Trey Robotic Arms стандартты бағасынан өзгеше.</span><span class="sxs-lookup"><span data-stu-id="929d8-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]