---
title: De hoofdsite is klassiek met een moderne site wisselen
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
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270739"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>De hoofdsite is klassiek met een moderne site wisselen

Als uw omgeving vóór April 2019 is ingesteld, kunt u uw hoofdsite met een moderne site met Microsoft PowerShell:

- Als u een andere site die u wilt gebruiken als uw hoofdsite hebt, kunt u (swap) de hoofdmap van de site kunt vervangen door deze. 
    - Gebruik [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) te verwisselen van de locatie van een site met een andere site bij het archiveren van de oorspronkelijke site. Beschikbaar voor zowel Team Site (niet verbonden aan een groep) en communicatie-Site. 

- Extra functies geïntroduceerd spoedig waarmee u te houden met de inhoud op de site, maar de bestaande site converteren naar een communicatiesite. 
>[!Important]
>Deze mogelijkheden zullen geleidelijk worden uitgerold. Houd het berichtencentrum van Office 365 voor updates. 

## <a name="known-issues-with-swapping-sites"></a>Bekende problemen bij het wisselen van sites

- De doelsite retourneert gedurende korte tijd een "niet gevonden" (HTTP 404)-fout.
- Inhoud moet opnieuw worden verkend om het bijwerken van de zoekindex. Er is geen handmatige stap vereist - dit wordt automatisch gedaan.
- Alles wat afhankelijk is van een 'static' koppelingen (zoals bestand synchroniseren als OneNote-bestanden) moeten handmatig worden gecorrigeerd.
- Als de bronsite een organisatie-nieuwssite is, werken de URL.Een lijst van alle organisatie-nieuwssites opvragen.
- Project Server-sites mogelijk moet worden gevalideerd om ervoor te zorgen dat ze nog steeds gekoppeld correct worden.





