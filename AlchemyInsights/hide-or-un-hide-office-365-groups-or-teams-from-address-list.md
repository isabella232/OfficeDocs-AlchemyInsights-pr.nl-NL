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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="11d8b-102">Office 365-groepen of -teams verbergen of ontverbergen uit adreslijst</span><span class="sxs-lookup"><span data-stu-id="11d8b-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="11d8b-103">Gebruik de volgende OPDRACHT EXO PowerShell om Office 365-groep/teams te verbergen of te verwijderen uit adreslijsten (GAL) van Exchange-clients (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="11d8b-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="11d8b-104">Gebruik de volgende OPDRACHT EXO PowerShell om de Office365-groep/teams te verbergen voor Exchange-clients (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="11d8b-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="11d8b-105">Zie [Office 365-groepen verbergen van de GAL- en Exchange-clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)voor gedetailleerde instructies.</span><span class="sxs-lookup"><span data-stu-id="11d8b-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
