---
title: 1491-zoeken met niet-verwachte resultaten-resultaten
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740469"
---
# <a name="content-search-not-returning-expected-results"></a>Inhouds zoekactie levert geen verwachte resultaten op

Wanneer u inhouds zoekopdrachten uitvoert vanuit het compliance-beveiligings & van Microsoft 365, krijgt u mogelijk onverwachte zoekresultaten. Houd rekening met de volgende dingen die van invloed kunnen zijn op de zoekresultaten:

- **Inhoudslocaties en zoekvoorwaarden**: Zorg ervoor dat u de juiste inhoudslocaties en zoekvoorwaarden hebt geselecteerd. Als u een grote zoekopdracht met een groot aantal locaties hebt uitgevoerd, kunt u deze in meerdere zoekopdrachten verdelen.

- **Gedeeltelijk geïndexeerde items**:  [gedeeltelijk geïndexeerde items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) uit postvakken worden opgenomen in de geschatte zoekresultaten. Gedeeltelijk geïndexeerde items van sites in SharePoint en OneDrive worden echter niet opgenomen in de zoek raming.

- **Zoek fouten**: bij het zoeken in een groot aantal postvakken (meer dan 100.000 postvakken), worden mogelijk Zoek fouten weergegeven, met foutcodes zoals CS008-009 en CS012-002. In dit geval kunt u de zoekfunctie alleen opnieuw uitvoeren voor de mislukte inhoudslocaties. Zie  [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) voor meer informatie.
