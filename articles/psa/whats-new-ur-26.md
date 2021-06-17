---
title: Project Service Automation бағдарламасының 26-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл тақырыпта Project Service Automation бағдарламасының 26-жаңарту шығарылымының 3-нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 6aafe66fe8c63dc886455a36e93f32d4a581d5cc
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005573"
---
# <a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="377dd-103">Project Service Automation бағдарламасының 26-жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="377dd-103">Project Service Automation Update Release 26, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="377dd-104">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="377dd-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="377dd-105">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="377dd-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="377dd-106">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="377dd-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="377dd-107">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="377dd-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="377dd-108">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="377dd-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="377dd-109">Бұл бөлімде Project Service Automation бағдарламасының 26-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="377dd-109">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="377dd-110">Бұл нұсқаның құрастыру нөмірі — V3.10.44.59 және бұл нұсқа әдетте 2020 жылдың желтоқсан айында дербес жаңарту арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="377dd-110">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

## <a name="update-release-26"></a><span data-ttu-id="377dd-111">26-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="377dd-111">Update Release 26</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="377dd-112">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="377dd-112">Bug fixes</span></span>

<span data-ttu-id="377dd-113">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="377dd-113">**Time and Expense**</span></span>

<span data-ttu-id="377dd-114">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="377dd-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="377dd-115">Пайдаланушылар тапсырманы бекітілген/жіберілген уақыт жазбасы бойынша өзгерте алады.</span><span class="sxs-lookup"><span data-stu-id="377dd-115">Users are able to change the task on a time entry that has been approved/submitted.</span></span>
- <span data-ttu-id="377dd-116">Уақыт жазбасын сақтау кезінде "Нысан сілтемесі орнатылмаған" қатесі орын алды.</span><span class="sxs-lookup"><span data-stu-id="377dd-116">"Object Reference Not Set" error when saving time entry.</span></span>
- <span data-ttu-id="377dd-117">Ресурс тағайындауларынан уақыт жазбасының импорты DateTime мәні дұрыс емес уақыт жазбаларын жасайды.</span><span class="sxs-lookup"><span data-stu-id="377dd-117">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>
- <span data-ttu-id="377dd-118">Project Service Automation және Field Service бағдарламаларының екеуі де орнатылған кезде, **Жаңа** түймешігі Field Service бағдарламасындағы уақыт жазбалары үшін пәрмен жолағында екі рет көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="377dd-118">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>
- <span data-ttu-id="377dd-119">**Рұқсат етілген бірлік** және **Бірлік тобы** ұяшықтарының жаңартулары қазір **Шығын болжамдары** торында іске асырылады.</span><span class="sxs-lookup"><span data-stu-id="377dd-119">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>
- <span data-ttu-id="377dd-120">**Уақыт жазбасын өңдеуді жаңарту** пішіні **Уақыт шкаласы** ұяшығын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="377dd-120">**Update Time Entry Edit** form includes **Timeline**.</span></span>
- <span data-ttu-id="377dd-121">Жобадан тыс уақыт жазбаларына арналған уақыт растауы жобаны растаушы рөлін іздеу кезінде жүйені бұғаттайды.</span><span class="sxs-lookup"><span data-stu-id="377dd-121">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="377dd-122">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="377dd-122">**Resource Management**</span></span>

<span data-ttu-id="377dd-123">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="377dd-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="377dd-124">Негізгі талапты жасамас бұрын, оны тексеру үшін **PostProjectCreate** қосылатын модулінде тексеру қосылды.</span><span class="sxs-lookup"><span data-stu-id="377dd-124">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>
- <span data-ttu-id="377dd-125">Өрістер пішіннен алынып тасталған жағдайда, **Жоба тобының мүшесі** тез жасау пішіні null reference exception қатесін шығарады.</span><span class="sxs-lookup"><span data-stu-id="377dd-125">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>
- <span data-ttu-id="377dd-126">1 жылдан артық 12 сағатқа қойылатын талаптар орындалмайды.</span><span class="sxs-lookup"><span data-stu-id="377dd-126">Generate requirements for 12 hours over 1 year will fail.</span></span>
- <span data-ttu-id="377dd-127">Ресурстарға қойылатын талаптарды жасау кезіндегі null reference exception қате туралы хабары жетілдірілді.</span><span class="sxs-lookup"><span data-stu-id="377dd-127">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="377dd-128">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="377dd-128">**Project Management**</span></span>

<span data-ttu-id="377dd-129">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="377dd-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="377dd-130">**PreProjectUpdate** қосылатын модулінде құрылатын null reference exception қатесін жіберу үшін тексеру жетілдірілді.</span><span class="sxs-lookup"><span data-stu-id="377dd-130">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>
- <span data-ttu-id="377dd-131">Microsoft Project жұмыс үстелі қондырмасы жариялаған жобалар тағайындалмаған тағайындауларды жояды.</span><span class="sxs-lookup"><span data-stu-id="377dd-131">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>
- <span data-ttu-id="377dd-132">**PreValidateProjectTaskUpdate** қосылатын модуліндегі null reference exception қатесі себебінен тапсырма жобасына сілтеме жарамсыз болған кезде жаңа тексеру қосылды.</span><span class="sxs-lookup"><span data-stu-id="377dd-132">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>
- <span data-ttu-id="377dd-133">Топ мүшесі торы топ мүшесінің жазбасында нақты тағайындауларды көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="377dd-133">Team Member grid does not show distinct assignments on the team member record.</span></span>
- <span data-ttu-id="377dd-134">**PreProjectTaskDelete** қосылатын модулінде null reference exception қатесі себебінен жаңа тексеру және қате туралы хабарлалар қосылды.</span><span class="sxs-lookup"><span data-stu-id="377dd-134">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="377dd-135">**Sales**</span><span class="sxs-lookup"><span data-stu-id="377dd-135">**Sales**</span></span>

<span data-ttu-id="377dd-136">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="377dd-136">The following issues have been fixed:</span></span>

- <span data-ttu-id="377dd-137">Баға ұсынуды немесе келісім-шартта жоба негізіндегі жолды таңдағанда, **Ұсыныс** түймешігі бұрыннан бар өніммен байланысты өнім негізіндегі жолды таңдаған кезде ғана көрінуі керек.</span><span class="sxs-lookup"><span data-stu-id="377dd-137">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>
- <span data-ttu-id="377dd-138">**Create_Product** артықшылығын **Create_ProjectContract** артықшылығынан бөліңіз.</span><span class="sxs-lookup"><span data-stu-id="377dd-138">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>
- <span data-ttu-id="377dd-139">Есеп-шот жолын жою **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice** қосылатын модулінде бос сілтеме қатесіне әкеледі.</span><span class="sxs-lookup"><span data-stu-id="377dd-139">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]