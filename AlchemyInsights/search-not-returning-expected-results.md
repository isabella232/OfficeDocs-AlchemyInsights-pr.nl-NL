---
title: 1491-search-not-return-expected-results
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
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709222"
---
# <a name="content-search-not-returning-expected-results"></a>Content Search levert geen verwachte resultaten op

Wanneer u inhoudszoekopdrachten uitvoert vanuit het Microsoft 365-beveiligingscentrum & Compliance Center, ontvangt u mogelijk onverwachte zoekresultaten. Houd rekening met de volgende dingen die van invloed kunnen zijn op uw zoekresultaten:

- **Inhoudslocaties en zoekomstandigheden:** zorg ervoor dat u de juiste inhoudslocaties en zoekomstandigheden hebt geselecteerd. Als u een grote zoekopdracht hebt uitgevoerd (met veel locaties), u overwegen deze op te splitsen in meerdere zoekopdrachten.

- **Gedeeltelijk geïndexeerde items**: [Gedeeltelijk geïndexeerde items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) uit postvakken worden opgenomen in de geschatte zoekresultaten. Gedeeltelijk geïndexeerde items van sites in SharePoint en OneDrive worden echter niet opgenomen in de zoekschatting.

- **Zoekfouten**: Bij het doorzoeken van een groot aantal postvakken (meer dan 100.000 postvakken) u zoekfouten krijgen, met foutcodes zoals CS008-009 en CS012-002). Probeer in dit geval de zoekopdracht alleen opnieuw naar de mislukte inhoudslocaties. Zie [dit artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) voor meer informatie.
