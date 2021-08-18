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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331154"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Bepalen wanneer extern doorsturen van e-mail is geconfigureerd in postvakken

Wanneer een Microsoft 365 externe **e-mail** doorsturen configureert in een postvak, wordt de activiteit gecontroleerd als onderdeel van de cmdlet Postvak instellen. U kunt de activiteit zien met behulp van zoeken in auditlogboek. U doet dit als eerste.

1. Ga op een van de volgende stappen te werk:
   - Ga in Microsoft 365-compliancecentrum naar <https://compliance.microsoft.com> Solutions  \> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://compliance.microsoft.com/auditlogsearch> u .
   - Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://sip.security.microsoft.com/auditlogsearch> u .

2. Controleer op **de** pagina Controle of **het** tabblad Zoeken is geselecteerd en configureer vervolgens de volgende instellingen:
   - Selecteer het datum-/tijdbereik in de vakken **Begin** **en** Einde.
   - Controleer of **het vak** Activiteiten resultaten weergeven voor alle **activiteiten bevat.**

3. Wanneer u klaar bent, klikt u op **Zoeken**. De activiteiten worden weergegeven op de nieuwe **pagina Controle** zoeken.

4. Klik in de resultaten op **Resultaten filteren** en typ **Postvak** instellen in het vak activiteitsfilter.

5. Selecteer een auditrecord in de resultaten. Klik in **het** fly-out Details op **Meer informatie.** U moet de details van elke auditrecord bekijken om te bepalen of de activiteit betrekking heeft op het doorsturen van e-mail.

   - **ObjectId:** de aliaswaarde van het postvak dat is gewijzigd.
   - **Parameters:** _ForwardingSmtpAddress_ geeft het doel-e-mailadres aan.
   - **UserId:** de gebruiker die het doorsturen van e-mail heeft geconfigureerd in het postvak in het **veld ObjectId.**

Zie Bepalen wie e-mail doorsturen voor een postvak heeft [ingesteld voor meer informatie.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
