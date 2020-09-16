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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionering van oudere eDiscovery-Hulpprogramma's

Als gevolg van de nieuwe en verbeterde eDiscovery-functionaliteit in Microsoft 365 compliance, worden de volgende oudere eDiscovery-hulpprogramma's en Commandlets in de komende maanden buiten gebruik gesteld:

- [In-place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) en [in-place bewarings ruimte](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in het Exchange-Beheercentrum.

- De Exchange Online PowerShell-cmdlets die in-place eDiscovery en in-place bewaring ondersteunen. (Deze cmdlets worden gezamenlijk aangeduid als MailboxSearch-cmdlets.) Dit omvat de volgende cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- De cmdlet [Search-mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.
- De volgende bewerkingen in de Exchange Web Services-API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Geavanceerd eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tijdlijn voor pensionering**:
- Woensdag **1 juli 2020** U kunt niet langer nieuwe zoekopdrachten en wachtruimten maken, maar u kunt op uw eigen risico bestaande zoekopdrachten uitvoeren, bewerken en verwijderen. Microsoft ondersteuning biedt niet langer ondersteuning voor in-place eDiscovery-& bewaard in het Exchange-Beheercentrum.
    
- Maandag **1 oktober 2020** In-place eDiscovery-& Bewaar functies in het Exchange-Beheercentrum worden in de modus alleen-lezen gezet, zodat u alleen bestaande zoekopdrachten en wachtstand kunt verwijderen.

**Zie voor meer informatie**:

 - [Verouderde eDiscovery-zoekopdrachten en wachtruimten naar het nalevings centrum voor Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Buitengebruikstelling van verouderde eDiscovery-hulpprogramma's](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Veelgestelde vragen over in-place eDiscovery en wachtstand](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



