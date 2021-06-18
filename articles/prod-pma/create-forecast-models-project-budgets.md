---
title: Жоба бюджеттерінің болжамды үлгілерін жасау
description: Бұл тақырыпта қалған бюджеттер үшін болжамды үлгіні жасау жолы туралы сипатталады.
author: Yowelle
ms.date: 04/24/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 3549b41fce72b44230ab27de081dade15a912266
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006294"
---
# <a name="create-forecast-models-for-project-budgets"></a><span data-ttu-id="e4167-103">Жоба бюджеттерінің болжамды үлгілерін жасау</span><span class="sxs-lookup"><span data-stu-id="e4167-103">Create forecast models for project budgets</span></span> 

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e4167-104">Бұл тақырыпта қалған бюджеттер үшін болжамды үлгіні жасау жолы туралы сипатталады.</span><span class="sxs-lookup"><span data-stu-id="e4167-104">This topic describes how to create a forecast model for remaining budgets.</span></span> <span data-ttu-id="e4167-105">Бюджеттік бақылауға жататын жоба бюджеттің екі түрін пайдаланады: бастапқы және қалдық.</span><span class="sxs-lookup"><span data-stu-id="e4167-105">A project that is subject to budget control uses two types of budgets: original and remaining.</span></span> <span data-ttu-id="e4167-106">Жобаның бюджетін құрған кезде, **Болжамды үлгілер** бетінде жасалған бастапқы және қалған бюджеттік болжамды үлгілерді көрсетуіңіз керек.</span><span class="sxs-lookup"><span data-stu-id="e4167-106">When you create a project budget, you must specify the original and remaining budget forecast models that were created in the **Forecast models** page.</span></span> <span data-ttu-id="e4167-107">Көрсетілген үлгілерге негізделген жоба бюджеттері сіз жоба бюджетін жасаған кезде жасалады.</span><span class="sxs-lookup"><span data-stu-id="e4167-107">Project budgets based on the specified models are created when you commit the project budget.</span></span>

> [!NOTE]
> <span data-ttu-id="e4167-108">Бюджеттік бақылау үшін пайдаланылатын болжамдық үлгіде ішкі үлгі болмайды немесе ішкі үлгі ретінде пайдалануға болмайды.</span><span class="sxs-lookup"><span data-stu-id="e4167-108">A forecast model that is used for budget control can’t have a submodel or be used as a submodel.</span></span>

1. <span data-ttu-id="e4167-109">**Жобаларды басқару және есепке алу** > **Орнату** > **Болжамдар**  > **Болжамды үлгілер** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-109">Select **Project management and accounting** > **Setup** > **Forecasts**  > **Forecast models**.</span></span>
2. <span data-ttu-id="e4167-110">Жаңа болжамды үлгі құру үшін **Жаңа** мәнін таңдаңыз, содан кейін үлгінің идентификатор нөмірін және жаңа үлгі атауын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="e4167-110">Select **New** to create a new forecast model, and then enter a model ID number and name for the new model.</span></span> 
3. <span data-ttu-id="e4167-111">Болжамды үлгі бойынша болжам жолдарының өзгеруіне жол бермеу үшін **Тоқтатылды** опциясын **Иә** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-111">Set the **Stopped** option to **Yes** to prevent any changes to the forecast lines for the forecast model.</span></span> 
4. <span data-ttu-id="e4167-112">Егер үлгімен байланысты болжам жолдары бас кітапта ақша ағындарының болжамдарын құруы керек болса, **Ақша ағыны болжамдарына қосу** пәрменін **Иә** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-112">If the forecast lines that the model is associated with should generate cash flow forecasts in the general ledger, set **Include in Cash flow forecasts** to **Yes.**</span></span> 
5. <span data-ttu-id="e4167-113">Жоба күнін есеп-шот күні ретінде пайдалану үшін **Болжалды есеп-шот күні** пәрменін **Иә** күйіне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-113">To use the project date as the invoice date, set **Forecast Invoice date** to **Yes**.</span></span> 
6. <span data-ttu-id="e4167-114">**Бюджет түрі** өрісінде, келесі үлгі түрлерінің бірін таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="e4167-114">In the **Budget type** field, select one of the following model types:</span></span>

   - <span data-ttu-id="e4167-115">**Бастапқы бюджет**: бастапқы бюджетті құру және бекіту кезінде жасалатын бюджеттің бастапқы сомаларын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-115">**Original budget**: Use the original budget amounts that are committed when the initial budget is created and approved.</span></span>
   - <span data-ttu-id="e4167-116">**Қалған бюджет**: жобаны іске асыру барысында бюджеттің қалған сомаларын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-116">**Remaining budget**: Use the remaining budget amounts during the life of the project.</span></span> <span data-ttu-id="e4167-117">Осы болжамды үлгідегі қалдықтар нақты транзакциялармен азаяды және бюджетті нақтылау кезінде көбейтіледі немесе азаяды.</span><span class="sxs-lookup"><span data-stu-id="e4167-117">The balances in this forecast model are reduced by actual transactions and increased or decreased by budget revisions.</span></span>
   - <span data-ttu-id="e4167-118">**Көшіру**: жоба үшін көшірілген бюджеттің сомаларын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-118">**Carry-forward**: Use the carry-forward budget amounts for the project.</span></span> <span data-ttu-id="e4167-119">Көшіру – бюджеттің пайдаланылмаған сомаларын бір қаржы жылынан екіншісіне аудару үшін жүргізілуі мүмкін қосымша процесс.</span><span class="sxs-lookup"><span data-stu-id="e4167-119">Carry-forward is an optional process that can be run to transfer unused budget amounts from one fiscal year to another.</span></span>

7. <span data-ttu-id="e4167-120">Төмендегі параметрлерді қажетінше орнатыңыз:</span><span class="sxs-lookup"><span data-stu-id="e4167-120">Set the following options as required:</span></span>

   - <span data-ttu-id="e4167-121">Жоба күнін есеп-шот күні ретінде пайдалану үшін **Болжалды есеп-шот күні** пәрменін қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-121">Enable **Forecast invoice date** to use the project date as the invoice date.</span></span>
   - <span data-ttu-id="e4167-122">Орындалып жатқан жұмыс (WIP) негізінде болжам жасау үшін **WIP көмегімен болжау** пәрменін қосыңыз, содан кейін WIP түрін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-122">Enable **Forecast with WIP** to forecast based on work in progress (WIP), and then select the type of WIP.</span></span> 
   - <span data-ttu-id="e4167-123">Әдепкі **Бюджет түрін** **Жоқ** ретінде сақтауға немесе жаңа түрін енгізуге болады.</span><span class="sxs-lookup"><span data-stu-id="e4167-123">You can keep the default **Budget type** as **None** or enter a new type.</span></span> <span data-ttu-id="e4167-124">Жазбаны өзгерткеннен кейін бюджет түрін өзгерту мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="e4167-124">The budget type can't be changed after you change a record.</span></span>     
    > [!NOTE]
    > <span data-ttu-id="e4167-125">Егер сіз әдепкі бюджет түрін өзгертсеңіз, онда барлық басқа опциялар жаңартуға қолжетімді болмайды және сіз осы болжамды үлгіні қайта пайдалана алмайсыз.</span><span class="sxs-lookup"><span data-stu-id="e4167-125">If you change the default budget type, all other options will become unavailable for updates, and you can't reuse this forecast model.</span></span> 
   


 



[!INCLUDE[footer-include](../includes/footer-banner.md)]