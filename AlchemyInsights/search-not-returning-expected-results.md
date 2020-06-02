---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510567"
---
# <a name="content-search-not-returning-expected-results"></a>Content Search retourneren geen verwachte resultaten

Wanneer u inhoudszoekopdrachten uitvoert vanuit het Microsoft 365-beveiligingscentrum & Compliance Center, ontvangt u mogelijk onverwachte zoekresultaten. Houd rekening met de volgende zaken die van invloed kunnen zijn op uw zoekresultaten:

- **Inhoudslocaties en zoekomstandigheden**: zorg ervoor dat u de juiste inhoudslocaties en zoekomstandigheden hebt geselecteerd. Als u een grote zoekopdracht hebt uitgevoerd (met veel locaties), u overwegen deze op te splitsen in meerdere zoekopdrachten.

- **Gedeeltelijk geïndexeerde items**: [Gedeeltelijk geïndexeerde items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) uit postvakken worden opgenomen in de geschatte zoekresultaten. Gedeeltelijk geïndexeerde items van sites in SharePoint en OneDrive worden echter niet opgenomen in de zoekschatting.

- **Zoekfouten**: Bij het doorzoeken van een groot aantal postvakken (meer dan 100.000 postvakken) u zoekfouten krijgen, met foutcodes zoals CS008-009 en CS012-002). Probeer in dit geval alleen opnieuw zoeken naar de mislukte inhoudslocaties. Zie [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) voor meer informatie.
