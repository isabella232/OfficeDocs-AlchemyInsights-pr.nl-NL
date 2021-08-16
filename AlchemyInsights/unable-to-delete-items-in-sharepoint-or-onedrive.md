---
title: Items in SharePoint of OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038512"
---
# <a name="unable-to-delete-items"></a>Items kunnen niet worden verwijderd

- Bewaarbeleid kan dit veroorzaken, u moet de respectievelijke bewaring uitschakelen of uitsluiten die dit probleem veroorzaakt. Nadat een bewaarbeleid of bewaring is verwijderd, kan het tot 24 uur duren voordat de wijziging van kracht wordt. Zorg ervoor dat er geen [bewaarbeleid](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) is ingesteld voor het item.

- De site heeft mogelijk de opslaglimiet overschreden, het [sitequotum vergroot](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) en het item verwijderd.

- Controleer of het item niet [is uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) bij een andere gebruiker.

- Ten slotte kunnen beheerders [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) gebruiken die een bibliotheek met PowerShell-opdrachten bevat waarmee u complexe beheeracties kunt uitvoeren, zoals het gedwongen verwijderen van hardnekkige items.
- [PNP-bestand verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Map PNP verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-lijstitem verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lijst verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-veld verwijderen (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)