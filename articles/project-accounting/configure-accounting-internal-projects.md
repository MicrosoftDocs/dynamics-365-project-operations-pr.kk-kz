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
ms.openlocfilehash: 9f1cc75b12fec81d726e46f8d970dcfe030f6b29
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287605"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="2b7de-103">Ішкі жобалар үшін есепті конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="2b7de-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="2b7de-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="2b7de-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="2b7de-105">Ішкі жобалар компанияларға тұтынушыға есеп айырыспайтын әрекеттерге байланысты шығындарды бақылауға мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="2b7de-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="2b7de-106">Ішкі жобалардың мысалдары:</span><span class="sxs-lookup"><span data-stu-id="2b7de-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="2b7de-107">Мобильді құрылғы бағдарламасы сияқты өнімді әзірлеу және оны әзірлеуге байланысты шығындарды қадағалау.</span><span class="sxs-lookup"><span data-stu-id="2b7de-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="2b7de-108">Сату алдындағы уақыт пен шығындарды басқару.</span><span class="sxs-lookup"><span data-stu-id="2b7de-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="2b7de-109">Бұл сату алдындағы ішкі жоба, егер баға ұсынысы жеңіске жетсе, кейінірек ақылы жобаға айналуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="2b7de-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="2b7de-110">Dynamics 365 Project Operations бағдарламасында келісім-шартпен байланысты емес кез келген жоба ішкі ретінде қарастырылады.</span><span class="sxs-lookup"><span data-stu-id="2b7de-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="2b7de-111">Жоба құны мен түсім профильдері жоба бойынша есеп ережелерін анықтау үшін пайдаланылмайды.</span><span class="sxs-lookup"><span data-stu-id="2b7de-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="2b7de-112">Жобаның ішкі құны әрқашан пайда мен шығын ережелерін пайдалана отырып орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="2b7de-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="2b7de-113">Енгізу деректеріне арналған бухгалтерлік кітап шоттары **Бас кітапқа енгізу деректерін орнату** бетінде анықталады.</span><span class="sxs-lookup"><span data-stu-id="2b7de-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="2b7de-114">Мерзімдік мәмілелер **Шығын** шотын дебеттеп, сондай-ақ **Жалақының жалпы сомасын бөлу** шотын есептеу арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="2b7de-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="2b7de-115">Шығыс операциялары **Шығын** шотын дебеттеп, сондай-ақ **Шығыстың өтемақы шотын** есептеу арқылы орналастырылады.</span><span class="sxs-lookup"><span data-stu-id="2b7de-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>

<span data-ttu-id="2b7de-116">Операциялар жобаға орналастырылғаннан кейін, егер жоба жобалық келісім-шартпен байланысты болса, жүйе барлық жинақталған операцияларды кері қайтарып, жаңа ақылы операцияларды жасайды.</span><span class="sxs-lookup"><span data-stu-id="2b7de-116">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="2b7de-117">Ақылы операциялар жобаның шығындары мен кірістерінің тиісті профилінде айқындалған бухгалтерлік есеп ережелеріне сәйкес орындалады.</span><span class="sxs-lookup"><span data-stu-id="2b7de-117">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]