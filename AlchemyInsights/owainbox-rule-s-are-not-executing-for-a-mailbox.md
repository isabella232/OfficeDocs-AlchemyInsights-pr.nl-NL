---
title: 1332 OWA - Regels voor Postvak IN worden niet uitgevoerd voor een postvak
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
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040897"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Een regel voor Postvak IN werkt niet zoals verwacht

Controleer de volgende instellingen in webversie van Outlook:

- Een bericht kan slechts één keer worden omgeleid, doorgestuurd of beantwoord op basis van regels voor Postvak IN. Met een omleidingsregel (een regel voor Postvak IN of een e-mailstroomregel, ook wel transportregel genoemd) kunnen maximaal tien geadresseerden aan een bericht worden doorgestuurd. Zie Regellimieten [voor logboeken, transport en Postvak IN](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)voor meer informatie.

- Regels voor Postvak IN werken niet in het postvak voor alternatieve logboeken. Zie Alternatief postvak voor logboeken voor meer informatie over het postvak voor alternatieve [logboeken.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Zie KB-2829319. [](https://support.microsoft.com/kb/2829319)

Als de vorige problemen niet van toepassing zijn, moet u het diagnostische rapport Postvak IN uitvoeren voordat u het probleem escaleert naar Microsoft-ondersteuning:

1. Open het postvak in webversie van Outlook en klik op <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Instellingen**  >  **Alle Outlook Instellingen**  >  **E-mail**  >  **Regels**.

2. Klik onder aan de pagina op Als uw regels niet werken, klik hier om **een diagnostisch rapport te genereren.**
