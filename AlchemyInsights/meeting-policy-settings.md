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
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Vergaderbeleid beheren in Microsoft Teams

**Opmerking: Het kan tot 24 uur duren voordat beleidswijzigingen voor gebruikers zijn doorgevoerd.** Mogelijk kunt u niet direct wijzigingen aanbrengen in nieuw gemaakte beleidsregels. wacht 4 uur en probeer opnieuw een nieuw beleid te wijzigen.

Vergaderbeleid wordt gebruikt om de functies te bepalen die beschikbaar zijn voor deelnemers aan een vergadering voor vergaderingen die worden gepland door gebruikers in uw organisatie. Sommige functies van vergaderbeleid worden mogelijk nog niet geïmplementeerd in het Teams-beheercentrum (deze hebben het label 'binnenkort beschikbaar' in de documentatie). In dit geval, of als u een foutbericht krijgt zoals 'Het beleid kan momenteel niet worden bijgewerkt, maar probeer het later opnieuw' in het Microsoft Teams-beheercentrum, raden we u aan PowerShell te gebruiken om vergaderbeleid voor Teams te maken of te wijzigen. 

Zie de volgende bronnen voor meer informatie over vergaderbeleid:

- Zie Vergaderbeleid beheren in Teams voor meer informatie over het maken van beleidsregels, het aanbrengen van wijzigingen en het toewijzen van gebruikers [aan het beleid.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Zie Overzicht van [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)als u beleidswijzigingen wilt aanbrengen met behulp van PowerShell-cmdlets. 
    - U moet de Skype voor [Bedrijven PowerShell-module voor](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) vergaderbeleid voor Teams gebruiken. 
    - Lees de [documentatie van de *-CsTeamsMeetingPolicy-cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) voor meer informatie.

