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
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="6ef82-102">Uw archief postvak is bijna vol</span><span class="sxs-lookup"><span data-stu-id="6ef82-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="6ef82-103">Als de gebruiker de waarschuwing ontvangt. **Uw archief postvak is bijna vol**, of u moet de grootte van het archief postvak groter maken en hier volgen enkele tips:</span><span class="sxs-lookup"><span data-stu-id="6ef82-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="6ef82-104">Als aan de gebruiker een abonnement 1 voor Exchange Online is toegewezen, voert u een upgrade uit naar **Exchange Online plan 2** -licentie om de grootte van 50 GB naar 100 GB te vergroten.</span><span class="sxs-lookup"><span data-stu-id="6ef82-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="6ef82-105">Als aan de gebruiker al een van de volgende een van de volgende gebruikers is toegewezen: **Exchange Online abonnement 2** of Exchange Online abonnement 1 met een invoegtoepassing voor Exchange Online archivering, voert u de onderstaande stappen uit om het automatisch uitbreiden van de archiveringsfunctie in te schakelen:.</span><span class="sxs-lookup"><span data-stu-id="6ef82-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="6ef82-106">[Maak verbinding met Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6ef82-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="6ef82-107">Voer de volgende commandlet uit voor de gebruiker:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="6ef82-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="6ef82-108">Voer de volgende commandlet uit om te controleren of deze functie is ingeschakeld voor de gebruiker:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="6ef82-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="6ef82-109">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="6ef82-109">For more information see:</span></span>

- [<span data-ttu-id="6ef82-110"> Onbeperkt archivering inschakelen-Help voor beheerders: Microsoft 365 compliance | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="6ef82-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="6ef82-111">Limieten voor Exchange Online-Service beschrijvingen | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="6ef82-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="6ef82-112">Upgrade naar een ander Business-abonnement | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="6ef82-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

