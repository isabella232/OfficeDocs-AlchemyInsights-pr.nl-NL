---
title: Uw klassieke hoofdsite ruilen met een moderne site
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741539"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Uw klassieke hoofdsite ruilen met een moderne site

Als uw omgeving vóór april 2019 is ingesteld, u uw hoofdsite wijzigen in een moderne site met Microsoft PowerShell:

- Als u een andere site hebt die u als hoofdsite wilt gebruiken, u [de hoofdsite erdoor vervangen (ruilen).](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Gebruik [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site te ruilen met een andere site terwijl u de oorspronkelijke site archiveert. Beschikbaar voor zowel teamsite (niet verbonden met een groep) als voor communicatiesite. 

- Er worden binnenkort extra mogelijkheden geïntroduceerd waarmee u de inhoud op de site blijven gebruiken, maar de bestaande site converteren naar een communicatiesite. 
>[!Important]
>Deze mogelijkheden zullen geleidelijk worden uitgerold. Blijf het Berichtencentrum controleren op updates. 

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen met het verwisselen van sites

- De doelsite kan een fout 'niet gevonden' (HTTP 404) voor een korte periode retourneren.
- Inhoud moet opnieuw worden gecrawld om de zoekindex bij te werken. Er is geen handmatige stap vereist - dit wordt automatisch gedaan.
- Alles wat afhankelijk is van 'statische' koppelingen (zoals Bestandssynchronisatie en OneNote-bestanden) moet handmatig worden gecorrigeerd.
- Als de bronsite een nieuwssite van de organisatie was, werkt u de URL bij.Ontvang een lijst met alle nieuwssites van de organisatie.
- Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld.
