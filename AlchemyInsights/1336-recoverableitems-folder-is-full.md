---
title: 1336 RecoverableItems map is vol
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: dbf4930c34e4175a14b77fab4eafc953bb37cc02
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29909283"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="fb53b-102">De herstelbare Items map is vol</span><span class="sxs-lookup"><span data-stu-id="fb53b-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="fb53b-p101">Voor de Exchange Online-postvakken in Office 365 is de standaard opslaglimiet voor de map herstelbare Items 30 GB. De opslaglimiet voor de map herstelbare Items automatisch verhoogd naar 100 GB als het postvak op de rechtszaak houdt, eDiscovery-wacht wordt geplaatst of is toegewezen aan een bewaarbeleid Office 365.</span><span class="sxs-lookup"><span data-stu-id="fb53b-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="fb53b-105">Als de map herstelbare Items de opslaglimiet bereikt, postbus functionaliteit is waarin dit probleem optreedt op de volgende manieren:</span><span class="sxs-lookup"><span data-stu-id="fb53b-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="fb53b-106">De gebruiker kan items uit het postvak verwijderen.</span><span class="sxs-lookup"><span data-stu-id="fb53b-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="fb53b-107">De beheerde Mapassistent verwijderen artikelen op basis van inhoudingen tag of instellingen van beheerde mappen niet.</span><span class="sxs-lookup"><span data-stu-id="fb53b-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="fb53b-108">Voor postvakken die één Item herstellen ingeschakeld of in de wachtstand worden geplaatst, kan niet de bescherming pagina kopiëren tijdens het schrijven proces versies van items bewerkt door de gebruiker onderhouden.</span><span class="sxs-lookup"><span data-stu-id="fb53b-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="fb53b-109">Voor postvakken die postbus controlegebeurtenissen vastleggen is ingeschakeld, kunnen geen logboekvermeldingen postbus controle worden opgeslagen in de submap kunnen worden opgeslagen in de map Items terug te vorderen.</span><span class="sxs-lookup"><span data-stu-id="fb53b-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="fb53b-p102">Postvakken die niet in de wachtstand, beheerders kunt gebruiken de `Search-Mailbox -SearchDumpsterOnly -DeleteContent` opdracht in Exchange Online PowerShell verwijderen van items in de map Items terug te vorderen. Zie de volgende onderwerpen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="fb53b-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="fb53b-112">Zoek en verwijder berichten</span><span class="sxs-lookup"><span data-stu-id="fb53b-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="fb53b-113">Zoeken-postbus</span><span class="sxs-lookup"><span data-stu-id="fb53b-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="fb53b-p103">Voor postbussen die geblokkeerd zijn, moeten beheerders de blokkering verwijderen voordat ze verwijderde items uit de map Items terug te vorderen kunnen. Zie de [items in de map van de postvakken op cloud-gebaseerde houdt herstelbare Items verwijderen](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="fb53b-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="fb53b-p104">Om te voorkomen dat de herstelbare Items map vol raken, kan beheerders de opslaglimiet van de herstelbare Items, map voor postvakken op houdt en instellen van een postbus bewaarbeleid die items uit de map herstelbare Items naar het archief van de gebruiker verplaatst toenemen postbus. Zie het [verhogen van de herstelbare Items voor postvakken op houdt](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="fb53b-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

