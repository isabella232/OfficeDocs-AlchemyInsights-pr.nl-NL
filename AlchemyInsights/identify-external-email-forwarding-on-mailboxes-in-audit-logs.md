---
title: Externe e-mailberichten doorsturen naar postvakken in controlelogboeken
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696292"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificeren wanneer externe e-mail forwarding is geconfigureerd voor postvakken

Wanneer een Microsoft 365-gebruiker externe e-mail forwarding configureert voor een postvak, wordt de activiteit gecontroleerd als onderdeel van de cmdlet **set-mailbox** . U kunt de activiteit zien met de zoekfunctie voor auditlogboeken in de beveiligings & compliance Center.

1. Meld u aan bij het [Microsoft 365-beveiligings & nalevings centrum](https://protection.office.com/).

2. Ga **naar de pagina zoeken in**het  >  **audit logboek** .

3. Selecteer het datumbereik in de velden **begindatum** en **einddatum** . U hoeft geen gebruikersnaam op te geven. Controleer of het veld **activiteiten** is ingesteld op **resultaten voor alle activiteiten weergeven**.

4. Klik op **zoeken**.

Klik in de resultaten op **resultaten filteren** en **Postvak** voor typen in het vak activiteiten filter. Selecteer een controlerecord in de resultaten. Klik in het vervolgmenu **Details** op **meer informatie**. U dient de details van elke controlerecord te bekijken om te bepalen of de activiteit betrekking heeft op het doorsturen van e-mail.

- **ObjectId**: de alias waarde van het postvak dat is gewijzigd.

- **Parameters**: _ForwardingSmtpAddress_ geeft het doel-e-mailadres aan.

- **UserID**: de gebruiker die e-mail heeft geconfigureerd voor het postvak in het veld **ObjectId** .

Zie voor meer informatie [bepalen wie het doorsturen van e-mail voor een postvak heeft ingesteld](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
