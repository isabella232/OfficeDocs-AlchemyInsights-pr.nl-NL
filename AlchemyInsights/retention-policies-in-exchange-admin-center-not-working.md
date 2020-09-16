---
title: Bewaarbeleid in het Exchange-Beheercentrum werkt niet
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740505"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Bewaarbeleid in het Exchange-Beheercentrum

Als u wilt dat wij geautomatiseerde controles uitvoeren voor de instellingen die hieronder worden vermeld, selecteert u de knop terug <--boven aan deze pagina en voert u het e-mailadres in van de gebruiker die problemen heeft met het bewaarbeleid.

 **Probleem:** Nieuw gemaakt of bijgewerkt bewaarbeleid in het Exchange-Beheercentrum is niet van toepassing op postvakken of items worden niet naar het archief postvak verplaatst of verwijderd. 
  
 **Hoofdoorzaken:**
  
- Dit kan zijn omdat de **beheerde assistent** de gebruikerspostvak van de gebruiker niet heeft verwerkt. De Managed folder Assistant probeert elke zeven dagen elk postvak in uw organisatie in de cloud te verwerken. Als u een Bewaar label wijzigt of een ander bewaarbeleid op een postvak toepast, kunt u wachten tot de beheerde map het postvak ondersteunt, of u kunt de cmdlet start-ManagedFolderAssistant uitvoeren om de beheerde map te starten voor het verwerken van een specifiek postvak. Het uitvoeren van deze cmdlet is handig voor het testen of het oplossen van problemen met een bewaarbeleid of bewaar label instellingen. Ga voor meer informatie naar [de Instellingsassistent voor beheerde mappen uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Oplossing:** Voer de volgende opdracht uit om de beheerde map voor een specifiek postvak te starten:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dit kan ook gebeuren als **RetentionHold** is **ingeschakeld** in het postvak. Als het postvak zich in een RetentionHold bevindt, wordt het bewaarbeleid voor het postvak niet gedurende die tijd verwerkt. Zie het volgende artikel voor meer gegevens over de instelling RetentionHold: [Postvak behoud bewaren](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Oplossingen**
    
  - Controleer de status van de instelling RetentionHold voor het specifieke postvak in [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Voer de volgende opdracht uit om RetentionHold **uit te schakelen** voor een specifiek postvak:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Voer nu de beheerde mappen-assistent opnieuw uit:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Opmerking:** Als een postvak kleiner is dan 10 MB, wordt het postvak niet automatisch verwerkt door de Instellingsassistent van de beheerde map.
 
Zie voor meer informatie over bewaarbeleid in het Exchange Admin Center:
- [Bewaar Tags en bewaarbeleid](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Een bewaarbeleid toepassen op postvakken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Bewaar Tags toevoegen of verwijderen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Het type bewaring voor een postvak identificeren](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
