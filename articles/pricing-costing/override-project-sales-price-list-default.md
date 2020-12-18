---
title: Жоба сатылымдарының бағатізбелерін алдын ала анықтау
description: Бұл тақырыпта реттелетін сатылым бағатізбелерін жасау туралы ақпарат беріледі.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: af9baca540d89f4e5e616bdfdd6111bef29abe28
ms.sourcegitcommit: 656a9d03f260c29e988e2ff05b6e07ae0365d6d0
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "4672238"
---
# <a name="override-project-sales-price-lists"></a><span data-ttu-id="d4200-103">Жоба сатылымдарының бағатізбелерін алдын ала анықтау</span><span class="sxs-lookup"><span data-stu-id="d4200-103">Override project sales price lists</span></span>

<span data-ttu-id="d4200-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="d4200-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="customer-specific-project-price-lists"></a><span data-ttu-id="d4200-105">Тұтынушыларға арналған жоба бағатізбелері</span><span class="sxs-lookup"><span data-stu-id="d4200-105">Customer-specific project price lists</span></span>

<span data-ttu-id="d4200-106">Тұтынушыларға арналған бағалық келісімдерді Dynamics 365 Project Operations жүйесіндегі шот жазбасында жобаның бағатізбесі ретінде орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="d4200-106">Customer-specific price agreements can be set up as project price lists on an account record in Dynamics 365 Project Operations.</span></span>

<span data-ttu-id="d4200-107">Тұтынушыларға арналған жоба бағатізбесін жасау үшін **Сатылым** аймағында шот жазбасына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="d4200-107">To set up a customer-specific project price list, in the **Sales** area, navigate to the account record.</span></span>

1. <span data-ttu-id="d4200-108">**Шоттар** тізім бетін ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-108">Open the **Accounts** list page.</span></span>
2. <span data-ttu-id="d4200-109">**Шот** мәліметтер бетін ашу үшін тұтынушы жазбасын тауып, екі рет шертіңіз.</span><span class="sxs-lookup"><span data-stu-id="d4200-109">Locate and double-click a customer record to open the **Account** details page.</span></span>
3. <span data-ttu-id="d4200-110">**Жобаның бағатізбелері** қойыншасында **+ Жаңа жобалық бағатізбе** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-110">On the **Project Price lists** tab, select **+ New Project Price List**.</span></span>
4. <span data-ttu-id="d4200-111">**Жаңа жобалық бағатізбе** бетінде ашылмалы тізімнен бағатізбені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-111">On the **New Project Price List** page, select a price list from the drop-down.</span></span> <span data-ttu-id="d4200-112">Тек контексті **Сатылым** күйіне орнатылған және валютасы шот валютасына сәйкес келетін бағатізбелер қосылады.</span><span class="sxs-lookup"><span data-stu-id="d4200-112">Only price lists that have the context set to **Sales** and whose currency matches the account currency are included.</span></span>
5. <span data-ttu-id="d4200-113">Байланыс атауын енгізіп, содан соң **Сақтау** түймешігін басыңыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-113">Name the association, and then select **Save**.</span></span> <span data-ttu-id="d4200-114">Тұтынушыларға арналған жоба бағатізбесі жасалды.</span><span class="sxs-lookup"><span data-stu-id="d4200-114">A customer-specific project price list is created.</span></span> <span data-ttu-id="d4200-115">Бұл бағатізбе баға ұсынысының немесе жобалық келісім-шарттың жасалған күні бағатізбенің күшіне ену күніне сәйкес келетін, тұтынушы үшін жасалған жобалық баға ұсыныстары мен келісім-шарттардағы әдепкі жобаға пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="d4200-115">This price list will be used to default project prices on project quotes or contracts created for this customer where the created date of the quote or project contract falls within the date effectivity of the price list.</span></span>

## <a name="custom-pricing-on-project-quotes"></a><span data-ttu-id="d4200-116">Жоба баға ұсыныстарындағы реттелетін баға белгілеу</span><span class="sxs-lookup"><span data-stu-id="d4200-116">Custom pricing on project quotes</span></span>

<span data-ttu-id="d4200-117">Жобалық баға ұсыныстарында тұтынушыдан немесе жобалық параметрлерден әдепкі бойынша алынатын әдепкі стандартты бағатізбеден басталатын жобалық бағаға ие боласыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-117">On project quotes, you can have project pricing that starts with a default standard price list that defaults from the customer or from the project parameters.</span></span>

<span data-ttu-id="d4200-118">Белгілі бір баға ұсынысы бойынша жобамен байланысты жұмыс үшін реттелетін баға белгілеу қажет болғанда, сіз оны жобалық бағатізбелермен байланысты нысаннан ала аласыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-118">When you need custom pricing for project-related work on a particular quote, you can get that from the project price lists associated entity.</span></span>

<span data-ttu-id="d4200-119">Баға ұсынысына арналған жобалық баға белгілеуді орнату үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-119">Complete the following steps to set up quote-specific project pricing.</span></span>

1. <span data-ttu-id="d4200-120">Жобалық баға ұсынысын ашып, **Жобаның бағатізбелері** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-120">Open the project quote and select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="d4200-121">Ішкі торда **Реттелетін баға жасау** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-121">In the subgrid, select **Create custom pricing**.</span></span>

<span data-ttu-id="d4200-122">Баға ұсынысына тіркелген жобаның барлық бағатізбелері жаңа бағатізбелерге көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="d4200-122">All the project price lists that are attached to the quote are copied to new price lists.</span></span> <span data-ttu-id="d4200-123">Жаңа бағатізбелер атаулары осы бағатізбелер жасалған кездегі күні мен уақыты көрсетілген баға ұсынысының атауын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="d4200-123">The names of the new price lists reflect the name of quote with a date-time stamp for when these price lists were created.</span></span>

<span data-ttu-id="d4200-124">Сіз осы бағатізбелердің әрқайсысын пайдалана аласыз, сондай-ақ еңбек (рөл бағасы) және шығындар (санат бағасы) бағаларына жаңартулар енгізе аласыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-124">You can use each of those price lists and make updates to labor (role price) and expense (category price) prices.</span></span> <span data-ttu-id="d4200-125">Бұл бағалар тек осы баға ұсыныстарына қолданылатын болады.</span><span class="sxs-lookup"><span data-stu-id="d4200-125">These prices will only be applicable to this project quote.</span></span>

## <a name="price-lists-on-a-project-contract"></a><span data-ttu-id="d4200-126">Жоба келісім-шартындағы бағатізбелер</span><span class="sxs-lookup"><span data-stu-id="d4200-126">Price lists on a project contract</span></span>

<span data-ttu-id="d4200-127">Жобалық келісім-шартта жоба бағасы келісім-шарт атауы мен атауға қосылатын жасалған күн уақыты белгісімен әрдайым реттелетін бағатізбе ретінде әдепкі мән ретінде алынады.</span><span class="sxs-lookup"><span data-stu-id="d4200-127">On a project contract, project pricing always defaults as a custom price list with the name of contract and the created date time stamp appended to the name.</span></span> <span data-ttu-id="d4200-128">Бұл келісім-шарт баға ұсынысы ұтқан кезде жасалуына немесе келісім-шарттың нөлден жасалуына тәуелсіз түрде рас болып табылады.</span><span class="sxs-lookup"><span data-stu-id="d4200-128">This is true whether the contract was created when the quote was won or if the contract was created from scratch.</span></span> <span data-ttu-id="d4200-129">Қажет болса, бұл байланысты реттелетін бағатізбемен алып тастай аласыз және оның орнына стандартты бағатізбені жоба келісім-шартымен байланыстыра аласыз.</span><span class="sxs-lookup"><span data-stu-id="d4200-129">If needed, you can remove this association to the custom price list and associate a standard price list to the project contract instead.</span></span>

<span data-ttu-id="d4200-130">Стандартты бағатізбені баға ұсынысы немесе келісім-шарттағы жобаның бағатізбелерге байланыстырған кезде, бағатізбедегі бағалардағы кез келген өзгертулер бағатізбені пайдаланатын барлық баға ұсыныстарына және келісім-шарттарға әсер етеді.</span><span class="sxs-lookup"><span data-stu-id="d4200-130">When you associate a standard price list to the project price lists on quote or contract, any changes made to the prices in the price list will impact all quotes and contracts that use the price list.</span></span>
