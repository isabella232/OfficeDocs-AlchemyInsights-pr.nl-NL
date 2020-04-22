---
title: Pensionering van Legacy eDiscovery Tools
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650563"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="fb92d-102">Pensionering van Legacy eDiscovery Tools</span><span class="sxs-lookup"><span data-stu-id="fb92d-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="fb92d-103">Als gevolg van de nieuwe en verbeterde eDiscovery-functionaliteit in het Microsoft 365 Compliance Center worden in de komende maanden de volgende verouderde eDiscovery-tools en -opdrachten uitgeschakeld:</span><span class="sxs-lookup"><span data-stu-id="fb92d-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="fb92d-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) en [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in het Exchange-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="fb92d-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="fb92d-105">De Exchange Online PowerShell-cmdlets die In-Place eDiscovery en In-Place Holds ondersteunen.</span><span class="sxs-lookup"><span data-stu-id="fb92d-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="fb92d-106">(Deze cmdlets zijn gezamenlijk geïdentificeerd als \*-MailboxSearch cmdlets.) Dit omvat de volgende cmdlets:</span><span class="sxs-lookup"><span data-stu-id="fb92d-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="fb92d-107">Nieuw-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fb92d-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="fb92d-108">Start-mailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fb92d-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="fb92d-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fb92d-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="fb92d-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fb92d-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="fb92d-111">De [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fb92d-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="fb92d-112">De volgende bewerkingen in de Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="fb92d-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="fb92d-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="fb92d-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="fb92d-114">SetHoldOnMailboxen</span><span class="sxs-lookup"><span data-stu-id="fb92d-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="fb92d-115">GetHoldOnMailboxen</span><span class="sxs-lookup"><span data-stu-id="fb92d-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="fb92d-116">Geavanceerde eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="fb92d-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="fb92d-117">**Tijdschema voor pensionering**:</span><span class="sxs-lookup"><span data-stu-id="fb92d-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="fb92d-118">1 april 2020: U geen nieuwe zoekopdrachten en wachtadressen maken, maar u bestaande zoekopdrachten nog steeds uitvoeren, bewerken en verwijderen op eigen risico.</span><span class="sxs-lookup"><span data-stu-id="fb92d-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="fb92d-119">Microsoft Support biedt geen ondersteuning meer voor In-Place eDiscovery & Holds in de EAC.</span><span class="sxs-lookup"><span data-stu-id="fb92d-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="fb92d-120">1 juli 2020: De In-Place eDiscovery & Holds-functionaliteit in de EAC wordt in een alleen-lezen modus geplaatst.</span><span class="sxs-lookup"><span data-stu-id="fb92d-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="fb92d-121">Dit betekent dat u alleen bestaande zoekopdrachten en houdt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="fb92d-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="fb92d-122">**Zie voor meer informatie:**</span><span class="sxs-lookup"><span data-stu-id="fb92d-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="fb92d-123">Oudere eDiscovery-zoekopdrachten en -voorschriften migreren naar het Microsoft 365-compliancecentrum</span><span class="sxs-lookup"><span data-stu-id="fb92d-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="fb92d-124">Pensionering van verouderde eDiscovery-tools</span><span class="sxs-lookup"><span data-stu-id="fb92d-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="fb92d-125">Veelgestelde vragen over In-Place eDiscovery en In-Place Holds</span><span class="sxs-lookup"><span data-stu-id="fb92d-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



