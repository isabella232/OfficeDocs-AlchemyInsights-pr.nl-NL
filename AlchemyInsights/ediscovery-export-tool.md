---
title: eDiscovery-exporthulpmiddel
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814583"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kunt u het eDiscovery-exportprogramma niet installeren of uitvoeren?

Als u het eDiscovery-exportprogramma niet kunt installeren of uitvoeren om zoekresultaten te downloaden, controleert u de volgende dingen:
  
- De computer die u gebruikt, voldoet aan de volgende vereisten:

  - 32- of 64-bits versies van Windows 7 en nieuwere versies

  - Microsoft .NET Framework 4.7

  - Een ondersteunde browser:

  - Microsoft Edge

    Of

  - Internet Explorer 10 en nieuwere versies

    Andere browsers, zoals Google Chrome en Mozilla Firefox, worden niet ondersteund.

- Uw organisatie kan verbinding maken met het eindpunt in Azure, dat **\* .blob.core.windows.net** is (het jokerteken vertegenwoordigt een unieke id voor uw exportklus).

- U krijgt de rol Exporteren toegewezen in het Microsoft 365 Security &amp; Compliance Center. Deze rol wordt standaard alleen toegewezen aan de rollengroep eDiscovery Manager. Zie [EDiscovery-machtigingen toewijzen.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Zie Inhoudszoekresultaten [exporteren voor meer informatie.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Als u meer dan 100.000 postvakken exporteert, moet u de volgende Powershell gebruiken om de exportresultaten te downloaden: Resultaten exporteren uit meer dan [100.000 postvakken.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)