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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522802"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="4b97c-102">Bewaarbeleid in Exchange-beheercentrum</span><span class="sxs-lookup"><span data-stu-id="4b97c-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="4b97c-103">Als u wilt dat we geautomatiseerde controles uitvoeren voor de onderstaande instellingen, selecteert u de terugknop <- boven aan deze pagina en voert u het e-mailadres in van de gebruiker die problemen heeft met het bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="4b97c-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="4b97c-104">**Probleem:** Nieuw gemaakt of bijgewerkt bewaarbeleid in het Exchange-beheercentrum is niet van toepassing op postvakken of items worden niet verplaatst naar het archiefpostvak of worden verwijderd.</span><span class="sxs-lookup"><span data-stu-id="4b97c-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="4b97c-105">**Oorzaken:**</span><span class="sxs-lookup"><span data-stu-id="4b97c-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="4b97c-106">Dit kan zijn omdat de **assistent beheerde mappen** het postvak van de gebruiker niet heeft verwerkt.</span><span class="sxs-lookup"><span data-stu-id="4b97c-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="4b97c-107">De Managed Folder Assistant probeert elk postvak in uw cloudorganisatie eens in de zeven dagen te verwerken.</span><span class="sxs-lookup"><span data-stu-id="4b97c-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="4b97c-108">Als u een bewaartag wijzigt of een ander bewaarbeleid toepast op een postvak, u wachten tot de assist voor beheerde map het postvak verwerkt of u de cmdlet Start-ManagedFolderAssistant uitvoeren om de assistent van beheerde mappen te starten om een specifiek postvak te verwerken.</span><span class="sxs-lookup"><span data-stu-id="4b97c-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="4b97c-109">Het uitvoeren van deze cmdlet is handig voor het testen of oplossen van een bewaarbeleid of het bewaren van tags.</span><span class="sxs-lookup"><span data-stu-id="4b97c-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="4b97c-110">Ga voor meer informatie naar [De assistent van de beheerde map uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="4b97c-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="4b97c-111">**Oplossing:** Voer de volgende opdracht uit om de assistent van beheerde mappen voor een specifiek postvak te starten:</span><span class="sxs-lookup"><span data-stu-id="4b97c-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="4b97c-112">Dit kan ook gebeuren als **RetentionHold** is **ingeschakeld** op het postvak.</span><span class="sxs-lookup"><span data-stu-id="4b97c-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="4b97c-113">Als het postvak op een Bewaarplaats is geplaatst, wordt het bewaarbeleid voor het postvak gedurende die tijd niet verwerkt.</span><span class="sxs-lookup"><span data-stu-id="4b97c-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="4b97c-114">Zie voor meer informaton op de instelling RetentionHold: [Postvakretentie.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="4b97c-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="4b97c-115">**Oplossing:**</span><span class="sxs-lookup"><span data-stu-id="4b97c-115">**Solution:**</span></span>
    
  - <span data-ttu-id="4b97c-116">Controleer de status van de instelling RetentionHold op het specifieke postvak in [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="4b97c-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="4b97c-117">Voer de volgende opdracht uit om RetentionHold uit te **schakelen** op een specifiek postvak:</span><span class="sxs-lookup"><span data-stu-id="4b97c-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="4b97c-118">Voer nu de assistent van de beheerde map opnieuw uit:</span><span class="sxs-lookup"><span data-stu-id="4b97c-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="4b97c-119">**Let op:** Als een postvak kleiner is dan 10 MB, verwerkt de assistent van beheerde mappen het postvak niet automatisch.</span><span class="sxs-lookup"><span data-stu-id="4b97c-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="4b97c-120">Zie voor meer informatie over bewaarbeleid in het Exchange-beheercentrum:</span><span class="sxs-lookup"><span data-stu-id="4b97c-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="4b97c-121">Bewaartags en bewaarbeleid</span><span class="sxs-lookup"><span data-stu-id="4b97c-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="4b97c-122">Een bewaarbeleid toepassen op postvakken</span><span class="sxs-lookup"><span data-stu-id="4b97c-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="4b97c-123">Bewaartags toevoegen of verwijderen</span><span class="sxs-lookup"><span data-stu-id="4b97c-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="4b97c-124">Het type bewaring voor een postvak identificeren</span><span class="sxs-lookup"><span data-stu-id="4b97c-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
