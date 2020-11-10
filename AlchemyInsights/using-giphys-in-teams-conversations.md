---
title: Giphy's gebruiken in team gesprekken
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982460"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="5164f-102">Giphy's gebruiken in team gesprekken</span><span class="sxs-lookup"><span data-stu-id="5164f-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="5164f-103">Giphy's toegang in teams-chat is standaard ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="5164f-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="5164f-104">Als beheerder kunt u bepalen of Giphy's beschikbaar zijn voor gebruikers door [een berichten beleid](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) in te stellen en ervoor te zorgen dat **giphy's gebruiken in gesprekken** is **ingeschakeld**.</span><span class="sxs-lookup"><span data-stu-id="5164f-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="5164f-105">Als Gif's niet werken zoals verwacht in team gesprekken, controleert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="5164f-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="5164f-106">Voor het [bericht beleid](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) moet giphy's zijn toegestaan.</span><span class="sxs-lookup"><span data-stu-id="5164f-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="5164f-107">Verificatie via PowerShell-cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5164f-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="5164f-108">Ga na of u [teams kunt beheren met PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="5164f-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="5164f-109">Voer de PowerShell-opdracht [Get-CsTeamsMessagingPolicy-Identity globaal](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) uit en controleer of **AllowGiphy** is ingesteld op **waar**.</span><span class="sxs-lookup"><span data-stu-id="5164f-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="5164f-110">Als **AllowGiphy** is ingesteld op **False** , voert u de volgende opdracht uit voor de PowerShell-opdrachtenset [-CsTeamsMessagingPolicy-Identity globaal-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="5164f-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="5164f-111">U kunt de URL van de Giphy alleen gebruiken als u [optionele verbonden ervaring](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) hebt ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="5164f-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="5164f-112">Als u meerdere teams-berichten beleidsregels hebt geconfigureerd voor uw Tenant, kunt u de identiteit bepalen van het beleid dat is toegewezen aan de gebruiker die de gebruiker heeft beïnvloed met de opdracht [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selecteer TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="5164f-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
