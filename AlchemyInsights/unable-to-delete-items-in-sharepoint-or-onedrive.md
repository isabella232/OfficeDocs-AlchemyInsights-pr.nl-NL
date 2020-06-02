---
title: Items in SharePoint of OneDrive niet kunnen verwijderen
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511971"
---
# <a name="unable-to-delete-items"></a>Items niet kunnen verwijderen

Bewaarbeleid kan dit veroorzaken, u moet de betreffende blokkering die dit probleem veroorzaakt uitschakelen of uitsluiten. Nadat een bewaarbeleid of blokkering is verwijderd, kan het tot 24 uur duren voordat de wijziging van kracht wordt. Zorg ervoor dat er geen instelling voor [bewaarbeleid](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) op het item staat.

De site heeft mogelijk de opslaglimiet overschreden, het [sitequotum](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) verhoogd en het item verwijderd.

Zorg ervoor dat het item niet is [uitgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) bij een andere gebruiker.

Ten slotte kunnen beheerders [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) gebruiken die een bibliotheek met PowerShell-opdrachten bevat waarmee u complexe beheeracties uitvoeren, zoals het forceren van hardnekkige items.
- [PNP-bestand verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-map verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-lijstitem verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lijst verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-veld verwijderen (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)