---
title: Project Operations ресурстық/қосалқы емес сценарийлерге арналған Project Operations алдын ала қарау жазылымдарына кіру
description: Бұл тақырыпта ресурстық/қосалқы емес негіздегі сценарийлер үшін Project Operations жүйесіне жазылу және орналастыру туралы ақпарат берілген.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 75ee31e67018fe2a7655d8a8f11e40b433a9a5db6f8f2addac27844f18fffe8d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007873"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>Project Operations ресурстық/қосалқы емес сценарийлерге арналған Project Operations алдын ала қарау жазылымдарына кіру

_**Қолданылады:** Ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Бұл тақырып сынақ нұсқасы ұсынысына жазылу және ресурс/биржадан тыс негіздегі сценарийлерге арналған Project Operations бағдарламасын орналастыру жолын түсіндіреді.

## <a name="prerequisites"></a>Алғышарттар
- Алдын ала қарауды орналастыратын пайдаланушының Azure қатысушысының басты әкімші құқықтары болуы керек. Бірінші ұсыныс өтелімі кезінде қатысушыны жасауға болады. 
- Finance ортасын орналастыру үшін әр ортаға ұсынылатын жарамды Azure жазылымы қажет. Бастау үшін ұйымдарыңыздың бар жазылып немесе [Azure сынақ кезеңін](https://azure.microsoft.com/en-us/free/) пайдалануға болады. CDS ортасы шектеулі 30 күндік мерзімге тегін беріледі.

> [!IMPORTANT]
> Бұл тапсырманы ұйымда тек бір адам, яғни қатысушы әкімші орындауы қажет. Егер сіз осы шығарылымның жазылушысы болмасаңыз, ұйымның тіркеліп, пайдаланушы тіркелгі деректерін алғанға дейін күтіңіз.
> 
> Сынақ нұсқалары қатысушыда бір рет қолданылады. Сынақ нұсқасын тек бір рет ғана іске қосуға болады. Сынақ нұсқасы үшін жаңа қатысушы жасауға кеңес береміз.


### <a name="dynamics-365-project-operations-ce---preview-trial"></a>Dynamics 365 Project Operations (CE) - алдын ала қарау сынақ нұсқасы 

Бастамас бұрын, браузерге Project Operations алдын ала қарауды қалайтын пайдаланушының жұмыс тіркелгісімен кіргеніңізге көз жеткізіңіз.

1. **Dynamics 365 Project Operations** алғашқы ұсыныс кодын осы жерде [Project Operations сынақ нұсқасында](https://aka.ms/try-po) белсендіріңіз.
2. Тапсырысыңызды растаңыз.

  Растау ұсынысы сәтті өтелгенін көресіз.

### <a name="dynamics-365-finance-preview-trial"></a>Dynamics 365 Finance алдын ала қарау сынақ нұсқасы

[Dynamics 365 for Finance алдын-ала қарау сынақ нұсқасы](https://aka.ms/trypoche) бетіне өтіңіз және алдыңғы бөлімдегі қадамдарды ұсыныспен қайталаңыз, бұлт орналастырылған хостингті ортаға тіркеліңіз.  

## <a name="assign-licenses"></a>Лицензияларды тағайындау

> [!IMPORTANT]
> Келесі қадамдарды орындау үшін ұйымыңыздың Microsoft 365 порталына арналған әкімшілік қатынас қажет.

1. Пайдаланушыларыңызға лицензияларды тағайындау үшін [Microsoft 365 басқару орталығына](https://portal.office.com/) өтіңіз.

2. **Белсенді пайдаланушылар** бетінен лицензияны тағайындағыңыз келетін пайдаланушыларды таңдаңыз.

3. **Dynamics 365 Project Operations** лицензиясының таңдалғанын тексеріңіз және **Өзгерістерді сақтау** түймешігін таңдаңыз.

> [!NOTE]
> Finance сынақ ұсынысын пайдаланушыға тағайындаудың қажеті жоқ.

## <a name="start-a-new-project-in-lcs"></a>LCS параметрінде жаңа жобаны бастау

Тақырыпта сипатталғандай жаңа LCS жобасын жасаңыз,[ LCS қызметінде жаңа жобаны бастаңыз](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>LCS жобасына Azure жазылымын қосу

Бұл тапсырманы орындау үшін тақырыптағы қадамдарды орындаңыз, [LCS жобасына Azure жазылымын қосыңыз](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>Ресурстық/қосалқы емес сценарийлерге арналған Project Operations жүйесі үшін Finance демо-ортасын орналастыру

Орналастыруды аяқтау үшін тақырыптағы нұсқауларды орындаңыз, [Жаңа ортаны дайындаңыз](resource-provision-new-environment.md). Алдын ала қарау үшін [демо-орта](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) орналастыру түрін пайдаланыңыз. 

## <a name="install-cds-setup-and-configuration-data"></a>CDS параметрі және конфигурация деректерін орнату

CDS баптау және конфигурация туралы деректерді тақырыпта сипатталғандай орнатыңыз, [Common Data Service қызметіндегі конфигурация деректерін орнатыңыз және қолданыңыз](resource-apply-pro-setup-config-data.md).
Бұл қадамды қаржы демо ортасы орналастырылғаннан кейін және демо деректер дайын болғаннан кейін ғана орындаңыз.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
