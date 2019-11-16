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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768435"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="47b48-102">Controle lobby instellingen en participatiegraad</span><span class="sxs-lookup"><span data-stu-id="47b48-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="47b48-103">Als u wilt toestaan dat iedereen, met inbegrip van inbellen, externe en anonieme gebruikers de lobby in Microsoft-teams omzeilen, u PowerShell gebruiken om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="47b48-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="47b48-104">Hier is een voorbeeld van het wijzigen van het algemene vergaderings beleid voor uw organisatie:</span><span class="sxs-lookup"><span data-stu-id="47b48-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="47b48-105">Deze cmdlet vereist momenteel het gebruik van Skype voor Business PowerShell-module.</span><span class="sxs-lookup"><span data-stu-id="47b48-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="47b48-106">Als u wilt instellen voor het gebruik van deze cmdlet, uitchecken [beheerbeleid via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="47b48-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="47b48-107">U een nieuw beleid instellen, dat u vervolgens moet toepassen op gebruikers.</span><span class="sxs-lookup"><span data-stu-id="47b48-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="47b48-108">Als u het algemene beleid wijzigt, wordt dit automatisch toegepast op gebruikers.</span><span class="sxs-lookup"><span data-stu-id="47b48-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="47b48-109">Voor elke beleidswijziging moet u ten minste 4 uur en maximaal 24 uur wachten voordat het beleid van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="47b48-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="47b48-110">Controleer de onderstaande documentatie voordat u deze wijzigingen aanbrengt om precies te begrijpen wat dit toestaat.</span><span class="sxs-lookup"><span data-stu-id="47b48-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="47b48-111">Informatie over teams die voldoen aan lobbyen voor het beleid</span><span class="sxs-lookup"><span data-stu-id="47b48-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="47b48-112">[Automatisch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) toestaan dat mensen is een per-Organizer-beleid dat bepaalt of mensen rechtstreeks deelnemen aan een vergadering of wachten in de lobby totdat ze zijn toegestaan door een geverifieerde gebruiker.</span><span class="sxs-lookup"><span data-stu-id="47b48-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="47b48-113">[Toestaan dat anonieme mensen een vergadering starten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is een beleid per organisator dat bepaalt of anonieme personen, met inbegrip van B2B-en federatieve gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder een geverifieerde gebruiker van de organisatie in aanwezigheid.</span><span class="sxs-lookup"><span data-stu-id="47b48-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="47b48-114">[Inbelgebruikers toestaan om de lobby te omzeilen](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**binnenkort beschikbaar**) is een beleid per organisator dat bepaalt of mensen die inbellen via de telefoon rechtstreeks deelnemen aan de vergadering of in de lobby wachten, ongeacht de instelling **mensen automatisch laten toegeven** .</span><span class="sxs-lookup"><span data-stu-id="47b48-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="47b48-115">[Organisatoren toestaan om de instellingen van de lobby te negeren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (binnenkort**beschikbaar**) is een per-Organizer-beleid dat bepaalt of de organisator van de vergadering de lobby-instellingen kan overschrijven die een beheerder heeft ingesteld in **automatisch mensen** **toestaan en inbelgebruikers de lobby laten omzeilen** wanneer ze een nieuwe vergadering plannen.</span><span class="sxs-lookup"><span data-stu-id="47b48-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="47b48-116">**Opmerking:** Lees [beleid voor vergadering beheren in teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van Microsoft-teams vergadering beleid.</span><span class="sxs-lookup"><span data-stu-id="47b48-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
