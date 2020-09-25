---
title: hulpprogramma voor het exporteren van eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277931"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kunt u het hulpprogramma voor het maken van eDiscovery-export niet installeren of uitvoeren?

Controleer het volgende als u het hulpprogramma voor het maken van zoekresultaten niet kunt installeren of uitvoeren voor het gebruik van het hulpprogramma eDiscovery-export.
  
- De computer die u gebruikt voldoet aan de volgende vereisten:

  - 32-of 64-bits versies van Windows 7 en nieuwere versies

  - Microsoft .NET Framework 4.7

  - Een ondersteunde browser:

  - Microsoft Edge

    Of

  - Internet Explorer 10 en nieuwere versies

    Andere browsers zoals Google Chrome en Mozilla Firefox worden niet ondersteund.

- Uw organisatie kan verbinding maken met het eindpunt in azure, dat wil zeggen ** \* . blob.core.Windows.net** (het jokerteken vertegenwoordigt een unieke id voor de exporttaak).

- U bent in het Microsoft 365 beveiligings compliance van de export functie toegewezen &amp; . Standaard is deze rol alleen toegewezen aan de rollen groep van eDiscovery-beheerders. Zie [eDiscovery-machtigingen toewijzen](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Zie [inhoud van zoekresultaten exporteren](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)voor meer informatie.

Als u meer dan een afgesloten 100k postvakken exporteert, moet u de volgende PowerShell gebruiken om de export resultaten te downloaden:  [resultaten uit meer dan afgesloten 100k postvakken exporteren](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).