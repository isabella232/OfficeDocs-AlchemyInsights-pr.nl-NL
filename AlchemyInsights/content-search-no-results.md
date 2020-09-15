---
title: Inhoud zoeken geen resultaten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680642"
---
# <a name="no-results-from-content-searchexports"></a>Geen resultaten van inhouds zoekactie/-uitvoer

Problemen bij het zoeken naar inhoud en exporteren van inhoud kan worden veroorzaakt door een bepaald nalevings beveiligings filter dat door een specifieke beheerder is ingesteld en de communicatie met de beheerder niet naar alle beheerders hoeft te communiceren.

U kunt dit oplossen door te controleren of er beveiligings filters voor compliance zijn die dit mogelijk veroorzaken:
1. Verbinding maken met PowerShell van Beveiligingscentrum en compliance
2. Voer de volgende Commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organisatie $org