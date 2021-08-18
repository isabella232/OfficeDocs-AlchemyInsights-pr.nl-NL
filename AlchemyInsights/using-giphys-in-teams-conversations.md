---
title: Giphys gebruiken in Teams gesprekken
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323515"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphys gebruiken in Teams gesprekken

Giphys-toegang in Teams chat is standaard ingeschakeld. Als beheerder kunt u bepalen of Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) beschikbaar is voor gebruikers door een berichtenbeleid in te stellen en ervoor te zorgen dat **Giphys gebruiken in gesprekken** is **aan.**

Als GIF's niet werken zoals verwacht in Teams gesprekken, controleert u:

Het [berichtenbeleid](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) moet Giphys toestaan. U kunt dit controleren met behulp van PowerShell-cmdlets:

- Controleer of u uw [Teams met PowerShell kunt beheren.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Voer de [PowerShell-opdracht Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) uit en controleer of **AllowGiphy** is ingesteld op **WAAR.**
- Als **AllowGiphy** is ingesteld op **ONWAAR**, voer dan de volgende PowerShell-opdracht [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Optionele verbonden](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) ervaringen moeten zijn ingeschakeld om toegang tot de GIPHY-URL toe te staan.

**Opmerking:** Als u meerdere Teams Messaging-beleidsregels hebt geconfigureerd voor uw tenant, kunt u de identiteit bepalen van het beleid dat is toegewezen aan de beïnvloede gebruiker met de [PowerShell-opdracht Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selecteer TeamsMessagingPolicy.
