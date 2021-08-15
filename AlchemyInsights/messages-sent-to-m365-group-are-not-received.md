---
title: Berichten aan Microsoft 365-groep niet door alle leden ontvangen
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976500"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Berichten aan een Microsoft 365-groep worden niet door alle leden ontvangen

Controleer of alle groepsleden zich op de e-mails hebben geabonneerd. Zie [Een groep volgen in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Voer de volgende opdracht uit in [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) om de berichtstatus van leden die zich op groeps-e-mailberichten hebben geabonneerd te controleren:

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Gebruik de volgende EXO PowerShell-opdracht om alle groepsleden zo te configureren dat ze e-mails aan een Microsoft 365-groep in hun Postvak IN ontvangen:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Bijvoorbeeld:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`