---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964117"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Leveringsproblemen oplossen voor foutcode 550 5.4.1 relaytoegang geweigerd

Dit probleem treedt op bij het [controleren om te zien of een e-mailadres geldig is om te voorkomen dat bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) bij het invoeren van het netwerk van Office 365. Probeer het volgende:

1. Bepaal of het probleem specifiek is voor een volledig domein of voor één e-mailadres:
    - Hele domein: soms moet het domein worden gesynchroniseerd; Probeer [het domein in te stellen op intern en vervolgens terug naar gezaghebbend](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Eén e-mailadres: soms moet het adres worden gesynchroniseerd; Als u het SMTP-proxyadres wijzigt en vervolgens weer wijzigt, kan dit helpen.
2. Bepaal of het probleem specifiek is voor een groep of openbare map. Voor sommige objecttypen moeten de objecten mogelijk handmatig worden gemaakt in azure Active Directory.

Als u extra hulp nodig hebt, opent u een ondersteuningsticket en geeft u het bereik van het probleem op (includidng het type object waarnaar u verzendt), zodat we u beter kunnen helpen.