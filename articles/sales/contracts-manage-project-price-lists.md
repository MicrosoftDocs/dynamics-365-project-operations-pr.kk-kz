---
title: Жоба келісім-шарттары бойынша жоба бағатізбелерін басқару
description: Бұл тақырыпта жоба келісім-шарттары бойынша жоба бағатізбелерін басқару туралы ақпарат берілген.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ffc48782394995781535ae56142dc76afeb9a040
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858570"
---
# <a name="manage-project-price-lists-on-project-contracts"></a><span data-ttu-id="514fa-103">Жоба келісім-шарттары бойынша жоба бағатізбелерін басқару</span><span class="sxs-lookup"><span data-stu-id="514fa-103">Manage project price lists on project contracts</span></span>

<span data-ttu-id="514fa-104">_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_</span><span class="sxs-lookup"><span data-stu-id="514fa-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="514fa-105">Dynamics 365 Project Operations бағдарламасындағы жоба келісім-шарттары келісім-шарттағы бірнеше сатылымның жарамды мерзімдегі бағатізбелерін қолдауға арналған.</span><span class="sxs-lookup"><span data-stu-id="514fa-105">Project contracts in Dynamics 365 Project Operations are designed to support multiple date effective sales price lists on a contract.</span></span> <span data-ttu-id="514fa-106">Project Operations бағдарламасында **Жоба бағатізбелері** деп аталатын байланысты нысан бар.</span><span class="sxs-lookup"><span data-stu-id="514fa-106">In Project Operations, there is a new associated entity called **Project Price Lists**.</span></span> <span data-ttu-id="514fa-107">Бұл нысанда жоба келісім-шарты үшін біреу көпке қатынасы бар.</span><span class="sxs-lookup"><span data-stu-id="514fa-107">This entity has a one-to-many relationship to a project contract.</span></span>

<span data-ttu-id="514fa-108">Жоба бағатізбелері жоба бойынша уақытты, материалды және шығын транзакцияларын бағалау үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="514fa-108">Project price lists are used to price time, material, and expense transactions on a project.</span></span> <span data-ttu-id="514fa-109">Келісім-шартта бір немесе бірнеше жоба бағатізбесі болған кезде, бұл бағатізбелер уақыт, материал, шығындар болжамдарын және келісім-шарт жолы арқылы келісім-шартпен байланысты жобалардағы нақты көрсеткіштерді бағалау үшін қолданылады.</span><span class="sxs-lookup"><span data-stu-id="514fa-109">When a contract has one or more project price lists, these price lists are used to price for time, material, expense estimates, and actuals on projects that are associated to the contract through the contract line.</span></span>

<span data-ttu-id="514fa-110">Жоба келісім-шартында жоба бағатізбелері болмаған кезде, сіз жобаның бағатізбелері жоқ екендігі туралы ескерту хабарын көресіз және сіздің бағалауларыңыз, нақты жобалық жұмыстар, материалдар мен шығындарыңыз бағаланбайды.</span><span class="sxs-lookup"><span data-stu-id="514fa-110">When there are no project price lists on a project contract, you will see a warning message that there are no project price lists and your estimates, actual project work, material, and expenses logged will not be priced.</span></span> <span data-ttu-id="514fa-111">Сатылым мәндері үшін баға болмайды.</span><span class="sxs-lookup"><span data-stu-id="514fa-111">There will be no price for sales values.</span></span>

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a><span data-ttu-id="514fa-112">Жоба келісім-шарты бойынша жоба бағатізбесін байланыстыру немесе ажырату</span><span class="sxs-lookup"><span data-stu-id="514fa-112">Associate or unassociate a project price list on a project contract</span></span>

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-material-and-expenses"></a><span data-ttu-id="514fa-113">Жобалық жұмыстарды, материалдарды және шығындарды бағалау үшін нақты бағатізбені жасаңыз немесе байланыстырыңыз</span><span class="sxs-lookup"><span data-stu-id="514fa-113">Create or associate a specific price list for estimating project-based work, material, and expenses</span></span>

1. <span data-ttu-id="514fa-114">Жоба келісім-шартында **Жоба бағатізбелері** қойыншасын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-114">On the project contract, select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="514fa-115">Ішкі торда **+ жаңа жоба бағатізбесін қосу** тармағын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-115">In the subgrid, select **+ Add New Project Price List**.</span></span>
3. <span data-ttu-id="514fa-116">**Жылдам жасау** жүгірткісінде бағатізбені таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-116">On the **Quick Create** slider, select a price list.</span></span> 

  <span data-ttu-id="514fa-117">Ашылмалы тізімде мәтінмәні бағатізбедегі валюта келісім-шарттағы валютамен сәйкес келетін **Сатылым** опциясына орнатылған барлық бағатізбелерді көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="514fa-117">The drop-down list shows all price lists that have the context set to **Sales**, where the currency on the price list matches the currency on the contract.</span></span>
  
4. <span data-ttu-id="514fa-118">Жоба бағатізбесі байланысының сипаттамасын енгізіп, **Сақтау** опциясын таңдаңыз, содан кейін **Жылдам жасау** жүгірткісін жабыңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-118">Enter a description for the project price list association, select **Save**, and then close the **Quick Create** slider.</span></span>

   <span data-ttu-id="514fa-119">Жоба бағатізбегінің байланысы жасалады.</span><span class="sxs-lookup"><span data-stu-id="514fa-119">A project price list association is created.</span></span>
   
5. <span data-ttu-id="514fa-120">Жоба келісім-шартымен бірнеше жоба бағатізбесін байланыстыру үшін 1-4 қадамдарын қайталаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-120">Repeat steps 1-4 to associate more than one project price list to the project contract.</span></span> <span data-ttu-id="514fa-121">Байланысқан жоба бағатізбесінің әрқайсысында жарамдылық мерзімі әртүрлі болған жағдайда ғана бірнеше жоба бағатізбелерін жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-121">Only create multiple project price lists if you have different date effectivity on each of the associated project price list.</span></span>

> [!NOTE]
> <span data-ttu-id="514fa-122">Project Operations жоба бағатізбелерінің жарамдылық мерзімінің қабаттасуына қолдау көрсетпейді.</span><span class="sxs-lookup"><span data-stu-id="514fa-122">Project Operations doesn't support overlapping the date effectivity of the project price lists.</span></span> <span data-ttu-id="514fa-123">Егер берілген күні бар транзакцияға арналған бірнеше жоба бағатізбелері болса, онда бұл транзакциядағы баға нөлге дейін әдепкі бойынша орнатылады.</span><span class="sxs-lookup"><span data-stu-id="514fa-123">If there are multiple project prices lists for a transaction with a given date, the price on that transaction will be defaulted to zero.</span></span>

### <a name="remove-a-project-price-list-association"></a><span data-ttu-id="514fa-124">Жоба бағатізбесі байланысын жою</span><span class="sxs-lookup"><span data-stu-id="514fa-124">Remove a project price list association</span></span>

- <span data-ttu-id="514fa-125">Жоба бағатізбесін таңдаңыз, содан кейін ішкі торда **Келісім-шарт жобасының бағатізбесін жою** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-125">Select the project price list, and then select **Delete Contract Project Price List** on the subgrid.</span></span> 

  <span data-ttu-id="514fa-126">Бағатізбе келісім-шарттағы жоба бағатізбелерінен жойылады.</span><span class="sxs-lookup"><span data-stu-id="514fa-126">The price list is removed from the project price lists on the contract.</span></span> <span data-ttu-id="514fa-127">Бағатізбенің өзі жойылмайды.</span><span class="sxs-lookup"><span data-stu-id="514fa-127">The price list itself will not be deleted.</span></span> <span data-ttu-id="514fa-128">Тек келісім-шартпен байланыс жойылады.</span><span class="sxs-lookup"><span data-stu-id="514fa-128">Only the association to the contract will be deleted.</span></span>

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a><span data-ttu-id="514fa-129">Келісім-шарттағы жоба бағатізбелерінің әдепкі мәндерін автоматты түрде орнату</span><span class="sxs-lookup"><span data-stu-id="514fa-129">Set up automatic defaulting of project price lists on a contract</span></span>

<span data-ttu-id="514fa-130">Жоба бағатізбесін әдепкі жоба бағатізбе ретінде орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="514fa-130">A project price list can be set up as the default project price list.</span></span> <span data-ttu-id="514fa-131">Бұл орнатылым ұйымыңыздағы барлық келісім-шарттардың әрқашан осы баға кезеңіне арналған стандартты жоба бағатізбесінен басталуын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="514fa-131">This setup ensures that all contracts in your organization always start with a standard project price list for that price period.</span></span>

### <a name="set-up-the-organizational-default-for-project-price-lists"></a><span data-ttu-id="514fa-132">Жоба бағатізбелері үшін ұйымның әдепкі мәнін орнату</span><span class="sxs-lookup"><span data-stu-id="514fa-132">Set up the organizational default for project price lists</span></span>

1. <span data-ttu-id="514fa-133">**Параметрлер** > **Жалпы** тармағына өтіп, **Параметрлер** опциясын таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-133">Go to **Settings** > **General**, and then select **Parameters**.</span></span>
2. <span data-ttu-id="514fa-134">**Белсенді параметрлер** тізім бетінде жазбаны ашу үшін оны таңдап, екі рет басыңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-134">In the **Active Parameters** list page, select and double-click the record to open it.</span></span> <span data-ttu-id="514fa-135">Екі рет басу кезінде гиперсілтеме болып табылатын өріс мәнін баспағаныңызға көз жеткізіңіз.</span><span class="sxs-lookup"><span data-stu-id="514fa-135">While double–clicking, make sure that you are not clicking on a field value that is hyperlink.</span></span> 
3. <span data-ttu-id="514fa-136">**Белсенді параметрлер** бетінде **Бағатізбе** қойыншасын таңдаңыз. Ішкі тор әдепкі бағатізбелердің тізімін көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="514fa-136">On the **Active Parameters** page, select the **Price List** tab. A subgrid shows a list of default price lists.</span></span> <span data-ttu-id="514fa-137">Бұл — стандартты құн мен сатылым бағатізбелерінің тізімі.</span><span class="sxs-lookup"><span data-stu-id="514fa-137">This is a list of standard cost and sales price lists.</span></span> <span data-ttu-id="514fa-138">Сіз сататын әр валютамен **Сатылым** бағатізбесін байланыстыру сатылым бағатізбесінің осы валютада транзакциясын жасайтын тұтынушылар үшін жасаған кез келген келісім-шарт үшін стандартты болуын қамтамасыз етеді.</span><span class="sxs-lookup"><span data-stu-id="514fa-138">Having a **Sales** price list associated here for every currency that you sell in ensures that the sales price list is the default on any contract that you create for customers that transact in this currency.</span></span>

### <a name="set-up-a-customer-specific-project-price-list"></a><span data-ttu-id="514fa-139">Тұтынушыларға арналған жоба бағатізбесін орнату</span><span class="sxs-lookup"><span data-stu-id="514fa-139">Set up a customer-specific project price list</span></span>

<span data-ttu-id="514fa-140">Сіз сондай-ақ тұтынушылармен нақты баға келісімі бойынша келіссөздер жүргізген кезде тұтынушыларға арналған жоба бағатізбелерін орната аласыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-140">You can also set up customer–specific project price lists when you have negotiated a master pricing agreement with your customers.</span></span>

1. <span data-ttu-id="514fa-141">**Сатылым** > **Тұтынушылар** тармағына өтіңіз.</span><span class="sxs-lookup"><span data-stu-id="514fa-141">Go to **Sales** > **Customers**.</span></span>
2. <span data-ttu-id="514fa-142">Белсенді тіркелгілер тізімінен арнайы бағатізбесі бар тұтынушыны таңдаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-142">From the list of active accounts, select the customer for whom have special price list.</span></span>
3. <span data-ttu-id="514fa-143">Ашу үшін тұтынушы жазбасын таңдап, содан кейін **Жоба бағатізбелері** қойыншасын таңдаңыз. Ішкі торда осы тұтынушыға арналған жоба бағатізбелерінің тізімі көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="514fa-143">Select the customer record to open it and then select the **Project Price Lists** tab. A subgrid shows a list of project price lists specific to this customer.</span></span> 
4. <span data-ttu-id="514fa-144">Осы тұтынушыға арналған жоба бағатізбесі болу үшін мұнда жаңа бағатізбе байланысын жасаңыз.</span><span class="sxs-lookup"><span data-stu-id="514fa-144">Create a new price list association here to have project price list specific to this customer.</span></span>

## <a name="custom-pricing-on-a-project-contract"></a><span data-ttu-id="514fa-145">Жоба келісім-шарты бойынша реттелетін баға</span><span class="sxs-lookup"><span data-stu-id="514fa-145">Custom pricing on a project contract</span></span>

<span data-ttu-id="514fa-146">Сізде ұйымға және тұтынушыға арналған әдепкі жоба бағатізбелері болғаннан кейін, жоба келісім-шарттары осы жоба бағатізбесінің байланысымен автоматты түрде жасалады.</span><span class="sxs-lookup"><span data-stu-id="514fa-146">After you have organizational and customer-specific default project price lists, your project contracts will be created with these project price list associations automatically.</span></span> <span data-ttu-id="514fa-147">Алайда жоба келісім-шарты бойынша жоба бағатізбелері әрқашан оларға қосылған күн мен келісім-шарт атауымен көшіріледі.</span><span class="sxs-lookup"><span data-stu-id="514fa-147">However, project price lists on a project contract are always copied with the date and contract name appended to them.</span></span> <span data-ttu-id="514fa-148">Содан кейін тіркелгі және жоба менеджерлері осы көшірмелердегі бағаларға түзетулер енгізе бастайды.</span><span class="sxs-lookup"><span data-stu-id="514fa-148">The account and project managers can then begin making edits to prices on these copies.</span></span> <span data-ttu-id="514fa-149">Бұл өзгертілген бағалар тек осы жоба келісім-шартына қолданылатын болады.</span><span class="sxs-lookup"><span data-stu-id="514fa-149">These changed prices will be applicable to this project contract only.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
