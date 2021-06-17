---
title: Биржадан тыс материалдарды күтудегі жеткізуші есеп-шоты арқылы сатып алу
description: Бұл бөлімде күтудегі жеткізуші шот-фактураларын жазу жолы түсіндіріледі.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b5e6632d73c8a211b1f0d568be8e10ef47be77e2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993807"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="f7f2a-103">Биржадан тыс материалдарды күтудегі жеткізуші есеп-шоты арқылы сатып алу</span><span class="sxs-lookup"><span data-stu-id="f7f2a-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="f7f2a-104">_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_</span><span class="sxs-lookup"><span data-stu-id="f7f2a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f7f2a-105">Компания жоба үшін биржадан тыс материалдарды сатып алатындықтан, шығындар жобаға қатысты дереу жазылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="f7f2a-106">Мысалы, Contoso Robotics US компаниясы жабдықты жаңарту жобасын жүзеге асырады және бағдарламалық жасақтама лицензияларын қажет етеді.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="f7f2a-107">Бұл лицензиялар үшінші тарапты жеткізушіден сатып алынады.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="f7f2a-108">Dynamics 365 Finance арқылы несие берушілермен есеп айырысу жөніндегі қызметкер жеткізушінің күтілетін шот-фактура құжатын жазады және лицензия шығындарын жабдықты жаңарту жобасына тікелей жатқызады.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="f7f2a-109">Осы тақырыпта сипатталған функцияны пайдаланар алдында, қажетті конфигурацияларды қарап шығыңыз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="f7f2a-110">Қосымша ақпарат алу үшін [Биржадан тыс материалдарды және күтудегі жеткізуші шот-фактуралары](configure-materials-nonstocked.md) тақырыбын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="f7f2a-111">Жобаға қатысты күтудегі жеткізуші шот-фактурасы</span><span class="sxs-lookup"><span data-stu-id="f7f2a-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="f7f2a-112">Күтудегі жеткізуші шот-фактуралары **Күтудегі жеткізуші шот-фактуралары** бетінде (**Несие берушілер** > **Шот-фактуралар** > **Күтудегі жеткізуші шот-фактуралары)** жазылуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="f7f2a-113">Жобаға қатысты күтудегі жеткізуші шот-фактурасын орналастыру үшін келесі қадамдарды орындаңыз:</span><span class="sxs-lookup"><span data-stu-id="f7f2a-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="f7f2a-114">**Несие берушілер** > **Шот-фактуралар** және **Жаңа** опцияларын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="f7f2a-115">**Шот-фактура шоты** өрісінде жеткізушіні таңдап, **Нөмір** өрісінде жеткізушінің шот-фактура идентификациясын енгізіңіз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="f7f2a-116">Жеткізуші шот-фактурасына және **Элемент нөмірі** өрісіне жол қосып, жеткізушіден сатып алынған биржадан тыс элементті таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="f7f2a-117">Сатып алу санатына негізделген жеткізуші шот-фактурасының жолдарын жобаға қарсы жазу мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="f7f2a-118">Сатып алынған санын қосыңыз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-118">Add the quantity purchased.</span></span> <span data-ttu-id="f7f2a-119">Жүйе биржадан тыс элемент бағасының конфигурациясы негізінде бірлік бағасын толтырады.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="f7f2a-120">Жолдағы жалпы соманы және басқа қажетті мәліметтерді тексеріңіз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="f7f2a-121">Жол мәліметтерінде **Жоба** қойыншасында осы элемент жазылатын жобаның идентификаторын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="f7f2a-122">Қажет болса, әрекет нөмірін таңдап, жоба санаты мен жол сипатын жаңартыңыз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="f7f2a-123">Күтудегі жеткізуші шот-фактурасын орналастырыңыз.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-123">Post pending vendor invoice.</span></span> <span data-ttu-id="f7f2a-124">Шот-фактура орналастырылған кезде жүйе келесілерді жазады:</span><span class="sxs-lookup"><span data-stu-id="f7f2a-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="f7f2a-125">Жеткізушінің қалдық сомасы.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="f7f2a-126">Сатылым салығы сомасы.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-126">The sales tax amount.</span></span>
    - <span data-ttu-id="f7f2a-127">Жоба бойынша шығындар сатып алуды біріктіру шотына жазылады.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="f7f2a-128">Dataverse жүйесіндегі жобаның нақты транзакциясы.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="f7f2a-129">Бұл транзакция енді [Project Operations біріктіру журналы](../project-accounting/project-operations-integration-journal.md) арқылы өңделеді.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="f7f2a-130">Бұл журналды орналастыру сатып алуды біріктіру шотынан соманы жоба құны шотына ауыстырады.</span><span class="sxs-lookup"><span data-stu-id="f7f2a-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
