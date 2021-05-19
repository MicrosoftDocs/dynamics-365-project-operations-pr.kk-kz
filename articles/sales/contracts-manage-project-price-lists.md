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
# <a name="manage-project-price-lists-on-project-contracts"></a>Жоба келісім-шарттары бойынша жоба бағатізбелерін басқару

_**Қолданылу аясы:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations, Жеңілдетілген орналастыру - проформа-шотын ұсыну мәмілесі_

Dynamics 365 Project Operations бағдарламасындағы жоба келісім-шарттары келісім-шарттағы бірнеше сатылымның жарамды мерзімдегі бағатізбелерін қолдауға арналған. Project Operations бағдарламасында **Жоба бағатізбелері** деп аталатын байланысты нысан бар. Бұл нысанда жоба келісім-шарты үшін біреу көпке қатынасы бар.

Жоба бағатізбелері жоба бойынша уақытты, материалды және шығын транзакцияларын бағалау үшін қолданылады. Келісім-шартта бір немесе бірнеше жоба бағатізбесі болған кезде, бұл бағатізбелер уақыт, материал, шығындар болжамдарын және келісім-шарт жолы арқылы келісім-шартпен байланысты жобалардағы нақты көрсеткіштерді бағалау үшін қолданылады.

Жоба келісім-шартында жоба бағатізбелері болмаған кезде, сіз жобаның бағатізбелері жоқ екендігі туралы ескерту хабарын көресіз және сіздің бағалауларыңыз, нақты жобалық жұмыстар, материалдар мен шығындарыңыз бағаланбайды. Сатылым мәндері үшін баға болмайды.

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a>Жоба келісім-шарты бойынша жоба бағатізбесін байланыстыру немесе ажырату

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-material-and-expenses"></a>Жобалық жұмыстарды, материалдарды және шығындарды бағалау үшін нақты бағатізбені жасаңыз немесе байланыстырыңыз

1. Жоба келісім-шартында **Жоба бағатізбелері** қойыншасын таңдаңыз.
2. Ішкі торда **+ жаңа жоба бағатізбесін қосу** тармағын таңдаңыз.
3. **Жылдам жасау** жүгірткісінде бағатізбені таңдаңыз. 

  Ашылмалы тізімде мәтінмәні бағатізбедегі валюта келісім-шарттағы валютамен сәйкес келетін **Сатылым** опциясына орнатылған барлық бағатізбелерді көрсетеді.
  
4. Жоба бағатізбесі байланысының сипаттамасын енгізіп, **Сақтау** опциясын таңдаңыз, содан кейін **Жылдам жасау** жүгірткісін жабыңыз.

   Жоба бағатізбегінің байланысы жасалады.
   
5. Жоба келісім-шартымен бірнеше жоба бағатізбесін байланыстыру үшін 1-4 қадамдарын қайталаңыз. Байланысқан жоба бағатізбесінің әрқайсысында жарамдылық мерзімі әртүрлі болған жағдайда ғана бірнеше жоба бағатізбелерін жасаңыз.

> [!NOTE]
> Project Operations жоба бағатізбелерінің жарамдылық мерзімінің қабаттасуына қолдау көрсетпейді. Егер берілген күні бар транзакцияға арналған бірнеше жоба бағатізбелері болса, онда бұл транзакциядағы баға нөлге дейін әдепкі бойынша орнатылады.

### <a name="remove-a-project-price-list-association"></a>Жоба бағатізбесі байланысын жою

- Жоба бағатізбесін таңдаңыз, содан кейін ішкі торда **Келісім-шарт жобасының бағатізбесін жою** опциясын таңдаңыз. 

  Бағатізбе келісім-шарттағы жоба бағатізбелерінен жойылады. Бағатізбенің өзі жойылмайды. Тек келісім-шартпен байланыс жойылады.

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a>Келісім-шарттағы жоба бағатізбелерінің әдепкі мәндерін автоматты түрде орнату

Жоба бағатізбесін әдепкі жоба бағатізбе ретінде орнатуға болады. Бұл орнатылым ұйымыңыздағы барлық келісім-шарттардың әрқашан осы баға кезеңіне арналған стандартты жоба бағатізбесінен басталуын қамтамасыз етеді.

### <a name="set-up-the-organizational-default-for-project-price-lists"></a>Жоба бағатізбелері үшін ұйымның әдепкі мәнін орнату

1. **Параметрлер** > **Жалпы** тармағына өтіп, **Параметрлер** опциясын таңдаңыз.
2. **Белсенді параметрлер** тізім бетінде жазбаны ашу үшін оны таңдап, екі рет басыңыз. Екі рет басу кезінде гиперсілтеме болып табылатын өріс мәнін баспағаныңызға көз жеткізіңіз. 
3. **Белсенді параметрлер** бетінде **Бағатізбе** қойыншасын таңдаңыз. Ішкі тор әдепкі бағатізбелердің тізімін көрсетеді. Бұл — стандартты құн мен сатылым бағатізбелерінің тізімі. Сіз сататын әр валютамен **Сатылым** бағатізбесін байланыстыру сатылым бағатізбесінің осы валютада транзакциясын жасайтын тұтынушылар үшін жасаған кез келген келісім-шарт үшін стандартты болуын қамтамасыз етеді.

### <a name="set-up-a-customer-specific-project-price-list"></a>Тұтынушыларға арналған жоба бағатізбесін орнату

Сіз сондай-ақ тұтынушылармен нақты баға келісімі бойынша келіссөздер жүргізген кезде тұтынушыларға арналған жоба бағатізбелерін орната аласыз.

1. **Сатылым** > **Тұтынушылар** тармағына өтіңіз.
2. Белсенді тіркелгілер тізімінен арнайы бағатізбесі бар тұтынушыны таңдаңыз.
3. Ашу үшін тұтынушы жазбасын таңдап, содан кейін **Жоба бағатізбелері** қойыншасын таңдаңыз. Ішкі торда осы тұтынушыға арналған жоба бағатізбелерінің тізімі көрсетіледі. 
4. Осы тұтынушыға арналған жоба бағатізбесі болу үшін мұнда жаңа бағатізбе байланысын жасаңыз.

## <a name="custom-pricing-on-a-project-contract"></a>Жоба келісім-шарты бойынша реттелетін баға

Сізде ұйымға және тұтынушыға арналған әдепкі жоба бағатізбелері болғаннан кейін, жоба келісім-шарттары осы жоба бағатізбесінің байланысымен автоматты түрде жасалады. Алайда жоба келісім-шарты бойынша жоба бағатізбелері әрқашан оларға қосылған күн мен келісім-шарт атауымен көшіріледі. Содан кейін тіркелгі және жоба менеджерлері осы көшірмелердегі бағаларға түзетулер енгізе бастайды. Бұл өзгертілген бағалар тек осы жоба келісім-шартына қолданылатын болады.


[!INCLUDE[footer-include](../includes/footer-banner.md)]