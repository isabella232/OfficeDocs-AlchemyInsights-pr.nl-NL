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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707906"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Leveringsproblemen oplossen voor foutcode 550 5.4.1 Relay-toegang geweigerd

Dit probleem treedt op bij [het controleren of een e-mailadres geldig is om bouncebacks te voorkomen](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) bij het invoeren van het Microsoft-netwerk. Probeer het volgende:

1. Bepaal of het probleem specifiek is voor een heel domein of één e-mailadres:
    - Hele domein: Soms moet het domein worden gesynchroniseerd; probeer [het domein in te stellen op Intern en vervolgens terug naar Gezaghebbend](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Eén e-mailadres: Soms moet het adres worden gesynchroniseerd; het wijzigen van de smtp proxy-adres en vervolgens het veranderen van het terug kan helpen.
2. Bepaal of het probleem specifiek is voor een groep of openbare map. Voor sommige objecttypen moeten de objecten mogelijk handmatig worden gemaakt in Azure Active Directory.

Als je extra hulp nodig hebt, open dan een ondersteuningsticket en geef de omvang van het probleem op (inclusief het type object waarnaar je stuurt) zodat we je beter kunnen helpen.