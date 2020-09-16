---
title: 2419-niet-ingeschakeld-controleren
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767594"
---
# <a name="unable-to-enable-unified-auditing"></a>Kan geen Unified auditfunctie inschakelen

Wanneer u Unified auditing voor uw organisatie probeert in te schakelen, krijgt u mogelijk een foutmelding die er als volgt uitziet:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Voer de volgende stappen uit om dit probleem op te lossen:

1. [Maak verbinding met Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Voer de volgende cmdlet uit:

   ```
   Enable-OrganizationCustomization
   ```

3. Wacht tot 60 minuten voordat de vorige instelling van kracht wordt.

4. Voer de volgende opdracht uit in Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Zie de volgende artikelen voor meer informatie:

- [Verbinding maken met Exchange Online PowerShell met multi-factor Authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Auditlogboeken zoeken in- of uitschakelen](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off).
