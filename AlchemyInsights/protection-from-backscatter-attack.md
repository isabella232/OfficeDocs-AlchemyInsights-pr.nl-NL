---
title: Beveiliging tegen backscatter-aanval
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035410"
---
# <a name="protection-from-backscatter-attack"></a>Beveiliging tegen backscatter-aanval

Backscatter is niet-bezorgingsrapporten (ook wel NDR's of niet-bezorgde berichten genoemd) die u ontvangt voor berichten die u niet hebt verzonden. Spammers vervalsen (spoof) het **Van:-adres** van hun berichten en ze gebruiken vaak echte e-mailadressen om hun berichten geloofwaardig te maken. Dus wanneer spammers onvermijdelijk berichten verzenden naar niet-bestaande geadresseerden, wordt de doel-e-mailserver in feite misleid om het niet-verkeerbare bericht in een NDR terug te sturen naar de vervalste afzender in het **Adres van:** van.

Aanvullende informatie vindt u in [Backscatter in EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)

**Backscatterbeveiliging inschakelen**

Als u backscatterbeveiliging wilt inschakelen, volgt u het onderstaande pad.

**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to "On"**

Als u denkt dat een account is gehackt, gaat u als volgt te werk:

- [Reageren op een gehackt e-mailaccount](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Geblokkeerde gebruikers verwijderen uit de portal Beperkte gebruikers in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



