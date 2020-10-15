---
title: Шығысқа шолу
description: Бұл тақырыпта Project Operations жүйесіндегі шығыс функциясы туралы ақпарат берілген.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 6da831fef5dba060b8019d7689645405c7ebdbed
ms.sourcegitcommit: 0874b3d89e1dc0e65a51cedb82bf8f80831ca0bb
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "3967373"
---
# <a name="expense-home-page"></a><span data-ttu-id="09a5c-103">"Шығыс" басты беті</span><span class="sxs-lookup"><span data-stu-id="09a5c-103">Expense home page</span></span>

<span data-ttu-id="09a5c-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="09a5c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="09a5c-105">Dynamics 365 Project Operations шығындарды өңдеу мүмкіндігін қолдайды.</span><span class="sxs-lookup"><span data-stu-id="09a5c-105">Dynamics 365 Project Operations supports the ability to process expenses.</span></span> <span data-ttu-id="09a5c-106">Шығындарды өңдеу жобалармен немесе онсыз реттелетін жұмыс процесі саясатымен, транзакциялар санаттарымен және мәлімдемелермен жүзеге асырылады.</span><span class="sxs-lookup"><span data-stu-id="09a5c-106">Expense processing occurs with or without projects by using a customizable workflow of policies, transaction categories, and approvals.</span></span>

<span data-ttu-id="09a5c-107">Project Operations жүйесінде шығысқа арналған орналастырудың екі қолдау үлгісі бар:</span><span class="sxs-lookup"><span data-stu-id="09a5c-107">In Project Operations, there are two supported deployment models for Expense:</span></span> 

- <span data-ttu-id="09a5c-108">**Толық**: Толық орналастыру **Ресурстық/қосалқы емес негіздегі сценарийлерге арналған Project Operations** немесе **Өндірістік тапсырысқа негізделген сценарийлер бойынша Project Operations** үшін қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="09a5c-108">**Full**: Full deployment is available for **Project Operations for resource/non-stocked based scenarios** or **Project Operations for production order based scenarios**.</span></span>
- <span data-ttu-id="09a5c-109">**Негізгі**: Негізгі орналастыру **Ресурстық/қосалқы емес негіздегі сценарийлерге арналған Project Operations** және **Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі** үшін қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="09a5c-109">**Basic**: Basic deployment is available for **Project Operations for resource/non-stocked based scenarios** and **Lite deployment – deal to proforma invoicing**.</span></span>

## <a name="full"></a><span data-ttu-id="09a5c-110">Толық</span><span class="sxs-lookup"><span data-stu-id="09a5c-110">Full</span></span> 
<span data-ttu-id="09a5c-111">Шығындарды толық орналастыру саясат құру мүмкіндігін қамтитын саясаттың толық орындалуын қамтамасыз етеді, мысалы:</span><span class="sxs-lookup"><span data-stu-id="09a5c-111">Full Expense deployment provides a complete policy enforcement which includes the ability to create policies, such as:</span></span>

  - <span data-ttu-id="09a5c-112">Шығыс санатының шектеулері</span><span class="sxs-lookup"><span data-stu-id="09a5c-112">Expense category limits</span></span>
  - <span data-ttu-id="09a5c-113">Саяхат</span><span class="sxs-lookup"><span data-stu-id="09a5c-113">Travel</span></span>
  - <span data-ttu-id="09a5c-114">Тәуліктік</span><span class="sxs-lookup"><span data-stu-id="09a5c-114">Per diem</span></span>
  - <span data-ttu-id="09a5c-115">Несиелік карта импорттаулары</span><span class="sxs-lookup"><span data-stu-id="09a5c-115">Credit card imports</span></span>
  - <span data-ttu-id="09a5c-116">Оптикалық таңбаны тану туралы түбіртек</span><span class="sxs-lookup"><span data-stu-id="09a5c-116">Receipt optical character recognition</span></span>

## <a name="basic"></a><span data-ttu-id="09a5c-117">Негізгі</span><span class="sxs-lookup"><span data-stu-id="09a5c-117">Basic</span></span> 
<span data-ttu-id="09a5c-118">Негізгі шығыстарды орналастыру сценарийі тек негізгі шығындарды жобаға қарсы есепке алуға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="09a5c-118">Basic Expense deployment scenario only allows you to record basic expenses against a project.</span></span> 

<span data-ttu-id="09a5c-119">Қосымша ақпарат алу үшін [Шығындарды енгізу (жеңілдетілген)](basic-expense.md) қараңыз</span><span class="sxs-lookup"><span data-stu-id="09a5c-119">For more information, see [Expense entry (lite)](basic-expense.md)</span></span>

## <a name="determine-your-expense-deployment"></a><span data-ttu-id="09a5c-120">Шығыс орналастыруын анықтау</span><span class="sxs-lookup"><span data-stu-id="09a5c-120">Determine your Expense deployment</span></span>
<span data-ttu-id="09a5c-121">Негізгі шығыстарды басқаруды қолданатыныңызды анықтау үшін мекенжай URL мекенжайы **. crm.dynamics.com** деп аяқталатынына көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="09a5c-121">To determine if you're running the Basic Expense management deployment, verify that the address URL ends with **.crm.dynamics.com**.</span></span> 