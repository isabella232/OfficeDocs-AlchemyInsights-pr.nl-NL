---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932272"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Bezorgingsproblemen oplossen voor foutcode 550 5.4.1 Doorlevertoegang geweigerd

Dit probleem treedt op bij het controleren of een e-mailadres geldig is om [stuiterbacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) te voorkomen bij het invoeren van het Microsoft-netwerk. Probeer het volgende:

1. Bepaal of het probleem specifiek is voor een heel domein of één e-mailadres:
    - Hele domein: Soms moet het domein worden gesynchroniseerd. probeer [het domein in te stellen op Intern en vervolgens terug te gaan naar Gezaghebbend.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Eén e-mailadres: Soms moet het adres worden gesynchroniseerd; het wijzigen van het smtp-proxyadres en het vervolgens wijzigen van het adres kan helpen.
2. Bepaal of het probleem specifiek is voor een groep of openbare map. Voor sommige objecttypen moeten de objecten mogelijk handmatig worden gemaakt in Azure Active Directory.

Als u extra hulp nodig hebt, opent u een ondersteuningsticket en geeft u het bereik van het probleem op (inclusief het type object dat u wilt verzenden) zodat we u beter kunnen helpen.