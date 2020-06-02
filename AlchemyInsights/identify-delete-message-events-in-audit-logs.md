---
title: Gebeurtenissen voor verwijderenberichten identificeren in controlelogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508983"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Controlelogboeken voor verwijderde e-mailberichten

Vanaf januari 2019 zet Microsoft standaard logboekregistratie van postvakken in. Anders moet u de verwijderacties voor een bepaalde gebruiker handmatig inschakelen als u de verwijdergebeurtenissen voor controle wilt controleren. Als de controleregistratie van postvakken al is ingeschakeld voor uw organisatie of voor de specifieke gebruiker, voert u de onderstaande stappen uit.

1. Inloggen bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klik **op Zoeken en onderzoeken** en selecteer Zoeken in **controlelogboek**.

3. Selecteer het datumbereik in de velden **Begindatum** en **Einddatum.** Geef gebruikersnaam op voor de gebruiker die u wilt onderzoeken (de gebruiker die de items heeft verwijderd). Selecteer in het veld **Activiteiten** de optie **Verwijderde berichten uit de map Verwijderde items** en **Berichten verplaatsen naar map Verwijderde items**.

4. Klik **op Zoeken**.

Selecteer in de resultaten een controlerecord. Klik in de flyout details op **Meer informatie**. Aanvullende informatie over het verwijderde item (bijvoorbeeld de onderwerpregel en de locatie van het item toen het is verwijderd) wordt weergegeven in het veld **AffectedItems.** De eigenschap **ClientInfoString** geeft aan of de verwijdering is opgetreden in Outlook, de webversie van Outlook (voorheen Outlook Web App) of een ander apparaat.

Zie [Bepalen wie e-mail doorstuurt voor een postvak voor](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)meer informatie.

**Opmerking**: U verwijderde items niet ophalen met de functie controlelogboek. Zie [Verwijderde items herstellen](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)in Outlook Web App als u verwijderde berichten wilt ophalen in de webversie van Outlook.
