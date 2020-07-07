---
title: Berichten die naar de Microsoft 365-groep worden verzonden, worden niet door alle leden ontvangen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: nl-NL
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051490"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Berichten die naar een Microsoft 365-groep worden verzonden, worden niet door alle leden ontvangen

Zorg ervoor dat alle groepsleden zich hebben geabonneerd om de e-mails te ontvangen. Zie [Een groep volgen in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Voer de volgende opdracht uit op [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)om de berichtstatus te controleren van leden die zich hebben geabonneerd op groepse-mails:

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`