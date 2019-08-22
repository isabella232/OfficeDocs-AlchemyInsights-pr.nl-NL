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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516774"
---
# <a name="no-results-from-content-searchexports"></a>Er zijn geen resultaten uit inhoud zoeken-uitvoer

Problemen met inhoud zoeken-uitvoer retourneren van gegevens niet kunnen worden veroorzaakt door bepaalde naleving beveiligingsfilter dat is ingesteld door een specifieke Admin en communiceert niet met alle beheerders.

U kunt dit oplossen door te controleren op conformiteit beveiligingsfilters die wordt veroorzaakt door dit te controleren:
1. Verbinding maken met de veiligheid en conformiteit Powershell
2. Voer de volgende commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org-organisatie