---
title: eDiscovery export tool
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 7e2964ef0a44ddf421e4aae007acbdbda196e20f
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769298"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan het eDiscovery-export programma niet installeren of uitvoeren?

Als u de Office 365 eDiscovery-export tool niet installeren of uitvoeren om zoekresultaten te downloaden, controleert u de volgende dingen:
  
- De computer die u gebruikt, voldoet aan deze vereisten:

  - 32-of 64-bits versies van Windows 7 en latere versies

  - Microsoft .NET Framework 4,7

  - Een ondersteunde browser:

  - Microsoft Edge

    Of

  - Internet Explorer 10 en latere versies

    Andere browsers, zoals Google Chrome en Mozilla Firefox worden niet ondersteund.

- Uw organisatie kan verbinding maken met het eindpunt in azure, dit is ** \*. blob.core.Windows.net** (het jokerteken vertegenwoordigt een unieke id voor uw exporttaak).

- U hebt de rol exporteren in het Office 365 Security &amp; compliance Center toegewezen. Deze rol is standaard alleen toegewezen aan de rol groep eDiscovery Manager. Zie [eDiscovery-machtigingen toewijzen](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Zie [Zoekresultaten voor inhoud exporteren](https://docs.microsoft.com/office365/securitycompliance/export-search-results)voor meer informatie.
  