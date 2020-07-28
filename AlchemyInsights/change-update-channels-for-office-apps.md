---
title: Updatekanalen voor Office-apps wijzigen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439017"
---
# <a name="change-update-channels-for-office-apps"></a>Updatekanalen voor Office-apps wijzigen

Voor nieuwe Office-installaties gebruikt u Office-softwaredownloadinstellingen om het gewenste updatekanaal te selecteren en Office-apps vervolgens te installeren (of opnieuw te installeren). Zie [Instellingen voor software downloaden beheren in Office 365 voor](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365)meer informatie. 

**Opmerking** Het updatekanaal dat is geselecteerd met de instellingen voor het downloaden van Office-software, is van toepassing op alle gebruikers die nieuwe installaties uitvoeren met de O365-portal. Zie [Microsoft 365 of Office 2019 downloaden en installeren of opnieuw installeren op een pc of Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)voor meer informatie.   

Gebruik voor bestaande Office-installaties het Office Deployment Tool (ODT) om over te schakelen naar een ander updatekanaal:  

1. Download de nieuwste versie van het Office Deployment Tool (setup.exe) in het [Microsoft Downloadcentrum](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identificeer de naam van het kanaal waar je naar wilt overschakelen. Zie [Configuratieopties voor het Office Deployment Tool voor](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)meer informatie .
3. Maak een XML-configuratiebestand met de juiste kanaalnaam, bijvoorbeeld update.xml.  
    a. <Configuration>  
    b. <Updates **Channel="Maandelijks"** />  
    c. </Configuration>
4. Schakel vanaf een opdrachtprompt met verhoogde bevoegdheid over naar de maplocatie waar setup.exe zich bevindt en voer de volgende opdracht uit:  
    a. setup.exe /configureren update.xml
5. Start een Office-toepassing (zoals Excel) en selecteer **Bestandsaccount**  >  **Account**. Selecteer nu **bijwerken van updateopties**bijwerken in de sectie Productgegevens  >  **Update Now**.

Zie [Updatekanalen voor bestaande Office Apps voor](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel)meer informatie. 

Configureer de instelling Updatekanaal met GPO voor het schakelen van updatekanalen voor een geselecteerde groep gebruikers of met Behulp van Configuratiebeheer (SCCM). Zie [Overzicht van updatekanalen voor Microsoft 365-apps voor](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy)meer informatie. Zie Office [365 ProPlus-kanalen voor IT-professionals beheren](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) en [updates voor Microsoft 365-apps beheren met Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)voor meer informatie.