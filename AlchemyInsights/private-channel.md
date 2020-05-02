---
title: Privékanaal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005433"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="d0210-102">Privékanalen in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d0210-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="d0210-103">Privékanalen is een nieuwe functie in Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d0210-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="d0210-104">Houd er rekening mee dat privékanalen niet kunnen worden geconverteerd vanuit standaardkanalen of vice versa.</span><span class="sxs-lookup"><span data-stu-id="d0210-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="d0210-105">Zie [Privékanalen in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels)voor meer informatie over privékanalen, zoals informatie over [het maken van privékanalen en lidmaatschapen](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) en [sharepoint-sites voor privékanalen.](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)</span><span class="sxs-lookup"><span data-stu-id="d0210-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="d0210-106">**Let op:** Omdat configuratie voor het bewaren van privékanaalberichten nog niet wordt ondersteund, hebben huurders met een bewaarbeleid ingeschakeld niet standaard privékanalen ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="d0210-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="d0210-107">Privékanalen kunnen worden ingeschakeld in het Team-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="d0210-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="d0210-108">Houd er ook rekening mee dat, hoewel het bewaren van privékanaalberichten niet wordt ondersteund, het bewaren van bestanden die worden gedeeld in privékanalen, wordt ondersteund.</span><span class="sxs-lookup"><span data-stu-id="d0210-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="d0210-109">**Heb je een nieuwe teameigenaar nodig?**</span><span class="sxs-lookup"><span data-stu-id="d0210-109">**Need a new team owner?**</span></span>

<span data-ttu-id="d0210-110">Als je eigenaar van je privékanaal vertrekt, kun je via Teams Powershell een nieuwe teameigenaar toevoegen.</span><span class="sxs-lookup"><span data-stu-id="d0210-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="d0210-111">Ga [hier](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) om Teams Powershell te installeren.</span><span class="sxs-lookup"><span data-stu-id="d0210-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="d0210-112">Hier is de cmdlet die u nodig hebt:</span><span class="sxs-lookup"><span data-stu-id="d0210-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="d0210-113">Zie [Teams PowerShell-overzicht](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)voor meer informatie over Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="d0210-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
