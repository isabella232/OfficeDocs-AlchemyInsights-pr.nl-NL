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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="3c0da-102">Kan geen Unified auditfunctie inschakelen</span><span class="sxs-lookup"><span data-stu-id="3c0da-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="3c0da-103">Wanneer u Unified auditing voor uw organisatie probeert in te schakelen, krijgt u mogelijk een foutmelding die er als volgt uitziet:</span><span class="sxs-lookup"><span data-stu-id="3c0da-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="3c0da-104">Voer de volgende stappen uit om dit probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="3c0da-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="3c0da-105">[Maak verbinding met Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="3c0da-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="3c0da-106">Voer de volgende cmdlet uit:</span><span class="sxs-lookup"><span data-stu-id="3c0da-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="3c0da-107">Wacht tot 60 minuten voordat de vorige instelling van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="3c0da-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="3c0da-108">Voer de volgende opdracht uit in Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="3c0da-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="3c0da-109">Zie de volgende artikelen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="3c0da-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="3c0da-110">Verbinding maken met Exchange Online PowerShell met multi-factor Authentication</span><span class="sxs-lookup"><span data-stu-id="3c0da-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  <span data-ttu-id="3c0da-111">[Auditlogboeken zoeken in- of uitschakelen](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off).</span><span class="sxs-lookup"><span data-stu-id="3c0da-111">[Turn audit log search on or off](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)</span></span>
