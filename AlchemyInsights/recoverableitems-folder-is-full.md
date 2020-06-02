---
title: Map 1336 RecoverableItems is vol
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510747"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="6447f-102">De map Herstelbare items is vol</span><span class="sxs-lookup"><span data-stu-id="6447f-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="6447f-103">Voor Exchange Online-postvakken is de standaardopslaglimiet voor de map Herstelbare items 30 GB.</span><span class="sxs-lookup"><span data-stu-id="6447f-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="6447f-104">De opslaglimiet voor de map Herstelbare items wordt automatisch verhoogd tot 100 GB als het postvak wordt geplaatst in Litigation Hold, eDiscovery hold of is toegewezen aan een bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="6447f-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="6447f-105">Wanneer de map Herstelbare items de opslaglimiet bereikt, wordt de functionaliteit van het postvak op de volgende manieren beïnvloed:</span><span class="sxs-lookup"><span data-stu-id="6447f-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="6447f-106">De gebruiker kan geen items uit het postvak verwijderen.</span><span class="sxs-lookup"><span data-stu-id="6447f-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="6447f-107">De assistent voor beheerde mappen kan items niet verwijderen op basis van bewaartag of instellingen voor beheerde mappen.</span><span class="sxs-lookup"><span data-stu-id="6447f-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="6447f-108">Voor postvakken waarvoor single itemherstel is ingeschakeld of in de wacht wordt gezet, kan het proces voor kopieerpaginabeveiliging geen versies van door de gebruiker bewerkte items onderhouden.</span><span class="sxs-lookup"><span data-stu-id="6447f-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="6447f-109">Voor postvakken waarvoor postvakcontroleregistratie is ingeschakeld, kunnen geen logboekgegevens van postvakken worden opgeslagen in de submap Audits in de map Herstelbare items.</span><span class="sxs-lookup"><span data-stu-id="6447f-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="6447f-110">Voor postvakken die niet in de wacht staan, kunnen beheerders de opdracht in Exchange Online PowerShell gebruiken `Search-Mailbox -SearchDumpsterOnly -DeleteContent` om items in de map Herstelbare items te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="6447f-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="6447f-111">Lees de volgende onderwerpen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="6447f-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="6447f-112">Berichten zoeken en verwijderen</span><span class="sxs-lookup"><span data-stu-id="6447f-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="6447f-113">Zoekpostvak</span><span class="sxs-lookup"><span data-stu-id="6447f-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="6447f-114">Voor postvakken die in de wacht staan, moeten beheerders de wachtruimte verwijderen voordat ze items uit de map Herstelbare items kunnen verwijderen.</span><span class="sxs-lookup"><span data-stu-id="6447f-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="6447f-115">Zie [Items verwijderen in de map Herstelbare items van postvakken in de cloud in de wachtstand](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="6447f-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="6447f-116">Om te voorkomen dat de map Herstelbare items vol raakt, kunnen beheerders de opslaglimiet van de map Herstelbare items voor postvakken in de wacht verhogen en een beleid voor het bewaren van postvakken instellen dat items verplaatst vanuit de map Herstelbare items naar het archiefpostvak van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="6447f-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="6447f-117">Zie [Het quotum herstelbare items voor postvakken in de wacht vergroten](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="6447f-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
