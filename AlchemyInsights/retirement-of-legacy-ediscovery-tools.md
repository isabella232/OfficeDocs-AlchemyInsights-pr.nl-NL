---
title: Pensionering van oudere eDiscovery-Hulpprogramma's
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727778"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="ab92c-102">Pensionering van oudere eDiscovery-Hulpprogramma's</span><span class="sxs-lookup"><span data-stu-id="ab92c-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="ab92c-103">Als gevolg van de nieuwe en verbeterde eDiscovery-functionaliteit in Microsoft 365 compliance, worden de volgende oudere eDiscovery-hulpprogramma's en Commandlets in de komende maanden buiten gebruik gesteld:</span><span class="sxs-lookup"><span data-stu-id="ab92c-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="ab92c-104">[In-place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) en [in-place bewarings ruimte](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in het Exchange-Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ab92c-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="ab92c-105">De Exchange Online PowerShell-cmdlets die in-place eDiscovery en in-place bewaring ondersteunen.</span><span class="sxs-lookup"><span data-stu-id="ab92c-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="ab92c-106">(Deze cmdlets worden gezamenlijk aangeduid als MailboxSearch-cmdlets.) Dit omvat de volgende cmdlets:</span><span class="sxs-lookup"><span data-stu-id="ab92c-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="ab92c-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ab92c-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="ab92c-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ab92c-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="ab92c-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ab92c-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="ab92c-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ab92c-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="ab92c-111">De cmdlet [Search-mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ab92c-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="ab92c-112">De volgende bewerkingen in de Exchange Web Services-API:</span><span class="sxs-lookup"><span data-stu-id="ab92c-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="ab92c-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="ab92c-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="ab92c-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ab92c-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="ab92c-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ab92c-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="ab92c-116">Geavanceerd eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="ab92c-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="ab92c-117">**Tijdlijn voor pensionering**:</span><span class="sxs-lookup"><span data-stu-id="ab92c-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="ab92c-118">Woensdag **1 juli 2020** U kunt niet langer nieuwe zoekopdrachten en wachtruimten maken, maar u kunt op uw eigen risico bestaande zoekopdrachten uitvoeren, bewerken en verwijderen.</span><span class="sxs-lookup"><span data-stu-id="ab92c-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="ab92c-119">Microsoft ondersteuning biedt niet langer ondersteuning voor in-place eDiscovery-& bewaard in het Exchange-Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ab92c-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="ab92c-120">Maandag **1 oktober 2020** In-place eDiscovery-& Bewaar functies in het Exchange-Beheercentrum worden in de modus alleen-lezen gezet, zodat u alleen bestaande zoekopdrachten en wachtstand kunt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="ab92c-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="ab92c-121">**Zie voor meer informatie**:</span><span class="sxs-lookup"><span data-stu-id="ab92c-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="ab92c-122">Verouderde eDiscovery-zoekopdrachten en wachtruimten naar het nalevings centrum voor Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ab92c-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="ab92c-123">Buitengebruikstelling van verouderde eDiscovery-hulpprogramma's</span><span class="sxs-lookup"><span data-stu-id="ab92c-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="ab92c-124">Veelgestelde vragen over in-place eDiscovery en wachtstand</span><span class="sxs-lookup"><span data-stu-id="ab92c-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



