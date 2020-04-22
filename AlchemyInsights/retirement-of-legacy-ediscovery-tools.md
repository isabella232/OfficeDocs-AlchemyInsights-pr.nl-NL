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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionering van Legacy eDiscovery Tools

Als gevolg van de nieuwe en verbeterde eDiscovery-functionaliteit in het Microsoft 365 Compliance Center worden in de komende maanden de volgende verouderde eDiscovery-tools en -opdrachten uitgeschakeld:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) en [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in het Exchange-beheercentrum.

- De Exchange Online PowerShell-cmdlets die In-Place eDiscovery en In-Place Holds ondersteunen. (Deze cmdlets zijn gezamenlijk geïdentificeerd als *-MailboxSearch cmdlets.) Dit omvat de volgende cmdlets:

    - [Nieuw-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-mailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- De [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.
- De volgende bewerkingen in de Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxen](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxen](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Geavanceerde eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tijdschema voor pensionering**:
- 1 april 2020: U geen nieuwe zoekopdrachten en wachtadressen maken, maar u bestaande zoekopdrachten nog steeds uitvoeren, bewerken en verwijderen op eigen risico. Microsoft Support biedt geen ondersteuning meer voor In-Place eDiscovery & Holds in de EAC.

- 1 juli 2020: De In-Place eDiscovery & Holds-functionaliteit in de EAC wordt in een alleen-lezen modus geplaatst. Dit betekent dat u alleen bestaande zoekopdrachten en houdt verwijderen.

**Zie voor meer informatie:**

 - [Oudere eDiscovery-zoekopdrachten en -voorschriften migreren naar het Microsoft 365-compliancecentrum](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensionering van verouderde eDiscovery-tools](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Veelgestelde vragen over In-Place eDiscovery en In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



