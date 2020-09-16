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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="1e6c2-102">Bewaarbeleid in het Exchange-Beheercentrum</span><span class="sxs-lookup"><span data-stu-id="1e6c2-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="1e6c2-103">Als u wilt dat wij geautomatiseerde controles uitvoeren voor de instellingen die hieronder worden vermeld, selecteert u de knop terug <--boven aan deze pagina en voert u het e-mailadres in van de gebruiker die problemen heeft met het bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="1e6c2-104">**Probleem:** Nieuw gemaakt of bijgewerkt bewaarbeleid in het Exchange-Beheercentrum is niet van toepassing op postvakken of items worden niet naar het archief postvak verplaatst of verwijderd.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="1e6c2-105">**Hoofdoorzaken:**</span><span class="sxs-lookup"><span data-stu-id="1e6c2-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="1e6c2-106">Dit kan zijn omdat de **beheerde assistent** de gebruikerspostvak van de gebruiker niet heeft verwerkt.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="1e6c2-107">De Managed folder Assistant probeert elke zeven dagen elk postvak in uw organisatie in de cloud te verwerken.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="1e6c2-108">Als u een Bewaar label wijzigt of een ander bewaarbeleid op een postvak toepast, kunt u wachten tot de beheerde map het postvak ondersteunt, of u kunt de cmdlet start-ManagedFolderAssistant uitvoeren om de beheerde map te starten voor het verwerken van een specifiek postvak.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="1e6c2-109">Het uitvoeren van deze cmdlet is handig voor het testen of het oplossen van problemen met een bewaarbeleid of bewaar label instellingen.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="1e6c2-110">Ga voor meer informatie naar [de Instellingsassistent voor beheerde mappen uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="1e6c2-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="1e6c2-111">**Oplossing:** Voer de volgende opdracht uit om de beheerde map voor een specifiek postvak te starten:</span><span class="sxs-lookup"><span data-stu-id="1e6c2-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="1e6c2-112">Dit kan ook gebeuren als **RetentionHold** is **ingeschakeld** in het postvak.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="1e6c2-113">Als het postvak zich in een RetentionHold bevindt, wordt het bewaarbeleid voor het postvak niet gedurende die tijd verwerkt.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="1e6c2-114">Zie het volgende artikel voor meer gegevens over de instelling RetentionHold: [Postvak behoud bewaren](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="1e6c2-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="1e6c2-115">**Oplossingen**</span><span class="sxs-lookup"><span data-stu-id="1e6c2-115">**Solution:**</span></span>
    
  - <span data-ttu-id="1e6c2-116">Controleer de status van de instelling RetentionHold voor het specifieke postvak in [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="1e6c2-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="1e6c2-117">Voer de volgende opdracht uit om RetentionHold **uit te schakelen** voor een specifiek postvak:</span><span class="sxs-lookup"><span data-stu-id="1e6c2-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="1e6c2-118">Voer nu de beheerde mappen-assistent opnieuw uit:</span><span class="sxs-lookup"><span data-stu-id="1e6c2-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="1e6c2-119">**Opmerking:** Als een postvak kleiner is dan 10 MB, wordt het postvak niet automatisch verwerkt door de Instellingsassistent van de beheerde map.</span><span class="sxs-lookup"><span data-stu-id="1e6c2-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="1e6c2-120">Zie voor meer informatie over bewaarbeleid in het Exchange Admin Center:</span><span class="sxs-lookup"><span data-stu-id="1e6c2-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="1e6c2-121">Bewaar Tags en bewaarbeleid</span><span class="sxs-lookup"><span data-stu-id="1e6c2-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="1e6c2-122">Een bewaarbeleid toepassen op postvakken</span><span class="sxs-lookup"><span data-stu-id="1e6c2-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="1e6c2-123">Bewaar Tags toevoegen of verwijderen</span><span class="sxs-lookup"><span data-stu-id="1e6c2-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="1e6c2-124">Het type bewaring voor een postvak identificeren</span><span class="sxs-lookup"><span data-stu-id="1e6c2-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
