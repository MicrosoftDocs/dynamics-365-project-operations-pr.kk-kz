---
title: Жобаның баға ұсыныстарын басқару
description: Бұл тақырыпта жобаның баға ұсыныстары туралы ақпарат берілген.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8e0b20d4780a14edc3c242e261e22d4905f783a4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994818"
---
# <a name="manage-project-quotes"></a><span data-ttu-id="2b564-103">Жобаның баға ұсыныстарын басқару</span><span class="sxs-lookup"><span data-stu-id="2b564-103">Manage project quotes</span></span>

<span data-ttu-id="2b564-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="2b564-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2b564-105">Dynamics 365 Project Operations бағдарламасында жобаның баға ұсыныстары жобалық жұмыс үшін ұсыныстар жасауға көмектесу үшін жасалған.</span><span class="sxs-lookup"><span data-stu-id="2b564-105">In Dynamics 365 Project Operations, project quotes are designed to help build proposals for project work.</span></span> <span data-ttu-id="2b564-106">Project Operations бағдарламасындағы жобалық баға ұсынысының құрылымы жобалық ұсыныстарға келесі құрамдастармен құрылымдалған:</span><span class="sxs-lookup"><span data-stu-id="2b564-106">The structure of a project quote in Project Operations is structured for project proposals with the following components:</span></span>

  - <span data-ttu-id="2b564-107">Жоғары деңгей құрамдастары ретінде ұсынылатын жұмыстың дискретті құрамдастарын анықтайтын баға ұсынысы жолдары.</span><span class="sxs-lookup"><span data-stu-id="2b564-107">Quote lines that identify the discrete components of work that will be presented as high-level components.</span></span>
  - <span data-ttu-id="2b564-108">Әрбір жоғары деңгейлі құрамдас немесе баға ұсынысы жолы үшін жұмыстарды анықтайтын және бағалайтын баға ұсынысы жолының мәліметтері.</span><span class="sxs-lookup"><span data-stu-id="2b564-108">Quote line details that identify and estimate the work for each high-level component or quote line.</span></span> <span data-ttu-id="2b564-109">Кесте немесе күн болжамдары және жұмыс бойынша қаржылық аспектілер сол баға ұсынысы жолына байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="2b564-109">Schedule or date estimates and the financial aspects for the work are tied to that quote line.</span></span>
  - <span data-ttu-id="2b564-110">Әрбір баға ұсынысы үшін келісім-шарттық үлгілер мен ақылы құрамдастар орнатылған.</span><span class="sxs-lookup"><span data-stu-id="2b564-110">Contracting models and chargeable components are set up for each quote line.</span></span> <span data-ttu-id="2b564-111">Бұл параметр кірістердің таралуын, шығындар және әрбір баға ұсынысы жолы мен жалпы баға ұсынысына арналған табыстылықты бағалауға көмектеседі.</span><span class="sxs-lookup"><span data-stu-id="2b564-111">This set up helps estimate the spread of revenue, spend, and profitability for each quote line and the overall quote.</span></span>

## <a name="view-all-project-based-quotes"></a><span data-ttu-id="2b564-112">Барлық жобаға негізделген баға ұсыныстарын қарау</span><span class="sxs-lookup"><span data-stu-id="2b564-112">View all project-based quotes</span></span>

<span data-ttu-id="2b564-113">Барлық жобалық баға ұсыныстары тізімін **Баға ұсыныстары** тізімінің бетінен көруге болады.</span><span class="sxs-lookup"><span data-stu-id="2b564-113">A list of all the project quotes can be seen from the **Quotes** list page.</span></span> 

1. <span data-ttu-id="2b564-114">**Сатылым** > **Баға ұсынулар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="2b564-114">Go to **Sales** > **Quotes**.</span></span> <span data-ttu-id="2b564-115">Жүйедегі барлық жобалық баға ұсыныстарының тізімі көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="2b564-115">A list of all your project quotes in the system are shown.</span></span> 
2. <span data-ttu-id="2b564-116">Баға ұсыныстарының басқа сүзілген көріністерін таңдау үшін **Көріністі ауыстыру құралын** пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="2b564-116">Use the **View Switcher** to select other filtered views of the quotes.</span></span> <span data-ttu-id="2b564-117">Реттелетін сүзгі шарттарын пайдалана отырып, өз көріністеріңізді және навигация параметрлерін конфигурациялауға болады.</span><span class="sxs-lookup"><span data-stu-id="2b564-117">Using custom filter criteria, you can configure your own views and navigation options.</span></span>

<span data-ttu-id="2b564-118">Баға ұсыныстары осы тізім парағынан немесе мәліметтер бетінен жойылуы немесе жасалуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="2b564-118">Quotes can be created or deleted from this list page or detail pages.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]