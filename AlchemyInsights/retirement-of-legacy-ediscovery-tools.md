---
title: Pensioen van Legacy eDiscovery Tools
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600359"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensioen van Legacy eDiscovery Tools

Als gevolg van de nieuwe en verbeterde eDiscovery-functionaliteit in Microsoft 365 Compliance Center, zullen de volgende legacy eDiscovery-tools en commandlets in de komende maanden worden teruggetrokken:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) en [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in het Exchange-beheercentrum.

- De Exchange Online PowerShell-cmdlets die In-Place eDiscovery en In-Place Holds ondersteunen. (Deze cmdlets worden gezamenlijk geïdentificeerd als *-MailboxSearch cmdlets.) Dit omvat de volgende cmdlets:

    - [Nieuw-PostvakZoeken](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- De [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.
- De volgende bewerkingen in de Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tijdlijn voor pensionering**:
- 1 april 2020: U geen nieuwe zoekopdrachten en wachtstanden maken, maar u bestaande zoekopdrachten nog steeds op eigen risico uitvoeren, bewerken en verwijderen. Microsoft Support biedt geen ondersteuning meer voor In-Place eDiscovery & Holds in de EAC.

- 1 juli 2020: De in-place eDiscovery & Holds functionaliteit in de EAC zal worden geplaatst in een alleen-lezen modus. Dit betekent dat u alleen bestaande zoekopdrachten en wachtstanden verwijderen.

**Zie voor meer informatie:**

 - [Oudere eDiscovery-zoekopdrachten migreren en vasthoudt aan het Microsoft 365-compliancecenter](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensioen van legacy eDiscovery-tools](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Veelgestelde vragen over In-Place eDiscovery en In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



