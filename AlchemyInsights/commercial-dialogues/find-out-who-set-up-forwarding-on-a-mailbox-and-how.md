---
title: Ontdek wie doorsturen in een postvak heeft ingesteld en hoe
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988174"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ontdek wie doorsturen in een postvak heeft ingesteld en hoe

Als extern doorsturen is ingesteld op een postvak, wordt de activiteit gecontroleerd als onderdeel van de Set-Mailbox cmdlet. U vindt als volgende de activiteit in het auditlogboek:

1. Ga naar het [Office 365 Beveiligings- & compliancecentrum.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecteer **Zoeken in** >  **auditlogboek zoeken**.
    > [!NOTE]
    > Als u een melding ziet dat u auditing moet in- of uit- zetten, gaat u door en zet u deze nu in. Als deze functie niet is ingeschakeld, kunnen zoekresultaten geen gegevens uit eerdere datums halen.
1. Zorg ervoor dat **het veld** Activiteiten is ingesteld op Resultaten voor alle **activiteiten (de** standaardinstelling). Geef het datumbereik op. U hoeft geen gebruikersnaam op te geven.
1. Selecteer **Zoeken**. De activiteiten worden weergegeven onder **Resultaten**.
1. Selecteer **Filterresultaten** en voer vervolgens **Postvak instellen** in het veld **Activiteitsfilter** in. Hiermee worden alle activiteiten **voor Postvak instellen** als retourneert.
1. Als u de details wilt bekijken, selecteert u een activiteit en selecteert u **vervolgens Meer informatie.** Onder **Parameters** ziet u het doorsturende e-mailadres dat is ingesteld in het postvak. De **UserID** vertegenwoordigt de gebruiker die extern doorsturen in het postvak heeft ingesteld.
Zie Het auditlogboek van het Office 365 zoeken om veelvoorkomende scenario's op te lossen voor meer [informatie.](https://go.microsoft.com/fwlink/?linkid=2103944)