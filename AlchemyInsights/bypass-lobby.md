---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889077"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controle lobby instellingen en participatiegraad in teams

Als u wilt toestaan dat iedereen, met inbegrip van inbellen, externe en anonieme gebruikers, **de lobby omzeilen**, gebruikt u PowerShell om deze taak te voltooien. Hier is een voorbeeld van het wijzigen van het algemene vergaderings beleid voor uw organisatie.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Deze cmdlet vereist momenteel het gebruik van Skype voor Business PowerShell-module. Als u wilt instellen voor het gebruik van deze cmdlet, uitchecken [beheerbeleid via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Nadat u een beleid hebt ingesteld, moet u dit toepassen op gebruikers. Als u het algemene beleid hebt gewijzigd, wordt dit automatisch toegepast op gebruikers. Voor elke beleidswijziging moet u ten minste **4 uur tot 24 uur** wachten voordat het beleid van kracht wordt. 

Controleer de onderstaande documentatie voordat u deze wijzigingen aanbrengt om precies te begrijpen wat dit toestaat.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Informatie over teams die voldoen aan lobbyen voor het beleid

Deze instellingen bepalen welke deelnemers aan de vergadering in de lobby wachten voordat ze worden toegelaten tot de vergadering en de mate van deelname die ze in een vergadering hebben toegestaan. U PowerShell gebruiken voor het bijwerken van vergadering beleidsinstellingen die nog niet zijn geïmplementeerd (met het label ' binnenkort beschikbaar ') in het Beheercentrum voor teams. Zie hieronder voor een voorbeeld PowerShell-cmdlet waarmee alle gebruikers de lobby omzeilen.

- [Automatisch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) toestaan dat mensen is een per-Organizer-beleid dat bepaalt of mensen rechtstreeks deelnemen aan een vergadering of wachten in de lobby totdat ze zijn toegestaan door een geverifieerde gebruiker.

- [Toestaan dat anonieme mensen een vergadering starten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is een beleid per organisator dat bepaalt of anonieme personen, met inbegrip van B2B-en federatieve gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder een geverifieerde gebruiker van de organisatie in aanwezigheid.

- [Inbelgebruikers toestaan om de lobby te omzeilen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**binnenkort beschikbaar**) is een beleid per organisator dat bepaalt of mensen die inbellen via de telefoon rechtstreeks deelnemen aan de vergadering of in de lobby wachten, ongeacht de instelling **mensen automatisch laten toegeven** .

- [Organisatoren toestaan om de instellingen van de lobby te negeren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (binnenkort**beschikbaar**) is een per-Organizer-beleid dat bepaalt of de organisator van de vergadering de lobby-instellingen kan overschrijven die een beheerder heeft ingesteld in **automatisch mensen** **toestaan en inbelgebruikers de lobby laten omzeilen** wanneer ze een nieuwe vergadering plannen.

**Opmerking:** Lees [beleid voor vergadering beheren in teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van Microsoft-teams vergadering beleid.
