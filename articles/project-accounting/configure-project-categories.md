---
title: Жоба санаттарын конфигурациялау
description: Бұл бөлімде жоба санаттарын орнату туралы ақпарат берілген.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b7adf61a82714a0148d9c8b1d2b2b37fd611c1cf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287515"
---
# <a name="configure-project-categories"></a><span data-ttu-id="9b1be-103">Жоба санаттарын конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="9b1be-103">Configure project categories</span></span>

<span data-ttu-id="9b1be-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="9b1be-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="9b1be-105">Project Operations жобалар бойынша кірістер мен шығыстарды санаттаудың мықты мүмкіндіктерін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-105">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="9b1be-106">Санаттар жоба транзакциялары туралы есеп беру және талдау және жалпы тіркелімге хабарламалар жіберу мүмкіндігін қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="9b1be-106">Categories provide the ability to report on and analyze project transactions, and drive posting to the general ledger.</span></span>

<span data-ttu-id="9b1be-107">Келесі диаграмма транзакция санаттары, ортақ санаттар және жоба санаттары арасындағы өзара қатынасты көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="9b1be-107">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span> 

<span data-ttu-id="9b1be-108">Транзакция санаттары - жоба транзакциялары үшін негізгі топтау.</span><span class="sxs-lookup"><span data-stu-id="9b1be-108">Transaction categories are the basic grouping for project transactions.</span></span> <span data-ttu-id="9b1be-109">Бұл топта бағдарламалар мен модульдер бойынша ортақ пайдалануға болатын ортақ санаттар жиынтығы бар.</span><span class="sxs-lookup"><span data-stu-id="9b1be-109">Within that grouping, there is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="9b1be-110">Ерекшеліктерге жету үшін жоба санаттары санаттардың толық мәліметті деңгейі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-110">Getting even further into specifics, project categories are the most granular level of categories.</span></span> <span data-ttu-id="9b1be-111">Жоба санаттары заңды нысанға, модульге және бағдарламаға тән.</span><span class="sxs-lookup"><span data-stu-id="9b1be-111">Project categories are specific to legal entity, module, and application.</span></span>

![Транзакция санаттары, ортақ санаттар және жоба санаттары арасындағы өзара қатынас](media/project-categories.png)

## <a name="transaction-categories"></a><span data-ttu-id="9b1be-113">Транзакция санаттары</span><span class="sxs-lookup"><span data-stu-id="9b1be-113">Transaction categories</span></span>

<span data-ttu-id="9b1be-114">Транзакция санаттары жоба транзакцияларына арналған негізгі топ компанияға немесе транзакция түріне тән емес екенін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="9b1be-114">Transaction categories represent the basic grouping for project transactions and are not company or transaction type-specific.</span></span> <span data-ttu-id="9b1be-115">Мысалы, Contoso Robotics жоба транзакцияларын топтастыру үшін құрылым, сапар, орнату және қызмет транзакциясы санаттарын қолданады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-115">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group Project transactions.</span></span>

<span data-ttu-id="9b1be-116">Транзакция санаттары Project Operations модулінде анықталады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-116">Transaction categories are defined in the Project Operations module.</span></span> 
1. <span data-ttu-id="9b1be-117">Пішінді ашу үшін **Параметрлер** \> **Транзакция санаттары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="9b1be-117">Go to **Settings** \> **Transaction Categories** to open the form.</span></span> 
2. <span data-ttu-id="9b1be-118">Жаңа транзакция санатын не **Жаңа** пәрменін таңдау арқылы немесе **Excel бағдарламасынан импорттау** пәрменін таңдау арқылы жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b1be-118">Create a new transaction category either by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="9b1be-119">Ортақ санаттар</span><span class="sxs-lookup"><span data-stu-id="9b1be-119">Shared categories</span></span>

<span data-ttu-id="9b1be-120">Dynamics 365 Finance, Dynamics 365 Supply Chain және Dynamics 365 Project Operations сияқты түрлі бағдарламаларда шығыстарды санаттарға бөлу үшін Dynamics 365 ортақ пайдаланылатын санаттар тұжырымдамасын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-120">Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as Dynamics 365 Finance, Dynamics 365 Supply Chain, and Dynamics 365 Project Operations.</span></span> <span data-ttu-id="9b1be-121">Әрбір жасалған транзакция санаты үшін Project Operations автоматты түрде қатысты төрт санатты жасайды: сағат, шығыс, алымдар және элемент.</span><span class="sxs-lookup"><span data-stu-id="9b1be-121">For each Transaction category created, Project Operations automatically creates four related Shared categories: Hours, Expense, Fees, and Item.</span></span> <span data-ttu-id="9b1be-122">**Жобаларды басқару және есептеу** \> **Орнату** \> **Санаттар** \>**Ортақ санаттар** тармағына өту арқылы ортақ санаттарды қарап шығуға және реттеуге болады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-122">You can review and adjust the shared categories by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="9b1be-123">Жоба санаттары</span><span class="sxs-lookup"><span data-stu-id="9b1be-123">Project categories</span></span>

<span data-ttu-id="9b1be-124">Жоба санаттары санат конфигурациясының толық мәліметті деңгейін білдіреді және оларды әр компания үшін бөлек жоба есепшісі конфигурациялауы керек.</span><span class="sxs-lookup"><span data-stu-id="9b1be-124">Project categories represent most granular level of category configuration and must be configured separately, and for each company, by a Project accountant.</span></span>

1. <span data-ttu-id="9b1be-125">**Жобаларды басқару және есепке алу** \> **Орнату** \> **Санаттар** \> **Жоба санаттары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="9b1be-125">Go to **Project Management and Accounting** \> **Setup** \> **Categories** \> **Project categories**.</span></span>
2. <span data-ttu-id="9b1be-126">**Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b1be-126">Select **New**.</span></span>
3. <span data-ttu-id="9b1be-127">Алдыңғы бөлімде жасалған ортақ санаттың **Санат идентификаторын** таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b1be-127">Select the **Category ID** of the Shared category you created in the previous section.</span></span> <span data-ttu-id="9b1be-128">Project Operations тек транзакция санаттарымен байланысты ортақ санаттарды пайдалануға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="9b1be-128">Project Operations allows using only those shared categories that are associated with transaction categories.</span></span>
4. <span data-ttu-id="9b1be-129">Санат тобын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9b1be-129">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="9b1be-130">Санат топтары</span><span class="sxs-lookup"><span data-stu-id="9b1be-130">Category groups</span></span>

<span data-ttu-id="9b1be-131">Санаттар топтары сипаттарды, бірінші кезекте профильдерді орналастыруды, қатысты жоба санаттары арасында ортақ пайдалану үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-131">Category groups are used to share properties, primarily posting profiles, between related Project categories.</span></span> <span data-ttu-id="9b1be-132">Әр транзакция түрі үшін кемінде бір санат тобы болуы керек және әр жоба санатына топ тағайындалады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-132">There must be at least one category group for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="9b1be-133">Project Operations бағдарламасында орналастыру сипаттамалары жоба құны мен кіріс профилі ережелерімен, жоба санаттарымен және санат топтарымен анықталады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-133">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="9b1be-134">**Жобаларды басқару және есепке алу** \> **Орнату** \> **Санаттар** \> **Санат топтары** тармағына өту арқылы санат топтарын орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="9b1be-134">You can set up category groups by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Category groups**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]