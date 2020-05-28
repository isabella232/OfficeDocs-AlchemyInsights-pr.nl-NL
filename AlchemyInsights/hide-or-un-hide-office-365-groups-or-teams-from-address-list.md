---
title: Office 365-groepen of -teams verbergen of ontverbergen uit adreslijst
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225374"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365-groepen of -teams verbergen of ontverbergen uit adreslijst

Gebruik de volgende OPDRACHT EXO PowerShell om Office 365-groep/teams te verbergen of te verwijderen uit adreslijsten (GAL) van Exchange-clients (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Gebruik de volgende OPDRACHT EXO PowerShell om de Office365-groep/teams te verbergen voor Exchange-clients (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Zie [Office 365-groepen verbergen van de GAL- en Exchange-clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)voor gedetailleerde instructies.
