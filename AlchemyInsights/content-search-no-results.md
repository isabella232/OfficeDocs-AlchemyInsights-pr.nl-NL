---
title: Inhoud zoeken geen resultaten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800282"
---
# <a name="no-results-from-content-searchexports"></a>Er zijn geen resultaten uit inhoud zoeken-uitvoer

Problemen met inhoud zoeken-uitvoer retourneren van gegevens niet kunnen worden veroorzaakt door bepaalde naleving beveiligingsfilter dat is ingesteld door een specifieke Admin en communiceert niet met alle beheerders.

U kunt dit oplossen door te controleren op conformiteit beveiligingsfilters die wordt veroorzaakt door dit te controleren:
1. Verbinding maken met de veiligheid en conformiteit Powershell
2. Voer de volgende commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org-organisatie