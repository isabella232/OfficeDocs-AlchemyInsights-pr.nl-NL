---
title: Kan geen items verwijderen in SharePoint of OneDrive
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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049512"
---
# <a name="unable-to-delete-items"></a>Kan items niet verwijderen

Hebt u problemen met het verwijderen van SharePoint-items?

- Zorg er altijd voor dat u over de [juiste machtigingen](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) beschikt om het item te verwijderen of dat de beheerder van een [siteverzameling](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) het item probeert te verwijderen.

- Zorg ervoor dat er geen [bewaarbeleid](https://docs.microsoft.com/office365/securitycompliance/retention-policies) is ingesteld voor het item.

- Controleer of het item niet is [uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) naar een andere gebruiker.

- Ten slotte kunnen beheerders [SharePoint-patronen en-procedures](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) gebruiken die een bibliotheek met PowerShell-opdrachten bevatten waarmee u complexe beheeracties uitvoeren, zoals geforceerd verwijderen van hardnekkige items.
- [PNP-bestand verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-map verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-lijst item verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lijst verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-veld verwijderen (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)