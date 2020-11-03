---
title: Жеткізушінің төлемін сақтау шарттарын жасау және қолдану
description: Бұл тақырыпта жеткізушілердің төлемдерін сақтау шарттарын белгілеу және сақтау жолдары туралы ақпарат берілген.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
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
ms.openlocfilehash: 1970a24a5073de6af43db1f1c068332c9ba9c8fe
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079797"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a><span data-ttu-id="ea5fa-103">Жеткізушінің төлемін сақтау шарттарын жасау және қолдану</span><span class="sxs-lookup"><span data-stu-id="ea5fa-103">Create and apply vendor payment retention terms</span></span>

[!include [banner](../includes/banner.md)] 

<span data-ttu-id="ea5fa-104">Жоба үшін сатушының төлемін сақтау мерзімдерін белгілеу сіздің ұйымыңыз жеткізушіге төленген төлемдердің бір бөлігін сақтап қалғысы келгенде пайдалы.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-104">Setting up vendor payment retention terms for a project is useful when your organization wants to retain part of the payments made to a vendor.</span></span> <span data-ttu-id="ea5fa-105">Мысалы, жеткізушіге жеткізілген өнім сіздің күткеніңізге дейін төлем жасау керек болғанда.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-105">For example, when you want to hold payment to a vendor until the products delivered meet your expectations.</span></span> <span data-ttu-id="ea5fa-106">Сатушы төлемін сақтау шарттары сатушы келісім-шартымен келісілген кезде анықталуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-106">Vendor payment retention terms can be specified when you negotiate a vendor contract.</span></span>

## <a name="create-vendor-payment-retention-terms"></a><span data-ttu-id="ea5fa-107">Сатушы төлемін сақтау шарттарын жасау</span><span class="sxs-lookup"><span data-stu-id="ea5fa-107">Create vendor payment retention terms</span></span>

<span data-ttu-id="ea5fa-108">Сіз сатушының сақтау үшін төлем пайызын және шығарылатын бұрын сақталған сомалардың пайызын енгізе аласыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-108">You can enter the percentage of vendor payment for retention and the percentage of the previously retained amounts to be released.</span></span> <span data-ttu-id="ea5fa-109">Сомалар сатушы есеп-шоттарында келісім-шарт белгіленген аяқталу кезеңіне жеткенге дейін сақталады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-109">Amounts are automatically retained on vendor invoices until the contract reaches the specified state of completion.</span></span> <span data-ttu-id="ea5fa-110">Сақтау шарттарын орнатқаннан кейін, оларды сатушыға арналған кез келген жобаға қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-110">After you set up the retention terms, you can apply them to any project for that vendor.</span></span>

<span data-ttu-id="ea5fa-111">Сатушы төлемдерін сақтау шарттарын орнату және сақтау үшін келесі қадамдарды пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-111">Use the following steps to set up and maintain retention terms for vendor payments.</span></span> 

1. <span data-ttu-id="ea5fa-112">**Жобаларды басқару және есепке алу** > **Сақтау** > **Сатушының төлемін сақтау шарттары** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-112">Go to **Project management and accounting** > **Retention** > **Vendor payment retention terms**.</span></span>
2. <span data-ttu-id="ea5fa-113">Сатушының жаңа сақтау шартын қосу үшін **Жаңа** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-113">Select **New** to add a new vendor retention term.</span></span> <span data-ttu-id="ea5fa-114">Жаңа шартқа арналған **Ереже идентификаторы** мәні автоматты түрде енгізіледі.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-114">The **Rule ID** value for the new term is automatically entered.</span></span> 
3. <span data-ttu-id="ea5fa-115">**Сипаттама** өрісіне қысқаша сипаттама енгізіп, **Шарттар** FastTab қойыншасында келесі үшін шарт мәндерін енгізу үшін **Жол қосу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-115">Enter a brief description in the **Description** field, and on the **Terms** FastTab, select **Add line** to enter term values for the following:</span></span>

   - <span data-ttu-id="ea5fa-116">**Жеткізілген бірліктер пайызы** : шарттың аяқталу пайызын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-116">**Percentage of units delivered** : Enter a percentage of completion for the term.</span></span> <span data-ttu-id="ea5fa-117">Сомалар сатушы есеп-шоттарында жобаның аяқталу кезеңі белгіленген пайызға тең болғанға дейін сақталады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-117">Amounts are automatically retained on vendor invoices until the project stage of completion is equal to the specified percentage.</span></span> <span data-ttu-id="ea5fa-118">Мысалы, егер сіз 50,00 енгізсеңіз, онда жоба 50 пайыз аяқталғанға дейін сақталады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-118">For example, if you enter 50.00, amounts are retained until the project is 50 percent completed.</span></span>
   - <span data-ttu-id="ea5fa-119">**Сақтау пайызы** : сақталатын сатушы есеп-шотының сома пайызын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-119">**Percentage to retain** : Enter a percentage of the vendor invoice amount to be retained.</span></span> <span data-ttu-id="ea5fa-120">Мысалы, егер сіз 10,00 енгізсеңіз, онда сатушы есеп-шоты сомасының 10 пайызы жоба **Өріске жеткізілген бірлік пайызы** мәнінде белгіленгендей аяқтау пайызына жеткенге дейін сақталады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-120">For example, if you enter 10.00, then 10 percent of the amount on a vendor invoice is retained until the project reaches the percentage of completion as set in the **Percentage of units delivered field**.</span></span>
   - <span data-ttu-id="ea5fa-121">**Шығару пайызы** : жоба аяқталуының таңдалған деңгейіне шығарылатын бұрын сақталған кез келген соманың пайызын енгізу үшін **Жол қосу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-121">**Percentage to release** : Select **Add line** to enter a percentage of any previously retained amounts to be released for the selected level of project completion.</span></span>

> [!NOTE]
> <span data-ttu-id="ea5fa-122">Егер сізде жоба аяқталуының әртүрлі деңгейлері үшін бірнеше кезеңдер болса, әр сақтау ережелері үшін жеке сатушының сақтау шарты жолын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-122">If you have more than one milestone for different levels of project completion, enter a separate vendor retention term line for each retention rule.</span></span> <span data-ttu-id="ea5fa-123">Әрбір жолда жоба аяқталуының әр белгіленген деңгейі үшін әртүрлі сақтау пайызы және әртүрлі шығару пайызы көрсетілуі мүмкін.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-123">Each line can specify a different retention percentage and a different release percentage for each designated level of project completion.</span></span>

<span data-ttu-id="ea5fa-124">Сатушыға арналған сақтау шарттарын жасағаннан кейін, шарттарды жобаға қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-124">After you create vendor retention terms for a vendor, you can apply the terms to a project.</span></span>

## <a name="apply-vendor-retention-terms-to-a-project"></a><span data-ttu-id="ea5fa-125">Жобаға сатушының сақтау шарттарын қолдану</span><span class="sxs-lookup"><span data-stu-id="ea5fa-125">Apply vendor retention terms to a project</span></span>

1. <span data-ttu-id="ea5fa-126">**Жобаларды басқару және есепке алу** > **Жобалар** > **Барлық жобалар** тармағына өтіп, жоба тізімі бетінен жобаны ашыңыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-126">Go to **Project management and accounting** > **Projects** > **All projects** and open a project from the project list page.</span></span>
2. <span data-ttu-id="ea5fa-127">**Сатушы келісімдері** FastTab қойыншасында **Жол қосу** пәрменін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="ea5fa-128">**Тіркелгі кодының өрісі** параметрінде, келесі параметрлердің бірін таңдаңыз:</span><span class="sxs-lookup"><span data-stu-id="ea5fa-128">In the **Account code field** , select one of the following options:</span></span> 

   - <span data-ttu-id="ea5fa-129">**Кесте** : сатушының сақтау шарттары бір сатушыға қолданылады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-129">**Table** : The vendor retention terms apply to a single vendor.</span></span>
   - <span data-ttu-id="ea5fa-130">**Топ** : сатушының сақтау шарттары сатушылар тобындағы барлық сатушыларға қолданылады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-130">**Group** : The vendor retention terms apply to all vendors in a vendor group.</span></span>
   - <span data-ttu-id="ea5fa-131">**Барлығы** : сатушының сақтау шарттары барлық сатушыға қолданылады.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-131">**All** : The vendor retention terms apply to all vendors.</span></span>

4. <span data-ttu-id="ea5fa-132">**Сатушы/сатушы топ өрісі** параметрінде, сатушының сақтау шарттары қолданылатын сатушыны немесе сатушы тобын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-132">In the **Vendor/Vendor group field** , select the vendor or vendor group to which the vendor retention terms apply.</span></span> <span data-ttu-id="ea5fa-133">Алдыңғы қадамда **Барлық** параметрін таңдаған болсаңыз, бұл өріс қолжетімді болмайды.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-133">If you selected **All** in the previous step, this field is unavailable.</span></span>
5. <span data-ttu-id="ea5fa-134">**Сатушының сақтау шарттары** өрісінде, алдыңғы процедурада жасалған сақтау шарттарын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-134">In the **Vendor retention terms** field, select the retention terms that you created in the previous procedure.</span></span>
6. <span data-ttu-id="ea5fa-135">Егер де жобада сатушыға арналған төленген кезде төлеу (PWP) шарттары бар болса, жобаға **PWP шекті пайызы** өрісінде шекті пайызды енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-135">If the project also has pay-when-paid (PWP) terms set up for the vendor, enter the threshold percentage for the project in the **PWP threshold percentage** field.</span></span>

<span data-ttu-id="ea5fa-136">Сатушының сақтау шарттары сіздің сатушы үшін жасаған сатып алу тапсырыстарында да көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="ea5fa-136">The vendor retention terms are also displayed on purchase orders that you create for the vendor.</span></span>
