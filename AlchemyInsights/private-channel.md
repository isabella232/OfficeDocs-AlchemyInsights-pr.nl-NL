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
# <a name="private-channels-in-microsoft-teams"></a>Privékanalen in Microsoft Teams

Privékanalen is een nieuwe functie in Microsoft Teams. Houd er rekening mee dat privékanalen niet kunnen worden geconverteerd vanuit standaardkanalen of vice versa.

Zie [Privékanalen in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels)voor meer informatie over privékanalen, zoals informatie over [het maken van privékanalen en lidmaatschapen](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) en [sharepoint-sites voor privékanalen.](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites) 

**Let op:** Omdat configuratie voor het bewaren van privékanaalberichten nog niet wordt ondersteund, hebben huurders met een bewaarbeleid ingeschakeld niet standaard privékanalen ingeschakeld. Privékanalen kunnen worden ingeschakeld in het Team-beheercentrum. Houd er ook rekening mee dat, hoewel het bewaren van privékanaalberichten niet wordt ondersteund, het bewaren van bestanden die worden gedeeld in privékanalen, wordt ondersteund.

**Heb je een nieuwe teameigenaar nodig?**

Als je eigenaar van je privékanaal vertrekt, kun je via Teams Powershell een nieuwe teameigenaar toevoegen.


- Ga [hier](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) om Teams Powershell te installeren.

Hier is de cmdlet die u nodig hebt:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Zie [Teams PowerShell-overzicht](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)voor meer informatie over Teams Powershell.
