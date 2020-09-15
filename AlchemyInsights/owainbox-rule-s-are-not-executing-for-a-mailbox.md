---
title: 1332 OWA-regels voor Postvak in worden niet uitgevoerd voor een postvak
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721586"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Een regel voor Postvak in werkt niet zoals verwacht

Controleer de volgende instellingen in de webversie van Outlook:

- U kunt automatisch een bericht omleiden, doorschakelen of antwoorden op basis van slechts één keer in regels voor Postvak in. Een omleidings regel (een regel voor het postvak in of de e-mail stroom regel, ook wel wel een transportregel genoemd), kan maximaal tien doorstuur geadresseerden toevoegen aan een bericht. Zie voor meer informatie [regel beperkingen voor logboeken, transport en Postvak in](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Regels voor Postvak in werken niet op het alternatief postvak voor Logboeken. Zie voor meer informatie over het alternatief postvak voor Logboeken het [alternatief postvak voor logboeken](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Zie [KB 2829319](https://support.microsoft.com/kb/2829319)om deze problemen op te lossen.

Als de vorige problemen niet van toepassing zijn, voert u het rapport regels voor Postvak in in voordat u het probleem naar Microsoft ondersteunt:

1. Open het postvak in de webversie van Outlook en klik op <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Instellingen**  >  voor **Alle Outlook-instellingen**  >  weergeven **E-mail**  >  **Regels**.

2. Klik onder aan de pagina op **als uw regels niet werken, klik hier om een diagnostisch rapport te genereren**.
