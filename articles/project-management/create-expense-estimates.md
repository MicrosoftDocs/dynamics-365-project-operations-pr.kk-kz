---
title: Шығыс болжамдары
description: Бұл тақырыпта жобаға негізделген шығыстарды анықтау немесе бағалау туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 10872366453985561bda0c07e50cff7f5f6d333e
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131710"
---
# <a name="expense-estimates"></a><span data-ttu-id="3f061-103">Шығыс болжамдары</span><span class="sxs-lookup"><span data-stu-id="3f061-103">Expense estimates</span></span>
<span data-ttu-id="3f061-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="3f061-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3f061-105">Ресурсқа негізделген болжамдарды анықтаумен қатар, Dynamics 365 Project Operations жоба менеджерлеріне әр жоба бойынша жобаға негізделген шығыстарды анықтауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="3f061-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="3f061-106">Әрбір шығыстарды белгілі бір жоба тапсырмасымен немесе шығыстар санатымен байланыстыруға болады.</span><span class="sxs-lookup"><span data-stu-id="3f061-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="3f061-107">Шығыс санаттары әдетте ұйымдық деңгейде анықталады.</span><span class="sxs-lookup"><span data-stu-id="3f061-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="3f061-108">Әр шығыс санаты үшін баға келесі иерархияда анықталады:</span><span class="sxs-lookup"><span data-stu-id="3f061-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="3f061-109">ұйым</span><span class="sxs-lookup"><span data-stu-id="3f061-109">Organization</span></span>
- <span data-ttu-id="3f061-110">Тұтынушы</span><span class="sxs-lookup"><span data-stu-id="3f061-110">Customer</span></span>
- <span data-ttu-id="3f061-111">Баға ұсыну/келісім-шарт</span><span class="sxs-lookup"><span data-stu-id="3f061-111">Quote/contract</span></span>

<span data-ttu-id="3f061-112">Жоба шығындарын қарау, қосу немесе жою үшін келесі қадамдарды орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="3f061-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="3f061-113">**Жобалар** бөліміне өтіп, жұмыс жасау керек жобаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3f061-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="3f061-114">**Жоба болжамдары** қойыншасын таңдап, жоба шығындарының тізімін қараңыз.</span><span class="sxs-lookup"><span data-stu-id="3f061-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="3f061-115">Шығыс қосу үшін **Жаңа шығыс** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3f061-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="3f061-116">Болмаса жою үшін шығысты таңдап, содан кейін **Шығысты жою** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="3f061-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="3f061-117">Әр шығыс бабының элементі үшін келесі төлсипаттар анықталған:</span><span class="sxs-lookup"><span data-stu-id="3f061-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="3f061-118">**Санат**: жобаға жұмсалған барлық шығыстарды сипаттау үшін пайдаланылатын жалпы топтар.</span><span class="sxs-lookup"><span data-stu-id="3f061-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="3f061-119">**Басталу күні** : шығыстың шығуы болжанатын күн.</span><span class="sxs-lookup"><span data-stu-id="3f061-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="3f061-120">**Саны**: белгілі бір санат бойынша шығыс элементтерінің болжамды саны.</span><span class="sxs-lookup"><span data-stu-id="3f061-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="3f061-121">**Бірлік шығыны**: шығыстың өзіндік құнын есептеу үшін пайдаланылатын бірлік бағасы.</span><span class="sxs-lookup"><span data-stu-id="3f061-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="3f061-122">**Бірліктің сатылым бағасы**: шығыстың сатылым бағаларын есептеу үшін пайдаланылатын бірлік бағасы.</span><span class="sxs-lookup"><span data-stu-id="3f061-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>

