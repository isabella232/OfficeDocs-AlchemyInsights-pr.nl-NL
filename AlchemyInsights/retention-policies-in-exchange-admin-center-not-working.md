---
title: Bewaarbeleid in Exchange Admin Center werkt niet
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6c69511f6bcdad5793cd2473a20a2d168d2ac260
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660702"
---
 **Probleem:** Nieuwe of bijgewerkte bewaarbeleid in het beheercentrum van Exchange worden niet toegepast op postvakken of items worden niet verplaatst naar de archiefmap Postvak of verwijderd. 
  
 **Belangrijkste oorzaken:**
  
- Dit kan zijn omdat de **Mapassistent beheerde** postbus van de gebruiker niet verwerkt. De beheerde Mapassistent probeert te verwerken elk postvak in uw organisatie op basis van een wolk om de zeven dagen. Als u een tag bewaren of ander bewaarbeleid op een postbus toepassen, kunt u wachten tot de beheerde map helpen het postvak worden verwerkt, of u kunt de cmdlet Start ManagedFolderAssistant om te beginnen de beheerde map-assistent voor het verwerken van een specifieke uitvoeren postbus. Deze cmdlet wordt uitgevoerd is handig voor het testen of het oplossen van een bewaarbeleid of tag bewaarinstellingen. Voor meer informatie gaat u naar [de Managed Mapassistent uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Oplossing:** Voer de volgende opdracht start u de beheerde map-assistent van een bepaalde postbus: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dit kan ook worden optreden als **RetentionHold** is **ingeschakeld** voor de postbus. Als de postbus is geplaatst op een RetentionHold, worden het bewaarbeleid voor de postbus gedurende die tijd niet worden verwerkt. Voor meer informatie over de instelling van RetentionHold Zie: [Postvak bewaren houdt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Oplossing:**
    
  - Controleer de status van de instelling van de RetentionHold op het specifieke postvak in [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - De volgende opdracht uit te **schakelen** RetentionHold op een bepaalde postbus: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Nu de beheerde map assistent opnieuw uitvoeren:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Opmerking:** Als u een postbus kleiner is dan 10 MB, wordt de beheerde map-assistent niet automatisch verwerkt de postbus. 
  

