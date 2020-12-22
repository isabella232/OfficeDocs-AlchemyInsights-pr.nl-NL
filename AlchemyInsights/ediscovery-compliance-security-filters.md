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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727218"
---
# <a name="no-results-returned-during-content-searchexport"></a>Geen resultaten geretourneerd tijdens het zoeken naar inhoud en exporteren

Als u problemen ondervindt met de volgende eDiscovery-scenario's:

- Inhoud zoeken/exporteren geeft geen gegevens of onverwachte gegevens als resultaat
- eDiscovery-zoekopdrachten of exporteren mislukt

Dit kan te wijten zijn aan bepaalde compliance beveiligings filters die door een bepaalde beheerder zijn ingesteld en die niet aan alle beheerders zijn gecommuniceerd.

U kunt dit oplossen door te controleren of er beveiligings filters voor naleving zijn die deze problemen mogelijk veroorzaken:

1. Verbinding maken met PowerShell van Beveiligingscentrum en compliance
2. Voer de volgende Commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Zie voor meer informatie over beveiligings filters voor naleving de [machtigingen filters voor inhoud zoeken](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
