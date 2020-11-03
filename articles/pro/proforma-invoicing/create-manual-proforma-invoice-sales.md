---
title: Проформа-шотын қолмен жасау
description: Бұл тақырыпта Project Operations бағдарламасындағы қолмен жазылатын проформа есеп-шотын жасау туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5e93206737507bf6698a9746815c790d3dfc904
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/20/2020
ms.locfileid: "4079889"
---
# <a name="creating-a-manual-proforma-invoice"></a><span data-ttu-id="8e9f1-103">Проформа-шотын қолмен жасау</span><span class="sxs-lookup"><span data-stu-id="8e9f1-103">Creating a manual proforma invoice</span></span>

<span data-ttu-id="8e9f1-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="8e9f1-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8e9f1-105">Dynamics 365 Project Operations бағдарламасында есепшоттар қажет болған жағдайда қолмен жасалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="8e9f1-106">Проформа есеп-шотын **Жоба келісім-шарттары** тізім беті немесе **Жоба келісім-шарты** мәліметтер бетінен қолмен жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="8e9f1-107">Жоба келісім-шарттарының тізім беті</span><span class="sxs-lookup"><span data-stu-id="8e9f1-107">Project Contracts list page</span></span>

<span data-ttu-id="8e9f1-108">**Жоба келісім-шарттары** тізім бетінен, бір немесе бірнеше жоба келісімшарттарын таңдаңыз және барлық таңдалған жазбалар үшін есеп-шоттар жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="8e9f1-109">Жүйе таңдалған жоба келісім-шарттарының қайсысында бүгінгі күнге дейін жасалған **Есеп-шотқа дайын** тапсырыс барын тексереді.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="8e9f1-110">Осы келісім-шарттардан жүйе жобалық проформа есеп-шоттарын жасайды.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="8e9f1-111">Егер жоба келісім-шартында бірнеше тұтынушы болса, онда бір тұтынушыға бір есеп-шот және бір жоба келісім-шартына бірнеше есеп-шот жасалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="8e9f1-112">Барлық жасалған жоба есеп-шоттары **Сатылым** аймағының **Төлем жасау** бөліміндегі **Есеп-шот** бетінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="8e9f1-113">Жоба келісім-шарты мәліметтерінің беті</span><span class="sxs-lookup"><span data-stu-id="8e9f1-113">Project Contract details page</span></span>

<span data-ttu-id="8e9f1-114">Проформа есеп-шотын **Жоба келісім-шарты** мәліметтер бетінен жасауға болады, ол нақты жоба келісім-шартына есеп-шот жасайды.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="8e9f1-115">Жүйе жоба келісім-шартында бүгінгі күнге дейін жасалған **Есеп-шотқа дайын** тапсырыс болуын тексереді.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="8e9f1-116">Осы келісім-шарттардан, жүйе әр келісім-шарт жолы бойынша тұтынушылар санына негізделген жобалық проформа есеп-шоттарын жасайды.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="8e9f1-117">Бір проформа есеп-шоты жасалған кезде, **Есеп-шот** беті ашылады.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="8e9f1-118">Егер сол жоба келісім-шарты үшін бірнеше есеп-шот жасалған болса, онда **Есеп-шоттар** тізім беті барлық жасалған есеп-шоттарды көрсету үшін ашылады.</span><span class="sxs-lookup"><span data-stu-id="8e9f1-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
