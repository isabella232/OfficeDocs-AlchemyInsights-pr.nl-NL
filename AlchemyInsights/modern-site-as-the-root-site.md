---
title: Moderne site als basis site
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666865"
---
# <a name="modern-site-as-root-site"></a>Moderne site als basis site

We zijn begonnen met het implementeren van een nieuwe functie waarmee u [uw klassieke site-site met een moderne site kunt uitwisselen](https://docs.microsoft.com/sharepoint/modern-root-site). Met [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kunt u de locatie van een site met een andere site wisselen tijdens het archiveren van de oorspronkelijke site. Beschikbaar voor beide team sites (niet verbonden met een groep) en communicatie site.

>[!Important]
> Verwijder uw klassieke basis site niet voor het maken van een moderne communicatiesite. Dit wordt niet ondersteund door Microsoft. Als u de hoofdsite verwijdert, worden alle SharePoint-sites in uw organisatie niet toegankelijk voor alle gebruikers totdat u de site terugzet of een nieuwe site maakt met dezelfde URL. We communiceren deze functie via het berichtencentrum. Normaalgesproken moet de functie in uw Tenant worden ingeschakeld.

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen met het verwisselen van sites
- De doelsite kan een "niet gevonden" (HTTP 404)-fout retourneren gedurende een korte periode.
- Inhoud moet worden verkend om de zoekindex bij te werken. U hoeft hier geen handmatige stap te vinden, dit is automatisch gebeurd.
- Items die afhankelijk zijn van statische koppelingen (zoals bestandssynchronisatie en OneNote-bestanden), moeten handmatig worden gecorrigeerd.
- Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat deze correct worden gekoppeld. 
