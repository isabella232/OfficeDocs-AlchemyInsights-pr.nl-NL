---
title: Wix-website gebruiken met door Office 365 aangeschafte of beheerde domeinen
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
- "9001516"
- "3582"
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980172"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Wix-website gebruiken met door Office 365 aangeschafte of beheerde domeinen

- [DNS-records bijwerken als u uw website bij uw huidige hostingprovider wilt houden](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- In het Wix-artikel 'Connecting a Domain to Wix Using the Pointing Method' (Een domein verbinden met Wix met behulp van de aanwijsmethode) wordt het gebruik van aanwijzen aanbevolen (DNS-records toevoegen via de bovenstaande koppeling) in plaats van naamservers te wijzigen bij het gebruik van Office 365
- Als u er toch voor kiest om naamservers te wijzigen naar Wix, moet u [DNS-records maken bij Wix voor Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Als uw domein is aangeschaft bij Microsoft, kunnen de naamservers niet worden gewijzigd. Als u naamservers moet wijzigen, moet het door Microsoft gekochte domein [na zestig dagen worden overgedragen naar een andere hostingprovider](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)