---
title: Beleidsinstellingen voor vergadering
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825438"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Vergaderbeleid beheren in Microsoft Teams

**Opmerking: Het kan tot 24 uur duren voordat beleidswijzigingen van kracht worden voor gebruikers.** Mogelijk kunt u niet direct wijzigingen aanbrengen in nieuw gemaakte beleidsregels. wacht 4 uur en probeer een nieuw gemaakt beleid opnieuw te wijzigen.

Vergaderbeleid wordt gebruikt om de functies te bepalen die beschikbaar zijn voor deelnemers aan vergaderingen die zijn gepland door gebruikers in uw organisatie. Sommige functies van vergaderingsbeleid worden mogelijk nog niet geïmplementeerd in het Teams-beheercentrum (deze worden in de documentatie aangeduid als 'binnenkort beschikbaar'). In dit geval, of als u een foutmelding krijgt zoals 'We kunnen het beleid nu niet bijwerken, maar het later opnieuw proberen' in het Microsoft Teams-beheercentrum, raden we u aan PowerShell te gebruiken om teamsvergaderingsbeleid te maken of te wijzigen. 

Zie de volgende bronnen voor meer informatie over vergaderbeleid:

- Zie Vergaderbeleid beheren in Teams voor meer informatie over het maken van beleidsregels, het aanbrengen van wijzigingen en het toewijzen van [gebruikers aan het beleid.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Zie Overzicht van [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)als u beleidswijzigingen wilt aanbrengen met behulp van PowerShell-cmdlets. 
    - U moet de [Skype voor Bedrijven PowerShell-module voor](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) teams-vergaderbeleid gebruiken. 
    - Bekijk de [*-CsTeamsMeetingPolicy-cmdlets-documentatie](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) voor meer informatie.

