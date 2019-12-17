---
title: Zoeken in SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044038"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Inhoud crawlen en indexeren in SharePoint Online

Inhoud moet worden verkend en toegevoegd aan de zoekindex voor gebruikers om te vinden waarnaar ze zoeken in SharePoint Online. De inhoud wordt automatisch gecrawld op basis van een vooraf gedefinieerd verkennings schema (het verkennings schema kan niet worden gewijzigd). De crawler haalt inhoud op die sinds de laatste verkenning is gewijzigd en werkt de index bij. Let op het volgende om ervoor te zorgen dat de inhoud wordt verkend en de index wordt bijgewerkt:

- Zorg ervoor dat inhoud kan worden gevonden door [site-inhoud doorzoekbaar te maken](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Wanneer u een beheerde eigenschap hebt gewijzigd of als u de toewijzing van verkende en beheerde eigenschappen hebt gewijzigd, moet de site opnieuw worden verkend voordat de wijzigingen worden doorgevoerd in de zoekindex. 

    Omdat uw wijzigingen worden aangebracht in het zoekschema en niet op de werkelijke site, wordt de site niet automatisch opnieuw geïndexeerd door de crawler. 

    Zie voor meer informatie [handmatig crawlen en opnieuw indexeren van een site, een bibliotheek of een lijst aanvragen](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Wacht ten minste 24 uur na het handmatig aanvragen van een crawl en volledige re-index om te zien of u nog steeds een probleem ondervindt. 

    Als er meer dan 24 uur zijn verstreken sinds u de verkenning en volledige re-index hebt gestart, meldt u een ondersteuningsaanvraag. In veel gevallen werken we nu al aan een oplossing. Gelieve ons ten minste 24 uur te geven om een oplossing te voltooien.

> [!IMPORTANT]
> Als een site, document (bibliotheek) of een lijst is verwijderd en nog steeds wordt weergegeven in de zoekresultaten, moeten gebruikers een **fout 404-bestand** ontvangen dat niet is gevonden wanneer u toegang probeert te krijgen. Dit probleem moet worden vastgelegd als een ondersteuningsaanvraag voor verder onderzoek. 



