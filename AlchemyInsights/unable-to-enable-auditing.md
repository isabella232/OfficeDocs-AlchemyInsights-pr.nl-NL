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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="28334-102">Kan geen uniforme controle inschakelen</span><span class="sxs-lookup"><span data-stu-id="28334-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="28334-103">Wanneer u probeert een uniforme controle voor uw organisatie Office 365 inschakelen, verschijnt een foutbericht zoals het volgende:</span><span class="sxs-lookup"><span data-stu-id="28334-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="28334-104">Dit probleem oplossen door de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="28334-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="28334-105">[Verbinding maken met Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="28334-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="28334-106">De volgende cmdlet uitvoert:</span><span class="sxs-lookup"><span data-stu-id="28334-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="28334-107">Wacht tot 60 minuten voor de vorige instelling te activeren.</span><span class="sxs-lookup"><span data-stu-id="28334-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="28334-108">Voer de volgende opdracht uit in Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="28334-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="28334-109">Raadpleeg de volgende artikelen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="28334-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="28334-110">Verbinding maken met Exchange Online PowerShell meerledige verificatie gebruiken</span><span class="sxs-lookup"><span data-stu-id="28334-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="28334-111">Office 365 audit-logboek zoeken inschakelen of uitschakelen</span><span class="sxs-lookup"><span data-stu-id="28334-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
