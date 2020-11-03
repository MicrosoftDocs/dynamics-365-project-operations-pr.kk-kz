---
title: Шығыс туралы есеп бойынша жеке шығындар
description: Бұл тақырып Microsoft Dynamics 365 Finance бағдарламасында жұмысшының жеке шығындарын шешудің екі әдісін түсіндіреді.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 825b6c131c8a65b99d5b7ebdadcd6389886f2d11
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079809"
---
# <a name="personal-expenses-on-an-expense-report"></a><span data-ttu-id="04af6-103">Шығыс туралы есеп бойынша жеке шығындар</span><span class="sxs-lookup"><span data-stu-id="04af6-103">Personal expenses on an expense report</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="04af6-104">Іссапарлар кезінде жұмысшылар кейде жеке шығындарын корпоративті несие карталарынан шеше алады.</span><span class="sxs-lookup"><span data-stu-id="04af6-104">During business travel, workers might sometimes charge personal expenses to their corporate credit cards.</span></span> <span data-ttu-id="04af6-105">Егер сіз жеке шығындарды өңдеу процесін анықтамасаңыз, жұмысшылар егжей-тегжейлі шығындар туралы есептерін ұсынған кезде шығындар туралы есептерді бекіту процесі бұзылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="04af6-105">If you don't define a process for handling personal expenses, the approval process for expense reports might be disrupted when workers submit their itemized expense reports.</span></span> 

<span data-ttu-id="04af6-106">Жұмысшының жеке шығындарын басқарудың екі әдісі бар:</span><span class="sxs-lookup"><span data-stu-id="04af6-106">There are two methods for handling a worker's personal expenses:</span></span>

- <span data-ttu-id="04af6-107">**Қызметкер төлейтін** - Сіздің ұйымыңыз корпоративтік несие картасының шотында көрсетілген жеке шығындарды төлемейді.</span><span class="sxs-lookup"><span data-stu-id="04af6-107">**Paid by employee** – Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="04af6-108">Оның орнына, ол жеке шығындарды корпоративтік несие картасынан алынған корпоративтік шығындармен бірге көрсететін есеп жасайды.</span><span class="sxs-lookup"><span data-stu-id="04af6-108">Instead, it creates a report that shows personal expenses together with the corporate expenses that were charged to the corporate credit card.</span></span>
- <span data-ttu-id="04af6-109">**Компания төлейді** - Сіздің ұйымыңыз корпоративті несие картасының бүкіл шотын төлейді, содан кейін қызметкердің жеке шығындарын есептен шығарады.</span><span class="sxs-lookup"><span data-stu-id="04af6-109">**Paid by company** – Your organization pays the whole bill for the corporate credit card and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="04af6-110">Сіз өзіңіздің ұйымыңыз пайдаланатын әдісті **Шығындарды басқару параметрлері** бетінде таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="04af6-110">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>
