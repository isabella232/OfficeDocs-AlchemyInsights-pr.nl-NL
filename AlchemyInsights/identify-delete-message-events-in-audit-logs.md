---
title: Berichten verwijderen uit de logboekgebeurtenissen in auditlogboeken
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696508"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Controlelogboeken voor verwijderde e-mailberichten

Vanaf januari 2019 wordt in Microsoft de auditlogboek registratie voor Postvak in standaard ingeschakeld. Als u de berichten voor een bepaalde gebruiker ook wilt verwijderen, moet u de Delete-acties handmatig inschakelen voor de controle. Voer de onderstaande stappen uit als controlelogboeken voor de Postvak al zijn ingeschakeld voor uw organisatie of voor de specifieke gebruiker.

1. Meld u aan bij het [Microsoft 365-beveiligings & nalevings centrum](https://protection.office.com/)

2. Klik op **zoeken en onderzoeken** en selecteer **Zoeken in audit logboek**.

3. Selecteer het datumbereik in de velden **begindatum** en **einddatum** . Geef de gebruikersnaam op voor de gebruiker die u wilt onderzoeken (de gebruiker die de items heeft verwijderd). Selecteer in het veld **activiteiten** de optie **Verwijderde berichten uit de map Verwijderde items** en **verplaatste berichten naar de map Verwijderde items**.

4. Klik op **zoeken**.

Selecteer een controlerecord in de resultaten. Klik in het vervolgmenu Details op **meer informatie**. Aanvullende informatie over het verwijderde item (bijvoorbeeld de onderwerpregel en de locatie van het item na verwijdering) wordt weergegeven in het veld **AffectedItems** . De eigenschap **ClientInfoString** wordt weergegeven als de verwijdering is uitgevoerd in Outlook, de webversie van Outlook (voorheen Outlook Web app) of een ander apparaat.

Zie voor meer informatie [bepalen wie het doorsturen van e-mail voor een postvak heeft ingesteld](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Opmerking**: u kunt verwijderde items niet ophalen met de functie auditlogboek. Zie [Verwijderde items herstellen in Outlook Web app](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)voor informatie over het ophalen van verwijderde berichten in de webversie van Outlook.
