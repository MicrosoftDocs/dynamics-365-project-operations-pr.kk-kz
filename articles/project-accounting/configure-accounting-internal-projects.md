---
title: Ішкі жобалар үшін есепті конфигурациялау
description: Бұл тақырып Project Operations жүйесінде ішкі жобалар үшін бухгалтерлік есеп тәжірибелерін құру жолдары туралы ақпарат береді.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ea04178d4327ccd701ab431f172463a13a55154e
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "4132385"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="d07c5-103">Ішкі жобалар үшін есепті конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="d07c5-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="d07c5-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="d07c5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d07c5-105">Ішкі жобалар компанияларға тұтынушыға есеп айырыспайтын әрекеттерге байланысты шығындарды бақылауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="d07c5-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="d07c5-106">Ішкі жобалардың мысалдары:</span><span class="sxs-lookup"><span data-stu-id="d07c5-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="d07c5-107">Мобильді құрылғы бағдарламасы сияқты өнімді әзірлеу және оны әзірлеуге байланысты шығындарды қадағалау.</span><span class="sxs-lookup"><span data-stu-id="d07c5-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="d07c5-108">Сату алдындағы уақыт пен шығындарды басқару.</span><span class="sxs-lookup"><span data-stu-id="d07c5-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="d07c5-109">Бұл сату алдындағы ішкі жоба, егер баға ұсынысы жеңіске жетсе, кейінірек ақылы жобаға айналуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="d07c5-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="d07c5-110">Dynamics 365 Project Operations келісім-шартымен байланысты емес кез келген жоба ішкі жоба ретінде қарастырылады.</span><span class="sxs-lookup"><span data-stu-id="d07c5-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="d07c5-111">Жоба құны мен түсім профильдері жоба бойынша есеп ережелерін анықтау үшін пайдаланылмайды.</span><span class="sxs-lookup"><span data-stu-id="d07c5-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="d07c5-112">Жобаның ішкі құны әрқашан пайда мен шығын ережелерін пайдалана отырып орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="d07c5-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="d07c5-113">Енгізу деректеріне арналған бухгалтерлік кітап шоттары **Бас кітапқа енгізу деректерін орнату** бетінде анықталады.</span><span class="sxs-lookup"><span data-stu-id="d07c5-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="d07c5-114">Мерзімдік мәмілелер **Шығын** шотын дебеттеп, сондай-ақ **Жалақының жалпы сомасын бөлу** шотын есептеу арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="d07c5-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="d07c5-115">Шығыс операциялары **Шығын** шотын дебеттеп, сондай-ақ **Шығыстың өтемақы шотын** есептеу арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="d07c5-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>

<span data-ttu-id="d07c5-116">Операциялар жобаға орналастырылғаннан кейін, егер жоба жобалық келісім-шартпен байланысты болса, жүйе барлық жинақталған операцияларды кері қайтарып, жаңа ақылы операцияларды жасайды.</span><span class="sxs-lookup"><span data-stu-id="d07c5-116">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="d07c5-117">Ақылы операциялар жобаның шығындары мен кірістерінің тиісті профилінде айқындалған бухгалтерлік есеп ережелеріне сәйкес орындалады.</span><span class="sxs-lookup"><span data-stu-id="d07c5-117">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>


