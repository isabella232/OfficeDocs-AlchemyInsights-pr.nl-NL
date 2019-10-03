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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="30ec9-102">Controle lobby instellingen en participatiegraad</span><span class="sxs-lookup"><span data-stu-id="30ec9-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="30ec9-103">Deze instellingen bepalen welke deelnemers aan de vergadering in de lobby wachten voordat ze worden toegelaten tot de vergadering en de mate van deelname die ze in een vergadering hebben toegestaan.</span><span class="sxs-lookup"><span data-stu-id="30ec9-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="30ec9-104">U PowerShell gebruiken voor het bijwerken van vergadering beleidsinstellingen die nog niet zijn geïmplementeerd (met het label ' binnenkort beschikbaar ') in het Beheercentrum voor teams.</span><span class="sxs-lookup"><span data-stu-id="30ec9-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="30ec9-105">Zie hieronder voor een voorbeeld PowerShell-cmdlet waarmee alle gebruikers de lobby omzeilen.</span><span class="sxs-lookup"><span data-stu-id="30ec9-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="30ec9-106">[Automatisch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) toestaan dat mensen is een per-Organizer-beleid dat bepaalt of mensen rechtstreeks deelnemen aan een vergadering of wachten in de lobby totdat ze zijn toegestaan door een geverifieerde gebruiker.</span><span class="sxs-lookup"><span data-stu-id="30ec9-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="30ec9-107">[Toestaan dat anonieme mensen een vergadering starten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is een beleid per organisator dat bepaalt of anonieme personen, met inbegrip van B2B-en federatieve gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder een geverifieerde gebruiker van de organisatie in aanwezigheid.</span><span class="sxs-lookup"><span data-stu-id="30ec9-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="30ec9-108">[Inbelgebruikers toestaan om de lobby te omzeilen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**binnenkort beschikbaar**) is een beleid per organisator dat bepaalt of mensen die inbellen via de telefoon rechtstreeks deelnemen aan de vergadering of in de lobby wachten, ongeacht de instelling **mensen automatisch laten toegeven** .</span><span class="sxs-lookup"><span data-stu-id="30ec9-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="30ec9-109">[Organisatoren toestaan om de instellingen van de lobby te negeren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (binnenkort**beschikbaar**) is een per-Organizer-beleid dat bepaalt of de organisator van de vergadering de lobby-instellingen kan overschrijven die een beheerder heeft ingesteld in **automatisch mensen toelaten** en **Inbellen toestaan gebruikers de lobby omzeilen** wanneer ze een nieuwe vergadering plannen.</span><span class="sxs-lookup"><span data-stu-id="30ec9-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="30ec9-110">**Opmerking:** Lees [beleid voor vergadering beheren in teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van Microsoft-teams vergadering beleid.</span><span class="sxs-lookup"><span data-stu-id="30ec9-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="30ec9-111">**PowerShell-voorbeeld**</span><span class="sxs-lookup"><span data-stu-id="30ec9-111">**PowerShell example**</span></span>

<span data-ttu-id="30ec9-112">Als u wilt toestaan dat iedereen, met inbegrip van externe of anonieme gebruikers, voor het omzeilen van de lobby, u ook PowerShell gebruiken om deze taak te voltooien.</span><span class="sxs-lookup"><span data-stu-id="30ec9-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="30ec9-113">Hier is een voorbeeld van het wijzigen van het algemene vergaderings beleid voor uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="30ec9-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="30ec9-114">(Controleer de bovenstaande documentatie voordat u deze wijzigingen aanbrengt om precies te begrijpen wat dit toelaat.)</span><span class="sxs-lookup"><span data-stu-id="30ec9-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="30ec9-115">Set-CsTeamsMeetingPolicy-Identity Global-Autotoetedusers "iedereen"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="30ec9-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="30ec9-116">Zie voor meer informatie, [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="30ec9-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
