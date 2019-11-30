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
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627569"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Vergaderings beleid beheren in Microsoft teams

Vergaderings beleid wordt gebruikt om de functies te beheren die beschikbaar zijn om deelnemers te ontmoeten voor vergaderingen die zijn gepland door gebruikers in uw organisatie. Sommige functies van het Vergader beleid kunnen niet worden geïmplementeerd in het Beheercentrum van de teams nog (deze zijn gelabeld "binnenkort" in de documentatie). In dit geval of als u een foutmelding krijgt als ' we kunnen het beleid nu niet bijwerken, maar probeer het later opnieuw ' in het Microsoft-teams Admin Center, wordt u aangeraden PowerShell gebruiken om te maken of wijzigen van beleid voor teams vergadering. 

Zie de volgende bronnen voor meer informatie over het beleid van de vergadering:

- Zie voor meer informatie over het maken van beleid, wijzigingen aanbrengen en toewijzen van gebruikers aan het beleid, [vergadering beleid in teams beheren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Voor het maken van beleidswijzigingen met behulp van PowerShell-cmdlets, Zie [teams PowerShell overzicht](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - U moet de [Skype voor Business PowerShell-module](https://www.microsoft.com/download/details.aspx?id=39366) voor teams vergadering beleid gebruiken. 
    - Lees de [*-csteamsmeetingpolicy cmdlets documentatie](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) voor meer informatie.

**Opmerking:** Het kan tot 24 uur duren voordat beleidswijzigingen van kracht worden voor gebruikers. Het is mogelijk dat u niet onmiddellijk wijzigingen aanbrengen in nieuw gemaakte beleidsregels. Wacht 4 uur en probeer een nieuw gemaakt beleid opnieuw te wijzigen. Als u nog steeds problemen ondervindt, probeert u PowerShell.  