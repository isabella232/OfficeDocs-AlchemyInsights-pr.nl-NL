---
title: 2419--te-enable-controle
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065625"
---
# <a name="unable-to-enable-unified-auditing"></a>Kan geen uniforme controle inschakelen

Wanneer u probeert een uniforme controle voor uw organisatie Office 365 inschakelen, verschijnt een foutbericht zoals het volgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Dit probleem oplossen door de volgende stappen uit:

1. [Verbinding maken met Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. De volgende cmdlet uitvoert:

   ```
   Enable-OrganizationCustomization
   ```

3. Wacht tot 60 minuten voor de vorige instelling te activeren.

4. Voer de volgende opdracht uit in Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Raadpleeg de volgende artikelen voor meer informatie:

- [Verbinding maken met Exchange Online PowerShell meerledige verificatie gebruiken](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365 audit-logboek zoeken inschakelen of uitschakelen](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
