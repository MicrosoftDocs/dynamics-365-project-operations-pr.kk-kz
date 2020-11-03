---
title: Ресурс күнтізбелерін анықтау
description: Бұл тақырыпта Project Operations бағдарламасындағы ресурстарға арналған жұмыс сағатының күнтізбелерін анықтау жолы туралы ақпарат берілген.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ab39d7e5dc2d8c01ed49ca0f1a4d1691aaf15637
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079508"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="93675-103">Ресурс күнтізбелерін анықтау</span><span class="sxs-lookup"><span data-stu-id="93675-103">Define resource calendars</span></span>

<span data-ttu-id="93675-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="93675-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="93675-105">Жобада жұмыс жасайтын әр тіркелетін ресурс олардың қолжетімділігін анықтау үшін жұмыс сағатының күнтізбесі болуы керек.</span><span class="sxs-lookup"><span data-stu-id="93675-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="93675-106">Ресурстың жұмыс сағатын екі жолмен анықтауға болады:</span><span class="sxs-lookup"><span data-stu-id="93675-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="93675-107">Ресурс үшін жеке күнтізбелік ережелерді анықтау</span><span class="sxs-lookup"><span data-stu-id="93675-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="93675-108">Ресурс үшін бұрыннан бар күнтізбе үлгісін қолданыңыз</span><span class="sxs-lookup"><span data-stu-id="93675-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="93675-109">Ресурстың жұмыс сағаттарын анықтау</span><span class="sxs-lookup"><span data-stu-id="93675-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="93675-110">**Ресурстар** мәзірінде **Ресурстар** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="93675-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="93675-111">Тор көрінісінен сәйкес **Тіркелетін ресурс** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="93675-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="93675-112">**Ресурс туралы мәліметтер** бетінде **Жұмыс сағаттары** қойыншасын таңдаңыз. Әдепкі бойынша, тіркелетін ресурстар күнтізбесі ұйым үшін анықталған әдепкі жұмыс сағаты үлгісінің жұмыс сағаттарына сәйкес келеді.</span><span class="sxs-lookup"><span data-stu-id="93675-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="93675-113">Жұмыс сағаттарын жаңарту үшін анықталатын ұсынылған күнтізбелік ереженің басталу күнін тінтуірдің оң жағымен басыңыз.</span><span class="sxs-lookup"><span data-stu-id="93675-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="93675-114">Күнтізбелік ережелер мәзірін белгілі бір күн, қатар қалдығы немесе бүкіл күнтізбеге арналған күнтізбе ережесін анықтау үшін пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="93675-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="93675-115">Опция таңдалғаннан кейін, мынаны анықтауға болады:</span><span class="sxs-lookup"><span data-stu-id="93675-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="93675-116">Жұмыс сағаты қолданатын аптаның күні.</span><span class="sxs-lookup"><span data-stu-id="93675-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="93675-117">Әр күн ішіндегі жұмыс уақыттары.</span><span class="sxs-lookup"><span data-stu-id="93675-117">The working times within each day.</span></span>
    - <span data-ttu-id="93675-118">Күнтізбе ережесіне арналған уақыт аумағы.</span><span class="sxs-lookup"><span data-stu-id="93675-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="93675-119">Қажет болса, жұмыс істемейтін уақытты ережеге сәйкес анықтауға болады.</span><span class="sxs-lookup"><span data-stu-id="93675-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="93675-120">Күнтізбе үлгісін ресурсқа қолдану</span><span class="sxs-lookup"><span data-stu-id="93675-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="93675-121">**Ресурстар** мәзірінде **Ресурстар** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="93675-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="93675-122">Тор көрінісінен жаңарту үшін 25 **Тіркелетін ресурстар** дейін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="93675-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="93675-123">**Күнтізбе орнату** таңдаңыз және диалогтік терезе жұмыс сағатының қолжетімді үлгілерінің тізімін ұсынады.</span><span class="sxs-lookup"><span data-stu-id="93675-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="93675-124">Пайдалану керек үлгіні таңдап, **Қолдану** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="93675-124">Select the template you want to use, and then select **Apply**.</span></span>
