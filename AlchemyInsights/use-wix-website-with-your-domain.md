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
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825942"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Wix-website gebruiken met door Office 365 aangeschafte of beheerde domeinen

- [DNS-records bijwerken als u uw website bij uw huidige hostingprovider wilt houden](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- In het Wix-artikel 'Connecting a Domain to Wix Using the Pointing Method' (Een domein verbinden met Wix met behulp van de aanwijsmethode) wordt het gebruik van aanwijzen aanbevolen (DNS-records toevoegen via de bovenstaande koppeling) in plaats van naamservers te wijzigen bij het gebruik van Office 365
- Als u er toch voor kiest om naamservers te wijzigen naar Wix, moet u [DNS-records maken bij Wix voor Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Als uw domein is aangeschaft bij Microsoft, kunnen de naamservers niet worden gewijzigd. Als u naamservers moet wijzigen, moet het door Microsoft gekochte domein [na zestig dagen worden overgedragen naar een andere hostingprovider](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)