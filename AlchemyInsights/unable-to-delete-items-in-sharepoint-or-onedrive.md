---
title: Items in SharePoint of OneDrive kan niet worden verwijderd
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571241"
---
# <a name="unable-to-delete-items"></a>Kan items niet verwijderen

Bewaarbeleid kan dit veroorzaken, u moet de respectievelijke blokkering uitschakelen of uitsluiten die dit probleem veroorzaakt. Nadat een bewaarbeleid of -blokkering is verwijderd, kan het tot 24 uur duren voordat de wijziging van kracht wordt. Zorg ervoor dat er geen [bewaarbeleid](https://docs.microsoft.com/office365/securitycompliance/retention-policies) is ingesteld op het item.

De site kan de opslaglimiet hebben overschreden, het [sitequotum](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) hebben verhoogd en het item verwijderen.

Zorg ervoor dat het item niet is [uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) naar een andere gebruiker.

Ten slotte kunnen beheerders [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) gebruiken die een bibliotheek met PowerShell-opdrachten bevat waarmee u complexe beheeracties uitvoeren, zoals het verwijderen van hardnekkige items afdwingen.
- [PNP-bestand verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-map verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-lijstitem verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lijst verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-veld verwijderen (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)