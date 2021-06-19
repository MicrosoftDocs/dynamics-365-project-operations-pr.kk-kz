---
title: Шығыс туралы есеп бойынша жеке шығындармен жұмыс істеу
description: Бұл тақырыпта іскерлік мақсатта сапар шегу кезінде қызметкерлердің жарататын жеке шығындарымен жұмыс істеу туралы ақпарат беріледі.
author: suvaidya
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: ae25eca08089d224f1e17e95eeb571054de8a5c0
ms.sourcegitcommit: fd6e9ff78392c7bac35591d9130c00d2750438ae
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025691"
---
# <a name="work-with-personal-expenses-on-an-expense-report"></a><span data-ttu-id="2e4f1-103">Шығыс туралы есеп бойынша жеке шығындармен жұмыс істеу</span><span class="sxs-lookup"><span data-stu-id="2e4f1-103">Work with personal expenses on an expense report</span></span>

<span data-ttu-id="2e4f1-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="2e4f1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2e4f1-105">Қызметтік іссапар кезінде қызметкер жеке шығындарын корпоративтік несиелік картасынан өндіріп алуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-105">During business travel, an employee might charge personal expenses to their corporate credit card.</span></span> <span data-ttu-id="2e4f1-106">Егер жеке шығындармен жұмыс істеу үдерісі анықталмаған болса, қызметкер шығындар туралы есептерін ұсынған кезде шығындар туралы есепті бекіту процесі бұзылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-106">If a process hasn't been defined for handling personal expenses, the expense report approval process might be disrupted when an employee submits their itemized expense report.</span></span>

<span data-ttu-id="2e4f1-107">Қызметкердің жеке шығындарымен жұмыс істеу үшін екі әдісті пайдалануға болады:</span><span class="sxs-lookup"><span data-stu-id="2e4f1-107">There are two methods you can use to work with an employee's personal expenses:</span></span>

  - <span data-ttu-id="2e4f1-108">**Қызметкер арқылы төленетін**: сіздің ұйымыңыз корпоративтік несие картасының шотында көрсетілген жеке шығындарды төлемейді.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-108">**Paid by employee**: Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="2e4f1-109">Оның орнына қызметкер шығындарды несие картасын жеткізушіге тікелей төлейді.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-109">Instead, the employee pays the credit card vendor directly for the expenses.</span></span> 
  - <span data-ttu-id="2e4f1-110">**Компания арқылы төленетін**: сіздің ұйымыңыз корпоративтік несие картасы үшін төлемді толық төлейді, содан кейін жеке шығындар үшін жұмысшының шотынан дебет жасайды.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-110">**Paid by company**: Your organization pays the full bill for the corporate credit card, and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="2e4f1-111">Сіз өзіңіздің ұйымыңыз пайдаланатын әдісті **Шығындарды басқару параметрлері** бетінде таңдай аласыз.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-111">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>


## <a name="enable-split-expense-function-when-personal-amount-field-has-value-defined"></a><span data-ttu-id="2e4f1-112">Жеке сома өрісі мәнге ие болған кезде шығынды бөлу функциясын қосу</span><span class="sxs-lookup"><span data-stu-id="2e4f1-112">Enable split expense function when personal amount field has value defined</span></span>

<span data-ttu-id="2e4f1-113">**Жеке сома өрісі мәнге ие болған кезде шығынды бөлу функциясын қосу** функциясы тек жол деңгейіндегі жұмыс ағыны арқылы мақұлданған шығындар туралы есептерге қолданылады.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-113">The feature, **Enable split expense function when personal amount field has value defined** only applies to expense reports that are approved using a line-level workflow.</span></span> <span data-ttu-id="2e4f1-114">Есептерді **Шығындар туралы есептерді өңдеу** > **Маған тағайындалған шығындар туралы есептер** > **Шығындар туралы есепті ашу** тармағына өту арқылы мақұлдауға болады.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-114">Reports are approved by going to **Process expense reports** > **Expense reports assigned to me** > **Open expense report**.</span></span> 

<span data-ttu-id="2e4f1-115">Бұл функцияны қосу үшін **Жұмыс кеңістіктері** > **Функцияны басқару** тармағына өтіңіз және **Жеке сома өрісі мәнге ие болған кезде шығынды бөлу функциясын қосу** функциясын таңдаңыз, содан кейін **Қазір қосу** түймешігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-115">To enable this feature, go to **Workspaces** > **Feature Management**, select **Enable split expense function when personal amount field has value defined**, and then select **Enable now**.</span></span> 

<span data-ttu-id="2e4f1-116">Функция қосылған кезде, осы функцияны пайдаланатын шығындар жолы есеп ұсынылған кезде екі жол жасайды.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-116">When the feature is enabled, expense lines that use this functionality generate two lines when the report is submitted.</span></span> <span data-ttu-id="2e4f1-117">Мақұлдаушы әр жолды жеке-жеке мақұлдай алатындай екі жол жасалады.</span><span class="sxs-lookup"><span data-stu-id="2e4f1-117">Two lines are generated so that the approver can approve each line separately.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
