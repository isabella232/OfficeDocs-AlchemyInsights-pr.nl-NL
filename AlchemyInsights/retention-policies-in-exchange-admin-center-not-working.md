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
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786765"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="d44c2-102">Bewaarbeleid in Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="d44c2-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="d44c2-103">**Probleem:** Nieuwe of bijgewerkte bewaarbeleid in het beheercentrum van Exchange worden niet toegepast op postvakken of items worden niet verplaatst naar de archiefmap Postvak of verwijderd.</span><span class="sxs-lookup"><span data-stu-id="d44c2-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="d44c2-104">**Belangrijkste oorzaken:**</span><span class="sxs-lookup"><span data-stu-id="d44c2-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="d44c2-p101">Dit kan zijn omdat de **Mapassistent beheerde** postbus van de gebruiker niet verwerkt. De beheerde Mapassistent probeert te verwerken elk postvak in uw organisatie op basis van een wolk om de zeven dagen. Als u een tag bewaren of ander bewaarbeleid op een postbus toepassen, kunt u wachten tot de beheerde map helpen het postvak worden verwerkt, of u kunt de cmdlet Start ManagedFolderAssistant om te beginnen de beheerde map-assistent voor het verwerken van een specifieke uitvoeren postbus. Deze cmdlet wordt uitgevoerd is handig voor het testen of het oplossen van een bewaarbeleid of tag bewaarinstellingen. Voor meer informatie gaat u naar [de Managed Mapassistent uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="d44c2-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="d44c2-110">**Oplossing:** Voer de volgende opdracht start u de beheerde map-assistent van een bepaalde postbus:</span><span class="sxs-lookup"><span data-stu-id="d44c2-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="d44c2-p102">Dit kan ook worden optreden als **RetentionHold** is **ingeschakeld** voor de postbus. Als de postbus is geplaatst op een RetentionHold, worden het bewaarbeleid voor de postbus gedurende die tijd niet worden verwerkt. Voor meer informatie over de instelling van RetentionHold Zie: [Postvak bewaren houdt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="d44c2-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="d44c2-114">**Oplossing:**</span><span class="sxs-lookup"><span data-stu-id="d44c2-114">**Solution:**</span></span>
    
  - <span data-ttu-id="d44c2-115">Controleer de status van de instelling van de RetentionHold op het specifieke postvak in [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="d44c2-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="d44c2-116">De volgende opdracht uit te **schakelen** RetentionHold op een bepaalde postbus:</span><span class="sxs-lookup"><span data-stu-id="d44c2-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="d44c2-117">Nu de beheerde map assistent opnieuw uitvoeren:</span><span class="sxs-lookup"><span data-stu-id="d44c2-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="d44c2-118">**Opmerking:** Als u een postbus kleiner is dan 10 MB, wordt de beheerde map-assistent niet automatisch verwerkt de postbus.</span><span class="sxs-lookup"><span data-stu-id="d44c2-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

