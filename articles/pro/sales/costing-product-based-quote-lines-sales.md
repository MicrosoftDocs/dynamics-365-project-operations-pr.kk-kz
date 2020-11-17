---
title: Өнімге негізделген баға ұсыну жолдарын есептеу
description: Бұл тақырыпта өнімге негізделген баға ұсыну жолына шығынды қолдану туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d21ab159294cac66ffeb8abcf0943b4babd7b360
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4118930"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="25931-103">Өнімге негізделген баға ұсыну жолдарын есептеу</span><span class="sxs-lookup"><span data-stu-id="25931-103">Costing product-based quote lines</span></span>

<span data-ttu-id="25931-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="25931-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="25931-105">Dynamics 365 Project Operations бағдарламасында өнімге негізделген баға ұсыну жолдары сондай-ақ **Шығын** өрісіне ие.</span><span class="sxs-lookup"><span data-stu-id="25931-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="25931-106">Бұл өріс баға ұсыну жолындағы өнім шығынын бақылау үшін және төменгі табыстылығын есептеу үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="25931-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="25931-107">Каталог өнімі үшін өнімге негізделген баға ұсыну жолы жасалған кезде, өнімге негізделген баға ұсыну жолының құны өнім каталогындағы **Стандартты құн** өрісіне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="25931-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="25931-108">Өнім каталогындағы стандартты құн өрісі ұйымның негізгі валютасымен белгіленеді.</span><span class="sxs-lookup"><span data-stu-id="25931-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="25931-109">Өнімге негізделген баға ұсыну жолындағы әдепкі бірлік құны баға ұсынысындағы сату валютасына ауыстырылады.</span><span class="sxs-lookup"><span data-stu-id="25931-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="25931-110">Өнімге негізделген баға ұсыну жолындағы бірлік құны</span><span class="sxs-lookup"><span data-stu-id="25931-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="25931-111">Өнімге негізделген баға ұсыну жолындағы бірлік құнының мақсаты - әр сатылым үшін өнімге әртүрлі құн беру.</span><span class="sxs-lookup"><span data-stu-id="25931-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="25931-112">Бұл әдеттегі сценарий емес, бірақ кейде өнімнің өзіндік құнын жеткізуші соңғы сатылымның тұтынушысына байланысты төмендетуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="25931-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="25931-113">Мысалы:</span><span class="sxs-lookup"><span data-stu-id="25931-113">For example:</span></span>

<span data-ttu-id="25931-114">Fabrikam Robotics компаниясы A Datum корпорациясының құрастыру жолдарына робот қаруын орнатуда.</span><span class="sxs-lookup"><span data-stu-id="25931-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="25931-115">Fabrikam орнату қызметін ұсынады, бірақ роботты қару Trey робототехникасынан сатып алынады.</span><span class="sxs-lookup"><span data-stu-id="25931-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="25931-116">Егер А Datum корпорациясында робот қаруының орнатылуы Trey робот қаруы үшін жаңа индустрияны ашса, Trey бұл келісім үшін Fabrikam компаниясына арнайы жеңілдік бере алады.</span><span class="sxs-lookup"><span data-stu-id="25931-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="25931-117">Бұл жағдайда, Fabrikam роботты қару үшін өнімге негізделген баға ұсыну жолдарын жасайды және осы баға ұсынысы үшін бір дананың өзіндік құнын арнайы енгізеді.</span><span class="sxs-lookup"><span data-stu-id="25931-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="25931-118">Бұл шығын Trey Robotic Arms стандартты бағасынан өзгеше.</span><span class="sxs-lookup"><span data-stu-id="25931-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>
