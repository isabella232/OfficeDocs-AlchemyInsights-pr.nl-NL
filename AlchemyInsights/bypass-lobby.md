---
title: Lobby omzeilen
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820029"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Lobbyinstellingen en deelnameniveau in Teams beheren

Als u wilt toestaan dat iedereen, inclusief inbelgebruikers, externe en anonieme gebruikers, de **lobby** overzeilt, gebruikt u PowerShell om deze taak uit te voeren. Hier volgen een voorbeeld van het wijzigen van het algemene vergaderingsbeleid voor uw organisatie.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Deze cmdlet vereist momenteel het gebruik van de Skype voor Bedrijven PowerShell-module. Als u deze cmdlet wilt gebruiken, raadpleegt u Beleid [beheren via PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Nadat u een beleid hebt ingesteld, moet u dit toepassen op gebruikers. of, als u het algemene beleid hebt gewijzigd, wordt dit automatisch toegepast op gebruikers. Voor een beleidswijziging moet u ten minste 4 uur tot **24** uur wachten voordat het beleid van kracht wordt. 

Controleer de documentatie hieronder voordat u deze wijzigingen aan gaat brengen om precies te begrijpen wat dit toestaat.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Besturingselementen voor lobbybeleid van Teams-vergadering

Deze instellingen bepalen welke deelnemers aan de vergadering in de lobby wachten voordat ze worden toegelaten tot de vergadering en het niveau van deelname dat ze aan een vergadering mogen deelnemen. U kunt PowerShell gebruiken om instellingen voor vergaderingsbeleid bij te werken die nog niet zijn geïmplementeerd (met het label 'binnenkort beschikbaar') in het Teams-beheercentrum. Zie hieronder een voorbeeld van PowerShell-cmdlet waarmee alle gebruikers de lobby kunnen omzeilen.

- [Personen automatisch toelaten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is een beleid per organisator dat bepaalt of personen rechtstreeks deelnemen aan een vergadering of wachten in de lobby totdat ze worden toegelaten door een geverifieerde gebruiker.

- [Anonieme personen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) toestaan een vergadering te starten is een beleid per organisator dat bepaalt of anonieme personen, waaronder B2B en federatief gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder een geverifieerde gebruiker van de organisatie die aanwezig is.

- [Toestaan dat inbelgebruikers](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) de lobby (binnenkort) omzeilen, is een beleid per organisator dat bepaalt of personen die via  de telefoon inbellen, rechtstreeks deelnemen aan de vergadering of wachten in de lobby, ongeacht de instelling Personen automatisch toelaten.

- Organisatoren toestaan lobby-instellingen te overschrijven [(binnenkort](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **beschikbaar)** is een beleid per organisator dat bepaalt of de organisator van de vergadering de lobbyinstellingen kan overschrijven die door een beheerder **zijn** ingesteld in Automatisch personen toestaan en inbelgebruikers toestaan de **lobby** te omzeilen wanneer ze een nieuwe vergadering plannen.

**Opmerking:** Lees [Vergaderbeleid beheren in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van het vergaderbeleid van Microsoft Teams.
