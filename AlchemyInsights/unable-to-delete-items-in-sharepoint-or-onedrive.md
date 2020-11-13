---
title: Kan geen items verwijderen in SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019578"
---
# <a name="unable-to-delete-items"></a>Items kunnen niet worden verwijderd

- Het bewaarbeleid kan dit veroorzaken, u dient de juiste bewaring uit te schakelen of te uitsluiten die dit probleem veroorzaakt. Nadat het bewaarbeleid of de bewaring is verwijderd, duurt het maximaal 24 uur voordat de wijziging is doorgevoerd. Zorg ervoor dat er geen [bewaarbeleid](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) is ingesteld voor het item.

- De site heeft mogelijk een beperkte opslagruimte, Verhoog de [Sitequota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) en verwijder het item.

- Zorg ervoor dat het item niet is [uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) door een andere gebruiker.

- Ten slotte kunnen beheerders gebruikmaken van [SharePoint-patronen en-procedures](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) met een bibliotheek met PowerShell-opdrachten waarmee u complexe beheeracties kunt uitvoeren, zoals het verwijderen van stubborn-items.
- [PNP-bestand verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-map verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-lijst item verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lijst verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-veld (kolom) verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)