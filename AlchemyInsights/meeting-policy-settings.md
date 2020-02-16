---
title: Beleidsinstellingen voor vergadering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042839"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="5ebc7-102">Vergaderbeleid beheren in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5ebc7-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="5ebc7-103">**Opmerking: het kan tot 24 uur duren voordat beleidswijzigingen van kracht worden voor gebruikers.**</span><span class="sxs-lookup"><span data-stu-id="5ebc7-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="5ebc7-104">Mogelijk u niet onmiddellijk wijzigingen aanbrengen in nieuw gemaakt beleid. wacht 4 uur en probeer een nieuw gemaakt beleid opnieuw te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="5ebc7-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="5ebc7-105">Vergaderbeleid wordt gebruikt om de functies te beheren die beschikbaar zijn voor deelnemers aan vergaderingen voor vergaderingen die zijn gepland door gebruikers in uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="5ebc7-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="5ebc7-106">Sommige functies van het vergaderbeleid worden mogelijk nog niet geïmplementeerd in het beheercentrum van Teams (deze worden in de documentatie als 'binnenkort' gelabeld).</span><span class="sxs-lookup"><span data-stu-id="5ebc7-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="5ebc7-107">In dit geval, of als u een foutmelding krijgt als 'We kunnen het beleid nu niet bijwerken, maar het later opnieuw proberen' in het Microsoft Teams-beheercentrum, raden we u aan PowerShell te gebruiken om het beleid voor teams en vergaderingen te maken of te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="5ebc7-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="5ebc7-108">Zie de volgende bronnen voor meer informatie over vergaderbeleid:</span><span class="sxs-lookup"><span data-stu-id="5ebc7-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="5ebc7-109">Zie [Vergaderingsbeleid beheren in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)voor meer informatie over het maken van beleid, het aanbrengen van wijzigingen en het toewijzen van gebruikers aan het beleid.</span><span class="sxs-lookup"><span data-stu-id="5ebc7-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="5ebc7-110">Zie Overzicht van [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)om beleidswijzigingen aan te brengen met PowerShell-cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5ebc7-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="5ebc7-111">U moet de [PowerShell-module van Skype voor Bedrijven](https://www.microsoft.com/download/details.aspx?id=39366) gebruiken voor het voldoensbeleid van Teams.</span><span class="sxs-lookup"><span data-stu-id="5ebc7-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="5ebc7-112">Bekijk de [\*-CsTeamsMeetingPolicy cmdlets documentatie](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="5ebc7-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

