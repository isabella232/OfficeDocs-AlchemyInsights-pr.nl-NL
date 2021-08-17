---
title: De auditlogboeken voor verwijderde gebeurtenissen lezen
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896010"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>De auditlogboeken voor verwijderde gebeurtenissen lezen

U doet dit als volgende:

1. Een van de volgende acties uitvoeren:
   - Ga in Microsoft 365-compliancecentrum naar <https://compliance.microsoft.com> Solutions  \> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://compliance.microsoft.com/auditlogsearch> u .
   - Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://security.microsoft.com/auditlogsearch> u .

    > [!NOTE]
    > Als u een melding ziet dat u de functie moet in- of uit- zetten, gaat u door en zet u deze nu in. Als de functie niet is ingeschakeld, kunnen zoekresultaten geen gegevens uit eerdere datums halen.

2. Configureer **op het** tabblad Zoeken van de pagina **Controle** de volgende instellingen:
   - **Datum en tijdbereik:** Selecteer het datum-/tijdbereik in de vakken **Begin** **en** Einde.
   - **Activiteiten:** Voer Exchange **postvakactiviteiten in en** selecteer de volgende waarden:
     - **Berichten verwijderd uit de map Verwijderde items**
     - **Berichten verplaatst naar map Verwijderde Items**

       Wanneer u klaar bent, klikt u buiten het deelvenster om het deelvenster **Activiteiten te** minimaliseren.

   - **Gebruikers:** Accepteer de lege standaardwaarde om resultaten voor alle gebruikers te retourneren of voer een of meer gebruikers in.

3. Wanneer u klaar bent, klikt u op **Zoeken**. De activiteiten worden weergegeven op de nieuwe **pagina Controle** zoeken.

4. Selecteer een activiteit in de resultaten om de details flyout te openen. Aanvullende informatie over het verwijderde item, zoals de onderwerpregel en de locatie van het item toen het werd verwijderd, wordt weergegeven in het veld **AffectedItems.**

   > [!NOTE]
   > U kunt verwijderde items niet herstellen met de functie auditlogboek. Zie Verwijderde e-mailberichten herstellen [in](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)webversie van Outlook .

Zie Het auditlogboek doorzoeken om [veelvoorkomende ondersteuningsproblemen te onderzoeken](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)voor meer informatie.
