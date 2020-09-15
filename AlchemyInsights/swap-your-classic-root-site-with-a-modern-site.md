---
title: Uw klassieke basis site met een moderne site uitwisselen
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691174"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Uw klassieke basis site met een moderne site uitwisselen

Als uw omgeving vóór april 2019 is geconfigureerd, kunt u uw hoofdsite wijzigen in een moderne site met behulp van Microsoft PowerShell:

- Als u een andere site hebt die u wilt gebruiken als basis site, kunt u [de hoofdsite vervangen (verwisselen)](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Met [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kunt u de locatie van een site met een andere site wisselen tijdens het archiveren van de oorspronkelijke site. Beschikbaar voor beide team sites (niet verbonden met een groep) en communicatie site. 

- Er worden binnenkort extra functies geïntroduceerd waarmee u de inhoud op de site kunt blijven gebruiken, maar de bestaande site moet converteren naar een communicatiesite. 
>[!Important]
>Deze mogelijkheden worden geleidelijk uitgerold. Ga verder naar het berichtencentrum controleren op updates. 

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen met het verwisselen van sites

- De doelsite kan een "niet gevonden" (HTTP 404)-fout retourneren gedurende een korte periode.
- Inhoud moet worden verkend om de zoekindex bij te werken. U hoeft dit niet handmatig te doen, dit wordt automatisch uitgevoerd.
- Items die afhankelijk zijn van statische koppelingen (zoals bestandssynchronisatie en OneNote-bestanden), moeten handmatig worden gecorrigeerd.
- Als de bronsite een nieuwssite van een organisatie was, moet u de URL bijwerken.U ontvangt een lijst met alle nieuwssites van uw organisatie.
- Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat deze correct worden gekoppeld.
