---
title: Gehoste voicemail inschakelen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677335"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="b00d4-102">Gehoste voicemail inschakelen</span><span class="sxs-lookup"><span data-stu-id="b00d4-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="b00d4-103">Als u voicemail wilt inschakelen, moet **HostedVoicemail** zijn ingesteld op $True.</span><span class="sxs-lookup"><span data-stu-id="b00d4-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="b00d4-104">De **HostedVoicemail** -eigenschap voor de gebruiker via Remote PowerShell (RPS).</span><span class="sxs-lookup"><span data-stu-id="b00d4-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="b00d4-105">Zie voor meer informatie over het maken van verbinding met RPS een [overzicht van Microsoft PowerShell PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) voor meer informatie over verbinding maken met RPS.</span><span class="sxs-lookup"><span data-stu-id="b00d4-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="b00d4-106">De team beheerder moet worden aangemeld bij Remote PowerShell voor teams.</span><span class="sxs-lookup"><span data-stu-id="b00d4-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="b00d4-107">Via PowerShell-prompt de beheerder van de teams kan **set-csuser-user@contoso.com-HostedVoiceMail $True** waarbij de SIP URI van de gebruiker in kwestie is.</span><span class="sxs-lookup"><span data-stu-id="b00d4-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="b00d4-108">Het kan maximaal 24 uur duren voordat de wijzigingen zijn doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="b00d4-108">Changes to policies can take up to 24 hours to replicate.</span></span>