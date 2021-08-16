---
title: Moderne site als hoofdsite
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000381"
---
# <a name="modern-site-as-root-site"></a>Moderne site als hoofdsite

We zijn begonnen met het uitrollen van een nieuwe functie waarmee u uw klassieke [site-hoofdsite](https://docs.microsoft.com/sharepoint/modern-root-site)kunt wisselen met een moderne site. Gebruik [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site te verwisselen met een andere site tijdens het archiveren van de oorspronkelijke site. Beschikbaar voor zowel teamsite (niet verbonden met een groep) als Communicatiesite.

>[!Important]
> Verwijder de klassieke hoofdsite niet om een moderne communicatiesite te maken. Dit wordt niet ondersteund door Microsoft. Als u de hoofdsite verwijderd, zijn alle SharePoint in uw organisatie ontoegankelijk voor alle gebruikers, totdat u de site herstelt of een nieuwe site maakt op dezelfde URL. We communiceren deze functie via het berichtencentrum. U kunt verwachten dat de functie binnenkort wordt ingeschakeld in uw tenant.

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen met het wisselen van sites
- De doelsite kan een fout 'niet gevonden' (HTTP 404) voor een korte periode retourneren.
- Inhoud moet worden gereraweerd om de zoekindex bij te werken. Er is hier geen handmatige stap vereist, dit wordt automatisch uitgevoerd.
- Alles wat afhankelijk is van 'statische' koppelingen (zoals Bestandssynchronisatie en OneNote bestanden) moet handmatig worden gecorrigeerd.
- Project Serversites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld. 
