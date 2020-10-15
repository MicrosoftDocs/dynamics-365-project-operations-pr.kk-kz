---
title: Тәуліктік
description: Бұл тақырыпта шығысты басқаруда пайдаланылатын тәуліктік ережелер туралы ақпарат берілген.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 7d1c4ac7781cb711e2cc0d09606d422b4dd554f3
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908322"
---
# <a name="per-diems"></a><span data-ttu-id="8b1d6-103">Тәуліктік</span><span class="sxs-lookup"><span data-stu-id="8b1d6-103">Per diems</span></span>

<span data-ttu-id="8b1d6-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="8b1d6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="8b1d6-105">Тәулік - бұл жұмыс орнына бара жатқан жұмысшыға төленетін жәрдемақы.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-105">A per diem is an allowance that is paid to a worker who is traveling for work.</span></span> <span data-ttu-id="8b1d6-106">Шығысты басқаруда әр түрлі сапар жағдайлары үшін тәуліктік ережелерді жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-106">In Expense management, you can create per diem rules for  various travel situations.</span></span> <span data-ttu-id="8b1d6-107">Тәуліктік тарифтер жылдың уақытына, сапар орнына немесе екеуіне де байланысты болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-107">Per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="8b1d6-108">Тәуліктік ережені жасаған кезде, жұмысшы тегін тамақтанса немесе қызмет алса, тәуліктік тарифтің пайыздық мөлшерінің ұсталатынын көрсетуге болады.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-108">When you create a per diem  rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="8b1d6-109">Сонымен қатар жұмысшылардың сапарына қолданылатын тәуліктік тарифтің минималды және максималды сағаттарын орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-109">You can also set a minimum and maximum number of hours that the per diem rate can apply to a worker's travel.</span></span>

## <a name="configuration"></a><span data-ttu-id="8b1d6-110">Теңшелім</span><span class="sxs-lookup"><span data-stu-id="8b1d6-110">Configuration</span></span> 

1. <span data-ttu-id="8b1d6-111">Тәуліктік орындарды қосу үшін **Орнату** > **Есептеулер мен кодтар** > **Тәуліктік орындар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-111">To add per diem locations, go to **Set up** > **Calculations and codes** > **Per diem locations**.</span></span>
2. <span data-ttu-id="8b1d6-112">Жоғарыда қосылған орындардың әрқайсысы үшін белгілі бір басталу мен аяқталу күні арасында қонақ үйге, тамақтануға және басқа шығындарға жарамды тәуліктік тариф мен валютаны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-112">For each of the locations added above, select a per diem rate and currency that is valid between a specific start and end date for hotel, meals, and other expenses.</span></span> <span data-ttu-id="8b1d6-113">Тәуліктік тарифтер мен валюталарды **Орнату** > **Есептеулер мен кодтар** > **Тәуліктік** тармағында конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-113">Per diem rates and currencies are configured under **Set up** > **Calculations and codes** > **Per diems**.</span></span>
3. <span data-ttu-id="8b1d6-114">**Тәуліктік орындар** бетінде тәуліктік тариф деңгейлерін конфигурациялаңыз.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-114">On the **Per diem locations** page, configure per diem rate tiers.</span></span> <span data-ttu-id="8b1d6-115">Тәуліктік тариф деңгейлері қонақ үйге, тамақтануға және басқа шығыстарға күнделікті жәрдемақының пайыздық бөлінуін анықтауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-115">Per diem rate tiers allow you to define the percentage split of a daily allowance for hotel, meal, and other expenses.</span></span> 
4. <span data-ttu-id="8b1d6-116">Таңертеңгілік, түскі немесе кешкі ас кезінде тамақтану пайызының төмендеуін көрсету үшін **Шығысты басқару параметрлері** бетіндегі **Тәуліктік** қойыншасында өрістерді жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-116">To specify the meal percentage reduction for breakfast, lunch, or dinner, update the fields on the **Expense management parameters** page on the **Per diem** tab.</span></span> 
    
## <a name="submit-expenses-using-per-diem"></a><span data-ttu-id="8b1d6-117">Тәуліктік тарифті пайдаланып шығыстарды жіберу</span><span class="sxs-lookup"><span data-stu-id="8b1d6-117">Submit expenses using per diem</span></span>
<span data-ttu-id="8b1d6-118">Бір тәуліктік шығыстарды жіберу үшін шығыс туралы есепті жасаған кезде **Тәуліктік** шығыс санатын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-118">To submit expenses utilizing per diems, use the **Per diem** expense category when you create an expense report.</span></span> <span data-ttu-id="8b1d6-119">**Күнінен бастап алынған тәуліктік тариф**, **Бүгінгі күнге дейінгі тәуліктік тариф** және **Тәуліктік орын** енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-119">Enter the **Per diem from date**, **Per diem to date**,  and the **Per diem location**.</span></span> <span data-ttu-id="8b1d6-120">Бұл сома таңдалған орын үшін тәуліктік тарифтер негізінде есептеледі, ал тамақтануды төмендету тәуліктік тариф деңгейлері бойынша есептеледі.</span><span class="sxs-lookup"><span data-stu-id="8b1d6-120">The amount will be calculated based on the per diem rates for the selected location and meal reduction will be calculated based on the per diem rate tiers.</span></span>
