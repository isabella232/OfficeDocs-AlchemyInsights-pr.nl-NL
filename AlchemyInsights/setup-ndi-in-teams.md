---
title: NDI-technologie inleveren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935098"
---
# <a name="turn-on-ndi-technology"></a>NDI-technologie inleveren

Voor NDI-technologie moeten twee stappen worden ingeschakeld voor een gebruiker:

1. De tenantbeheerder moet de eigenschap AllowNDIStreaming in CsTeamsMeetingPolicy inschakelen.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Nadat deze wijziging is ingevuld, moet de eindgebruiker NDI®-technologie voor zijn of haar specifieke client inleveren vanuit **Instellingen > Machtigingen.**

Zie NDI-technologie gebruiken [in Microsoft Teams voor meer informatie.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
