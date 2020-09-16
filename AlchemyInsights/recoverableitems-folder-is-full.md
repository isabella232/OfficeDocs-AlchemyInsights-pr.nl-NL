---
title: de map 1336 RecoverableItems is vol
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741262"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="c6e65-102">De map herstelbare items is vol</span><span class="sxs-lookup"><span data-stu-id="c6e65-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="c6e65-103">Voor postvakken van Exchange Online is de standaardopslagruimte voor de map herstelbare items 30 GB.</span><span class="sxs-lookup"><span data-stu-id="c6e65-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="c6e65-104">De opslaglimiet voor de map herstelbare items wordt automatisch verhoogd naar 100 GB als het postvak wordt geplaatst op een gerechtelijke, eDiscovery-bewaring of aan een bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="c6e65-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="c6e65-105">Wanneer de map herstelbare items de opslaglimiet bereikt, heeft dit gevolgen voor de functionaliteit van het postvak op de volgende manieren:</span><span class="sxs-lookup"><span data-stu-id="c6e65-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="c6e65-106">De gebruiker kan items uit het postvak niet verwijderen.</span><span class="sxs-lookup"><span data-stu-id="c6e65-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="c6e65-107">De Instellingsassistent voor beheerde mappen kan geen items verwijderen op basis van het Bewaar label of de instellingen van de beheerde map.</span><span class="sxs-lookup"><span data-stu-id="c6e65-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="c6e65-108">Voor postvakken waarop eenmalige items hersteld zijn of die in de wachtstand staan, kunnen de versies van door de gebruiker bewerkte pagina's niet worden bijgehouden.</span><span class="sxs-lookup"><span data-stu-id="c6e65-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="c6e65-109">Voor postvakken met een auditlogboek voor Postvak in, kunnen auditlogboek vermeldingen van het postvak niet worden opgeslagen in de submap audits in de map herstelbare items.</span><span class="sxs-lookup"><span data-stu-id="c6e65-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="c6e65-110">Voor postvakken die niet in bewaring zijn, kunnen beheerders de `Search-Mailbox -SearchDumpsterOnly -DeleteContent` opdracht in PowerShell van Exchange Online gebruiken om items in de map herstelbare items te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="c6e65-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="c6e65-111">Zie de volgende onderwerpen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="c6e65-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="c6e65-112">Berichten zoeken en verwijderen</span><span class="sxs-lookup"><span data-stu-id="c6e65-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="c6e65-113">Zoeken-Postvak</span><span class="sxs-lookup"><span data-stu-id="c6e65-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="c6e65-114">Voor postvakken die in de wacht staan, moeten beheerders de bewaring verwijderen voordat ze items kunnen verwijderen uit de map herstelbare items.</span><span class="sxs-lookup"><span data-stu-id="c6e65-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="c6e65-115">Zie voor meer informatie [items verwijderen in de map herstelbare items van de Cloud postvakken in bewaring](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="c6e65-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="c6e65-116">Om te voorkomen dat de map herstelbare items volledig wordt, kan het zijn dat beheerders de opslaglimiet van de map herstelbare items voor postvakken in de wacht zetten en het bewaarbeleid voor Postvak in instellen voor het opslaan van items in de map herstelbare items in het archief postvak van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="c6e65-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="c6e65-117">Zie [het quotum voor herstelbare items voor postvakken in de wacht zetten](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="c6e65-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
