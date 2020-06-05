---
title: 1332 OWA - Inboxregel(s) worden niet uitgevoerd voor een postvak
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576555"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Een regel Postvak IN werkt niet zoals verwacht

Controleer de volgende instellingen in de webversie van Outlook:

- Een bericht kan automatisch worden doorgestuurd, doorgestuurd of beantwoord op basis van regels voor Postvak IN slechts één keer. Een omleidingsregel (een regel voor postvak IN of e-mailstroomregel, ook wel een transportregel genoemd) kan maximaal tien ontvangers van doorsturen aan een bericht toevoegen. Zie [Regels voor journal, Transport en Postvak IN voor](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)meer informatie.

- Regels voor postvak IN werken niet in het postvak voor logboeken. Zie [Postvak Wisseltijdschriften](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)voor meer informatie over het alternatieve postvak voor dagboeken .

Zie [KB 2829319](https://support.microsoft.com/kb/2829319)om deze problemen op te lossen.

Als de vorige problemen niet van toepassing zijn, voert u het diagnoserapport van de regel inposten uit voordat u het probleem escaleert naar Microsoft Support:

1. Het postvak openen in de webversie van Outlook en klik op <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Instellingen**  >  **Alle Outlook-instellingen weergeven**  >  **E-mail**  >  **Regels**.

2. Klik onder aan de pagina op **Als uw regels niet werken, klik hier om een diagnostisch rapport te genereren.**
