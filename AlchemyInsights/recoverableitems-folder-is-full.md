---
title: 1336 Map RecoverableItems is vol
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
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720247"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="99d35-102">De map Herstelbare items is vol</span><span class="sxs-lookup"><span data-stu-id="99d35-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="99d35-103">Voor Exchange Online-postvakken is de standaardopslaglimiet voor de map Herstelbare items 30 GB.</span><span class="sxs-lookup"><span data-stu-id="99d35-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="99d35-104">De opslaglimiet voor de map Herstelbare items wordt automatisch verhoogd tot 100 GB als het postvak wordt geplaatst in De wachtruimte voor geschillen, eDiscovery-blokkering of is toegewezen aan een bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="99d35-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="99d35-105">Wanneer de map Herstelbare items de opslaglimiet bereikt, wordt de postvakfunctionaliteit op de volgende manieren beïnvloed:</span><span class="sxs-lookup"><span data-stu-id="99d35-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="99d35-106">De gebruiker kan items niet uit het postvak verwijderen.</span><span class="sxs-lookup"><span data-stu-id="99d35-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="99d35-107">De beheerde mapassistent kan items niet verwijderen op basis van bewaartag of beheerde mapinstellingen.</span><span class="sxs-lookup"><span data-stu-id="99d35-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="99d35-108">Voor postvakken waarvoor herstel met één item is ingeschakeld of in de wachtstand is geplaatst, kan het kopieer-on-write-paginabeveiligingsproces geen versies van items onderhouden die door de gebruiker zijn bewerkt.</span><span class="sxs-lookup"><span data-stu-id="99d35-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="99d35-109">Voor postvakken waarvoor logboekregistratie voor postvakcontrole is ingeschakeld, kunnen geen postvakcontrolelogboekvermeldingen worden opgeslagen in de submap Audits in de map Herstelbare items.</span><span class="sxs-lookup"><span data-stu-id="99d35-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="99d35-110">Voor postvakken die niet in de wacht `Search-Mailbox -SearchDumpsterOnly -DeleteContent` staan, kunnen beheerders de opdracht in Exchange Online PowerShell gebruiken om items in de map Herstelbare items te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="99d35-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="99d35-111">Lees de volgende onderwerpen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="99d35-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="99d35-112">Berichten zoeken en verwijderen</span><span class="sxs-lookup"><span data-stu-id="99d35-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="99d35-113">Zoekpostvak</span><span class="sxs-lookup"><span data-stu-id="99d35-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="99d35-114">Voor postvakken die in de wachtstaan, moeten beheerders de blokkering verwijderen voordat ze items uit de map Herstelbare items kunnen verwijderen.</span><span class="sxs-lookup"><span data-stu-id="99d35-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="99d35-115">Zie [Items verwijderen in de map Items met herstelbare items in de wachtstand](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)in de cloud voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="99d35-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="99d35-116">Om te voorkomen dat de map Herstelbare items vol raakt, kunnen beheerders de opslaglimiet van de map Herstelbare items voor postvakine in de wacht zetten en een postvakbehoudbeleid instellen dat items van de map Herstelbare items naar het archiefpostvak van de gebruiker verplaatst.</span><span class="sxs-lookup"><span data-stu-id="99d35-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="99d35-117">Zie [Het quotum voor herstelbare items voor postvak in de wacht verhogen](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="99d35-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
