---
title: Bewaarbeleid in Exchange Admin Center werkt niet
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502602"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Bewaarbeleid in Exchange-beheercentrum

 **Probleem:** Nieuw gemaakt of bijgewerkt bewaarbeleid in het Exchange-beheercentrum is niet van toepassing op postvakken of items worden niet verplaatst naar het archiefpostvak of worden verwijderd. 
  
 **Oorzaken:**
  
- Dit kan zijn omdat de **assistent beheerde mappen** het postvak van de gebruiker niet heeft verwerkt. De Managed Folder Assistant probeert elk postvak in uw cloudorganisatie eens in de zeven dagen te verwerken. Als u een bewaartag wijzigt of een ander bewaarbeleid toepast op een postvak, u wachten tot de assist voor beheerde map het postvak verwerkt of u de cmdlet Start-ManagedFolderAssistant uitvoeren om de assistent van beheerde mappen te starten om een specifiek postvak te verwerken. Het uitvoeren van deze cmdlet is handig voor het testen of oplossen van een bewaarbeleid of het bewaren van tags. Ga voor meer informatie naar [De assistent van de beheerde map uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Oplossing:** Voer de volgende opdracht uit om de assistent van beheerde mappen voor een specifiek postvak te starten:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dit kan ook gebeuren als **RetentionHold** is **ingeschakeld** op het postvak. Als het postvak op een Bewaarplaats is geplaatst, wordt het bewaarbeleid voor het postvak gedurende die tijd niet verwerkt. Zie voor meer informaton op de instelling RetentionHold: [Postvakretentie.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **Oplossing:**
    
  - Controleer de status van de instelling RetentionHold op het specifieke postvak in [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Voer de volgende opdracht uit om RetentionHold uit te **schakelen** op een specifiek postvak:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Voer nu de assistent van de beheerde map opnieuw uit:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Let op:** Als een postvak kleiner is dan 10 MB, verwerkt de assistent van beheerde mappen het postvak niet automatisch.
 
Zie voor meer informatie over bewaarbeleid in het Exchange-beheercentrum:
- [Bewaartags en bewaarbeleid](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Een bewaarbeleid toepassen op postvakken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Bewaartags toevoegen of verwijderen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Het type wacht op een postvak identificeren](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
