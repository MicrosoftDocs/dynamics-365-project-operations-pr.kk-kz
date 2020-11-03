---
title: iOS және Android жүйесіндегі Microsoft Dynamics 365 Project Timesheet мобильді құрылғы бағдарламасы үшін реттелмелі өрістерді ендіру
description: Бұл тақырыпта реттелмелі өрістерді ендіру үшін кеңейтімдерді пайдалануға арналған жалпы үлгілер беріледі.
author: Yowelle
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 1ea1ca002a8f68f86808831b398e452244471322
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079714"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a><span data-ttu-id="a459e-103">iOS және Android жүйесіндегі Microsoft Dynamics 365 Project Timesheet мобильді құрылғы бағдарламасы үшін реттелмелі өрістерді ендіру</span><span class="sxs-lookup"><span data-stu-id="a459e-103">Implement custom fields for the Microsoft Dynamics 365 Project Timesheet mobile app on iOS and Android</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="a459e-104">Бұл тақырыпта реттелмелі өрістерді ендіру үшін кеңейтімдерді пайдалануға арналған жалпы үлгілер беріледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-104">This topic provides common patterns for using extensions to implement custom fields.</span></span> <span data-ttu-id="a459e-105">Келесі тақырыптарда қамтылады:</span><span class="sxs-lookup"><span data-stu-id="a459e-105">The following topics are covered:</span></span>

- <span data-ttu-id="a459e-106">Реттелмелі өріс құрылымында қолдау көрсетілетін әртүрлі деректер түрлері</span><span class="sxs-lookup"><span data-stu-id="a459e-106">The various data types that the custom field framework supports</span></span>
- <span data-ttu-id="a459e-107">Уақыт кестесінің жазбаларында тек оқуға арналған немесе өңделетін өрістерді көрсету және пайдаланушы ұсынған мәндерді дерекқорға сақтау жолы</span><span class="sxs-lookup"><span data-stu-id="a459e-107">How to show read-only or editable fields on timesheet entries, and save user-provided values back to the database</span></span>
- <span data-ttu-id="a459e-108">Уақыт кестесінің тақырыбында тек оқуға арналған өрістерді көрсету жолы</span><span class="sxs-lookup"><span data-stu-id="a459e-108">How to show read-only fields on the timesheet header</span></span>
- <span data-ttu-id="a459e-109">Әдепкі мәндерді өрістерге енгізіп, қосымша тексеру жүргізу үшін басқа реттелмелі бизнес логикасын біріктіру жолы</span><span class="sxs-lookup"><span data-stu-id="a459e-109">How to integrate other custom business logic to enter default values in fields and do additional validation</span></span>

## <a name="audience"></a><span data-ttu-id="a459e-110">Аудитория</span><span class="sxs-lookup"><span data-stu-id="a459e-110">Audience</span></span>

<span data-ttu-id="a459e-111">Бұл тақырып реттелмелі өрістерін Apple iOS және Google Android үшін қолжетімді болатын Microsoft Dynamics 365 Project Timesheet мобильді құрылғы бағдарламасында біріктіретін әзірлеушілерге арналған.</span><span class="sxs-lookup"><span data-stu-id="a459e-111">This topic is intended for developers who are integrating their custom fields into the Microsoft Dynamics 365 Project Timesheet mobile application that is available for Apple iOS and Google Android.</span></span> <span data-ttu-id="a459e-112">Оқырмандар X++ әзірлеуімен және жобаның уақыт кестесі функциясымен таныс деп болжанады.</span><span class="sxs-lookup"><span data-stu-id="a459e-112">The assumption is that readers are familiar with X++ development and project timesheet functionality.</span></span>

## <a name="data-contract--tstimesheetcustomfield-x-class"></a><span data-ttu-id="a459e-113">Деректер келісім-шарты – TSTimesheetCustomField X++ класы</span><span class="sxs-lookup"><span data-stu-id="a459e-113">Data contract – TSTimesheetCustomField X++ class</span></span>

<span data-ttu-id="a459e-114">**TSTimesheetCustomField** класы – уақыт кестесі функциясы үшін реттелмелі өріс туралы ақпаратты көрсететін X++ деректер келісім-шарты класы.</span><span class="sxs-lookup"><span data-stu-id="a459e-114">The **TSTimesheetCustomField** class is the X++ data contract class that represents information about a custom field for timesheet functionality.</span></span> <span data-ttu-id="a459e-115">Мобильді құрылғы бағдарламасында реттелмелі өрістерді көрсету үшін реттелмелі өріс нысандарының тізімдері TSTimesheetDetails деректер келісім-шартында да, TSTimesheetEntry деректер келісім-шартында да беріледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-115">Lists of the custom field objects are passed on both the TSTimesheetDetails data contract and the TSTimesheetEntry data contract to show custom fields in the mobile app.</span></span>

- <span data-ttu-id="a459e-116">**TSTimesheetDetails** - уақыт кестесінің тақырып келісім-шарты.</span><span class="sxs-lookup"><span data-stu-id="a459e-116">**TSTimesheetDetails** - The timesheet header contract.</span></span>
- <span data-ttu-id="a459e-117">**TSTimesheetEntry** - уақыт кестесінің транзакция келісім-шарты.</span><span class="sxs-lookup"><span data-stu-id="a459e-117">**TSTimesheetEntry** - The timesheet transaction contract.</span></span> <span data-ttu-id="a459e-118">Бірдей жоба туралы ақпарат пен **timesheetLineRecId** мәні бар осы нысандардың топтары жол құрайды.</span><span class="sxs-lookup"><span data-stu-id="a459e-118">Groups of these objects that have the same project information and **timesheetLineRecId** value constitute a line.</span></span>

### <a name="fieldbasetype-types"></a><span data-ttu-id="a459e-119">fieldBaseType (түрлері)</span><span class="sxs-lookup"><span data-stu-id="a459e-119">fieldBaseType (Types)</span></span>

<span data-ttu-id="a459e-120">**TsTimesheetCustom** нысанындағы **FieldBaseType** сипаты бағдарламаларда пайда болатын өріс түрін анықтайды.</span><span class="sxs-lookup"><span data-stu-id="a459e-120">The **FieldBaseType** property on the **TsTimesheetCustom** object determines the type of the field that appears in the app.</span></span> <span data-ttu-id="a459e-121">Қолдау көрсетілетін келесі **Түрлер** мәндері.</span><span class="sxs-lookup"><span data-stu-id="a459e-121">The following **Types** values that are supported.</span></span>

| <span data-ttu-id="a459e-122">Түрлер мәні</span><span class="sxs-lookup"><span data-stu-id="a459e-122">Types value</span></span> | <span data-ttu-id="a459e-123">Түрі</span><span class="sxs-lookup"><span data-stu-id="a459e-123">Type</span></span>              | <span data-ttu-id="a459e-124">Есктулер</span><span class="sxs-lookup"><span data-stu-id="a459e-124">Notes</span></span> |
|-------------|-------------------|-------|
| <span data-ttu-id="a459e-125">0</span><span class="sxs-lookup"><span data-stu-id="a459e-125">0</span></span>           | <span data-ttu-id="a459e-126">Жол (және бағалау)</span><span class="sxs-lookup"><span data-stu-id="a459e-126">String (and Enum)</span></span> | <span data-ttu-id="a459e-127">Өріс мәтін өрісі ретінде пайда болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-127">The field appears as a text field.</span></span> |
| <span data-ttu-id="a459e-128">1</span><span class="sxs-lookup"><span data-stu-id="a459e-128">1</span></span>           | <span data-ttu-id="a459e-129">Integer</span><span class="sxs-lookup"><span data-stu-id="a459e-129">Integer</span></span>           | <span data-ttu-id="a459e-130">Мән ондық белгілері жоқ сан ретінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-130">The value is shown as a number without decimal places.</span></span> |
| <span data-ttu-id="a459e-131">2</span><span class="sxs-lookup"><span data-stu-id="a459e-131">2</span></span>           | <span data-ttu-id="a459e-132">Нақты</span><span class="sxs-lookup"><span data-stu-id="a459e-132">Real</span></span>              | <span data-ttu-id="a459e-133">Мән ондық белгілері бар сан ретінде көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-133">The value is shown as a number that has decimal places.</span></span><p><span data-ttu-id="a459e-134">Нақты мәндерді бағдарламада ағымдағы мән ретінде көрсету үшін, **fieldExtenededType** сипатын пайдаланыңыз.</span><span class="sxs-lookup"><span data-stu-id="a459e-134">To show the real value as a currency in the app, use the **fieldExtenededType** property.</span></span> <span data-ttu-id="a459e-135">Көрсетілетін ондық белгілердің санын орнату үшін **numberOfDecimals** сипатын пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-135">You can use the **numberOfDecimals** property to set the number of decimal places that are shown.</span></span></p> |
| <span data-ttu-id="a459e-136">3</span><span class="sxs-lookup"><span data-stu-id="a459e-136">3</span></span>           | <span data-ttu-id="a459e-137">Күн</span><span class="sxs-lookup"><span data-stu-id="a459e-137">Date</span></span>              | <span data-ttu-id="a459e-138">Күн пішімдері **Пайдаланушы параметрлері** ішіндегі **Тіл және ел/аймақ параметрі** астында көрсетілген пайдаланушының **Күні, уақыттар және нөмір пішімі** бойынша анықталады.</span><span class="sxs-lookup"><span data-stu-id="a459e-138">Date formats are determined by the user's **Date, times, and number format** setting that is specified under **Language and country/region preference** in **User options**.</span></span> |
| <span data-ttu-id="a459e-139">4</span><span class="sxs-lookup"><span data-stu-id="a459e-139">4</span></span>           | <span data-ttu-id="a459e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="a459e-140">Boolean</span></span>           | |
| <span data-ttu-id="a459e-141">15</span><span class="sxs-lookup"><span data-stu-id="a459e-141">15</span></span>          | <span data-ttu-id="a459e-142">GUID</span><span class="sxs-lookup"><span data-stu-id="a459e-142">GUID</span></span>              | |
| <span data-ttu-id="a459e-143">16</span><span class="sxs-lookup"><span data-stu-id="a459e-143">16</span></span>          | <span data-ttu-id="a459e-144">Int64</span><span class="sxs-lookup"><span data-stu-id="a459e-144">Int64</span></span>             | |

- <span data-ttu-id="a459e-145">**stringOptions** сипаты **TSTimesheetCustomField** нысанында берілмесе, пайдаланушыға еркін мәтін өрісі беріледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-145">If the **stringOptions** property isn't provided on the **TSTimesheetCustomField** object, a free-text field is provided to the user.</span></span>

    <span data-ttu-id="a459e-146">**stringLength** сипатын пайдаланушылар енгізе алатын максималды жол ұзындығын орнату үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-146">The **stringLength** property can be used to set the maximum string length that users can enter.</span></span>

- <span data-ttu-id="a459e-147">**stringOptions** сипаты **TSTimesheetCustomField** нысанында берілсе, осы тізім элементтері пайдаланушылар ажыратпа-қосқыштар (радио түймешіктер) көмегімен таңдай алатын мәндер болып табылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-147">If the **stringOptions** property is provided on the **TSTimesheetCustomField** object, those list elements are the only values that users can select by using option buttons (radio buttons).</span></span>

    <span data-ttu-id="a459e-148">Бұл жағдайда жол өрісі пайдаланушы жазбасының мақсатында бағалау өрісі ретінде әрекет етеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-148">In this case, the string field can act as an enum value for the purpose of user entry.</span></span> <span data-ttu-id="a459e-149">Мәнді дерекқорға бағалау мәні ретінде сақтау үшін, пәрмен тізбегінің көмегімен дерекқорға сақтау алдында жол мәнін бағалау мәнімен қолмен салыстырыңыз (Мысалды кейін осы тақырыптағы “Уақыт кестесінің жазбасын бағдарламадан дерекқорға сақтау үшін TSTimesheetEntryService класындағы пәрмен тізбегін пайдалану” бөлімінен қараңыз).</span><span class="sxs-lookup"><span data-stu-id="a459e-149">To save the value to the database as an enum, manually map the string value back to the enum value before you save to the database by using chain of command (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a><span data-ttu-id="a459e-150">fieldExtendedType (TSCustomFieldExtendedType)</span><span class="sxs-lookup"><span data-stu-id="a459e-150">fieldExtendedType (TSCustomFieldExtendedType)</span></span>

<span data-ttu-id="a459e-151">Бұл сипатты нақты мәндерді ағымдағы мәндер ретінде пішімдеу үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-151">You can use this property to format real values as currency.</span></span> <span data-ttu-id="a459e-152">Бұл тәсілді **fieldBaseType** мәні **Нақты** мән болған кезде қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-152">This approach is applicable only when the **fieldBaseType** value is **Real**.</span></span>

- <span data-ttu-id="a459e-153">**TSCustomFieldExtendedType:жоқ** – пішімдеу қолданылмайды.</span><span class="sxs-lookup"><span data-stu-id="a459e-153">**TSCustomFieldExtendedType:None** – No formatting is applied.</span></span>
- <span data-ttu-id="a459e-154">**TSCustomFieldExtendedType::ағымдағы** – мәнді ағымдағы мән ретінде пішімдеу.</span><span class="sxs-lookup"><span data-stu-id="a459e-154">**TSCustomFieldExtendedType::Currency** – Format the value as currency.</span></span>

    <span data-ttu-id="a459e-155">Ағымдағы пішімдеу белсенді болған кезде, **stringValue** өрісін бағдарламада көрсетілуі керек валюта кодын өткізу үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-155">When currency formatting is active, the **stringValue** field can be used pass the currency code that should be shown in the app.</span></span> <span data-ttu-id="a459e-156">Мән – тек оқуға арналған мән.</span><span class="sxs-lookup"><span data-stu-id="a459e-156">The value is a read-only value.</span></span>

    <span data-ttu-id="a459e-157">**realValue** өрісінде дерекқорға сақталуы керек ақша мөлшері бар.</span><span class="sxs-lookup"><span data-stu-id="a459e-157">The **realValue** field contains the money amount that should be saved to the database.</span></span>

### <a name="fieldsection-tscustomfieldsection"></a><span data-ttu-id="a459e-158">fieldSection (TSCustomFieldSection)</span><span class="sxs-lookup"><span data-stu-id="a459e-158">fieldSection (TSCustomFieldSection)</span></span>

<span data-ttu-id="a459e-159">Бұл сипатты бағдарламада пайда болуы керек реттелмелі өрісті көрсету үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-159">You can use this property specify where the custom field should appear in the app.</span></span>

- <span data-ttu-id="a459e-160">**TSCustomFieldSection::тақырып** – өріс бағдарламадағы **Қосымша мәліметтерді көру** бөлімінде пайда болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-160">**TSCustomFieldSection::Header** – The field will appear in the **View more details** section in the app.</span></span> <span data-ttu-id="a459e-161">Осы өрістер әрқашан тек оқуға арналады.</span><span class="sxs-lookup"><span data-stu-id="a459e-161">These fields are always read-only.</span></span>
- <span data-ttu-id="a459e-162">**TSCustomFieldSection::жол** – өріс уақыт кестесінің жазбаларындағы барлық кірістірілген жол өрістерінен кейін пайда болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-162">**TSCustomFieldSection::Line** – The field will appear after all the out-of-box line fields on timesheet entries.</span></span> <span data-ttu-id="a459e-163">Осы өрістерді өңдеуге немесе тек оқуға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-163">These fields can be either editable or read-only.</span></span>

### <a name="fieldname-fieldnameshort"></a><span data-ttu-id="a459e-164">fieldName (FieldNameShort)</span><span class="sxs-lookup"><span data-stu-id="a459e-164">fieldName (FieldNameShort)</span></span>

<span data-ttu-id="a459e-165">Бұл сипат өрісті бағдарлама беретін мәндер дерекқорға қайта сақталған кезде анықтайды.</span><span class="sxs-lookup"><span data-stu-id="a459e-165">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="tablename-tablenameshort"></a><span data-ttu-id="a459e-166">tableName (TableNameShort)</span><span class="sxs-lookup"><span data-stu-id="a459e-166">tableName (TableNameShort)</span></span>

<span data-ttu-id="a459e-167">Бұл сипат өрісті бағдарлама беретін мәндер дерекқорға қайта сақталған кезде анықтайды.</span><span class="sxs-lookup"><span data-stu-id="a459e-167">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="iseditable-noyes"></a><span data-ttu-id="a459e-168">isEditable (NoYes)</span><span class="sxs-lookup"><span data-stu-id="a459e-168">isEditable (NoYes)</span></span>

<span data-ttu-id="a459e-169">Бұл сипатты уақыт кестесінің жазбасы бөліміндегі өрісті пайдаланушылар өңдей алатынын көрсету үшін **Иә** параметріне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a459e-169">Set this property to **Yes** to specify that the field in the timesheet entry section should be editable by users.</span></span> <span data-ttu-id="a459e-170">Өрісті тек оқуға арналған ету үшін сипатты **Жоқ** параметріне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a459e-170">Set the property to **No** to make the field read-only.</span></span>

### <a name="ismandatory-noyes"></a><span data-ttu-id="a459e-171">isMandatory (NoYes)</span><span class="sxs-lookup"><span data-stu-id="a459e-171">isMandatory (NoYes)</span></span>

<span data-ttu-id="a459e-172">Бұл сипатты уақыт кестесінің жазба бөліміндегі өріс міндетті екенін көрсету үшін **Иә** параметріне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a459e-172">Set this property to **Yes** to specify that the field in the timesheet entry section should be mandatory.</span></span>

### <a name="label-str"></a><span data-ttu-id="a459e-173">белгі (жол)</span><span class="sxs-lookup"><span data-stu-id="a459e-173">label (str)</span></span>

<span data-ttu-id="a459e-174">Бұл сипат бағдарламадағы келесі өрісте көрсетілетін белгіні көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-174">This property specifies the label that is shown next the field in the app.</span></span>

### <a name="stringoptions-list-of-strings"></a><span data-ttu-id="a459e-175">stringOptions (жолдар тізімі)</span><span class="sxs-lookup"><span data-stu-id="a459e-175">stringOptions (List of Strings)</span></span>

<span data-ttu-id="a459e-176">Бұл сипатты **fieldBaseType** мәні **Жол** мәніне орнатылған кезде қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-176">This property is applicable only when **fieldBaseType** is set to **String**.</span></span> <span data-ttu-id="a459e-177">**stringOptions** сипаты орнатылса, ажыратпа-қосқыштар (радио түймешіктер) арқылы таңдау үшін қолжетімді болатын жол мәндері тізімдегі жол арқылы көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-177">If **stringOptions** is set, the string values that are available for selection via option buttons (radio buttons) are specified by the strings in the list.</span></span> <span data-ttu-id="a459e-178">Егер жол берілмесе, жол өрісіндегі еркін мәтін жазбасына рұқсат етіледі (Мысалды кейін осы тақырыптағы “Уақыт кестесінің жазбасын бағдарламадан дерекқорға сақтау үшін TSTimesheetEntryService класындағы пәрмен тізбегін пайдалану” бөлімінен қараңыз).</span><span class="sxs-lookup"><span data-stu-id="a459e-178">If no strings are provided, free-text entry in the string field is allowed (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="stringlength-int"></a><span data-ttu-id="a459e-179">stringLength (int)</span><span class="sxs-lookup"><span data-stu-id="a459e-179">stringLength (int)</span></span>

<span data-ttu-id="a459e-180">Бұл сипат жол өрісі үшін максималды ұзындықты көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-180">This property specifies the maximum length for a string field.</span></span> <span data-ttu-id="a459e-181">Оны **fieldBaseType** мәні **Жол** мәніне орнатылған кезде қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-181">It's applicable only when **fieldBaseType** is set to **String**.</span></span>

### <a name="numberofdecimals-int"></a><span data-ttu-id="a459e-182">numberOfDecimals (int)</span><span class="sxs-lookup"><span data-stu-id="a459e-182">numberOfDecimals (int)</span></span>

<span data-ttu-id="a459e-183">Бұл сипат нақты өріс үшін көрсетілетін ондық белгілердің санын көрсетеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-183">This property specifies the number of decimal places that are shown for a real field.</span></span> <span data-ttu-id="a459e-184">Оны тек **fieldBaseType** мәні **Нақты** мәнге орнатылған кезде қолдануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-184">It's applicable only when **fieldBaseType** is set to **Real**.</span></span>

### <a name="ordersequence-int"></a><span data-ttu-id="a459e-185">orderSequence (int)</span><span class="sxs-lookup"><span data-stu-id="a459e-185">orderSequence (int)</span></span>

<span data-ttu-id="a459e-186">Бұл сипат бірнеше реттелмелі өріс көрсетілген кезде бағдарламада реттелмелі өрістердің көрсетілу ретін басқарады.</span><span class="sxs-lookup"><span data-stu-id="a459e-186">This property controls the order in which the custom fields are shown in the app when more than one custom field is specified.</span></span> <span data-ttu-id="a459e-187">Алдымен төмен саны бар өрістер көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-187">Fields that have lower numbers are shown first.</span></span>

### <a name="booleanvalue-boolean"></a><span data-ttu-id="a459e-188">booleanValue (логикалық)</span><span class="sxs-lookup"><span data-stu-id="a459e-188">booleanValue (boolean)</span></span>

<span data-ttu-id="a459e-189">**Логикалық** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің логикалық мәнін өткізеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-189">For fields of the **Boolean** type, this property passes the Boolean value of the field between the server and the app.</span></span>

### <a name="guidvalue-guid"></a><span data-ttu-id="a459e-190">guidValue (guid)</span><span class="sxs-lookup"><span data-stu-id="a459e-190">guidValue (guid)</span></span>

<span data-ttu-id="a459e-191">**GUID** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің глобалдық бірегей идентификатор (GUID) мәнін өткізеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-191">For fields of the **GUID** type, this property passes the globally unique identifier (GUID) value of the field between the server and the app.</span></span>

### <a name="int64value-int64"></a><span data-ttu-id="a459e-192">int64Value (int64)</span><span class="sxs-lookup"><span data-stu-id="a459e-192">int64Value (int64)</span></span>

<span data-ttu-id="a459e-193">**Int64** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің int64 мәнін өткізеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-193">For fields of the **Int64** type, this property passes the int64 value of the field between the server and the app.</span></span>

### <a name="intvalue-int"></a><span data-ttu-id="a459e-194">intValue (int)</span><span class="sxs-lookup"><span data-stu-id="a459e-194">intValue (int)</span></span>

<span data-ttu-id="a459e-195">**Int** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің int мәнін өткізеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-195">For fields of the **Int** type, this property passes the int value of the field between the server and the app.</span></span>

### <a name="realvalue-real"></a><span data-ttu-id="a459e-196">realValue (нақты)</span><span class="sxs-lookup"><span data-stu-id="a459e-196">realValue (real)</span></span>

<span data-ttu-id="a459e-197">**Нақты** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің нақты мәнін өткізеді .</span><span class="sxs-lookup"><span data-stu-id="a459e-197">For fields of the **Real** type, this property passes the real value of the field between the server and the app .</span></span>

### <a name="stringvalue-str"></a><span data-ttu-id="a459e-198">stringValue (str)</span><span class="sxs-lookup"><span data-stu-id="a459e-198">stringValue (str)</span></span>

<span data-ttu-id="a459e-199">**Жол** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің жол мәнін өткізеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-199">For fields of the **String** type, this property passes the string value of the field between the server and the app.</span></span> <span data-ttu-id="a459e-200">Сондай-ақ ол ағымдағы түр ретінде пішімделген **Нақты** түрінің өрістері үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-200">It's also used for fields of the **Real** type that are formatted as currency.</span></span> <span data-ttu-id="a459e-201">Осы өрістер үшін, сипат ағымдағы кодты бағдарламаға өткізу үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-201">For those fields, the property is used to pass the currency code to the app.</span></span>

### <a name="datevalue-date"></a><span data-ttu-id="a459e-202">dateValue (күн)</span><span class="sxs-lookup"><span data-stu-id="a459e-202">dateValue (date)</span></span>

<span data-ttu-id="a459e-203">**Күн** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің күн мәнін өткізеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-203">For fields of the **Date** type, this property passes the date value of the field between the server and the app.</span></span>

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a><span data-ttu-id="a459e-204">Уақыт кестесінің жазба бөліміндегі реттелмелі өрістерді көрсету және сақтау</span><span class="sxs-lookup"><span data-stu-id="a459e-204">Show and save a custom field in the timesheet entry section</span></span>

<span data-ttu-id="a459e-205">Төмендегі уақыт кестесінің жазбасын жасаудың мобильді құрылғы бағдарламасының скриншоты.</span><span class="sxs-lookup"><span data-stu-id="a459e-205">Below is a screenshot from the mobile app of a timesheet entry creation.</span></span> <span data-ttu-id="a459e-206">Онда кірістірілген өрістер және орнатылған "Екінші параметр" бағалау мәні бар "Тексеру жолы" деп аталатын "Уақыт жазбасы" бөліміндегі реттелмелі өріс көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-206">It shows the out-of-box fields and a custom field in the "Time entry" section called "Test string" with an enum value of "Second option" already set.</span></span>

![Бағдарламадағы тексеру жолының реттелмелі өрісі](media/timesheet-entry.jpg)



<span data-ttu-id="a459e-208">Төмендегі "Тексеру жол" реттелмелі өрісі үшін қолжетімді бағалау параметрлерінің бірін таңдайтын пайдаланушының мобильді құрылғы бағдарламасының скриншоты.</span><span class="sxs-lookup"><span data-stu-id="a459e-208">Below is a screenshot from the mobile app of the user selecting one of the enum options available for the "Test string" custom field.</span></span>  <span data-ttu-id="a459e-209">Екі "Бірінші параметр" және "Екінші параметр" параметрі айырып-қосқыштар ретінде көрсетілген.</span><span class="sxs-lookup"><span data-stu-id="a459e-209">The two options are "First option" and "Second option" shown as radio buttons.</span></span> <span data-ttu-id="a459e-210">Екінші параметр ағымда таңдалады.</span><span class="sxs-lookup"><span data-stu-id="a459e-210">The second option is currently selected.</span></span>

!["Тексеру жолы" реттелмелі өрісіне арналған ажыратпа-қосқыштар (радио түймешіктер)](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="a459e-212">TSTimesheetLine кестесінде реттелмелі өріс болатындай етіп кеңейту</span><span class="sxs-lookup"><span data-stu-id="a459e-212">Extend the TSTimesheetLine table so that it has a custom field</span></span>

<span data-ttu-id="a459e-213">Әдеттегі сценарийлерде, уақыт кестесінің жазба бөліміндегі реттелмелі өріске арналған деректер TSTimesheetLine кестесіне сақталуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="a459e-213">In typical scenarios, it's likely that the data for a custom field in the timesheet entry section will be saved to the TSTimesheetLine table.</span></span> <span data-ttu-id="a459e-214">Сондықтан, деректерді берілген TSTimesheetTrans жазбасының негізінде шығару мүмкін болса немесе онда белгілі бір жазба контексті жоқ болған жағдайда (мысалы, өріс жоба параметрлерінде тек оқу үшін ретінде орнатылса) басқа кестелерді пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-214">However, other tables can be used if the data can be retrieved based on a TSTimesheetTrans record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="a459e-215">Реттелмелі өрістерде сақтық көшірмеленетін дерекқор жазбаларының болуы міндетті еместігін ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="a459e-215">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="a459e-216">Оларды X++ логикасының негізінде динамикалық түрде жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-216">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="a459e-217">Бұл тәсіл тек оқуға арналған сценарийлерде пайдалы болуы мүмкін (Динамикалық түрде жасалған реттелмелі мәндердің мысалын “Уақыт кестесі мәліметтерін толтыру үшін TSTimesheetDetails class, buildCustomFieldListForHeader әдісіндегі пәрмен тізбегін пайдалану” бөлімінен қараңыз).</span><span class="sxs-lookup"><span data-stu-id="a459e-217">This approach can be useful in read-only scenarios (see the “Use chain of command on the TSTimesheetDetails class, buildCustomFieldListForHeader method to fill in timesheet details” section for an example of dynamically generated custom field values.)</span></span>

<span data-ttu-id="a459e-218">Төмендегі бағдарлама нысаны дерекнамасының Visual Studio бағдарламасының скриншоты.</span><span class="sxs-lookup"><span data-stu-id="a459e-218">Below is a screenshot from Visual Studio of the Application Object Tree.</span></span> <span data-ttu-id="a459e-219">Онда ағымдағы өріс ретінде қосылған TestLineString өрісі бар TSTimesheetLine кестесінің кеңейтімі көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-219">It shows an extension of the TSTimesheetLine table with the TestLineString field added as a custom field.</span></span>

![Сызық жол](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a><span data-ttu-id="a459e-221">Уақыт кестесінің жазбасы бөліміндегі өрісті көрсету үшін TSTimesheetSettings класының buildCustomFieldList әдісіндегі пәрмен тізбегін пайдалану</span><span class="sxs-lookup"><span data-stu-id="a459e-221">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the timesheet entry section</span></span>

<span data-ttu-id="a459e-222">Бұл код бағдарламадағы өріске арналған бейнелеу параметрлерін басқарады.</span><span class="sxs-lookup"><span data-stu-id="a459e-222">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="a459e-223">Мысалы, ол өріс, белгі түрін, өрістің міндетті екенін/еместігін және өріс пайда болатын бөлім түрін басқарады.</span><span class="sxs-lookup"><span data-stu-id="a459e-223">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="a459e-224">Келесі мысалда уақыт жазбаларындағы жол өрісі көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-224">The following example shows a string field on time entries.</span></span> <span data-ttu-id="a459e-225">Бұл өрісте ажыратпа-қосқыштар (радио түймешіктер) арқылы қолжетімді болатын **Бірінші параметр** және **Екінші параметр** атты екі параметр бар.</span><span class="sxs-lookup"><span data-stu-id="a459e-225">This field has two options, **First option** and **Second option** , that are available via option buttons (radio buttons).</span></span> <span data-ttu-id="a459e-226">Бағдарламадағы өріс TSTimesheetLine кестесіне қосылатын **TestLineString** өрісімен байланыстырылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-226">The field in the app is associated with the **TestLineString** field that is added to the TSTimesheetLine table.</span></span>

<span data-ttu-id="a459e-227">Реттелмелі өріс сипаттарының баптандырылуын жеңілдету үшін **TSTimesheetCustomField::newFromMetatdata()** әдісін пайдалануды ескеріңіз: **fieldBaseType** , **tableName** , **fieldname** , **белгі** , **isEditable** , **isMandatory** , **stringLength** және **numberOfDecimals**.</span><span class="sxs-lookup"><span data-stu-id="a459e-227">Note the use of the **TSTimesheetCustomField::newFromMetatdata()** method to simplify the initialization of the custom field properties: **fieldBaseType** , **tableName** , **fieldname** , **label** , **isEditable** , **isMandatory** , **stringLength** , and **numberOfDecimals**.</span></span> <span data-ttu-id="a459e-228">Сондай-ақ осы параметрлерді қалауыңызша қолмен орнатуға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-228">You can also set these parameters manually, as you prefer.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('Second option');
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a><span data-ttu-id="a459e-229">Уақыт кестесінің жазбасына мәндерді енгізу үшін TSTimesheetEntry класының buildCustomFieldListForEntry әдісіндегі пәрмен тізбегін пайдалану</span><span class="sxs-lookup"><span data-stu-id="a459e-229">Use chain of command on the buildCustomFieldListForEntry method of the TSTimesheetEntry class to enter values in a timesheet entry</span></span>

<span data-ttu-id="a459e-230">**buildCustomFieldListForEntry** әдісі мобильді құрылғы бағдарламасында сақталған уақыт кестесінің жолдарына мәндерді енгізу үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-230">The **buildCustomFieldListForEntry** method is used to enter values on the saved timesheet lines in the mobile app.</span></span> <span data-ttu-id="a459e-231">Параметр ретінде TSTimesheetTrans жазбасы қажет.</span><span class="sxs-lookup"><span data-stu-id="a459e-231">It takes a TSTimesheetTrans record as a parameter.</span></span> <span data-ttu-id="a459e-232">Сол жазбадан алынған өрістерді бағдарламадағы реттелмелі өріс мәнін толтыру үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-232">Fields from that record can be used to fill in the custom field value in the app.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetEntry))]
final class TsTimesheetEntry_Extension
{
    protected List buildCustomFieldListForEntry(TSTimesheetTrans _tsTimesheetTrans)
    {
        List customFieldList = next buildCustomFieldListForEntry(_tsTimesheetTrans);
        TSTimesheetLine tsTimesheetLine = _tsTimesheetTrans.timesheetLine();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        tsTimesheetCustomField.parmStringValue(tsTimesheetLine.TestLineString);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('second option;);
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a><span data-ttu-id="a459e-233">Уақыт кестесінің жазбасын бағдарламадан дерекқорға сақтау үшін TSTimesheetEntryService класындағы пәрмен тізбегін пайдалану</span><span class="sxs-lookup"><span data-stu-id="a459e-233">Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database</span></span>

<span data-ttu-id="a459e-234">Реттелмелі өрісті әдеттегі қолданыстағы дерекқорға сақтау үшін, бірнеше әдісті кеңейту қажет:</span><span class="sxs-lookup"><span data-stu-id="a459e-234">To save a custom field back to the database in typical usage, you must extend multiple methods:</span></span>

- <span data-ttu-id="a459e-235">**timesheetLineNeedsUpdating** әдісі жол жазбасының пайдаланушы арқылы өзгертілгенін/өзгертілмегенін және дерекқорға сақталғанын анықтау үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-235">The **timesheetLineNeedsUpdating** method is used to determine whether the line record has been changed by the user in the app and must be saved to the database.</span></span> <span data-ttu-id="a459e-236">Егер өнімділік мәселе тудырмаса, бұл әдісті **шын** мәніне оралатындай етіп жеңілдетуге болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-236">If performance isn't a concern, this method can be simplified so that it always returns **true**.</span></span>
- <span data-ttu-id="a459e-237">**populateTimesheetLineFromEntryDuringCreate** және **populateTimesheetLineFromEntryDuringUpdate** әдістерін мәндерді TSTimesheetLine дерекқор жазбасына берілген TSTimesheetEntry деректер келісім-шартынан енгізетіндей етіп кеңейтуге болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-237">The **populateTimesheetLineFromEntryDuringCreate** and **populateTimesheetLineFromEntryDuringUpdate** methods can be extended so that they enter values in the TSTimesheetLine database record from the TSTimesheetEntry data contract record that is provided.</span></span> <span data-ttu-id="a459e-238">Келесі мысалда дерекқор өрісі мен жазба өрісінің арасындағы салыстыру X++ коды арқылы қолмен орындалған жолына назар аударыңыз.</span><span class="sxs-lookup"><span data-stu-id="a459e-238">In the example that follows, notice how the mapping between the database field and the entry field is manually done via X++ code.</span></span>
- <span data-ttu-id="a459e-239">Сондай-ақ **populateTimesheetWeekFromEntry** әдісін **TSTimesheetEntry** нысанымен салыстырылған реттелмелі өріс TSTimesheetLineweek дерекқор кестесіне жазуы қажет болған жағдайда кеңейтуге болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-239">The **populateTimesheetWeekFromEntry** method can also be extended if the custom field that is mapped to the **TSTimesheetEntry** object must write back to the TSTimesheetLineweek database table.</span></span>

> [!NOTE]
> <span data-ttu-id="a459e-240">Келесі мысалда пайдаланушы таңдайтын **firstOption** немесе **secondOption** мәні дерекқорға қатар жолының мәні ретінде сақталады.</span><span class="sxs-lookup"><span data-stu-id="a459e-240">The following example saves the **firstOption** or **secondOption** value that the user selects to the database as a raw string value.</span></span> <span data-ttu-id="a459e-241">Дерекқор өрісі **Бағалау** түрінің өрісі болса, осы мәндерді бағалау мәнімен қолмен салыстырып, дерекқор кестесіндегі бағалау өрісіне сақтауға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-241">If the database field is a field of the **Enum** type, those values can be manually mapped to an enum value and then saved to an enum field on the database table.</span></span>

```xpp
...
[ExtensionOf(classStr(TSTimesheetEntryService))]
final class TSTimesheetEntryService_Extension
{
    protected boolean timesheetLineNeedsUpdating(TSTimesheetLine _tsTimesheetLine,
    TsTimesheetEntry _tsTimesheetEntry)
    {
        boolean ret = next timesheetLineNeedsUpdating(_tsTimesheetLine,
        _tsTimesheetEntry);
        if (!ret)
        {
            */ Loop through custom fields to see if value needs updating*/
            ListEnumerator enumerator =  _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    */ If Custom field value for TestLineString field has changed, We need to update the timesheet line.*/
                    if (_tsTimesheetLine.TestLineString != customField.parmStringValue())
                    {
                        ret = true;
                    }
                }
            }
        }
        return ret;
    }
    protected void populateTimesheetLineFromEntryDuringCreate(TSTimesheetLine
    _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
    {
        next populateTimesheetLineFromEntryDuringCreate(_tsTimesheetLine,
        _tsTimesheetEntry);
        this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
        _tsTimesheetEntry);
        }
        protected void populateTimesheetLineFromEntryDuringUpdate(TSTimesheetLine
        \_tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            next populateTimesheetLineFromEntryDuringUpdate(_tsTimesheetLine,
            _tsTimesheetEntry);
            this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
            _tsTimesheetEntry);
        }
        private void populateTimesheetLineFromCustomFields(TSTimesheetLine
        _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            ListEnumerator enumerator =
            _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    _tsTimesheetLine.TestLineString = customField.parmStringValue();
                }
            }
        }
    }
...
```

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a><span data-ttu-id="a459e-242">Уақыт кестесінің тақырып бөліміндегі реттелмелі өрістерді көрсету</span><span class="sxs-lookup"><span data-stu-id="a459e-242">Show a custom field in the timesheet header section</span></span>

<span data-ttu-id="a459e-243">Төмендегі уақыт кестесін қарап жатқан пайдаланушының мобильді құрылғы бағдарламасының скриншоты.</span><span class="sxs-lookup"><span data-stu-id="a459e-243">Below is a screenshot from the mobile app of a user viewing a timesheet.</span></span> <span data-ttu-id="a459e-244">"Қосымша ақпарат" түймешігі "Қосымша мәліметтерді көру" параметрін көрсету үшін жоғарғы оң жақ бұрыштан таңдалды.</span><span class="sxs-lookup"><span data-stu-id="a459e-244">The "More information" button has been selected in the upper-right corner to show the "View more details" option.</span></span>  

![Қосымша мәліметтерді көру пәрмені](media/show-more.png)

<span data-ttu-id="a459e-246">Төмендегі уақыт кестесінің “Қосымша ақпарат” бөлімін көрсететін мобильді құрылғы бағдарламасының скриншоты.</span><span class="sxs-lookup"><span data-stu-id="a459e-246">Below is a screenshot from the mobile app showing the “More” section of a timesheet.</span></span> <span data-ttu-id="a459e-247">“Бұл уақыт кестесінің пайдалану коэффициенті (есептелген реттелмелі өріс)” деп аталатын реттелмелі өріс уақыт кестесінің тақырып бөліміне қосылды.</span><span class="sxs-lookup"><span data-stu-id="a459e-247">A custom field called “Utilization rate of this timesheet (computed custom field)” has been added to the timesheet header section.</span></span> <span data-ttu-id="a459e-248">Тек оқуға арналған "0,667" мәні реттелмелі өрісте орнатылды.</span><span class="sxs-lookup"><span data-stu-id="a459e-248">A read-only value of "0.667" is set on the custom field.</span></span>

![Қосымша бөлім](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="a459e-250">TSTimesheetTable кестесінде реттелмелі өріс болатындай етіп кеңейту</span><span class="sxs-lookup"><span data-stu-id="a459e-250">Extend the TSTimesheetTable table so that it has a custom field</span></span>

<span data-ttu-id="a459e-251">Әдеттегі сценарийлерде, тақырып бөліміндегі реттелмелі өріске арналған деректер TSTimesheetHeader кестесінен алынуы мүмкін.</span><span class="sxs-lookup"><span data-stu-id="a459e-251">In typical scenarios, it's likely that the data for a custom field in the header section will be pulled from the TSTimesheetHeader table.</span></span> <span data-ttu-id="a459e-252">Сондықтан, деректерді берілген TSTimesheetTable жазбасының негізінде шығару мүмкін болса немесе онда белгілі бір жазба контексті жоқ болған жағдайда (мысалы, өріс жоба параметрлерінде "тек оқу үшін" ретінде орнатылса) басқа кестелерді пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-252">However, other tables can be used if the data can be retrieved based on a TSTimesheetTable record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="a459e-253">Реттелмелі өрістерде сақтық көшірмеленетін дерекқор жазбаларының болуы міндетті еместігін ескеріңіз.</span><span class="sxs-lookup"><span data-stu-id="a459e-253">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="a459e-254">Оларды X++ логикасының негізінде динамикалық түрде жасауға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-254">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="a459e-255">Келесі мысалда осы тәсіл көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-255">The example that follows shows this approach.</span></span>

<span data-ttu-id="a459e-256">Тақырып бөліміндегі өрістер бағдарламада тек оқуға арналады.</span><span class="sxs-lookup"><span data-stu-id="a459e-256">Fields in the header section are always read-only in the app.</span></span>

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a><span data-ttu-id="a459e-257">Уақыт кестесінің тақырып бөліміндегі өрісті көрсету үшін TSTimesheetSettings класының buildCustomFieldList әдісіндегі пәрмен тізбегін пайдалану</span><span class="sxs-lookup"><span data-stu-id="a459e-257">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the header section</span></span>

<span data-ttu-id="a459e-258">Бұл код бағдарламадағы өріске арналған бейнелеу параметрлерін басқарады.</span><span class="sxs-lookup"><span data-stu-id="a459e-258">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="a459e-259">Мысалы, ол өріс, белгі түрін, өрістің міндетті екенін/еместігін және өріс пайда болатын бөлім түрін басқарады.</span><span class="sxs-lookup"><span data-stu-id="a459e-259">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="a459e-260">Келесі мысалды бағдарламадағы тақырып бөлімінде есептелген мән көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-260">The following example shows a computed value in the header section in the app.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a><span data-ttu-id="a459e-261">Уақыт кестесі мәліметтерін толтыру үшін TSTimesheetDetails класының buildCustomFieldListForHeader әдісіндегі пәрмен тізбегін пайдалану</span><span class="sxs-lookup"><span data-stu-id="a459e-261">Use chain of command on the buildCustomFieldListForHeader method of the TSTimesheetDetails class to fill in timesheet details</span></span>

<span data-ttu-id="a459e-262">**buildCustomFieldListForHeader** әдісі мобильді құрылғы бағдарламасындағы уақыт кестесінің тақырып мәліметтерін толтыру үшін пайдаланылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-262">The **buildCustomFieldListForHeader** method is used to fill in the timesheet header details in the mobile app.</span></span> <span data-ttu-id="a459e-263">Параметр ретінде TSTimesheetTable жазбасы қажет.</span><span class="sxs-lookup"><span data-stu-id="a459e-263">It takes a TSTimesheetTable record as a parameter.</span></span> <span data-ttu-id="a459e-264">Сол жазбадан алынған өрістерді бағдарламадағы реттелмелі өріс мәнін толтыру үшін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-264">Fields from that record can be used to fill in the custom field value in the app.</span></span> <span data-ttu-id="a459e-265">Келесі мысалда дерекқордан алынған мәндер оқылмайды.</span><span class="sxs-lookup"><span data-stu-id="a459e-265">The following example doesn't read any values from the database.</span></span> <span data-ttu-id="a459e-266">Оның орнына, ол кейін бағдарламада көрсетілетін есептелген мәнді жасау үшін X++ логикасын пайдаланады.</span><span class="sxs-lookup"><span data-stu-id="a459e-266">Instead, it uses X++ logic to generate a computed value that is then shown in the app.</span></span>


```xpp
...
[ExtensionOf(classStr(TSTimesheetDetails))]
final class TSTimesheetDetails_Extension
{
    protected List buildCustomFieldListForHeader(TSTimesheetTable
    _tsTimesheetTable)
    {
        List customFieldList = next buildCustomFieldListForHeader(_tsTimesheetTable);
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        real utilizationRate = 0;
        if (_tsTimesheetTable.totalHours() != 0)
        {
            utilizationRate = _tsTimesheetTable.totalHoursBillable() /
            _tsTimesheetTable.totalHours();
        }
        tsTimesheetCustomField.parmRealValue(utilizationRate);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

## <a name="other-configurabilityextensibility-opportunities"></a><span data-ttu-id="a459e-267">Басқа конфигурация/кеңейтілім мүмкіндіктері</span><span class="sxs-lookup"><span data-stu-id="a459e-267">Other configurability/extensibility opportunities</span></span>

### <a name="adding-additional-validation-for-the-app"></a><span data-ttu-id="a459e-268">Бағдарлама үшін қосымша тексеруді қосу</span><span class="sxs-lookup"><span data-stu-id="a459e-268">Adding additional validation for the app</span></span>

<span data-ttu-id="a459e-269">Дерекқор деңгейіндегі уақыт кестесінің функциясы үшін бұрыннан бар логика күтілгендей жұмыс істейді.</span><span class="sxs-lookup"><span data-stu-id="a459e-269">Existing logic for timesheet functionality at the database level will still work as expected.</span></span> <span data-ttu-id="a459e-270">Операцияларды сақтауды немесе жіберуді аяқтауды тоқтату және белгілі бір қате туралы хабарды көрсету үшін, пәрмен кеңейтімінің тізбегі арқылы кодқа **шақыру қатесін("пайдаланушыға хабарлау")** қосуға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-270">To interrupt the completion of save or submit operations and show a specific error message, you can add **throw error("message to user")** to the code via a chain of command extension.</span></span> <span data-ttu-id="a459e-271">Пайдалы кеңейтілетін әдістердің үш мысалы бар:</span><span class="sxs-lookup"><span data-stu-id="a459e-271">Here are three examples of useful extensible methods:</span></span>

- <span data-ttu-id="a459e-272">Егер TSTimesheetLine кестесіндегі **validateWrite** мәні уақыт кестесінің жолы үшін операцияны сақтау кезінде **жалған** мәніне оралса, мобильді құрылғы бағдарламасында қате туралы хабар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-272">If **validateWrite** on the TSTimesheetLine table returns **false** during a save operation for a timesheet line, an error message is shown in the mobile app.</span></span>
- <span data-ttu-id="a459e-273">Егер TSTimesheetTable кестесіндегі **validateSubmit** мәні бағдарламадағы уақыт кестесін жіберу кезінде **жалған** мәніне оралса, пайдаланушыға қате туралы хабар көрсетіледі.</span><span class="sxs-lookup"><span data-stu-id="a459e-273">If **validateSubmit** on the TSTimesheetTable table returns **false** during timesheet submission in the app, an error message is shown to the user.</span></span>
- <span data-ttu-id="a459e-274">Өрістерді (мысалы, **Жол сипаты** ) толтыратын логика TSTimesheetLine кестесіндегі **енгізу** әдісі кезінде орындалады.</span><span class="sxs-lookup"><span data-stu-id="a459e-274">Logic that fills in fields (for example, **Line Property** ) during the **insert** method on the TSTimesheetLine table will still run.</span></span>

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a><span data-ttu-id="a459e-275">Кірістірілген өрістерді конфигурация арқылы тек оқу үшін жасыру және белгілеу</span><span class="sxs-lookup"><span data-stu-id="a459e-275">Hiding and marking out-of-box fields as read-only via configuration</span></span>

<span data-ttu-id="a459e-276">Жоба параметрлерінен, кірістірілген өрістерді тек оқу үшін жасауға немесе мобильді құрылғы бағдарламасында жасыруға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-276">From the project parameters, you can make out-of-box fields read-only or hidden in the mobile app.</span></span> <span data-ttu-id="a459e-277">Параметрлерді **Жобаны басқару және есеп параметрлері** бетінің **Уақыт кестесі** қойыншасындағы **Мобильді уақыт кестелері** бөліміне орнатыңыз.</span><span class="sxs-lookup"><span data-stu-id="a459e-277">Set the options in the **Mobile timesheets** section on the **Timesheet** tab of the **Project management and accounting parameters** page.</span></span>

![Жоба параметрлері](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a><span data-ttu-id="a459e-279">Кеңейтімдер арқылы таңдау үшін қолжетімді болатын әрекеттерді өзгерту</span><span class="sxs-lookup"><span data-stu-id="a459e-279">Changing the activities that are available for selection via extensions</span></span>

<span data-ttu-id="a459e-280">Жобаны таңдау үшін қолжетімді болатын әрекеттер **TsTimesheetProjectService** класындағы **getActivitiesForProject()** және **getActivityQuery()** әдістері арқылы толтырылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-280">The activities that are available for selection for a project are filled in via the **getActivitiesForProject()** and **getActivityQuery()** methods in the **TsTimesheetProjectService** class.</span></span> <span data-ttu-id="a459e-281">Белгілі бір жобаны таңдау үшін қолжетімді болатын әрекеттерге жұмыс сценарийлерін сәйкестендіру үшін осы әрекетті өзгертуге арналған пәрмен тізбегін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-281">You can use chain of command to change this behavior to match your business scenario for the activities that are available for selection for a specific project.</span></span>

### <a name="entering-a-default-project-category-on-timesheet-entries"></a><span data-ttu-id="a459e-282">Уақыт кестесі жазбаларындағы әдепкі жоба санатын енгізу</span><span class="sxs-lookup"><span data-stu-id="a459e-282">Entering a default project category on timesheet entries</span></span>

<span data-ttu-id="a459e-283">Уақыт кестесі жазбаларындағы әдепкі жоба санатының жазбасы үш деңгейде орын алады.</span><span class="sxs-lookup"><span data-stu-id="a459e-283">Entry of a default project category on timesheet entries occurs at three levels.</span></span> <span data-ttu-id="a459e-284">Қажетті әрекетке жету үшін әрекетті осы деңгейлердің кез келгенінде немесе барлығында кеңейту үшін пәрмен тізбегін пайдалануға болады.</span><span class="sxs-lookup"><span data-stu-id="a459e-284">You can use chain of command to extend the behavior at any or all of these levels to achieve the desired behavior.</span></span> <span data-ttu-id="a459e-285">Келесі иерархия пайдаланылады:</span><span class="sxs-lookup"><span data-stu-id="a459e-285">The following hierarchy is used:</span></span>

1. <span data-ttu-id="a459e-286">Бағдарлама жоба ресурсынан әдепкі санатты қоюға әрекеттенеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-286">The app tries to put the default category from the project resource.</span></span> <span data-ttu-id="a459e-287">Бұл әдепкі санат **TSTimesheetSettingsService** класындағы **getCurrentUserResource** және **getDelegatedResourcesForCurrentUser** әдістерінде орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-287">This default category is set in the **getCurrentUserResource** and **getDelegatedResourcesForCurrentUser** methods in the **TSTimesheetSettingsService** class.</span></span>
2. <span data-ttu-id="a459e-288">Егер әдепкі санат жобаның ресурс деңгейінде берілмесе, бағдарлама оны жоба әрекетінен алуға әрекеттенеді.</span><span class="sxs-lookup"><span data-stu-id="a459e-288">If the default category isn't provided at the project resource level, the app tries to pull it from the project activity.</span></span> <span data-ttu-id="a459e-289">Бұл әдепкі санат **TSTimesheetProjectService** класының **getActivitiesForProject** әдісінде орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-289">This default category is set in the **getActivitiesForProject** method in the **TSTimesheetProjectService** class.</span></span>
3. <span data-ttu-id="a459e-290">Егер әдепкі санат жобаның әрекет деңгейінде берілмесе, әдепкі санат жоба параметрлерінен алынады.</span><span class="sxs-lookup"><span data-stu-id="a459e-290">If the default category isn't provided at the project activity level, the default category it taken from the project parameters.</span></span> <span data-ttu-id="a459e-291">Бұл әдепкі санат **TSTimesheetProjectService** класының **getProjectDetailsbyRule** әдісінде орнатылады.</span><span class="sxs-lookup"><span data-stu-id="a459e-291">This default category is set in the **getProjectDetailsbyRule** method in the **TSTimesheetProjectService** class.</span></span>
