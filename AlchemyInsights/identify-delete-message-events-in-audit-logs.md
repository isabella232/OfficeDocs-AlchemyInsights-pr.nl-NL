---
title: Berichtengebeurtenissen verwijderen in controlelogboeken identificeren
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
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716491"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Controlelogboeken voor verwijderde e-mailberichten

Vanaf januari 2019 schakelt Microsoft standaard de controlelogboekregistratie van het postvak in. Als u anders berichtgebeurtenissen voor een specifieke gebruiker wilt controleren, moet u de verwijderingsacties handmatig inschakelen voor controle. Als de controlelogboekregistratie voor postvakcontroles al is ingeschakeld voor uw organisatie of voor de specifieke gebruiker, voert u de onderstaande stappen uit.

1. Inloggen bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klik **op Zoeken en onderzoeken** en selecteer Zoeken in het **controlelogboek**.

3. Selecteer het datumbereik in de velden **Begindatum** en **Einddatum.** Geef de gebruikersnaam op voor de gebruiker die u wilt onderzoeken (de gebruiker die de items heeft verwijderd). Selecteer in het veld **Activiteiten** de optie **Verwijderde berichten uit de map Verwijderde items** en Berichten verplaatst naar de map Verwijderde **items**.

4. Klik **op Zoeken**.

Selecteer in de resultaten een controlerecord. Klik in de flyout met details op **Meer informatie**. Aanvullende informatie over het verwijderde item (bijvoorbeeld de onderwerpregel en de locatie van het item toen het werd verwijderd) wordt weergegeven in het veld **Getroffen Items.** In de eigenschap **ClientInfoString** wordt weergegeven of de verwijdering heeft plaatsgevonden in Outlook, de webversie van Outlook (voorheen Outlook Web App) of een ander apparaat.

Zie [Bepalen wie e-mail doorsturen voor een postvak heeft ingesteld voor](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)meer informatie.

**Opmerking:** U verwijderde items niet ophalen met de functie controlelogboek. Zie Verwijderde items herstellen [in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)als u verwijderde berichten wilt ophalen in de webversie van Outlook.
