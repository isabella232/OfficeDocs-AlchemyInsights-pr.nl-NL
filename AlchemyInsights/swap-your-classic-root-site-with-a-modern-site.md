---
title: Ruil je klassieke root site met een moderne site
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749255"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Ruil je klassieke root site met een moderne site

Als uw omgeving is ingesteld vóór 2019 april, u uw hoofdsite wijzigen naar een moderne site met behulp van Microsoft PowerShell:

- Als u een andere site die u wilt gebruiken als uw hoofdsite hebt, u vervangen [(wisselen) de hoofdsite](https://docs.microsoft.com/sharepoint/modern-root-site) met deze. 
    - Gebruik [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site met een andere site te wisselen tijdens het archiveren van de oorspronkelijke site. Beschikbaar voor beide team sites (niet verbonden met een groep) en een communicatiesite. 

- Er zullen binnenkort extra mogelijkheden worden geïntroduceerd waarmee u de inhoud op de site blijven gebruiken, maar de bestaande site naar een communicatiesite moet converteren. 
>[!Important]
>Deze mogelijkheden zullen geleidelijk worden uitgerold. Ga door met het controleren van het Office 365-berichtencentrum voor updates. 

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen met het uitwisselen van sites

- De doelsite kan een fout ' niet gevonden ' (HTTP 404) retourneren voor een korte periode.
- De inhoud moet opnieuw worden verkend om de zoekindex bij te werken. Er is geen handmatige stap vereist-dit wordt automatisch gedaan.
- Alles wat afhankelijk is van ' statische ' koppelingen (zoals bestandssynchronisatie en OneNote-bestanden) moet handmatig worden gecorrigeerd.
- Als de bronsite een nieuwssite voor de organisatie was, werkt u de URL bij.Krijg een lijst van alle organisatorische nieuwssites.
- Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld.





