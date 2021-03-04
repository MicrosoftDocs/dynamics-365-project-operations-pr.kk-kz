---
title: Проформа-шотын қолмен жасау - жеңілдетілген
description: Бұл тақырыпта Project Operations бағдарламасындағы қолмен жазылатын проформа есеп-шотын жасау туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5a924de6efc377e28a20e038e7deac04616b95aa
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764510"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="5c27d-103">Проформа-шотын қолмен жасау - жеңілдетілген</span><span class="sxs-lookup"><span data-stu-id="5c27d-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="5c27d-104">_**Қолданылады:** қарапайым орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="5c27d-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5c27d-105">Dynamics 365 Project Operations бағдарламасында проформа-шоттарын қажетінше қолмен жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="5c27d-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="5c27d-106">Проформа есеп-шотын **Жоба келісім-шарттары** тізім беті немесе **Жоба келісім-шарты** мәліметтер бетінен қолмен жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="5c27d-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="5c27d-107">Жоба келісім-шарттарының тізім беті</span><span class="sxs-lookup"><span data-stu-id="5c27d-107">Project Contracts list page</span></span>

<span data-ttu-id="5c27d-108">**Жоба келісім-шарттары** тізім бетінен, бір немесе бірнеше жоба келісімшарттарын таңдаңыз және барлық таңдалған жазбалар үшін есеп-шоттар жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="5c27d-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="5c27d-109">Жүйе таңдалған жоба келісімшарттарының қайсысында бүгінгі күнге дейін орындалмаған **Есеп-шотқа дайын** әрекеттерінің барын тексереді.</span><span class="sxs-lookup"><span data-stu-id="5c27d-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="5c27d-110">Осы келісім-шарттардан жүйе жобалық проформа есеп-шоттарын жасайды.</span><span class="sxs-lookup"><span data-stu-id="5c27d-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="5c27d-111">Егер жоба келісім-шартында бірнеше тұтынушы болса, онда бір тұтынушыға бір есеп-шот және бір жоба келісім-шартына бірнеше есеп-шот жасалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="5c27d-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="5c27d-112">Барлық жасалған жоба есеп-шоттары **Сатылым** аймағының **Төлем жасау** бөліміндегі **Есеп-шот** бетінде қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="5c27d-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="5c27d-113">Жоба келісім-шарты мәліметтерінің беті</span><span class="sxs-lookup"><span data-stu-id="5c27d-113">Project Contract details page</span></span>

<span data-ttu-id="5c27d-114">Сондай-ақ профома-шоты **Жобалық келісімшарт** мәліметтер бетінде жасалады.</span><span class="sxs-lookup"><span data-stu-id="5c27d-114">A proforma invoice can also be created from the **Project Contract** details page.</span></span> <span data-ttu-id="5c27d-115">Жүйе таңдалған жоба келісімшартының бүгінгі күнге дейін орындалмаған **Есеп-шотқа дайын** әрекеттерінің барын тексереді.</span><span class="sxs-lookup"><span data-stu-id="5c27d-115">The system verifies the project contract has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="5c27d-116">Осы келісім-шарттардан, жүйе әр келісім-шарт жолы бойынша тұтынушылар санына негізделген жобалық проформа есеп-шоттарын жасайды.</span><span class="sxs-lookup"><span data-stu-id="5c27d-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="5c27d-117">Бір проформа есеп-шоты жасалған кезде, **Есеп-шот** беті ашылады.</span><span class="sxs-lookup"><span data-stu-id="5c27d-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="5c27d-118">Егер осы жоба келісімшартына бірнеше есеп-шоттар жасалса, онда **Есеп-шоттар** тізім беті барлық жасалған есеп-шоттарды көрсету үшін ашылады.</span><span class="sxs-lookup"><span data-stu-id="5c27d-118">If multiple invoices are created for that project contract, the **Invoices** list page opens to show all of the created invoices.</span></span>
