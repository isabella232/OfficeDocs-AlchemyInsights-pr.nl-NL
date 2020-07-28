---
title: Grafiek toont verschillende aantal records in raster
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439002"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Grafiek toont verschillende aantal records in raster

**Symptoom**

Voor grafiek op dashboardpagina, wanneer u klikt op grafiek "..." en klik op 'Records weergeven', u navigeert naar de rasterpagina om alle records te bekijken. Soms verandert het aantal records.

**Oorzaak**

Dit is te wijten aan het verschil in weergaven tussen de grafiek op de oorspronkelijke dashboardpagina en de grafiek op de startpagina van het raster.  

**Oplossing**

1. Controleer de weergave vanaf de oorspronkelijke pagina en de weergave in het raster om te zien of ze anders zijn.
2. Wijzig de weergave in het raster om de weergave op de oorspronkelijke pagina aan te passen.
3. Als de juiste weergave niet kan worden gevonden, betekent dit meestal dat de weergave niet is ingeschakeld in app-ontwerper.
4. Ga naar app-ontwerper van de specifieke app, kies de entiteit en de weergave, controleer de weergave die u wilt in- of inschakelen, opslaan, publiceren en sluiten.
5. De pagina vernieuwen.