---
title: Lobby overslaan
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684945"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>De lobby-instellingen en het niveau van deelname aan teams beheren

Als u iedereen wilt toestaan, waaronder inbelverbindingen, externe gebruikers en anonieme gebruikers, kunt u dit voor **komen door Power**shell te gebruiken om deze taak uit te voeren. Hier ziet u een voorbeeld van het wijzigen van het globale beleid voor vergaderingen voor uw organisatie.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Voor deze cmdlet is momenteel het gebruik van de Skype voor bedrijven PowerShell-module vereist. Als u deze cmdlet wilt instellen voor het gebruik van deze cmdlet, raadpleegt u [beleid beheren via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Wanneer u de beleidsregels hebt ingesteld, moet u deze op gebruikers toepassen. Als u het globale beleid hebt gewijzigd, wordt dit automatisch op gebruikers toegepast. Voor elke beleidswijziging moet u minimaal **4 uur tot 24 uur** lang wachten voordat de beleidsregels van kracht worden. 

Lees de onderstaande documentatie voordat u deze wijzigingen aanbrengt in de onderstaande documentatie voordat u ze precies begrijpt wat dit toestaat.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Meer informatie over de besturingselementen van het team van de teamvergadering

Met deze instellingen wordt bepaald welke deelnemers aan de vergadering wachten voordat ze worden toegelaten tot de vergadering en het niveau van deelname aan een vergadering. U kunt PowerShell gebruiken voor het bijwerken van de beleidsinstellingen voor vergaderingen die nog niet zijn geïmplementeerd (met het label ' binnenkort beschikbaar ') in het Beheercentrum van teams. Zie hieronder voor een voorbeeld van een PowerShell-cmdlet waarmee alle gebruikers de lobby kunnen overslaan.

- [Personen automatisch toelaten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is een beleid per beheerder waarmee wordt bepaald of personen rechtstreeks deelnemen aan een vergadering of in de lobby wachten totdat ze worden toegelaten door een geverifieerde gebruiker.

- [Anonieme personen toestaan een vergadering te starten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is een beleid op basis van een beheerder waarmee wordt bepaald of anonieme gebruikers, waaronder B2B en federatieve gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder geverifieerde gebruiker van de organisatie in aanwezigheid.

- [Toestaan dat inbelgebruikers de lobby overslaan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**binnenkort**beschikbaar) is een beleidsregels van een beheerder waarmee wordt bepaald of personen die per telefoon inbellen bij de vergadering rechtstreeks of in de lobby wachten, ongeacht de instelling **personen automatisch toelaten** .

- Organisatoren [toestaan de lobby-instellingen te negeren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**binnenkort**beschikbaar) is een beleidsregels van een beheerder waarmee wordt bepaald of de organisator van de vergadering de instellingen voor de lobby kan overschrijven die een beheerder heeft ingesteld in het **automatisch toelaten** van gebruikers en **toestaan dat inbelgebruikers de lobby overslaan** wanneer ze een nieuwe vergadering plannen.

**Opmerking:** Lees [beleidsregels voor vergadering beheren in teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van de Vergader regels van Microsoft teams.
