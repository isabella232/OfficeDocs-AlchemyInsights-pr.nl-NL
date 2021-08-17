---
title: Ontdek wie doorsturen in een postvak heeft ingesteld en hoe
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895174"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ontdek wie doorsturen in een postvak heeft ingesteld en hoe

Als extern doorsturen is ingesteld op een postvak, wordt de activiteit gecontroleerd als onderdeel van **de** cmdlet Postvak instellen. U vindt als volgende de activiteit in het auditlogboek:

1. Een van de volgende acties uitvoeren:
   - Ga in Microsoft 365-compliancecentrum naar <https://compliance.microsoft.com> Solutions  \> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://compliance.microsoft.com/auditlogsearch> u .
   - Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://security.microsoft.com/auditlogsearch> u .

   > [!NOTE]
   > Als u een melding ziet dat u auditing moet in- of uit- zetten, gaat u door en zet u deze nu in. Als deze functie niet is ingeschakeld, kunnen zoekresultaten geen gegevens uit eerdere datums halen.

2. Controleer op **de** pagina Controle of **het** tabblad Zoeken is geselecteerd en configureer de volgende instellingen:
   - Selecteer het datum-/tijdbereik in de vakken **Begin** **en** Einde.
   - Controleer of **het vak** Activiteiten resultaten weergeven voor alle **activiteiten bevat.**

3. Wanneer u klaar bent, klikt u op **Zoeken**. De activiteiten worden weergegeven op de nieuwe **pagina Controle zoeken.**

4. Klik in de resultaten op de kolom **Activiteit** om de resultaten te sorteren en zoek naar **Postvakinzendingen** instellen.

5. Selecteer een activiteit in de resultaten om de details flyout te openen. U moet de details van elke auditrecord bekijken om te bepalen of de activiteit gerelateerd is aan het doorsturen van e-mail:
   - **ObjectId:** de aliaswaarde van het postvak dat is gewijzigd.
   - **Parameters:** _ForwardingSmtpAddress_ geeft het doel-e-mailadres aan.
   - **UserId:** de gebruiker die het doorsturen van e-mail heeft geconfigureerd in het postvak in het **veld ObjectId.**

Zie Bepalen wie e-mail doorsturen voor een postvak heeft [ingesteld voor meer informatie.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
