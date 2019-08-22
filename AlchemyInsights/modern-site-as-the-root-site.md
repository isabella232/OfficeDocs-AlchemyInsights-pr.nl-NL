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
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543848"
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
