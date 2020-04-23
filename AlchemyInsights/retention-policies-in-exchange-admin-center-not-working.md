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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="844c9-102">Bewaarbeleid in Exchange-beheercentrum</span><span class="sxs-lookup"><span data-stu-id="844c9-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="844c9-103">**Probleem:** Nieuw gemaakt of bijgewerkt bewaarbeleid in het Exchange-beheercentrum is niet van toepassing op postvakken of items worden niet verplaatst naar het archiefpostvak of worden verwijderd.</span><span class="sxs-lookup"><span data-stu-id="844c9-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="844c9-104">**Oorzaken:**</span><span class="sxs-lookup"><span data-stu-id="844c9-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="844c9-105">Dit kan zijn omdat de **beheerde mapassistent** het postvak van de gebruiker niet heeft verwerkt.</span><span class="sxs-lookup"><span data-stu-id="844c9-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="844c9-106">De managermapassistent probeert elk postvak in uw cloudorganisatie eens in de zeven dagen te verwerken.</span><span class="sxs-lookup"><span data-stu-id="844c9-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="844c9-107">Als u een bewaartag wijzigt of een ander bewaarbeleid toepast op een postvak, u wachten tot de Manager Map Assist het postvak verwerkt of u de cmdlet StartManagedFolderAssistant uitvoeren om de beheerde mapassistent te starten om een specifiek postvak te verwerken.</span><span class="sxs-lookup"><span data-stu-id="844c9-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="844c9-108">Het uitvoeren van deze cmdlet is handig voor het testen of oplossen van een bewaarbeleid of bewaartaginstellingen.</span><span class="sxs-lookup"><span data-stu-id="844c9-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="844c9-109">Ga voor meer informatie naar [De assistent beheerde map uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="844c9-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="844c9-110">**Oplossing:** Voer de volgende opdracht uit om de beheerde mapassistent voor een specifiek postvak te starten:</span><span class="sxs-lookup"><span data-stu-id="844c9-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="844c9-111">Dit kan ook gebeuren als **RetentionHold** is **ingeschakeld** in het postvak.</span><span class="sxs-lookup"><span data-stu-id="844c9-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="844c9-112">Als het postvak op een retentiewacht is geplaatst, wordt het bewaarbeleid voor het postvak gedurende die periode niet verwerkt.</span><span class="sxs-lookup"><span data-stu-id="844c9-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="844c9-113">Zie voor meer informaton op de instelling Retentiehold: [Postvakbehoud vasthouden](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="844c9-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="844c9-114">**Oplossing:**</span><span class="sxs-lookup"><span data-stu-id="844c9-114">**Solution:**</span></span>
    
  - <span data-ttu-id="844c9-115">Controleer de status van de instelling RetentionHold op de specifieke mailbox in [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="844c9-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="844c9-116">Voer de volgende opdracht uit om RetentionHold op een specifiek postvak uit te **schakelen:**</span><span class="sxs-lookup"><span data-stu-id="844c9-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="844c9-117">Voer nu de beheerde mapassistent opnieuw uit:</span><span class="sxs-lookup"><span data-stu-id="844c9-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="844c9-118">**Let op:** Als een postvak kleiner is dan 10 MB, verwerkt de beheerde mapassistent het postvak niet automatisch.</span><span class="sxs-lookup"><span data-stu-id="844c9-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="844c9-119">Zie voor meer informatie over bewaarbeleid in het Exchange-beheercentrum:</span><span class="sxs-lookup"><span data-stu-id="844c9-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="844c9-120">Bewaartags en bewaarbeleid</span><span class="sxs-lookup"><span data-stu-id="844c9-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="844c9-121">Een bewaarbeleid toepassen op postvakken</span><span class="sxs-lookup"><span data-stu-id="844c9-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="844c9-122">Bewaarlabels toevoegen of verwijderen</span><span class="sxs-lookup"><span data-stu-id="844c9-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="844c9-123">Het type wachtplaats op een postvak identificeren</span><span class="sxs-lookup"><span data-stu-id="844c9-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
