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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318643"
---
# <a name="how-to-enable-hosted-voicemail"></a>Gehoste voicemail inschakelen

Als u Voicemail wilt inschakelen, **moet HostedVoicemail** zijn ingesteld op $true.

De **eigenschap HostedVoicemail** van de gebruiker die Remote PowerShell (RPS) gebruikt.

Zie voor meer informatie over het maken van verbinding met RPS [Microsoft Teams PowerShell-overzicht](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) voor meer informatie over het maken van verbinding met RPS.

1. De Teams beheerder moet zijn aangemeld bij Externe PowerShell voor Teams.
1. Vraag vanuit PowerShell of de **Teams-beheerder set-csuser user@contoso.com -HostedVoiceMail $true** kan uitvoeren waar de sip uri van de gebruiker in kwestie is.

**Opmerking:** Het kan tot 24 uur duren voordat wijzigingen in beleidsregels worden gerepliceerd.