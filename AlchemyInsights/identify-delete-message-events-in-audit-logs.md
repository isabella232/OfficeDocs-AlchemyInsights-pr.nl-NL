---
title: Delete message gebeurtenissen in de controlelogboeken geïdentificeerd
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539204"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Controlelogboeken voor verwijderde e-mailberichten

Starten in januari 2019, is Microsoft inschakelen postbus controlelogboeken standaard. Anders verwijderen bericht om gebeurtenissen te bekijken voor een bepaalde gebruiker, moet u handmatig de delete-acties voor controle inschakelen. Als postvak controleren registratie al is ingeschakeld voor uw organisatie of voor de specifieke gebruiker, volg de onderstaande stappen.

1. Log in op de [Office 365 & conformiteit Beveiligingscentrum](https://protection.office.com/)

2. Klik op **Zoeken en onderzoek** en **Audit-logboek zoeken**selecteren.

3. Selecteer het datumbereik in de velden **begindatum** en **einddatum** . Geef de gebruikersnaam van de gebruiker die u wilt onderzoeken (de gebruiker die de artikelen verwijderd). Selecteer in het veld **activiteiten** **Verwijderde berichten uit de map Verwijderde Items** en **Moved berichten naar de map Verwijderde Items**.

4. Klik op **Zoeken**.

Selecteer een audit record in de resultaten. Klik op **Meer informatie**in het doel details. Meer informatie over het verwijderde item (bijvoorbeeld, de onderwerpregel en de locatie van het item is verwijderd) wordt weergegeven in het veld **AffectedItems** . De eigenschap **ClientInfoString** wordt weergegeven als het verwijderen is opgetreden in Outlook, Outlook op het web (voorheen bekend als Outlook Web App) of een ander apparaat.

Zie [vaststellen die e-mail doorsturen voor een postbus instellen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)voor meer informatie.

**Opmerking**: Verwijderde items met de functie van audit log niet ophalen. Zie [Verwijderde items in Outlook Web App herstellen](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)voor het ophalen van verwijderde berichten in Outlook op het web.
