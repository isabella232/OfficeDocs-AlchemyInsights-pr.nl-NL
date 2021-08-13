---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007785"
---
# <a name="unable-to-enable-unified-auditing"></a>Unified Auditing kan niet worden ingeschakeld

Wanneer u unified auditing voor uw organisatie probeert in te stellen, ziet u mogelijk een fout die vergelijkbaar is met de volgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Als u dit probleem wilt oplossen, gaat u als volgt te werk:

1. [Verbinding maken powershell Exchange Online gebruiken.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Voer de volgende cmdlet uit:

   ```
   Enable-OrganizationCustomization
   ```

3. Wacht 60 minuten totdat de vorige instelling van kracht wordt.

4. Voer de volgende opdracht uit in Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Zie de volgende artikelen voor meer informatie:

- [Verbinding maken powershell Exchange Online met meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Auditlogboeken zoeken in- of uitschakelen](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off).
