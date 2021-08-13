---
title: Project Service Automation бағдарламасының 17 жаңарту шығарылымы 3-нұсқасындағы жаңалықтар немесе өзгерістер
description: Бұл бөлімде Project Service Automation бағдарламасының 17 жаңарту шығарылымының 3 нұсқасындағы қолжетімді мүмкіндіктер мен түзетулер берілген.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: ba2bc9da1c6e7e2e2628980878f9201b1c732cc03f791f5259bbbd0ee279b31b
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "7006613"
---
# <a name="project-service-automation-update-release-17-v3"></a>Project Service Automation 17 жаңарту шығарылымының 3-нұсқасы

[!include [banner](../includes/psa-now-project-operations.md)]

Біз Dynamics 365 жүйесіне арналған Project Service Automation бағдарламасының соңғы жаңартуын хабарлауға қуаныштымыз. Бұл шығарылым сапаға, өнімділікке және қолдану мүмкіндігіне қатысты маңызды жақсартуларды қамтиды.  Бұл шығарылым Dynamics 365 жүйесінің 9.x нұсқасымен үйлесімді. Осы шығарылымды жаңарту үшін, желідегі Dynamics 365 басқару орталығына, жаңартуды орнату үшін шешімдер бетіне өтіңіз. Қосымша ақпарат алу үшін [Таңдаулы шешімді орнату, жаңарту немесе жою](/power-platform/admin/install-remove-preferred-solution) мақаласын қараңыз.

Бұл бөлімде PSA бағдарламасының 17 жаңарту шығарылымының 3 нұсқасындағы мүмкіндіктер мен түзетулер берілген. Бұл нұсқа V3.10.6.34 құрылым нөміріне ие және әдетте 2020 жылдың наурыз айында шыққан өзін-өзі жаңарту мүмкіндігі арқылы қолжетімді.


## <a name="update-release-17"></a>17-жаңарту шығарылымы

### <a name="bug-fixes"></a>Қателерді түзету

**Жалпы**

- Бекітілді: Топ мүшелерінің лицензияларын қамтамасыз ету үшін Project Service Automation жаңартыңыз (Жоба ресурсының хабы топ мүшесі қызметінің 3.х метадеректерін қамтиды)
 
**Уақыт және шығыс**

- Бекітілді: Шығыс бағалауын нөлдік емес бағадан нөлдік (0) бағаға өзгерту мүмкін емес. Өзгеріс еленбеді.

**Жоба басқармасы**

- Бекітілді: топ мүшелерінің лауазым атына бос мәндерді тексеру қосылды.
- Бекітілді: **msdyn_userresourceid** өрісі **msdyn_resourceassignment** нысанында ескірген.
- Бекітілді: 2.x нұсқасынан 3.x нұсқасына жаңарту енді тапсырма тағайындауларындағы бос талпыныс контурларын өңдейді.

**Sales**

- Бекітілді: **Invoice.PreValidateInvoiceUpdate** енді жазба иелерін қайта тағайындау сценарийлерін дұрыс өңдейді.
- Бекітілді: транзакция класы **Уақыт** болғанда, **UnitGroup** нысаны **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, және **ContractLineDetails** нысандарын қоса алғанда барлық нысандар үшін өңделмейтін болады. Дегенмен **Бірлік** тек **JournalLine** және **InvoiceLineDetails** нысандары үшін өңделмейтін болады.




[!INCLUDE[footer-include](../includes/footer-banner.md)]