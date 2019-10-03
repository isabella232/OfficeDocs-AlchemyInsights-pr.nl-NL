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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376597"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Controle lobby instellingen en participatiegraad

Deze instellingen bepalen welke deelnemers aan de vergadering in de lobby wachten voordat ze worden toegelaten tot de vergadering en de mate van deelname die ze in een vergadering hebben toegestaan. U PowerShell gebruiken voor het bijwerken van vergadering beleidsinstellingen die nog niet zijn geïmplementeerd (met het label ' binnenkort beschikbaar ') in het Beheercentrum voor teams.  Zie hieronder voor een voorbeeld PowerShell-cmdlet waarmee alle gebruikers de lobby omzeilen.  

- [Automatisch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) toestaan dat mensen is een per-Organizer-beleid dat bepaalt of mensen rechtstreeks deelnemen aan een vergadering of wachten in de lobby totdat ze zijn toegestaan door een geverifieerde gebruiker.

- [Toestaan dat anonieme mensen een vergadering starten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is een beleid per organisator dat bepaalt of anonieme personen, met inbegrip van B2B-en federatieve gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder een geverifieerde gebruiker van de organisatie in aanwezigheid.

- [Inbelgebruikers toestaan om de lobby te omzeilen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**binnenkort beschikbaar**) is een beleid per organisator dat bepaalt of mensen die inbellen via de telefoon rechtstreeks deelnemen aan de vergadering of in de lobby wachten, ongeacht de instelling **mensen automatisch laten toegeven** .

- [Organisatoren toestaan om de instellingen van de lobby te negeren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (binnenkort**beschikbaar**) is een per-Organizer-beleid dat bepaalt of de organisator van de vergadering de lobby-instellingen kan overschrijven die een beheerder heeft ingesteld in **automatisch mensen toelaten** en **Inbellen toestaan gebruikers de lobby omzeilen** wanneer ze een nieuwe vergadering plannen.

**Opmerking:** Lees [beleid voor vergadering beheren in teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van Microsoft-teams vergadering beleid. 


**PowerShell-voorbeeld**

Als u wilt toestaan dat iedereen, met inbegrip van externe of anonieme gebruikers, voor het omzeilen van de lobby, u ook PowerShell gebruiken om deze taak te voltooien.  Hier is een voorbeeld van het wijzigen van het algemene vergaderings beleid voor uw organisatie.   

(Controleer de bovenstaande documentatie voordat u deze wijzigingen aanbrengt om precies te begrijpen wat dit toelaat.)

Set-CsTeamsMeetingPolicy-Identity Global-Autotoetedusers "iedereen"-AllowPSTNUsersToBypassLobby $True

Zie voor meer informatie, [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
