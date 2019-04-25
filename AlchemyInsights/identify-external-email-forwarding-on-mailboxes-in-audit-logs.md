---
title: Externe e-mail doorsturen op postvakken in de controlelogboeken geïdentificeerd
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417207"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Bepalen wanneer externe e-mail doorsturen is geconfigureerd op de postvakken

Wanneer een gebruiker configureert externe e-mail doorsturen voor een postbus, wordt de activiteit gecontroleerd als onderdeel van de cmdlet **Set-Mailbox** . Hier ziet u de activiteit met audit-logboek zoeken in de & beveiliging conformiteit.

1. Log in op de [Office 365 & conformiteit Beveiligingscentrum](https://protection.office.com/)

2. Klik op **Zoeken en onderzoek** en **Audit-logboek zoeken**selecteren.

3. Selecteer het datumbereik in de velden **begindatum** en **einddatum** . U hoeft niet een gebruikersnaam opgeven. Controleer of dat de **activiteiten** -veld is ingesteld op het **weergeven van resultaten voor alle activiteiten**.

4. Klik op **Zoeken**.

In de resultaten, klikt u op **Filterresultaten** en **Set-Postvak** typt in het vak activiteit filter. Selecteer een audit record in de resultaten. Klik op **meer informatie**in het doel **Details** . U moet de details van elke record controleren om te bepalen of de activiteit betrekking heeft op het doorsturen van e-mail.

- **Object-id**: de waarde van de alias van het postvak dat is gewijzigd.

- **Parameters**: _ForwardingSmtpAddress_ geeft aan dat het doel-e-mailadres.

- **UserId**: de gebruiker die het doorsturen van e-mail in het postvak in in het veld **id** geconfigureerd.

Zie [vaststellen die e-mail doorsturen voor een postbus instellen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)voor meer informatie.
