---
title: Het IP-adres zoeken in het auditlogboek
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902255"
---
# <a name="find-the-ip-address-in-audit-log"></a>Het IP-adres zoeken in het auditlogboek

Het IP-adres dat overeenkomt met een activiteit die door een gebruiker of beheerder wordt uitgevoerd, wordt weergegeven in de auditlogboeken. De clientgegevens worden ook vastgelegd. U kunt als volgende het IP-adres identificeren:

1. Een van de volgende acties uitvoeren:
   - Ga in Microsoft 365-compliancecentrum naar <https://compliance.microsoft.com> Solutions  \> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://compliance.microsoft.com/auditlogsearch> u .
   - Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://security.microsoft.com/auditlogsearch> u .

    > [!NOTE]
    > Als u een melding ziet dat u auditing moet in- of uit- zetten, gaat u door en zet u deze nu in. Als deze functie niet is ingeschakeld, kunnen zoekresultaten geen gegevens uit eerdere datums halen.

2. Controleer op **de** pagina Controle of **het** tabblad Zoeken is geselecteerd en configureer de volgende instellingen:
   - **Datum en tijdbereik:** Selecteer het datum-/tijdbereik in de vakken **Begin** **en** Einde.
   - **Activiteiten:** Als u geïnteresseerd bent in een bepaalde activiteit, selecteert u deze in de lijst; anders worden alle activiteiten geretourneerd **met de** standaardwaarde Resultaten voor alle activiteiten tonen.. Houd er rekening mee dat bepaalde activiteiten mogelijk niet beschikbaar zijn voor selectie. Deze audititems worden echter geretourneerd als **Resultaten voor alle activiteiten** tonen is geselecteerd.
   - **Gebruikers:** Accepteer de lege standaardwaarde om resultaten voor alle gebruikers te retourneren of voer een of meer gebruikers in.

3. Wanneer u klaar bent, klikt u op **Zoeken**. De activiteiten worden weergegeven op de nieuwe **pagina Controle zoeken.**

4. Klik in de resultaten op **Resultaten filteren** en typ **Postvak** instellen in het vak activiteitsfilter.

5. Selecteer een auditrecord in de resultaten om het fly-out **Details** te openen.

Zie Het auditlogboek doorzoeken om [veelvoorkomende ondersteuningsproblemen te onderzoeken](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)voor meer informatie.
