---
title: Geen resultaten geretourneerd tijdens het zoeken naar inhoud en exporteren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677682"
---
# <a name="no-results-returned-during-content-searchexport"></a>Geen resultaten geretourneerd tijdens het zoeken naar inhoud en exporteren

Als u problemen ondervindt met de volgende eDiscovery-scenario's:

- Inhoud zoeken/exporteren geeft geen gegevens of onverwachte gegevens als resultaat
- eDiscovery-zoekopdrachten of exporteren mislukt

Dit kan gebeuren vanwege beveiligings filters voor naleving die door een bepaalde beheerder zijn ingesteld en die niet zijn gecommuniceerd aan alle beheerders.

U kunt dit oplossen door te controleren of er beveiligings filters voor naleving zijn die deze problemen mogelijk veroorzaken:

1. Verbinding maken met PowerShell van Beveiligingscentrum en compliance
2. Voer de volgende Commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Zie voor meer informatie over beveiligings filters voor naleving de [machtigingen filters voor inhoud zoeken](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
