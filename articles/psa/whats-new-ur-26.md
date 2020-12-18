---
title: Project Service Automation бағдарламасының 26-жаңарту шығарылымы, 3-нұсқасындағы жаңалықтар немесе өзгерістер
ms.openlocfilehash: 849e7288ee91d3e9360c0b03f6b8b37ff29338e7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643270"
---
<a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="881f6-102">Project Service Automation бағдарламасының 26-жаңарту шығарылымының 3-нұсқасы</span><span class="sxs-lookup"><span data-stu-id="881f6-102">Project Service Automation Update Release 26, V3</span></span>
================================================

<span data-ttu-id="881f6-103">Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз.</span><span class="sxs-lookup"><span data-stu-id="881f6-103">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="881f6-104">Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.</span><span class="sxs-lookup"><span data-stu-id="881f6-104">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="881f6-105">Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді.</span><span class="sxs-lookup"><span data-stu-id="881f6-105">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="881f6-106">Бұл шығарылымды жаңарту үшін, жаңартуды орнату мақсатында Dynamics 365 онлайн шешімдер бетінің басқару орталығына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="881f6-106">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="881f6-107">Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.</span><span class="sxs-lookup"><span data-stu-id="881f6-107">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="881f6-108">Бұл бөлімде Project Service Automation бағдарламасының 26-жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген.</span><span class="sxs-lookup"><span data-stu-id="881f6-108">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="881f6-109">Бұл нұсқаның құрастыру нөмірі — V3.10.44.59 және бұл нұсқа әдетте 2020 жылдың желтоқсан айында дербес жаңарту арқылы қолжетімді.</span><span class="sxs-lookup"><span data-stu-id="881f6-109">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

<a name="update-release-26"></a><span data-ttu-id="881f6-110">26-жаңарту шығарылымы</span><span class="sxs-lookup"><span data-stu-id="881f6-110">Update Release 26</span></span>
-----------------

### <a name="bug-fixes"></a><span data-ttu-id="881f6-111">Қателерді түзету</span><span class="sxs-lookup"><span data-stu-id="881f6-111">Bug fixes</span></span>

<span data-ttu-id="881f6-112">**Уақыт және шығыс**</span><span class="sxs-lookup"><span data-stu-id="881f6-112">**Time and Expense**</span></span>

<span data-ttu-id="881f6-113">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="881f6-113">The following issues have been fixed:</span></span>

-   <span data-ttu-id="881f6-114">Пайдаланушылар тапсырманы бекітілген/жіберілген уақыт жазбасы бойынша өзгерте алады.</span><span class="sxs-lookup"><span data-stu-id="881f6-114">Users are able to change the task on a time entry that has been approved/submitted.</span></span>

-   <span data-ttu-id="881f6-115">Уақыт жазбасын сақтау кезінде "Нысан сілтемесі орнатылмаған" қатесі орын алды.</span><span class="sxs-lookup"><span data-stu-id="881f6-115">"Object Reference Not Set" error when saving time entry.</span></span>

-   <span data-ttu-id="881f6-116">Ресурс тағайындауларынан уақыт жазбасының импорты DateTime мәні дұрыс емес уақыт жазбаларын жасайды.</span><span class="sxs-lookup"><span data-stu-id="881f6-116">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>

-   <span data-ttu-id="881f6-117">Project Service Automation және Field Service бағдарламаларының екеуі де орнатылған кезде, **Жаңа** түймешігі Field Service бағдарламасындағы уақыт жазбалары үшін пәрмен жолағында екі рет көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="881f6-117">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>

-   <span data-ttu-id="881f6-118">**Рұқсат етілген бірлік** және **Бірлік тобы** ұяшықтарының жаңартулары қазір **Шығын болжамдары** торында іске асырылады.</span><span class="sxs-lookup"><span data-stu-id="881f6-118">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>

-   <span data-ttu-id="881f6-119">**Уақыт жазбасын өңдеуді жаңарту** пішіні **Уақыт шкаласы** ұяшығын қамтиды.</span><span class="sxs-lookup"><span data-stu-id="881f6-119">**Update Time Entry Edit** form includes **Timeline**.</span></span>

-   <span data-ttu-id="881f6-120">Жобадан тыс уақыт жазбаларына арналған уақыт растауы жобаны растаушы рөлін іздеу кезінде жүйені бұғаттайды.</span><span class="sxs-lookup"><span data-stu-id="881f6-120">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="881f6-121">**Ресурсты басқару**</span><span class="sxs-lookup"><span data-stu-id="881f6-121">**Resource Management**</span></span>

<span data-ttu-id="881f6-122">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="881f6-122">The following issues have been fixed:</span></span>

-   <span data-ttu-id="881f6-123">Негізгі талапты жасамас бұрын, оны тексеру үшін **PostProjectCreate** қосылатын модулінде тексеру қосылды.</span><span class="sxs-lookup"><span data-stu-id="881f6-123">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>

-   <span data-ttu-id="881f6-124">Өрістер пішіннен алынып тасталған жағдайда, **Жоба тобының мүшесі** тез жасау пішіні null reference exception қатесін шығарады.</span><span class="sxs-lookup"><span data-stu-id="881f6-124">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>

-   <span data-ttu-id="881f6-125">1 жылдан артық 12 сағатқа қойылатын талаптар орындалмайды.</span><span class="sxs-lookup"><span data-stu-id="881f6-125">Generate requirements for 12 hours over 1 year will fail.</span></span>

-   <span data-ttu-id="881f6-126">Ресурстарға қойылатын талаптарды жасау кезіндегі null reference exception қате туралы хабары жетілдірілді.</span><span class="sxs-lookup"><span data-stu-id="881f6-126">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="881f6-127">**Жоба басқармасы**</span><span class="sxs-lookup"><span data-stu-id="881f6-127">**Project Management**</span></span>

<span data-ttu-id="881f6-128">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="881f6-128">The following issues have been fixed:</span></span>

-   <span data-ttu-id="881f6-129">**PreProjectUpdate** қосылатын модулінде құрылатын null reference exception қатесін жіберу үшін тексеру жетілдірілді.</span><span class="sxs-lookup"><span data-stu-id="881f6-129">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>

-   <span data-ttu-id="881f6-130">Microsoft Project жұмыс үстелі қондырмасы жариялаған жобалар тағайындалмаған тағайындауларды жояды.</span><span class="sxs-lookup"><span data-stu-id="881f6-130">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>

-   <span data-ttu-id="881f6-131">**PreValidateProjectTaskUpdate** қосылатын модуліндегі null reference exception қатесі себебінен тапсырма жобасына сілтеме жарамсыз болған кезде жаңа тексеру қосылды.</span><span class="sxs-lookup"><span data-stu-id="881f6-131">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>

-   <span data-ttu-id="881f6-132">Топ мүшесі торы топ мүшесінің жазбасында нақты тағайындауларды көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="881f6-132">Team Member grid does not show distinct assignments on the team member record.</span></span>

-   <span data-ttu-id="881f6-133">**PreProjectTaskDelete** қосылатын модулінде null reference exception қатесі себебінен жаңа тексеру және қате туралы хабарлалар қосылды.</span><span class="sxs-lookup"><span data-stu-id="881f6-133">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="881f6-134">**Sales**</span><span class="sxs-lookup"><span data-stu-id="881f6-134">**Sales**</span></span>

<span data-ttu-id="881f6-135">Келесі мәселелер түзетілді:</span><span class="sxs-lookup"><span data-stu-id="881f6-135">The following issues have been fixed:</span></span>

-   <span data-ttu-id="881f6-136">Баға ұсынуды немесе келісім-шартта жоба негізіндегі жолды таңдағанда, **Ұсыныс** түймешігі бұрыннан бар өніммен байланысты өнім негізіндегі жолды таңдаған кезде ғана көрінуі керек.</span><span class="sxs-lookup"><span data-stu-id="881f6-136">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>

-   <span data-ttu-id="881f6-137">**Create_Product** артықшылығын **Create_ProjectContract** артықшылығынан бөліңіз.</span><span class="sxs-lookup"><span data-stu-id="881f6-137">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>

-   <span data-ttu-id="881f6-138">Есеп-шот жолын жою **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice** қосылатын модулінде бос сілтеме қатесіне әкеледі.</span><span class="sxs-lookup"><span data-stu-id="881f6-138">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>
