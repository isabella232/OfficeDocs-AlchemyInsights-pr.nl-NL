---
title: Bewaarbeleid in Exchange Admin Center werkt niet
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444803"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="41cba-102">Bewaarbeleid in Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="41cba-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="41cba-103">**Probleem:** Nieuwe of bijgewerkte bewaarbeleid in het beheercentrum van Exchange worden niet toegepast op postvakken of items worden niet verplaatst naar de archiefmap Postvak of verwijderd.</span><span class="sxs-lookup"><span data-stu-id="41cba-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="41cba-104">**Belangrijkste oorzaken:**</span><span class="sxs-lookup"><span data-stu-id="41cba-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="41cba-105">Dit kan zijn omdat de **Mapassistent beheerde** postbus van de gebruiker niet verwerkt.</span><span class="sxs-lookup"><span data-stu-id="41cba-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="41cba-106">De beheerde Mapassistent probeert te verwerken elk postvak in uw organisatie op basis van een wolk om de zeven dagen.</span><span class="sxs-lookup"><span data-stu-id="41cba-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="41cba-107">Als u een tag bewaren of ander bewaarbeleid op een postbus toepassen, kunt u wachten tot de beheerde map helpen het postvak worden verwerkt, of u kunt de cmdlet Start ManagedFolderAssistant om te beginnen de beheerde map-assistent voor het verwerken van een specifieke uitvoeren postbus.</span><span class="sxs-lookup"><span data-stu-id="41cba-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="41cba-108">Deze cmdlet wordt uitgevoerd is handig voor het testen of het oplossen van een bewaarbeleid of tag bewaarinstellingen.</span><span class="sxs-lookup"><span data-stu-id="41cba-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="41cba-109">Voor meer informatie gaat u naar [de Managed Mapassistent uitvoeren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="41cba-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="41cba-110">**Oplossing:** Voer de volgende opdracht start u de beheerde map-assistent van een bepaalde postbus:</span><span class="sxs-lookup"><span data-stu-id="41cba-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="41cba-111">Dit kan ook worden optreden als **RetentionHold** is **ingeschakeld** voor de postbus.</span><span class="sxs-lookup"><span data-stu-id="41cba-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="41cba-112">Als de postbus is geplaatst op een RetentionHold, worden het bewaarbeleid voor de postbus gedurende die tijd niet worden verwerkt.</span><span class="sxs-lookup"><span data-stu-id="41cba-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="41cba-113">Voor meer informatie over de instelling van RetentionHold Zie: [Postvak bewaren houdt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="41cba-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="41cba-114">**Oplossing:**</span><span class="sxs-lookup"><span data-stu-id="41cba-114">**Solution:**</span></span>
    
  - <span data-ttu-id="41cba-115">Controleer de status van de instelling van de RetentionHold op het specifieke postvak in [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="41cba-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="41cba-116">De volgende opdracht uit te **schakelen** RetentionHold op een bepaalde postbus:</span><span class="sxs-lookup"><span data-stu-id="41cba-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="41cba-117">Nu de beheerde map assistent opnieuw uitvoeren:</span><span class="sxs-lookup"><span data-stu-id="41cba-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="41cba-118">**Opmerking:** Als u een postbus kleiner is dan 10 MB, wordt de beheerde map-assistent niet automatisch verwerkt de postbus.</span><span class="sxs-lookup"><span data-stu-id="41cba-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="41cba-119">Zie voor meer informatie over bewaarbeleid in het beheercentrum van Exchange:</span><span class="sxs-lookup"><span data-stu-id="41cba-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="41cba-120">Behoud tags en bewaarbeleid</span><span class="sxs-lookup"><span data-stu-id="41cba-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="41cba-121">Een bewaarbeleid voor postvakken van toepassing</span><span class="sxs-lookup"><span data-stu-id="41cba-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="41cba-122">Toevoegen of verwijderen van codes bewaren</span><span class="sxs-lookup"><span data-stu-id="41cba-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="41cba-123">Het identificeren van het type blokkering geplaatst op een postbus</span><span class="sxs-lookup"><span data-stu-id="41cba-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
