---
title: Externe e-mail doorsturen op postvakken identificeren in controlelogboeken
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
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508947"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificeren wanneer externe e-mail doorsturen is geconfigureerd op postvakken

Wanneer een Microsoft 365-gebruiker externe e-mail doorstuurt op een postvak, wordt de activiteit gecontroleerd als onderdeel van de cmdlet **Set-Mailbox.** U de activiteit bekijken met behulp van controlelogboekzoekopdrachten in het Security & Compliance Center.

1. Meld u aan bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Ga naar de zoekpagina **van het**  >  **zoekcontrolelogboek.**

3. Selecteer het datumbereik in de velden **Begindatum** en **Einddatum.** U hoeft geen gebruikersnaam op te geven. Controleer of het veld **Activiteiten** is ingesteld op **Resultaten weergeven voor alle activiteiten.**

4. Klik **op Zoeken**.

Klik in de resultaten op **Resultaten filteren** en typ **Set-Postvak** in het vak activiteitenfilter. Selecteer een controlerecord in de resultaten. Klik in de flyout **Details** op **Meer informatie**. U moet kijken naar de details van elke controlerecord om te bepalen of de activiteit gerelateerd is aan het doorsturen van e-mail.

- **ObjectId**: de aliaswaarde van het postvak dat is gewijzigd.

- **Parameters**: _ForwardingSmtpAddress_ geeft het doele-mailadres aan.

- **UserId**: De gebruiker die e-mail doorstuurt op het postvak in het veld **ObjectId.**

Zie [Bepalen wie e-mail doorstuurt voor een postvak voor](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)meer informatie.
