---
title: Bewaarbeleid in Exchange-beheercentrum werkt niet
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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742428"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Bewaarbeleid in Exchange-beheercentrum

 **Probleem:** Nieuw gemaakt of bijgewerkt bewaarbeleid in het Exchange-beheercentrum is niet van toepassing op postvakken of items worden niet verplaatst naar het archiefpostvak of worden verwijderd. 
  
 **Oorzaken:**
  
- Dit kan zijn omdat de **beheerde mapassistent** het postvak van de gebruiker niet heeft verwerkt. De managermapassistent probeert elk postvak in uw cloudorganisatie eens in de zeven dagen te verwerken. Als u een bewaartag wijzigt of een ander bewaarbeleid toepast op een postvak, u wachten tot de Manager Map Assist het postvak verwerkt of u de cmdlet StartManagedFolderAssistant uitvoeren om de beheerde mapassistent te starten om een specifiek postvak te verwerken. Het uitvoeren van deze cmdlet is handig voor het testen of oplossen van een bewaarbeleid of bewaartaginstellingen. Ga voor meer informatie naar [De assistent beheerde map uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Oplossing:** Voer de volgende opdracht uit om de beheerde mapassistent voor een specifiek postvak te starten:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dit kan ook gebeuren als **RetentionHold** is **ingeschakeld** in het postvak. Als het postvak op een retentiewacht is geplaatst, wordt het bewaarbeleid voor het postvak gedurende die periode niet verwerkt. Zie voor meer informaton op de instelling Retentiehold: [Postvakbehoud vasthouden](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Oplossing:**
    
  - Controleer de status van de instelling RetentionHold op de specifieke mailbox in [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Voer de volgende opdracht uit om RetentionHold op een specifiek postvak uit te **schakelen:**
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Voer nu de beheerde mapassistent opnieuw uit:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Let op:** Als een postvak kleiner is dan 10 MB, verwerkt de beheerde mapassistent het postvak niet automatisch.
 
Zie voor meer informatie over bewaarbeleid in het Exchange-beheercentrum:
- [Bewaartags en bewaarbeleid](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Een bewaarbeleid toepassen op postvakken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Bewaarlabels toevoegen of verwijderen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Het type wachtplaats op een postvak identificeren](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
