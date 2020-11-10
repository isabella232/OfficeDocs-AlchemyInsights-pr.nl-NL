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
# <a name="using-giphys-in-teams-conversations"></a>Giphy's gebruiken in team gesprekken

Giphy's toegang in teams-chat is standaard ingeschakeld. Als beheerder kunt u bepalen of Giphy's beschikbaar zijn voor gebruikers door [een berichten beleid](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) in te stellen en ervoor te zorgen dat **giphy's gebruiken in gesprekken** is **ingeschakeld**.

Als Gif's niet werken zoals verwacht in team gesprekken, controleert u het volgende:

Voor het [bericht beleid](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) moet giphy's zijn toegestaan. Verificatie via PowerShell-cmdlets:

- Ga na of u [teams kunt beheren met PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Voer de PowerShell-opdracht [Get-CsTeamsMessagingPolicy-Identity globaal](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) uit en controleer of **AllowGiphy** is ingesteld op **waar**.
- Als **AllowGiphy** is ingesteld op **False** , voert u de volgende opdracht uit voor de PowerShell-opdrachtenset [-CsTeamsMessagingPolicy-Identity globaal-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

U kunt de URL van de Giphy alleen gebruiken als u [optionele verbonden ervaring](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) hebt ingeschakeld.

> [!NOTE]
> Als u meerdere teams-berichten beleidsregels hebt geconfigureerd voor uw Tenant, kunt u de identiteit bepalen van het beleid dat is toegewezen aan de gebruiker die de gebruiker heeft beïnvloed met de opdracht [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selecteer TeamsMessagingPolicy.
