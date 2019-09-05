---
title: Moderne site als de hoofdsite
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753899"
---
# <a name="modern-site-as-root-site"></a>Moderne site als hoofdsite

We zijn begonnen met de uitrol van een nieuwe functie waarmee u [uw klassieke site hoofdsite met een moderne site verwisselen](https://docs.microsoft.com/sharepoint/modern-root-site). Gebruik [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site met een andere site te wisselen tijdens het archiveren van de oorspronkelijke site. Beschikbaar voor beide team sites (niet verbonden met een groep) en een communicatiesite.

>[!Important]
> Verwijder uw klassieke hoofdsite niet om een moderne communicatiesite te maken. Dit wordt niet ondersteund door Microsoft. Als u de hoofdsite verwijdert, worden alle SharePoint-sites in uw organisatie ontoegankelijk voor alle gebruikers, totdat u de site herstelt of een nieuwe site maakt op dezelfde URL. We communiceren deze functie via het berichtencentrum. U moet verwachten dat de functie moet worden ingeschakeld in uw Tenant binnenkort.

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen met het uitwisselen van sites
- De doelsite kan een fout ' niet gevonden ' (HTTP 404) retourneren voor een korte periode.
- De inhoud moet opnieuw worden verkend om de zoekindex bij te werken. Er is hier geen handmatige stap vereist, dit wordt automatisch gedaan.
- Alles wat afhankelijk is van ' statische ' koppelingen (zoals bestandssynchronisatie en OneNote-bestanden) moet handmatig worden gecorrigeerd.
- Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld. 
