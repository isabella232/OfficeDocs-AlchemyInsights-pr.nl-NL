---
title: Uw archief postvak is bijna vol
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974276"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Uw archief postvak is bijna vol

Als de gebruiker de waarschuwing ontvangt. **Uw archief postvak is bijna vol**, of u moet de grootte van het archief postvak groter maken en hier volgen enkele tips:

1. Als aan de gebruiker een abonnement 1 voor Exchange Online is toegewezen, voert u een upgrade uit naar **Exchange Online plan 2** -licentie om de grootte van 50 GB naar 100 GB te vergroten.
1. Als aan de gebruiker al een van de volgende een van de volgende gebruikers is toegewezen: **Exchange Online abonnement 2** of Exchange Online abonnement 1 met een invoegtoepassing voor Exchange Online archivering, voert u de onderstaande stappen uit om het automatisch uitbreiden van de archiveringsfunctie in te schakelen:.
 
    1. [Maak verbinding met Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Voer de volgende commandlet uit voor de gebruiker:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Voer de volgende commandlet uit om te controleren of deze functie is ingeschakeld voor de gebruiker:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Zie voor meer informatie:

- [ Onbeperkt archivering inschakelen-Help voor beheerders: Microsoft 365 compliance | Microsoft docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Limieten voor Exchange Online-Service beschrijvingen | Microsoft docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade naar een ander Business-abonnement | Microsoft docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

