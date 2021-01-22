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
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="4408f-102">NDI-technologie inleveren</span><span class="sxs-lookup"><span data-stu-id="4408f-102">Turn on NDI technology</span></span>

<span data-ttu-id="4408f-103">Voor NDI-technologie moeten twee stappen worden ingeschakeld voor een gebruiker:</span><span class="sxs-lookup"><span data-stu-id="4408f-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="4408f-104">De tenantbeheerder moet de eigenschap AllowNDIStreaming in CsTeamsMeetingPolicy inschakelen.</span><span class="sxs-lookup"><span data-stu-id="4408f-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="4408f-105">Nadat deze wijziging is ingevuld, moet de eindgebruiker NDI®-technologie voor zijn of haar specifieke client inleveren vanuit **Instellingen > Machtigingen.**</span><span class="sxs-lookup"><span data-stu-id="4408f-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="4408f-106">Zie NDI-technologie gebruiken [in Microsoft Teams voor meer informatie.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="4408f-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
