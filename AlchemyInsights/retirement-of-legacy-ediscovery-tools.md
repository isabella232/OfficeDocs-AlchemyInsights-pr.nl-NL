---
title: Pensioen van oudere eDiscovery-hulpprogramma's
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798544"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensioen van oudere eDiscovery-hulpprogramma's

Als gevolg van de nieuwe en verbeterde eDiscovery-functionaliteit in het Microsoft 365 Compliance center worden de volgende oudere eDiscovery-hulpprogramma's en commandlets in de komende maanden ingetrokken:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) en [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in het Exchange-beheercentrum.

- De Exchange Online PowerShell-cmdlets die ondersteuning bieden In-Place eDiscovery en In-Place Holds. (Deze cmdlets worden gezamenlijk geïdentificeerd als *-MailboxSearch-cmdlets.) Dit omvat de volgende cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Postvak zoeken instellen](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- De [cmdlet Zoekpostvak](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.
- De volgende bewerkingen in de Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Geavanceerde eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tijdlijn voor de uittreding:**
- **1 juli 2020** U kunt geen nieuwe zoekopdrachten meer maken, maar u kunt bestaande zoekopdrachten op eigen risico uitvoeren, bewerken en verwijderen. Microsoft Support biedt geen ondersteuning meer In-Place eDiscovery-& in het EAC.
    
- **1 oktober 2020** In-Place eDiscovery & Holds-functionaliteit in de EAC wordt in de modus Alleen-lezen geplaatst, zodat u alleen bestaande zoekopdrachten en inhoudsfuncties kunt verwijderen.

**Zie voor meer informatie:**

 - [Oudere eDiscovery-zoekopdrachten migreren naar het Microsoft 365-compliancecentrum](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Buitengebruikstelling van verouderde eDiscovery-hulpprogramma's](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Veelgestelde vragen over In-Place eDiscovery en In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



