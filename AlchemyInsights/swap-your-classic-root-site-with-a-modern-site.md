---
title: Uw klassieke hoofdsite verwisselen met een moderne site
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316135"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Uw klassieke hoofdsite verwisselen met een moderne site

Als uw omgeving vóór april 2019 is ingesteld, kunt u de hoofdsite wijzigen in een moderne site met Microsoft PowerShell:

- Als u een andere site hebt die u als hoofdsite wilt gebruiken, kunt u de hoofdsite vervangen [(vervangen).](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Gebruik [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site te verwisselen met een andere site tijdens het archiveren van de oorspronkelijke site. Beschikbaar voor zowel teamsite (niet verbonden met een groep) als Communicatiesite. 

- Er worden binnenkort extra mogelijkheden geïntroduceerd waarmee u de inhoud op de site kunt blijven gebruiken, maar de bestaande site kunt converteren naar een communicatiesite. 

**Belangrijk:** deze mogelijkheden worden geleidelijk uitgerold. Blijf het Berichtencentrum controleren op updates. 

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen met het wisselen van sites

- De doelsite kan een fout 'niet gevonden' (HTTP 404) voor een korte periode retourneren.
- Inhoud moet worden gereraweerd om de zoekindex bij te werken. Er is geen handmatige stap vereist: dit wordt automatisch uitgevoerd.
- Alles wat afhankelijk is van 'statische' koppelingen (zoals Bestandssynchronisatie en OneNote bestanden) moet handmatig worden gecorrigeerd.
- Als de bronsite een nieuwssite van de organisatie was, moet u de URL bijwerken. Een lijst met alle nieuwssites van de organisatie krijgen.
- Project Serversites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld.
