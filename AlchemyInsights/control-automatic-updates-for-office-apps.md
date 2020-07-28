---
title: Automatische updates voor Office Apps beheren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438993"
---
# <a name="control-automatic-updates-for-office-apps"></a>Automatische updates voor Office Apps beheren

Updates voor Office Apps worden standaard automatisch gedownload en op de achtergrond toegepast zonder tussenkomst van de gebruiker. Beheerders kunnen echter bepalen hoe updates worden toegepast met behulp van Office Update-instellingen. Met de update-instellingen kunnen beheerders automatische updates in- of uitschakelen, de knop **Nu bijwerken** in Office weergeven of verbergen, updatedeadlines instellen en meer. Zie voor gedetailleerde informatie:

- [Update-instellingen voor Office configureren](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatisch bijwerken voor Office is niet ingeschakeld](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definiëren hoe Office wordt bijgewerkt nadat het is geïnstalleerd](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Voer de volgende stappen uit om de bestaande updates-instellingen te controleren die op een clientmachine zijn toegepast:

1. Open de registereditor door naar **Start**  >  **Run**  >  **regedit**te gaan.
2. Ga naar de volgende locatie en bekijk de instellingen van Office Update:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuratie

**Opmerking**  Als de OfficeMgmtCOM-sleutel is ingesteld, ziet u mogelijk het bericht **Office**'Updates worden beheerd door uw systeembeheerder' in  >  **Office-updates voor**Office office van Office  >  **Office Updates**. Zie [Updates voor Microsoft 365-apps beheren met Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)voor meer informatie.  