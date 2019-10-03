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
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376592"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="225a2-102">Vergaderings beleid beheren in Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="225a2-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="225a2-103">Vergaderings beleid wordt gebruikt om de functies te beheren die beschikbaar zijn om deelnemers te ontmoeten voor vergaderingen die zijn gepland door gebruikers in uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="225a2-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="225a2-104">Sommige functies van het Vergader beleid kunnen niet worden geïmplementeerd in het Beheercentrum van de teams nog (deze zijn gelabeld "binnenkort" in de documentatie).</span><span class="sxs-lookup"><span data-stu-id="225a2-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="225a2-105">In dit geval of als u een foutmelding krijgt als ' we kunnen het beleid nu niet bijwerken, maar probeer het later opnieuw ' in het Microsoft-teams Admin Center, wordt u aangeraden PowerShell gebruiken om te maken of wijzigen van beleid voor teams vergadering.</span><span class="sxs-lookup"><span data-stu-id="225a2-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="225a2-106">Zie de volgende bronnen voor meer informatie over het beleid van de vergadering:</span><span class="sxs-lookup"><span data-stu-id="225a2-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="225a2-107">Zie voor meer informatie over het maken van beleid, wijzigingen aanbrengen en toewijzen van gebruikers aan het beleid, [vergadering beleid in teams beheren](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="225a2-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="225a2-108">Voor het maken van beleidswijzigingen met behulp van PowerShell-cmdlets, Zie [teams PowerShell overzicht](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="225a2-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="225a2-109">U moet de [Skype voor Business PowerShell-module](https://www.microsoft.com/download/details.aspx?id=39366) voor teams vergadering beleid gebruiken.</span><span class="sxs-lookup"><span data-stu-id="225a2-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="225a2-110">Lees de [\*-csteamsmeetingpolicy cmdlets documentatie](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="225a2-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="225a2-111">**Opmerking:** Het kan tot 24 uur duren voordat beleidswijzigingen van kracht worden voor gebruikers.</span><span class="sxs-lookup"><span data-stu-id="225a2-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="225a2-112">Het is mogelijk dat u niet onmiddellijk wijzigingen aanbrengen in nieuw gemaakte beleidsregels. Wacht 4 uur en probeer een nieuw gemaakt beleid opnieuw te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="225a2-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="225a2-113">Als u nog steeds problemen ondervindt, probeert u PowerShell.</span><span class="sxs-lookup"><span data-stu-id="225a2-113">If you're still having problems, try PowerShell.</span></span>  