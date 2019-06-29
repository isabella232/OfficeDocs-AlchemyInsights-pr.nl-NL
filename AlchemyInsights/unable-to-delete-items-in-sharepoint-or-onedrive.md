---
title: Kan niet verwijderen van items in SharePoint of OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366528"
---
# <a name="unable-to-delete-items"></a>Kan geen items verwijderen

Hebt u problemen items verwijderen?

- Controleer altijd of u beschikt over de [juiste machtigingen](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) te verwijderen van het item of een poging tot [beheerder van de siteverzameling](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) het item verwijderen.

- Zorg ervoor dat er niet een [bewaarbeleid](https://docs.microsoft.com/office365/securitycompliance/retention-policies) instellen op het item.

- Controleer dat het item niet is [uitgecheckt door](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) een andere gebruiker.

- Ten slotte kunnen beheerders gebruiken [SharePoint patronen en werkwijzen](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) met een bibliotheek met PowerShell-opdrachten waarmee u acties uit te voeren complexe management, zoals force stubborn items verwijderen.
- [PNP-bestand verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-map verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Met PNP-lijstitem verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Plug en Play lijst verwijderen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Verwijderen van PNP-veld (kolom)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)