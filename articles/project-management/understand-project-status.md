---
title: Жоба күйін түсіну
description: Бұл тақырыпта Dynamics 365 Project Operations бағдарламасындағы жобаға тағайындалған күй туралы ақпарат беріледі.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 336e479ad39653af14cca7930fe63e906b7de489
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965683"
---
# <a name="understand-project-status"></a><span data-ttu-id="e4d37-103">Жоба күйін түсіну</span><span class="sxs-lookup"><span data-stu-id="e4d37-103">Understand project status</span></span>

<span data-ttu-id="e4d37-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="e4d37-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="e4d37-105"> **Жоба нысаны**  бетіндегі **Күй**  бөлімінде құн мен талпынысқа негізделген жобаның денсаулық туралы қорытындысы келтірілген.</span><span class="sxs-lookup"><span data-stu-id="e4d37-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="e4d37-106">Күй қорытындысының өрістері</span><span class="sxs-lookup"><span data-stu-id="e4d37-106">Status summary fields</span></span>

- <span data-ttu-id="e4d37-107"> **Жобаның жалпы күйі**  өрісі — бұл жобаның жалпы күйін көрсететін өңделетін өріс.</span><span class="sxs-lookup"><span data-stu-id="e4d37-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="e4d37-108">Бұл өріс артып келе жатқан қауіпті көрсету үшін жасыл, сары және қызыл сияқты түрлі түсті кодтауды пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="e4d37-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="e4d37-109"> **Комментарийлер**  өрісі жоба менеджеріне күй туралы нақты комментарийлер енгізуге мүмкіндік береді.</span><span class="sxs-lookup"><span data-stu-id="e4d37-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="e4d37-110"> **Күйі жаңартылған күн**  өрісін өңдеу мүмкін емес.</span><span class="sxs-lookup"><span data-stu-id="e4d37-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="e4d37-111">Бұл өрістегі мән күйдің соңғы рет жаңартылған күнін көрсететін уақыт белгісі болып табылады.</span><span class="sxs-lookup"><span data-stu-id="e4d37-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="e4d37-112"> **Кесте өнімділігі** және  **Құн өнімділігі** өрістері бақылау торынан бастап орнатылады.</span><span class="sxs-lookup"><span data-stu-id="e4d37-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="e4d37-113"> **Талпынысты бақылау** көрінісіндегі түбірлік түйіннің кесте мен құн ауытқуы оң болғанда, бұл өрістер  **Алдында** мәніне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="e4d37-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="e4d37-114">Түбірлік түйіннің кесте мен құн ауытқуы теріс болса, бұл өрістер  **Артында** мәніне орнатылады.</span><span class="sxs-lookup"><span data-stu-id="e4d37-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>
