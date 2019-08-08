---
title: Moderne site als de hoofdsite
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232710"
---
# <a name="modern-site-as-root-site"></a>Moderne site als hoofdsite

We begonnen te implementatie een nieuwe functie waarmee u uw hoofdsite klassieke site met een moderne site wisselen. Gebruik [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) te verwisselen van de locatie van een site met een andere site bij het archiveren van de oorspronkelijke site. Beschikbaar voor zowel Team Site (niet verbonden aan een groep) en communicatie-Site. 

>[!Important]
> Verwijder niet de klassieke hoofdsite om een moderne communicatie-Site te maken. Dit wordt niet ondersteund door Microsoft. Verwijderen van de hoofdsite brengt alle SharePoint-sites in uw organisatie niet toegankelijk voor alle gebruikers, totdat u de site terugzetten of maak een nieuwe site op dezelfde URL. We zullen deze functie via het berichtencentrum communiceren. U kunt de functie moet worden ingeschakeld in uw huurder binnenkort verwachten.

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen bij het wisselen van sites
- De doelsite retourneert gedurende korte tijd een "niet gevonden" (HTTP 404)-fout.
- Inhoud moet opnieuw worden verkend om het bijwerken van de zoekindex. Er is geen handmatige stap hier nodig is, wordt dit automatisch gedaan.
- Alles wat afhankelijk is van een 'static' koppelingen (zoals bestand synchroniseren als OneNote-bestanden) moeten handmatig worden gecorrigeerd.
- Project Server-sites mogelijk moet worden gevalideerd om ervoor te zorgen dat ze nog steeds gekoppeld correct worden. 
