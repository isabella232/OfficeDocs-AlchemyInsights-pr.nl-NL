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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="e7f18-102">Controle lobby instellingen en participatiegraad in teams</span><span class="sxs-lookup"><span data-stu-id="e7f18-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="e7f18-103">Als u wilt toestaan dat iedereen, met inbegrip van inbellen, externe en anonieme gebruikers, **de lobby omzeilen**, gebruikt u PowerShell om deze taak te voltooien.</span><span class="sxs-lookup"><span data-stu-id="e7f18-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="e7f18-104">Hier is een voorbeeld van het wijzigen van het algemene vergaderings beleid voor uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="e7f18-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="e7f18-105">Deze cmdlet vereist momenteel het gebruik van Skype voor Business PowerShell-module.</span><span class="sxs-lookup"><span data-stu-id="e7f18-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="e7f18-106">Als u wilt instellen voor het gebruik van deze cmdlet, uitchecken [beheerbeleid via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="e7f18-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="e7f18-107">Nadat u een beleid hebt ingesteld, moet u dit toepassen op gebruikers. Als u het algemene beleid hebt gewijzigd, wordt dit automatisch toegepast op gebruikers.</span><span class="sxs-lookup"><span data-stu-id="e7f18-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="e7f18-108">Voor elke beleidswijziging moet u ten minste **4 uur tot 24 uur** wachten voordat het beleid van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="e7f18-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="e7f18-109">Controleer de onderstaande documentatie voordat u deze wijzigingen aanbrengt om precies te begrijpen wat dit toestaat.</span><span class="sxs-lookup"><span data-stu-id="e7f18-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="e7f18-110">Informatie over teams die voldoen aan lobbyen voor het beleid</span><span class="sxs-lookup"><span data-stu-id="e7f18-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="e7f18-111">Deze instellingen bepalen welke deelnemers aan de vergadering in de lobby wachten voordat ze worden toegelaten tot de vergadering en de mate van deelname die ze in een vergadering hebben toegestaan.</span><span class="sxs-lookup"><span data-stu-id="e7f18-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="e7f18-112">U PowerShell gebruiken voor het bijwerken van vergadering beleidsinstellingen die nog niet zijn geïmplementeerd (met het label ' binnenkort beschikbaar ') in het Beheercentrum voor teams.</span><span class="sxs-lookup"><span data-stu-id="e7f18-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="e7f18-113">Zie hieronder voor een voorbeeld PowerShell-cmdlet waarmee alle gebruikers de lobby omzeilen.</span><span class="sxs-lookup"><span data-stu-id="e7f18-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="e7f18-114">[Automatisch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) toestaan dat mensen is een per-Organizer-beleid dat bepaalt of mensen rechtstreeks deelnemen aan een vergadering of wachten in de lobby totdat ze zijn toegestaan door een geverifieerde gebruiker.</span><span class="sxs-lookup"><span data-stu-id="e7f18-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="e7f18-115">[Toestaan dat anonieme mensen een vergadering starten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is een beleid per organisator dat bepaalt of anonieme personen, met inbegrip van B2B-en federatieve gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder een geverifieerde gebruiker van de organisatie in aanwezigheid.</span><span class="sxs-lookup"><span data-stu-id="e7f18-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="e7f18-116">[Inbelgebruikers toestaan om de lobby te omzeilen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**binnenkort beschikbaar**) is een beleid per organisator dat bepaalt of mensen die inbellen via de telefoon rechtstreeks deelnemen aan de vergadering of in de lobby wachten, ongeacht de instelling **mensen automatisch laten toegeven** .</span><span class="sxs-lookup"><span data-stu-id="e7f18-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="e7f18-117">[Organisatoren toestaan om de instellingen van de lobby te negeren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (binnenkort**beschikbaar**) is een per-Organizer-beleid dat bepaalt of de organisator van de vergadering de lobby-instellingen kan overschrijven die een beheerder heeft ingesteld in **automatisch mensen** **toestaan en inbelgebruikers de lobby laten omzeilen** wanneer ze een nieuwe vergadering plannen.</span><span class="sxs-lookup"><span data-stu-id="e7f18-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="e7f18-118">**Opmerking:** Lees [beleid voor vergadering beheren in teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van Microsoft-teams vergadering beleid.</span><span class="sxs-lookup"><span data-stu-id="e7f18-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
