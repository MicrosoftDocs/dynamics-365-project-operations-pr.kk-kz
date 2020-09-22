---
title: iOS және Android жүйесіндегі Microsoft Dynamics 365 Project Timesheet мобильді құрылғы бағдарламасы үшін реттелмелі өрістерді ендіру
description: Бұл тақырыпта реттелмелі өрістерді ендіру үшін кеңейтімдерді пайдалануға арналған жалпы үлгілер беріледі.
author: KimANelson
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: 4564bbda-34ea-4647-a9bc-f6ef17b1038b
ms.search.region: Global
ms.search.industry: Service industries
ms.author: knelson
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 16c3b79dcaaf8c5c491587618256694f82f44753
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 03/24/2020
ms.locfileid: "3753026"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a>iOS және Android жүйесіндегі Microsoft Dynamics 365 Project Timesheet мобильді құрылғы бағдарламасы үшін реттелмелі өрістерді ендіру

[!include [banner](../includes/banner.md)]

Бұл тақырыпта реттелмелі өрістерді ендіру үшін кеңейтімдерді пайдалануға арналған жалпы үлгілер беріледі. Келесі тақырыптарда қамтылады:

- Реттелмелі өріс құрылымында қолдау көрсетілетін әртүрлі деректер түрлері
- Уақыт кестесінің жазбаларында тек оқуға арналған немесе өңделетін өрістерді көрсету және пайдаланушы ұсынған мәндерді дерекқорға сақтау жолы
- Уақыт кестесінің тақырыбында тек оқуға арналған өрістерді көрсету жолы
- Әдепкі мәндерді өрістерге енгізіп, қосымша тексеру жүргізу үшін басқа реттелмелі бизнес логикасын біріктіру жолы

## <a name="audience"></a>Аудитория

Бұл тақырып реттелмелі өрістерін Apple iOS және Google Android үшін қолжетімді болатын Microsoft Dynamics 365 Project Timesheet мобильді құрылғы бағдарламасында біріктіретін әзірлеушілерге арналған. Оқырмандар X++ әзірлеуімен және жобаның уақыт кестесі функциясымен таныс деп болжанады.

## <a name="data-contract--tstimesheetcustomfield-x-class"></a>Деректер келісім-шарты – TSTimesheetCustomField X++ класы

**TSTimesheetCustomField** класы – уақыт кестесі функциясы үшін реттелмелі өріс туралы ақпаратты көрсететін X++ деректер келісім-шарты класы. Мобильді құрылғы бағдарламасында реттелмелі өрістерді көрсету үшін реттелмелі өріс нысандарының тізімдері TSTimesheetDetails деректер келісім-шартында да, TSTimesheetEntry деректер келісім-шартында да беріледі.

- **TSTimesheetDetails** - уақыт кестесінің тақырып келісім-шарты.
- **TSTimesheetEntry** - уақыт кестесінің транзакция келісім-шарты. Бірдей жоба туралы ақпарат пен **timesheetLineRecId** мәні бар осы нысандардың топтары жол құрайды.

### <a name="fieldbasetype-types"></a>fieldBaseType (түрлері)

**TsTimesheetCustom** нысанындағы **FieldBaseType** сипаты бағдарламаларда пайда болатын өріс түрін анықтайды. Қолдау көрсетілетін келесі **Түрлер** мәндері.

| Түрлер мәні | Түрі              | Есктулер |
|-------------|-------------------|-------|
| 0           | Жол (және бағалау) | Өріс мәтін өрісі ретінде пайда болады. |
| 1           | Integer           | Мән ондық белгілері жоқ сан ретінде көрсетіледі. |
| 2           | Нақты              | Мән ондық белгілері бар сан ретінде көрсетіледі.<p>Нақты мәндерді бағдарламада ағымдағы мән ретінде көрсету үшін, **fieldExtenededType** сипатын пайдаланыңыз. Көрсетілетін ондық белгілердің санын орнату үшін **numberOfDecimals** сипатын пайдалануға болады.</p> |
| 3           | Күн              | Күн пішімдері **Пайдаланушы параметрлері** ішіндегі **Тіл және ел/аймақ параметрі** астында көрсетілген пайдаланушының **Күні, уақыттар және нөмір пішімі** бойынша анықталады. |
| 4           | Boolean           | |
| 15          | GUID              | |
| 16          | Int64             | |

- **stringOptions** сипаты **TSTimesheetCustomField** нысанында берілмесе, пайдаланушыға еркін мәтін өрісі беріледі.

    **stringLength** сипатын пайдаланушылар енгізе алатын максималды жол ұзындығын орнату үшін пайдалануға болады.

- **stringOptions** сипаты **TSTimesheetCustomField** нысанында берілсе, осы тізім элементтері пайдаланушылар ажыратпа-қосқыштар (радио түймешіктер) көмегімен таңдай алатын мәндер болып табылады.

    Бұл жағдайда жол өрісі пайдаланушы жазбасының мақсатында бағалау өрісі ретінде әрекет етеді. Мәнді дерекқорға бағалау мәні ретінде сақтау үшін, пәрмен тізбегінің көмегімен дерекқорға сақтау алдында жол мәнін бағалау мәнімен қолмен салыстырыңыз (Мысалды кейін осы тақырыптағы “Уақыт кестесінің жазбасын бағдарламадан дерекқорға сақтау үшін TSTimesheetEntryService класындағы пәрмен тізбегін пайдалану” бөлімінен қараңыз).

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a>fieldExtendedType (TSCustomFieldExtendedType)

Бұл сипатты нақты мәндерді ағымдағы мәндер ретінде пішімдеу үшін пайдалануға болады. Бұл тәсілді **fieldBaseType** мәні **Нақты** мән болған кезде қолдануға болады.

- **TSCustomFieldExtendedType:жоқ** – пішімдеу қолданылмайды.
- **TSCustomFieldExtendedType::ағымдағы** – мәнді ағымдағы мән ретінде пішімдеу.

    Ағымдағы пішімдеу белсенді болған кезде, **stringValue** өрісін бағдарламада көрсетілуі керек валюта кодын өткізу үшін пайдалануға болады. Мән – тек оқуға арналған мән.

    **realValue** өрісінде дерекқорға сақталуы керек ақша мөлшері бар.

### <a name="fieldsection-tscustomfieldsection"></a>fieldSection (TSCustomFieldSection)

Бұл сипатты бағдарламада пайда болуы керек реттелмелі өрісті көрсету үшін пайдалануға болады.

- **TSCustomFieldSection::тақырып** – өріс бағдарламадағы **Қосымша мәліметтерді көру** бөлімінде пайда болады. Осы өрістер әрқашан тек оқуға арналады.
- **TSCustomFieldSection::жол** – өріс уақыт кестесінің жазбаларындағы барлық кірістірілген жол өрістерінен кейін пайда болады. Осы өрістерді өңдеуге немесе тек оқуға болады.

### <a name="fieldname-fieldnameshort"></a>fieldName (FieldNameShort)

Бұл сипат өрісті бағдарлама беретін мәндер дерекқорға қайта сақталған кезде анықтайды.

### <a name="tablename-tablenameshort"></a>tableName (TableNameShort)

Бұл сипат өрісті бағдарлама беретін мәндер дерекқорға қайта сақталған кезде анықтайды.

### <a name="iseditable-noyes"></a>isEditable (NoYes)

Бұл сипатты уақыт кестесінің жазбасы бөліміндегі өрісті пайдаланушылар өңдей алатынын көрсету үшін **Иә** параметріне орнатыңыз. Өрісті тек оқуға арналған ету үшін сипатты **Жоқ** параметріне орнатыңыз.

### <a name="ismandatory-noyes"></a>isMandatory (NoYes)

Бұл сипатты уақыт кестесінің жазба бөліміндегі өріс міндетті екенін көрсету үшін **Иә** параметріне орнатыңыз.

### <a name="label-str"></a>белгі (жол)

Бұл сипат бағдарламадағы келесі өрісте көрсетілетін белгіні көрсетеді.

### <a name="stringoptions-list-of-strings"></a>stringOptions (жолдар тізімі)

Бұл сипатты **fieldBaseType** мәні **Жол** мәніне орнатылған кезде қолдануға болады. **stringOptions** сипаты орнатылса, ажыратпа-қосқыштар (радио түймешіктер) арқылы таңдау үшін қолжетімді болатын жол мәндері тізімдегі жол арқылы көрсетіледі. Егер жол берілмесе, жол өрісіндегі еркін мәтін жазбасына рұқсат етіледі (Мысалды кейін осы тақырыптағы “Уақыт кестесінің жазбасын бағдарламадан дерекқорға сақтау үшін TSTimesheetEntryService класындағы пәрмен тізбегін пайдалану” бөлімінен қараңыз).

### <a name="stringlength-int"></a>stringLength (int)

Бұл сипат жол өрісі үшін максималды ұзындықты көрсетеді. Оны **fieldBaseType** мәні **Жол** мәніне орнатылған кезде қолдануға болады.

### <a name="numberofdecimals-int"></a>numberOfDecimals (int)

Бұл сипат нақты өріс үшін көрсетілетін ондық белгілердің санын көрсетеді. Оны тек **fieldBaseType** мәні **Нақты** мәнге орнатылған кезде қолдануға болады.

### <a name="ordersequence-int"></a>orderSequence (int)

Бұл сипат бірнеше реттелмелі өріс көрсетілген кезде бағдарламада реттелмелі өрістердің көрсетілу ретін басқарады. Алдымен төмен саны бар өрістер көрсетіледі.

### <a name="booleanvalue-boolean"></a>booleanValue (логикалық)

**Логикалық** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің логикалық мәнін өткізеді.

### <a name="guidvalue-guid"></a>guidValue (guid)

**GUID** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің глобалдық бірегей идентификатор (GUID) мәнін өткізеді.

### <a name="int64value-int64"></a>int64Value (int64)

**Int64** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің int64 мәнін өткізеді.

### <a name="intvalue-int"></a>intValue (int)

**Int** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің int мәнін өткізеді.

### <a name="realvalue-real"></a>realValue (нақты)

**Нақты** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің нақты мәнін өткізеді .

### <a name="stringvalue-str"></a>stringValue (str)

**Жол** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің жол мәнін өткізеді. Сондай-ақ ол ағымдағы түр ретінде пішімделген **Нақты** түрінің өрістері үшін пайдаланылады. Осы өрістер үшін, сипат ағымдағы кодты бағдарламаға өткізу үшін пайдаланылады.

### <a name="datevalue-date"></a>dateValue (күн)

**Күн** түрінің өрістері үшін, осы сипат сервер мен бағдарлама арасындағы өрістің күн мәнін өткізеді.

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a>Уақыт кестесінің жазба бөліміндегі реттелмелі өрістерді көрсету және сақтау

Төмендегі уақыт кестесінің жазбасын жасаудың мобильді құрылғы бағдарламасының скриншоты. Онда кірістірілген өрістер және орнатылған "Екінші параметр" бағалау мәні бар "Тексеру жолы" деп аталатын "Уақыт жазбасы" бөліміндегі реттелмелі өріс көрсетіледі.

![Бағдарламадағы тексеру жолының реттелмелі өрісі](media/timesheet-entry.jpg)



Төмендегі "Тексеру жол" реттелмелі өрісі үшін қолжетімді бағалау параметрлерінің бірін таңдайтын пайдаланушының мобильді құрылғы бағдарламасының скриншоты.  Екі "Бірінші параметр" және "Екінші параметр" параметрі айырып-қосқыштар ретінде көрсетілген. Екінші параметр ағымда таңдалады.

!["Тексеру жолы" реттелмелі өрісіне арналған ажыратпа-қосқыштар (радио түймешіктер)](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a>TSTimesheetLine кестесінде реттелмелі өріс болатындай етіп кеңейту

Әдеттегі сценарийлерде, уақыт кестесінің жазба бөліміндегі реттелмелі өріске арналған деректер TSTimesheetLine кестесіне сақталуы мүмкін. Сондықтан, деректерді берілген TSTimesheetTrans жазбасының негізінде шығару мүмкін болса немесе онда белгілі бір жазба контексті жоқ болған жағдайда (мысалы, өріс жоба параметрлерінде тек оқу үшін ретінде орнатылса) басқа кестелерді пайдалануға болады.

Реттелмелі өрістерде сақтық көшірмеленетін дерекқор жазбаларының болуы міндетті еместігін ескеріңіз. Оларды X++ логикасының негізінде динамикалық түрде жасауға болады. Бұл тәсіл тек оқуға арналған сценарийлерде пайдалы болуы мүмкін (Динамикалық түрде жасалған реттелмелі мәндердің мысалын “Уақыт кестесі мәліметтерін толтыру үшін TSTimesheetDetails class, buildCustomFieldListForHeader әдісіндегі пәрмен тізбегін пайдалану” бөлімінен қараңыз).

Төмендегі бағдарлама нысаны дерекнамасының Visual Studio бағдарламасының скриншоты. Онда ағымдағы өріс ретінде қосылған TestLineString өрісі бар TSTimesheetLine кестесінің кеңейтімі көрсетіледі.

![Сызық жол](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a>Уақыт кестесінің жазбасы бөліміндегі өрісті көрсету үшін TSTimesheetSettings класының buildCustomFieldList әдісіндегі пәрмен тізбегін пайдалану

Бұл код бағдарламадағы өріске арналған бейнелеу параметрлерін басқарады. Мысалы, ол өріс, белгі түрін, өрістің міндетті екенін/еместігін және өріс пайда болатын бөлім түрін басқарады.

Келесі мысалда уақыт жазбаларындағы жол өрісі көрсетіледі. Бұл өрісте ажыратпа-қосқыштар (радио түймешіктер) арқылы қолжетімді болатын **Бірінші параметр** және **Екінші параметр** атты екі параметр бар. Бағдарламадағы өріс TSTimesheetLine кестесіне қосылатын **TestLineString** өрісімен байланыстырылады.

Реттелмелі өріс сипаттарының баптандырылуын жеңілдету үшін **TSTimesheetCustomField::newFromMetatdata()** әдісін пайдалануды ескеріңіз: **fieldBaseType**, **tableName**, **fieldname**, **белгі**, **isEditable**, **isMandatory**, **stringLength** және **numberOfDecimals**. Сондай-ақ осы параметрлерді қалауыңызша қолмен орнатуға болады.

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a>Уақыт кестесінің жазбасына мәндерді енгізу үшін TSTimesheetEntry класының buildCustomFieldListForEntry әдісіндегі пәрмен тізбегін пайдалану

**buildCustomFieldListForEntry** әдісі мобильді құрылғы бағдарламасында сақталған уақыт кестесінің жолдарына мәндерді енгізу үшін пайдаланылады. Параметр ретінде TSTimesheetTrans жазбасы қажет. Сол жазбадан алынған өрістерді бағдарламадағы реттелмелі өріс мәнін толтыру үшін пайдалануға болады.

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

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a>Уақыт кестесінің жазбасын бағдарламадан дерекқорға сақтау үшін TSTimesheetEntryService класындағы пәрмен тізбегін пайдалану

Реттелмелі өрісті әдеттегі қолданыстағы дерекқорға сақтау үшін, бірнеше әдісті кеңейту қажет:

- **timesheetLineNeedsUpdating** әдісі жол жазбасының пайдаланушы арқылы өзгертілгенін/өзгертілмегенін және дерекқорға сақталғанын анықтау үшін пайдаланылады. Егер өнімділік мәселе тудырмаса, бұл әдісті **шын** мәніне оралатындай етіп жеңілдетуге болады.
- **populateTimesheetLineFromEntryDuringCreate** және **populateTimesheetLineFromEntryDuringUpdate** әдістерін мәндерді TSTimesheetLine дерекқор жазбасына берілген TSTimesheetEntry деректер келісім-шартынан енгізетіндей етіп кеңейтуге болады. Келесі мысалда дерекқор өрісі мен жазба өрісінің арасындағы салыстыру X++ коды арқылы қолмен орындалған жолына назар аударыңыз.
- Сондай-ақ **populateTimesheetWeekFromEntry** әдісін **TSTimesheetEntry** нысанымен салыстырылған реттелмелі өріс TSTimesheetLineweek дерекқор кестесіне жазуы қажет болған жағдайда кеңейтуге болады.

> [!NOTE]
> Келесі мысалда пайдаланушы таңдайтын **firstOption** немесе **secondOption** мәні дерекқорға қатар жолының мәні ретінде сақталады. Дерекқор өрісі **Бағалау** түрінің өрісі болса, осы мәндерді бағалау мәнімен қолмен салыстырып, дерекқор кестесіндегі бағалау өрісіне сақтауға болады.

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

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a>Уақыт кестесінің тақырып бөліміндегі реттелмелі өрістерді көрсету

Төмендегі уақыт кестесін қарап жатқан пайдаланушының мобильді құрылғы бағдарламасының скриншоты. "Қосымша ақпарат" түймешігі "Қосымша мәліметтерді көру" параметрін көрсету үшін жоғарғы оң жақ бұрыштан таңдалды.  

![Қосымша мәліметтерді көру пәрмені](media/show-more.png)

Төмендегі уақыт кестесінің “Қосымша ақпарат” бөлімін көрсететін мобильді құрылғы бағдарламасының скриншоты. “Бұл уақыт кестесінің пайдалану коэффициенті (есептелген реттелмелі өріс)” деп аталатын реттелмелі өріс уақыт кестесінің тақырып бөліміне қосылды. Тек оқуға арналған "0,667" мәні реттелмелі өрісте орнатылды.

![Қосымша бөлім](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a>TSTimesheetTable кестесінде реттелмелі өріс болатындай етіп кеңейту

Әдеттегі сценарийлерде, тақырып бөліміндегі реттелмелі өріске арналған деректер TSTimesheetHeader кестесінен алынуы мүмкін. Сондықтан, деректерді берілген TSTimesheetTable жазбасының негізінде шығару мүмкін болса немесе онда белгілі бір жазба контексті жоқ болған жағдайда (мысалы, өріс жоба параметрлерінде "тек оқу үшін" ретінде орнатылса) басқа кестелерді пайдалануға болады.

Реттелмелі өрістерде сақтық көшірмеленетін дерекқор жазбаларының болуы міндетті еместігін ескеріңіз. Оларды X++ логикасының негізінде динамикалық түрде жасауға болады. Келесі мысалда осы тәсіл көрсетіледі.

Тақырып бөліміндегі өрістер бағдарламада тек оқуға арналады.

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a>Уақыт кестесінің тақырып бөліміндегі өрісті көрсету үшін TSTimesheetSettings класының buildCustomFieldList әдісіндегі пәрмен тізбегін пайдалану

Бұл код бағдарламадағы өріске арналған бейнелеу параметрлерін басқарады. Мысалы, ол өріс, белгі түрін, өрістің міндетті екенін/еместігін және өріс пайда болатын бөлім түрін басқарады.

Келесі мысалды бағдарламадағы тақырып бөлімінде есептелген мән көрсетіледі.

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a>Уақыт кестесі мәліметтерін толтыру үшін TSTimesheetDetails класының buildCustomFieldListForHeader әдісіндегі пәрмен тізбегін пайдалану

**buildCustomFieldListForHeader** әдісі мобильді құрылғы бағдарламасындағы уақыт кестесінің тақырып мәліметтерін толтыру үшін пайдаланылады. Параметр ретінде TSTimesheetTable жазбасы қажет. Сол жазбадан алынған өрістерді бағдарламадағы реттелмелі өріс мәнін толтыру үшін пайдалануға болады. Келесі мысалда дерекқордан алынған мәндер оқылмайды. Оның орнына, ол кейін бағдарламада көрсетілетін есептелген мәнді жасау үшін X++ логикасын пайдаланады.


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

## <a name="other-configurabilityextensibility-opportunities"></a>Басқа конфигурация/кеңейтілім мүмкіндіктері

### <a name="adding-additional-validation-for-the-app"></a>Бағдарлама үшін қосымша тексеруді қосу

Дерекқор деңгейіндегі уақыт кестесінің функциясы үшін бұрыннан бар логика күтілгендей жұмыс істейді. Операцияларды сақтауды немесе жіберуді аяқтауды тоқтату және белгілі бір қате туралы хабарды көрсету үшін, пәрмен кеңейтімінің тізбегі арқылы кодқа **шақыру қатесін("пайдаланушыға хабарлау")** қосуға болады. Пайдалы кеңейтілетін әдістердің үш мысалы бар:

- Егер TSTimesheetLine кестесіндегі **validateWrite** мәні уақыт кестесінің жолы үшін операцияны сақтау кезінде **жалған** мәніне оралса, мобильді құрылғы бағдарламасында қате туралы хабар көрсетіледі.
- Егер TSTimesheetTable кестесіндегі **validateSubmit** мәні бағдарламадағы уақыт кестесін жіберу кезінде **жалған** мәніне оралса, пайдаланушыға қате туралы хабар көрсетіледі.
- Өрістерді (мысалы, **Жол сипаты**) толтыратын логика TSTimesheetLine кестесіндегі **енгізу** әдісі кезінде орындалады.

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a>Кірістірілген өрістерді конфигурация арқылы тек оқу үшін жасыру және белгілеу

Жоба параметрлерінен, кірістірілген өрістерді тек оқу үшін жасауға немесе мобильді құрылғы бағдарламасында жасыруға болады. Параметрлерді **Жобаны басқару және есеп параметрлері** бетінің **Уақыт кестесі** қойыншасындағы **Мобильді уақыт кестелері** бөліміне орнатыңыз.

![Жоба параметрлері](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a>Кеңейтімдер арқылы таңдау үшін қолжетімді болатын әрекеттерді өзгерту

Жобаны таңдау үшін қолжетімді болатын әрекеттер **TsTimesheetProjectService** класындағы **getActivitiesForProject()** және **getActivityQuery()** әдістері арқылы толтырылады. Белгілі бір жобаны таңдау үшін қолжетімді болатын әрекеттерге жұмыс сценарийлерін сәйкестендіру үшін осы әрекетті өзгертуге арналған пәрмен тізбегін пайдалануға болады.

### <a name="entering-a-default-project-category-on-timesheet-entries"></a>Уақыт кестесі жазбаларындағы әдепкі жоба санатын енгізу

Уақыт кестесі жазбаларындағы әдепкі жоба санатының жазбасы үш деңгейде орын алады. Қажетті әрекетке жету үшін әрекетті осы деңгейлердің кез келгенінде немесе барлығында кеңейту үшін пәрмен тізбегін пайдалануға болады. Келесі иерархия пайдаланылады:

1. Бағдарлама жоба ресурсынан әдепкі санатты қоюға әрекеттенеді. Бұл әдепкі санат **TSTimesheetSettingsService** класындағы **getCurrentUserResource** және **getDelegatedResourcesForCurrentUser** әдістерінде орнатылады.
2. Егер әдепкі санат жобаның ресурс деңгейінде берілмесе, бағдарлама оны жоба әрекетінен алуға әрекеттенеді. Бұл әдепкі санат **TSTimesheetProjectService** класының **getActivitiesForProject** әдісінде орнатылады.
3. Егер әдепкі санат жобаның әрекет деңгейінде берілмесе, әдепкі санат жоба параметрлерінен алынады. Бұл әдепкі санат **TSTimesheetProjectService** класының **getProjectDetailsbyRule** әдісінде орнатылады.
