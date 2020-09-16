---
title: Beleidsinstellingen voor vergaderingen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794329"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="1de63-102">Beleidsregels voor vergaderingen beheren in Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="1de63-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="1de63-103">**Opmerking: het kan tot 24 uur duren voordat beleidswijzigingen zijn doorgevoerd voor gebruikers.**</span><span class="sxs-lookup"><span data-stu-id="1de63-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="1de63-104">U kunt mogelijk geen wijzigingen aanbrengen in nieuw gemaakte beleidsregels. Wacht 4 uur en probeer nogmaals een nieuw gemaakt beleid te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="1de63-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="1de63-105">Beleidsregels voor vergaderingen worden gebruikt voor het regelen van de functies die beschikbaar zijn voordeel nemers aan vergaderingen die zijn gepland door gebruikers in uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="1de63-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="1de63-106">Sommige functies van het beleid voor vergaderingen worden mogelijk niet geïmplementeerd in het team centrum voor teams (dit zijn de namen ' binnenkort beschikbaar ' in de documentatie).</span><span class="sxs-lookup"><span data-stu-id="1de63-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="1de63-107">In dit geval of als er een foutbericht wordt weergegeven zoals ' het beleid kan nu niet worden bijgewerkt, maar later opnieuw proberen ' in het Microsoft teams-Beheercentrum, raden we u aan dat u PowerShell gebruikt om beleidsregels voor vergaderingen te maken of te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="1de63-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="1de63-108">Raadpleeg de volgende bronnen voor meer informatie over het beleid voor de vergadering:</span><span class="sxs-lookup"><span data-stu-id="1de63-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="1de63-109">Zie [beleidsregels voor vergaderingen in teams beheren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)voor meer informatie over het maken van beleidsregels, het aanbrengen van wijzigingen en het toewijzen van gebruikers aan het beleid.</span><span class="sxs-lookup"><span data-stu-id="1de63-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="1de63-110">Zie [overzicht van PowerShell-PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)als u beleidswijzigingen wilt aanbrengen met PowerShell-cmdlets.</span><span class="sxs-lookup"><span data-stu-id="1de63-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="1de63-111">U moet de [Skype voor bedrijven PowerShell-module](https://www.microsoft.com/download/details.aspx?id=39366) gebruiken voor team vergaderings beleid.</span><span class="sxs-lookup"><span data-stu-id="1de63-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="1de63-112">Zie de [documentatie over de CsTeamsMeetingPolicy-cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="1de63-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

