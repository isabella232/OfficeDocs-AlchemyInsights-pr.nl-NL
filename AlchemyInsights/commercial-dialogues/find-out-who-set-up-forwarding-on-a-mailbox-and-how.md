---
title: Ontdek wie doorsturen heeft ingesteld voor een postvak en hoe
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481571"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ontdek wie doorsturen heeft ingesteld voor een postvak en hoe

Als extern doorsturen is ingesteld voor een postvak, wordt de activiteit gecontroleerd als onderdeel van de Set-Mailbox-cmdlet. U kunt de activiteit als volgen vinden in het auditlogboek:

1. Ga naar het [Office 365-& compliancecentrum.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecteer **Zoeken in** >  **auditlogboek zoeken.**
    > [!NOTE]
    > Als u een melding ziet dat u de controle moet in- of uitvoeren, gaat u door en schakel deze nu in. Als deze functie niet is ingeschakeld, kunnen er geen gegevens worden verzameld uit eerdere datums.
1. Zorg ervoor dat **het veld** Activiteiten is ingesteld op Resultaten tonen voor **alle activiteiten** (de standaardinstelling). Geef het datumbereik op. U hoeft geen gebruikersnaam op te geven.
1. Selecteer **Zoeken.** De activiteiten worden weergegeven onder **Resultaten.**
1. Selecteer **Filterresultaten** en typ **Postvak Instellen** in het **veld Activiteitsfilter.** Hiermee worden alle activiteiten **van Set-Mailbox** als retourneert.
1. Als u de details wilt weergeven, selecteert u een activiteit en vervolgens **Meer informatie.** Onder **Parameters** ziet u het doorsturende e-mailadres dat is ingesteld voor het postvak. De **UserID** vertegenwoordigt de gebruiker die extern doorsturen heeft ingesteld voor het postvak.
Zie Het Auditlogboek van Office 365 doorzoeken voor meer informatie [om veelvoorkomende scenario's op te lossen.](https://go.microsoft.com/fwlink/?linkid=2103944)