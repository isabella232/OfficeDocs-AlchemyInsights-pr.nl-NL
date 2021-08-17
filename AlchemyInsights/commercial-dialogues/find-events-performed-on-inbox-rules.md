---
title: Gebeurtenissen zoeken die zijn uitgevoerd met regels voor Postvak IN
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882630"
---
# <a name="find-events-performed-on-inbox-rules"></a>Gebeurtenissen zoeken die zijn uitgevoerd met regels voor Postvak IN

Wanneer regels voor Postvak IN worden gemaakt, gewijzigd of verwijderd, worden de gebeurtenissen opgenomen in het auditlogboek. U kunt ze als volgende controleren:

1. Ga op een van de volgende acties te werk:
   - Ga in Microsoft 365-compliancecentrum naar <https://compliance.microsoft.com> Solutions  \> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://compliance.microsoft.com/auditlogsearch> u .
   - Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://security.microsoft.com/auditlogsearch> u .

    > [!NOTE]
    > Als u een melding ziet dat u auditing moet in- of uit- zetten, gaat u door en zet u deze nu in. Als deze functie niet is ingeschakeld, kunnen zoekresultaten geen gegevens uit eerdere datums halen.

2. Configureer **op het** tabblad Zoeken van de pagina **Controle** de volgende instellingen:
   - **Datum en tijdbereik:** Selecteer het datum-/tijdbereik in de vakken **Begin** **en** Einde.
   - **Activiteiten:** Selecteer **Regel Nieuw Postvak INRule Maken van postvak IN van Outlook Web App**

3. Wanneer u klaar bent, klikt u op **Zoeken**. De activiteiten worden weergegeven op de nieuwe **pagina Controle** zoeken.

4. Selecteer een activiteit in de resultaten om de details flyout te openen. Onder de **sectie Parameters** ziet u de naam van de regel, de voorwaarden en de acties die de regel zal uitvoeren.

Zie Het auditlogboek doorzoeken om [veelvoorkomende ondersteuningsproblemen te onderzoeken](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)voor meer informatie.
