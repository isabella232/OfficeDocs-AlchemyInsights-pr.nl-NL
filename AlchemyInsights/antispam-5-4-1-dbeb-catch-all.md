---
title: Spam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717356"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Problemen met de bezorging bij foutcode 550 5.4.1 relay toegang geweigerd

Dit probleem doet zich voor wanneer [u controleert of een e-mailadres geldig is om te voorkomen dat bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) bij het invoeren van het Microsoft-netwerk. Probeert u het volgende:

1. Bepalen of het probleem specifiek is voor een volledig domein of één e-mailadres:
    - Volledig domein: soms moet het domein worden gesynchroniseerd. [Stel het domein in op interne en vervolgens terug naar de gemachtigde](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Eén e-mailadres: soms moet het adres worden gesynchroniseerd. Als u het adres van de SMTP-proxy wijzigt en daarna weer overschakelt, kan dit helpen.
2. Bepalen of het probleem specifiek is voor een groep of openbare map. Voor sommige objecttypen moet u de objecten mogelijk handmatig maken in azure Active Directory.

Als u extra hulp nodig hebt, opent u een ondersteuningsticket en geeft u het bereik van het probleem op, zoals het type object dat u verzendt, zodat we u beter kunnen helpen.