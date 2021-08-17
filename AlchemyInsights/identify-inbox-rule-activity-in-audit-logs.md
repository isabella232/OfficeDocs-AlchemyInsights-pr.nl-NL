---
title: Activiteit in postvak IN identificeren in auditlogboeken
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891290"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Activiteit in postvak IN identificeren in auditlogboeken

U kunt zoeken in auditlogboek in de Microsoft 365-compliancecentrum om regelgebeurtenissen voor Postvak IN weer te geven (regels voor postvak IN maken, wijzigen en verwijderen).

1. Ga op een van de volgende stappen te werk:
   - Ga in Microsoft 365-compliancecentrum naar <https://compliance.microsoft.com> Solutions  \> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://compliance.microsoft.com/auditlogsearch> u .
   - Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com> **Audit.** Of als u rechtstreeks naar de pagina **Controle wilt** gaan, gebruikt <https://security.microsoft.com/auditlogsearch> u .

2. Configureer **op het** tabblad Zoeken van de pagina **Controle** de volgende instellingen:
   - **Datum en tijdbereik:** Selecteer het datum-/tijdbereik in de vakken **Begin** **en** Einde.
   - **Activiteiten:** Selecteer een of meer van de volgende waarden:
     - **New-InBoxRule Create Inbox rule from Outlook Web App**
     - **Set-InBoxRule Modify rule from Outlook Web App**.
     - **Regels voor Postvak IN bijwerken van Outlook client**

3. Wanneer u klaar bent, klikt u op **Zoeken**. De activiteiten worden weergegeven op de nieuwe **pagina Controle** zoeken.

4. Selecteer een activiteit in de resultaten om de details flyout te openen. In het veld Parameters wordt informatie over de instellingen voor de regels voor **postvak** IN weergegeven.

Zie Bepalen of een gebruiker een regel [voor Postvak IN](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)heeft gemaakt voor meer informatie.
