---
title: Кезең түрлері
description: Бұл тақырып табыс болжамы үшін кезең түрлерін құру жолдары туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6bcd988fbd074c66d64f7e327b4329d3de27e950
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531479"
---
# <a name="period-types"></a><span data-ttu-id="9bec1-103">Кезең түрлері</span><span class="sxs-lookup"><span data-stu-id="9bec1-103">Period types</span></span>

<span data-ttu-id="9bec1-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="9bec1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="9bec1-105">Кезең түрі жоба бойынша табыстың қаншалықты жиі бағаланатынын анықтайды.</span><span class="sxs-lookup"><span data-stu-id="9bec1-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="9bec1-106">Бұл тақырып табыс болжамы үшін кезең түрлерін құру жолдары туралы ақпарат береді.</span><span class="sxs-lookup"><span data-stu-id="9bec1-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="9bec1-107">Кезең түрлерін жасап, олармен жұмыс істеу</span><span class="sxs-lookup"><span data-stu-id="9bec1-107">Create and work with period types</span></span>
<span data-ttu-id="9bec1-108">Кезең түрлерін құрып, олармен жұмыс істеу үшін келесі қадамдарды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="9bec1-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="9bec1-109">Dynamics 365 Finance ортасында **Жобаларды басқару және есеп** > **Орнату** > **Болжамдар** > **Кезең түрлері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="9bec1-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="9bec1-110">Жаңа кезең түрін жасау үшін **Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9bec1-110">Select **New** to create new period type.</span></span> <span data-ttu-id="9bec1-111">Атауы мен сипаттамасын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="9bec1-111">Enter a name and description.</span></span>
3. <span data-ttu-id="9bec1-112">**Жиілік** өрісінде жаңа мәнді таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="9bec1-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="9bec1-113">**Апта**, **Екі апта сайын**, **Жарты ай сайын**, **Ай**, **Күн**, **Тоқсан** немесе **Жыл** опциясын таңдасаңыз, кезеңдерді құру үшін күнтізбе пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="9bec1-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="9bec1-114">**Кітап кезеңі** опциясын таңдасаңыз, кезеңдерді құру үшін бас кітап конфигурациясындағы кітап кезеңдері пайдаланылатын болады.</span><span class="sxs-lookup"><span data-stu-id="9bec1-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="9bec1-115">**Шексіз** опциясын таңдасаңыз, теңшелетін кезеңдерді көрсетуге болады.</span><span class="sxs-lookup"><span data-stu-id="9bec1-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="9bec1-116">Кезең түрінің жазбасын таңдап, кезең түріне арналған кезеңдерді құру үшін **Кезеңдерді құру** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9bec1-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="9bec1-117">Таңдалған кезең жиілігінің негізінде сізде басталу күнін немесе жасалатын кезеңдер санын көрсету опциясы болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="9bec1-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="9bec1-118">Құрылған кезеңдерге шолу жасау үшін **Кезеңдер** параметрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="9bec1-118">Select **Periods** to review generated periods.</span></span>

