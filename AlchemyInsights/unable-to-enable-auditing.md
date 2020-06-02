---
title: 2419-niet-in staat-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510423"
---
# <a name="unable-to-enable-unified-auditing"></a>Kan uniforme controle niet inschakelen

Wanneer u probeert uniforme audits voor uw organisatie in te schakelen, ontvangt u mogelijk een vergelijkbare fout:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Voer de volgende stappen uit om dit probleem op te lossen:

1. [Maak verbinding met Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Voer de volgende cmdlet uit:

   ```
   Enable-OrganizationCustomization
   ```

3. Wacht 60 minuten voordat de vorige instelling van kracht wordt.

4. Voer de volgende opdracht uit in Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Zie voor meer informatie de volgende artikelen:

- [Verbinding maken met Exchange Online PowerShell met behulp van meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Auditlogboeken zoeken in- of uitschakelen](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off).
