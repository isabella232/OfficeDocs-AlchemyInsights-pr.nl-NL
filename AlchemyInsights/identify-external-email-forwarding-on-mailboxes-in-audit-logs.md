---
title: Externe e-mail doorsturen in postvakken identificeren in auditlogboeken
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630244"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Bepalen wanneer extern doorsturen van e-mail is geconfigureerd in postvakken

Wanneer een Microsoft 365 externe **e-mail** doorsturen configureert in een postvak, wordt de activiteit gecontroleerd als onderdeel van de cmdlet Postvak instellen. U kunt de activiteit zien met behulp van zoeken in het auditlogboek in & Compliancecentrum.

1. Meld u aan bij [Microsoft 365 compliancecentrum.](https://protection.office.com/)

2. Ga naar de **zoekpagina**  >  **Van het zoeklogboek zoeken.**

3. Selecteer het datumbereik in de **velden Begindatum** en **Einddatum.** U hoeft geen gebruikersnaam op te geven. Controleer of **het veld** Activiteiten is ingesteld op Resultaten voor alle **activiteiten tonen.**

4. Klik **op Zoeken**.

Klik in de resultaten op **Resultaten filteren** en typ **Postvak** instellen in het vak activiteitsfilter. Selecteer een auditrecord in de resultaten. Klik in **het** fly-out Details op **Meer informatie.** U moet de details van elke auditrecord bekijken om te bepalen of de activiteit betrekking heeft op het doorsturen van e-mail.

- **ObjectId:** de aliaswaarde van het postvak dat is gewijzigd.

- **Parameters:** _ForwardingSmtpAddress_ geeft het doel-e-mailadres aan.

- **UserId:** de gebruiker die het doorsturen van e-mail heeft geconfigureerd in het postvak in het **veld ObjectId.**

Zie Bepalen wie e-mail doorsturen voor een postvak heeft [ingesteld voor meer informatie.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
