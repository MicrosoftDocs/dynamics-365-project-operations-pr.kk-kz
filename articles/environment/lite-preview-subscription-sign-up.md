---
title: Алдын ала қарау жазылымына тіркелу
description: Бұл тақырыпта Project Operations жеңілдетілген орналастыру бағдарламасына жазылу және оны орналастыру амалы туралы ақпарат берілген - проформа-шотын ұсыну мәмілесі.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5342466f308ab62a9f73a85fbd838d7c33bb1f47
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: kk-KZ
ms.lasthandoff: 10/16/2020
ms.locfileid: "4079523"
---
# <a name="sign-up-for-a-preview-subscription-for-lite-deployment--deal-to-proforma-invoicing"></a>Жеңілдетілген орналастыруды алдын-ала қарауға жазылыңыз - проформа-шотын ұсыну мәмілесі

Бұл тақырыпта серіктестің алдын ала ұсыныстарына және Dynamics 365 Project Operations жеңілдетілген орналастыру бағдарламасына жазылу мен оны орналастыру амалы туралы түсіндірілген - проформа-шотын ұсыну мәмілесі.

> [!NOTE]
> Бұл процесс Project Operations алдағы шығарылымдарында өзгереді.

## <a name="prerequisites"></a>Алғышарттар

- Сізге алдын-ала қарауға қатысуға шақыратын электрондық хат келеді. Алдын-ала қарауды [Project Operations веб-сайтынан](https://dynamics.microsoft.com/en-us/project-operations/overview/) сұратуға болады.
- Алдын ала қарауды орналастыратын пайдаланушының Azure қатысушысының басты әкімші құқықтары болуы керек.
- Барлық шарттар және талаптарды қарап шығыңыз.

## <a name="subscribe"></a>Жазылу

Сіз [алдын ала қарауды сұрау](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) растауын алған кезде, сізге Microsoft корпорациясынан электрондық пошта арқылы екі ұсыныс жіберіледі. Бұл ұсыныстар Project Operations алдын-ала қарауын орналастыруға мүмкіндік береді:

- Dynamics 365 Project Operations (CRM) - алдын-ала қарау нұсқасы
- Office 365 Project Operations - алдын ала қарау сынақ нұсқасы

> [!IMPORTANT]
> Бұл тапсырманы ұйымда тек бір адам, яғни қатысушы әкімші орындауы қажет. Егер сіз осы шығарылымның жазылушысы болмасаңыз, ұйымның тіркеліп, пайдаланушы тіркелгі деректерін алғанға дейін күтіңіз.

### <a name="dynamics-365-project-operations-crm---preview-trial"></a>Dynamics 365 Project Operations (CRM) - алдын-ала қарау нұсқасы 

Бастамас бұрын, браузерге Project Operations алдын ала қарауды қалайтын пайдаланушының жұмыс тіркелгісімен кіргеніңізге көз жеткізіңіз.

1. Бірінші ұсыныс кодын **Dynamics 365 Project Operations (CRM) - алдын ала қарау сынақ нұсқасы** браузердің URL мекенжайына қою арқылы оны белсендіріңіз.

![Ұсынысты белсендіру](./media/16RedeemFirstOfferNew.png)

2. Тапсырысыңызды растаңыз.
![Тапсырысты растау](./media/17ConfirmOrderNew.png)

Растау ұсынысы сәтті өтелгенін көресіз.

![Расталым](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a>Office 365 Project Operations - алдын ала қарау сынақ нұсқасы

Бірінші ұсыныс кодындағыдай қадамдарды қайталаңыз. Екінші ұсыныс кодын бірінші ұсыныс кодымен пайдаланылған пайдаланушы тіркелгісі арқылы қосқаныңызға көз жеткізіңіз.

## <a name="assign-licenses"></a>Лицензияларды тағайындау

> [!IMPORTANT]
> Келесі қадамдарды орындау үшін ұйымыңыздың Microsoft 365 порталына арналған әкімшілік қатынас қажет.


1. Пайдаланушыларыңызға лицензияларды тағайындау үшін [Microsoft 365 басқару орталығына](https://portal.office.com/) өтіңіз.

![Басқару орталығының басты беті](./media/14AdminPortal.png)

2. **Белсенді пайдаланушылар** бетінен лицензияны тағайындағыңыз келетін пайдаланушыларды таңдаңыз.

![Лицензияларды тағайындау](./media/15AssignLicenses.png)

3. **Dynamics 365 Project Operations (CRM) алдын-ала қарау** және **Office 365 Project Operations - алдын ала қарау** лицензиялары таңдалғанын тексеріңіз. 
4. **Өзгерістерді сақтау** параметрін таңдаңыз.

## <a name="create-a-new-cds-environment"></a>Жаңа CDS ортасын жасау

1. [CDS орналастыру үлгісі](lite-deployment.md) бөліміндегі нұсқауларды орындау арқылы жаңа Project Operations CDS орналастыру ортасын дайындаңыз. Орта түрін таңдағанда, міндетті түрде **Сынақ (жазылымға негізделген)** пайдаланыңыз.
![Жаңа орта](./media/19CreateEnvironment.png)

2. **Dynamics 365 бағдарламаларын қосу** параметрін таңдап, **Бағдарламаларды автоматты түрде орналастыру** өрісін бос қалдырыңыз.  
3. Орта жасау үшін **Сақтау** пәрменін таңдаңыз.

![Дерекқорды қосу](./media/20CreateEnvironment1.png)

4. Орта жасалғаннан кейін, **Microsoft Dynamics 365 Project Operations** шешімін орнатыңыз. 

![Шешім орнату](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>CDS конфигурациясын орнатып, демо деректерді реттеңіз

[Демо нұсқа параметрлері мен конфигурация деректерін қолдану](lite-apply-demo-setup-config-data.md) бөліміндегі нұсқауларды орындау арқылы CDS конфигурациясын орнатып, демо деректерді реттеңіз.
