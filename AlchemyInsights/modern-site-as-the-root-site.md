---
title: Moderne site als hoofdsite
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713786"
---
# <a name="modern-site-as-root-site"></a>Moderne site als hoofdsite

We zijn begonnen met de uitrol van een nieuwe functie waarmee u uw klassieke site root site te [ruilen met een moderne site.](https://docs.microsoft.com/sharepoint/modern-root-site) Gebruik [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site te ruilen met een andere site terwijl u de oorspronkelijke site archiveert. Beschikbaar voor zowel teamsite (niet verbonden met een groep) als voor communicatiesite.

>[!Important]
> Verwijder uw klassieke hoofdsite niet om een moderne communicatiesite te maken. Dit wordt niet ondersteund door Microsoft. Als u de hoofdsite verwijderde, worden alle SharePoint-sites in uw organisatie ontoegankelijk voor alle gebruikers, totdat u de site herstelt of een nieuwe site met dezelfde URL maakt. We communiceren deze functie via het berichtencentrum. U mag verwachten dat de functie binnenkort in uw tenant wordt ingeschakeld.

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen met het verwisselen van sites
- De doelsite kan een fout 'niet gevonden' (HTTP 404) voor een korte periode retourneren.
- Inhoud moet opnieuw worden gecrawld om de zoekindex bij te werken. Er is hier geen handmatige stap vereist, dit gebeurt automatisch.
- Alles wat afhankelijk is van 'statische' koppelingen (zoals Bestandssynchronisatie en OneNote-bestanden) moet handmatig worden gecorrigeerd.
- Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld. 
