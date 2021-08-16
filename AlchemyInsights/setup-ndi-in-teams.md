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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023517"
---
# <a name="turn-on-ndi-technology"></a>NDI-technologie inleveren

Voor NDI-technologie moeten twee stappen worden ingeschakeld voor een gebruiker:

1. De tenantbeheerder moet de eigenschap AllowNDIStreaming in CsTeamsMeetingPolicy inschakelen.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Nadat deze wijziging is ingevuld, moet de eindgebruiker NDI®-technologie voor zijn of haar specifieke client in Instellingen > **machtigingen**.

Zie [NDI-technologie](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)gebruiken in Microsoft Teams.
