---
title: Project Operations интеграциясын әр заңды тұлға үшін конфигурациялау
description: Бұл тақырыпта Project Operations жүйесінде заңды тұлға арқылы интеграцияны орнату туралы ақпарат берілген.
author: sigitac
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: c0e02ef2d17bf49209369f7adad681d9a5981e2a
ms.sourcegitcommit: 91ad491e94a421f256a378b0f4b26ed48c67bc93
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/22/2020
ms.locfileid: "4096759"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a><span data-ttu-id="ee076-103">Project Operations интеграциясын әр заңды тұлға үшін конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="ee076-103">Configure Project Operations integration per legal entity</span></span> 

<span data-ttu-id="ee076-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="ee076-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ee076-105">Бұл тақырып заңды тұлғаларға арналған Dynamics 365 Project Operations конфигурациясы үшін қажетті қадамдар сипатталады.</span><span class="sxs-lookup"><span data-stu-id="ee076-105">This topic walks you through the steps required to configure Dynamics 365 Project Operations per legal entity.</span></span>

## <a name="enable-feature-keys-in-dynamics-365-finance"></a><span data-ttu-id="ee076-106">Dynamics 365 Finance жүйесінде мүмкіндік кілттерін қосу</span><span class="sxs-lookup"><span data-stu-id="ee076-106">Enable feature keys in Dynamics 365 Finance</span></span>

<span data-ttu-id="ee076-107">Қажетті мүмкіндіктерді қосу үшін келесі әрекеттерді орындаңыз.</span><span class="sxs-lookup"><span data-stu-id="ee076-107">Complete the following steps to enable required features.</span></span>

1. <span data-ttu-id="ee076-108">Dynamics 365 Finance бөлімінде **Мүмкіндікті басқару** жұмыс кеңістігіне өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="ee076-108">In Dynamics 365 Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="ee076-109">**Мүмкіндіктер тізімі** өрісінде келесі мүмкіндіктерді тауып қосыңыз:</span><span class="sxs-lookup"><span data-stu-id="ee076-109">In **Feature list** , find and enable the following features:</span></span>
  
    - <span data-ttu-id="ee076-110">**Жоба үшін бірнеше келісім-шарт жолдарын қосыңыз**</span><span class="sxs-lookup"><span data-stu-id="ee076-110">**Enable multiple contract lines for a project**</span></span>
    - <span data-ttu-id="ee076-111">**Dynamics 365 Customer Engagement жүйесінде Project Operations қызметін қосу**</span><span class="sxs-lookup"><span data-stu-id="ee076-111">**Enable Project Operations on Dynamics 365 Customer Engagement**</span></span>

> [!NOTE]
> <span data-ttu-id="ee076-112">Тізімделген **Мүмкіндік кілттері** параметрін көрмесеңіз, Finance нұсқаңыздың ең төменгі нұсқа талаптарына сәйкес келетіндігін тексеріңіз (бағдарламаның 10.0.13 нұсқасы барлық сапалы жаңартулар қолданылған немесе одан жоғары).</span><span class="sxs-lookup"><span data-stu-id="ee076-112">If you don't see **Feature keys** listed, verify that your Finance version meets the minimum version requirement (application version 10.0.13 with all quality updates applied or higher).</span></span> <span data-ttu-id="ee076-113">Функциялар тізімін жаңарту үшін **Жаңартуларды тексеру** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ee076-113">Select **Check for updates** to refresh the feature list.</span></span>

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a><span data-ttu-id="ee076-114">Заңды тұлға үшін Project Operations орналастыру сценарийін анықтаңыз</span><span class="sxs-lookup"><span data-stu-id="ee076-114">Define the Project Operations deployment scenario for a legal entity</span></span>

<span data-ttu-id="ee076-115">Project Operations жүйесін Dynamics 365 Customer Engagement қызметінде заңды тұлға деңгейінде қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="ee076-115">You can enable Project Operations on Dynamics 365 Customer Engagement on a legal entity level.</span></span> <span data-ttu-id="ee076-116">Ресурс/биржадан тыс негіздегі сценарийлерге арналған Dynamics 365 Customer Engagement жүйесінде Project Operations қызметін пайдаланатын бір заңды тұлғаңыз болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="ee076-116">You can have one legal entity using Project Operations on Dynamics 365 Customer Engagement for resource/non-stocked based scenarios.</span></span> <span data-ttu-id="ee076-117">Дәл сол ортада сізде қосалқы/өндіріс тапсырыс сценарийлері үшін Project Operations пайдаланатын басқа заңды тұлға болуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="ee076-117">In the same environment, you can have another legal entity using Project Operations for stocked/production order scenarios.</span></span>

1. <span data-ttu-id="ee076-118">Dynamics 365 Finance жүйесінде **Жобаларды басқару және есепке алу** > **Орнату** > **Жобаларды басқару және есепке алу параметрлері** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="ee076-118">In Dynamics 365 Finance, go to **Project management and accounting** > **Setup** > **Global project management and accounting parameters**.</span></span>
2. <span data-ttu-id="ee076-119">Қол жетімді заңды тұлғалар тізімінен бірнеше келісімшарттар мен Dynamics 365 Customer Engagement қызметіндегі мүмкіндіктер қосулы болатын Project Operations мүмкіндігін таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ee076-119">In the list of available legal entities, select entities where multiple contract lines and Project Operations on Dynamics 365 Customer Engagement features will be enabled.</span></span> <span data-ttu-id="ee076-120">Қосалқы/өндірістік тапсырыс сценарийлеріне арналған Project Operations мүмкіндігін пайдаланатын заңды тұлғаларды таңдамай қалдырыңыз.</span><span class="sxs-lookup"><span data-stu-id="ee076-120">Leave legal entities that will be using Project Operations for stocked/production order scenarios unselected.</span></span>

> [!NOTE]
> <span data-ttu-id="ee076-121">Заңды тұлғаны тек қолданыстағы жобалары болмаса ғана таңдауға болады.</span><span class="sxs-lookup"><span data-stu-id="ee076-121">A legal entity can be selected only if it doesn't have any existing projects.</span></span>

## <a name="configure-project-management-and-accounting-parameters"></a><span data-ttu-id="ee076-122">Жобаларды басқару және есепке алу параметрлерін конфигурациялау</span><span class="sxs-lookup"><span data-stu-id="ee076-122">Configure Project management and accounting parameters</span></span>

<span data-ttu-id="ee076-123">Dynamics 365 Customer Engagement жүйесінде Project Operations мүмкіндігін пайдаланатын әрбір заңды тұлға үшін әдепкі параметрлер жиынтығы қажет.</span><span class="sxs-lookup"><span data-stu-id="ee076-123">Each legal entity using Project Operations on Dynamics 365 Customer Engagement needs a set of default parameters.</span></span> <span data-ttu-id="ee076-124">Бұл параметрлер **Жобаларды басқару және есепке алу параметрлері** бетіндегі **Project Operations** қойыншасында конфигурацияланады.</span><span class="sxs-lookup"><span data-stu-id="ee076-124">These parameters are configured on the **Project Operations** tab on the **Project management and accounting parameters** page.</span></span> <span data-ttu-id="ee076-125">Параметрлер мыналар:</span><span class="sxs-lookup"><span data-stu-id="ee076-125">The parameters are:</span></span>

  - <span data-ttu-id="ee076-126">**Есепшот түрінің әдепкі мәндері** : Project Operations мүмкіндігі Finance жол сипаттарына сәйкес келуі керек есеп-шот түріндегі әдепкі мәндер жиынтығын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="ee076-126">**Billing type defaults** : Project Operations uses a fixed set of billing type defaults that must be mapped to line properties Finance.</span></span> <span data-ttu-id="ee076-127">Әрбір есеп-шот түрі үшін жазба жасаңыз: **Көрсетілмеген** , **Ақылы** , **Ақысыз** , **Тегін** және **Қолжетімді емес**.</span><span class="sxs-lookup"><span data-stu-id="ee076-127">Create a record for each billing type: **Not specified** , **Chargeable** , **Non-chargeable** , **Complimentary** , and **Not available**.</span></span>
  - <span data-ttu-id="ee076-128">**Жоба санатының әдепкі параметрлері** : Әрбір операция түрі үшін пайдаланылатын стандартты жоба санаттарын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ee076-128">**Project category defaults** : Select the default project categories to be used for each transaction type.</span></span> <span data-ttu-id="ee076-129">Бұл әдепкі шарттар **Project Operations Integration журналы** ішінде және нақты жоба үшін операция санаты көрсетілмеген бағаларда пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="ee076-129">These defaults will be used in the **Project Operations Integration journal** and in estimates where no transaction category is specified for the project actual.</span></span>
  - <span data-ttu-id="ee076-130">**Болжамдар** : Уақыт пен шығындарды бағалау үшін пайдаланылатын болжамды үлгіні таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="ee076-130">**Forecasts** : Select the forecast model to be used for time and expense estimates.</span></span>
