---
title: Berichtgebeurtenissen in auditlogboeken identificeren
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
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868413"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Auditlogboeken voor verwijderde e-mailberichten

Vanaf januari 2019 wordt de logboekregistratie voor postvakken standaard ingeschakeld door Microsoft. Als u anders berichtgebeurtenissen voor een specifieke gebruiker wilt controleren, moet u de verwijderacties handmatig inschakelen voor controle. Als de logboekregistratie voor postvakcontrole al is ingeschakeld voor uw organisatie of voor de specifieke gebruiker, volgt u de onderstaande stappen.

1. Meld u aan bij [het Microsoft 365 Compliance Center](https://protection.office.com/)

2. Klik **op Zoeken en onderzoeken** en selecteer **Auditlogboek zoeken.**

3. Selecteer het datumbereik in de **velden Begindatum** en **Einddatum.** Geef gebruikersnaam op voor de gebruiker die u wilt onderzoeken (de gebruiker die de items heeft verwijderd). Selecteer in **het** veld Activiteiten **Deleted messages from Deleted Items folder** and Moved messages to **Deleted Items folder**.

4. Klik **op Zoeken**.

Selecteer in de resultaten een auditrecord. Klik in de flyout details op **Meer informatie.** Aanvullende informatie over het verwijderde item (bijvoorbeeld de onderwerpregel en de locatie van het item toen het werd verwijderd) wordt weergegeven in het veld **AffectedItems.** De **eigenschap ClientInfoString** laat zien of de verwijdering heeft plaatsgevonden in Outlook, webversie van Outlook (voorheen bekend als Outlook Web App) of een ander apparaat.

Zie Bepalen wie e-mail doorsturen voor een postvak heeft [ingesteld voor meer informatie.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Opmerking:** U kunt verwijderde items niet ophalen met de functie auditlogboek. Als u verwijderde berichten in webversie van Outlook wilt ophalen, gaat u naar [Verwijderde items herstellen in Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
