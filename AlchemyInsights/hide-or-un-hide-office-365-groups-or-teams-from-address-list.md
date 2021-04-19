---
title: Office 365-groepen of teams verbergen of de adressenlijst in- of uit-
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811451"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365-groepen of teams verbergen of de adressenlijst in- of uit-

Gebruik de volgende OPDRACHT EXO PowerShell om Office 365-groep/teams te verbergen of te verbergen voor adreslijsten (GAL) van Exchange-clients (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Gebruik de volgende OPDRACHT EXO PowerShell om de Office365-groep/teams te verbergen voor Exchange-clients (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Zie Office 365 Groepen verbergen voor de [GAL- en Exchange-clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)voor gedetailleerde instructies.
