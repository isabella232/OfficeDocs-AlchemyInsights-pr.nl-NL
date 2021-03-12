---
title: Beleidsinstellingen voor vergadering
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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704601"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="f7d0b-102">Vergaderbeleid beheren in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f7d0b-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="f7d0b-103">**Opmerking: Het kan tot 24 uur duren voordat beleidswijzigingen voor gebruikers zijn doorgevoerd.**</span><span class="sxs-lookup"><span data-stu-id="f7d0b-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="f7d0b-104">Mogelijk kunt u niet direct wijzigingen aanbrengen in nieuw gemaakte beleidsregels. wacht 4 uur en probeer opnieuw een nieuw beleid te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="f7d0b-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="f7d0b-105">Vergaderbeleid wordt gebruikt om de functies te bepalen die beschikbaar zijn voor deelnemers aan een vergadering voor vergaderingen die worden gepland door gebruikers in uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="f7d0b-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="f7d0b-106">Sommige functies van vergaderbeleid worden mogelijk nog niet geïmplementeerd in het Teams-beheercentrum (deze hebben het label 'binnenkort beschikbaar' in de documentatie).</span><span class="sxs-lookup"><span data-stu-id="f7d0b-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="f7d0b-107">In dit geval, of als u een foutbericht krijgt zoals 'Het beleid kan momenteel niet worden bijgewerkt, maar probeer het later opnieuw' in het Microsoft Teams-beheercentrum, raden we u aan PowerShell te gebruiken om vergaderbeleid voor Teams te maken of te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="f7d0b-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="f7d0b-108">Zie de volgende bronnen voor meer informatie over vergaderbeleid:</span><span class="sxs-lookup"><span data-stu-id="f7d0b-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="f7d0b-109">Zie Vergaderbeleid beheren in Teams voor meer informatie over het maken van beleidsregels, het aanbrengen van wijzigingen en het toewijzen van gebruikers [aan het beleid.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="f7d0b-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="f7d0b-110">Zie Overzicht van [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)als u beleidswijzigingen wilt aanbrengen met behulp van PowerShell-cmdlets.</span><span class="sxs-lookup"><span data-stu-id="f7d0b-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="f7d0b-111">U moet de Skype voor [Bedrijven PowerShell-module voor](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) vergaderbeleid voor Teams gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f7d0b-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="f7d0b-112">Lees de [documentatie van de \*-CsTeamsMeetingPolicy-cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f7d0b-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

