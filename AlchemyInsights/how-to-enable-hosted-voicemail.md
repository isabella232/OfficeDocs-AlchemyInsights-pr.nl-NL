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
# <a name="how-to-enable-hosted-voicemail"></a>Gehoste voicemail inschakelen

Als u voicemail wilt inschakelen, moet **HostedVoicemail** zijn ingesteld op $True.

De **HostedVoicemail** -eigenschap voor de gebruiker via Remote PowerShell (RPS).

Zie voor meer informatie over het maken van verbinding met RPS een [overzicht van Microsoft PowerShell PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) voor meer informatie over verbinding maken met RPS.

1. De team beheerder moet worden aangemeld bij Remote PowerShell voor teams.
1. Via PowerShell-prompt de beheerder van de teams kan **set-csuser-user@contoso.com-HostedVoiceMail $True** waarbij de SIP URI van de gebruiker in kwestie is.

> [!NOTE]
> Het kan maximaal 24 uur duren voordat de wijzigingen zijn doorgevoerd.