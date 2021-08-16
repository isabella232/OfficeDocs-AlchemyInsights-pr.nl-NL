---
title: Uw archiefpostvak is bijna vol
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046747"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Uw archiefpostvak is bijna vol

Als de gebruiker de waarschuwing ontvangt; **Uw archiefpostvak is bijna vol** of u moet het archiefpostvak groter maken, hier vindt u enkele tips:

1. Als aan de gebruiker een abonnement Exchange Online abonnement 1 is toegewezen, upgradet u naar Exchange Online **abonnement 2-licentie** om de grootte te vergroten van 50 GB naar 100 GB.
1. Als aan de gebruiker al een van de volgende opties is toegewezen: **Exchange Online Plan 2 of** een Exchange Online-abonnement 1 met een Exchange Online Archiving-invoegactie, gebruikt u de onderstaande stappen om archivering automatisch uit te breiden:.
 
    1. [Verbinding maken powershell Exchange Online gebruiken.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Voer de volgende opdracht voor de gebruiker uit:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Voer de volgende opdracht uit om te bevestigen dat deze is ingeschakeld voor de gebruiker:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Zie voor meer informatie:

- [Onbeperkt archiveren inschakelen - Help voor beheerders - Microsoft 365 compliance | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online limieten - Servicebeschrijvingen | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgraden naar een ander bedrijfsplan | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

