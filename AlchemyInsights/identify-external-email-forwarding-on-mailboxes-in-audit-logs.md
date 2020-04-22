---
title: Externe e-maildoorsturen identificeren op postvakken in controlelogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716455"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificeren wanneer externe e-maildoorsturen is geconfigureerd op postvakken

Wanneer een Microsoft 365-gebruiker externe e-maildoorsturen in een postvak configureert, wordt de activiteit gecontroleerd als onderdeel van de cmdlet **Set-Mailbox.** U de activiteit bekijken met behulp van zoeken in het controlelogboek in het Beveiligings& Compliance Center.

1. Meld u aan bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Ga naar de**zoekpagina van het zoekcontrolelogboek.** **Search** > 

3. Selecteer het datumbereik in de velden **Begindatum** en **Einddatum.** U hoeft geen gebruikersnaam op te geven. Controleer of het veld **Activiteiten** is ingesteld op **Resultaten weergeven voor alle activiteiten**.

4. Klik **op Zoeken**.

Klik in de resultaten op **Resultaten filteren** en typ **Set-Mailbox** in het vak activiteitsfilter. Selecteer een controlerecord in de resultaten. Klik in de flyout **Details** op **Meer informatie**. Je moet kijken naar de details van elke audit record om te bepalen of de activiteit is gerelateerd aan e-mail doorsturen.

- **ObjectId:** de aliaswaarde van het postvak dat is gewijzigd.

- **Parameters**: _ForwardingSmtpAddress_ geeft het doel-e-mailadres aan.

- **UserId:** de gebruiker die e-mail doorsturen heeft geconfigureerd in het postvak in het **veld ObjectId.**

Zie [Bepalen wie e-mail doorsturen voor een postvak heeft ingesteld voor](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)meer informatie.
