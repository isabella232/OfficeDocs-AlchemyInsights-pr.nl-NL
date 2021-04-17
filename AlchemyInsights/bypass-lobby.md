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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="15c35-102">Lobbyinstellingen en deelnameniveau in Teams beheren</span><span class="sxs-lookup"><span data-stu-id="15c35-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="15c35-103">Als u wilt toestaan dat iedereen, inclusief inbelgebruikers, externe en anonieme gebruikers, de **lobby** overzeilt, gebruikt u PowerShell om deze taak uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="15c35-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="15c35-104">Hier volgen een voorbeeld van het wijzigen van het algemene vergaderingsbeleid voor uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="15c35-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="15c35-105">Deze cmdlet vereist momenteel het gebruik van de Skype voor Bedrijven PowerShell-module.</span><span class="sxs-lookup"><span data-stu-id="15c35-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="15c35-106">Als u deze cmdlet wilt gebruiken, raadpleegt u Beleid [beheren via PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="15c35-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="15c35-107">Nadat u een beleid hebt ingesteld, moet u dit toepassen op gebruikers. of, als u het algemene beleid hebt gewijzigd, wordt dit automatisch toegepast op gebruikers.</span><span class="sxs-lookup"><span data-stu-id="15c35-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="15c35-108">Voor een beleidswijziging moet u ten minste 4 uur tot **24** uur wachten voordat het beleid van kracht wordt.</span><span class="sxs-lookup"><span data-stu-id="15c35-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="15c35-109">Controleer de documentatie hieronder voordat u deze wijzigingen aan gaat brengen om precies te begrijpen wat dit toestaat.</span><span class="sxs-lookup"><span data-stu-id="15c35-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="15c35-110">Besturingselementen voor lobbybeleid van Teams-vergadering</span><span class="sxs-lookup"><span data-stu-id="15c35-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="15c35-111">Deze instellingen bepalen welke deelnemers aan de vergadering in de lobby wachten voordat ze worden toegelaten tot de vergadering en het niveau van deelname dat ze aan een vergadering mogen deelnemen.</span><span class="sxs-lookup"><span data-stu-id="15c35-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="15c35-112">U kunt PowerShell gebruiken om instellingen voor vergaderingsbeleid bij te werken die nog niet zijn geïmplementeerd (met het label 'binnenkort beschikbaar') in het Teams-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="15c35-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="15c35-113">Zie hieronder een voorbeeld van PowerShell-cmdlet waarmee alle gebruikers de lobby kunnen omzeilen.</span><span class="sxs-lookup"><span data-stu-id="15c35-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="15c35-114">[Personen automatisch toelaten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is een beleid per organisator dat bepaalt of personen rechtstreeks deelnemen aan een vergadering of wachten in de lobby totdat ze worden toegelaten door een geverifieerde gebruiker.</span><span class="sxs-lookup"><span data-stu-id="15c35-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="15c35-115">[Anonieme personen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) toestaan een vergadering te starten is een beleid per organisator dat bepaalt of anonieme personen, waaronder B2B en federatief gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder een geverifieerde gebruiker van de organisatie die aanwezig is.</span><span class="sxs-lookup"><span data-stu-id="15c35-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="15c35-116">[Toestaan dat inbelgebruikers](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) de lobby (binnenkort) omzeilen, is een beleid per organisator dat bepaalt of personen die via  de telefoon inbellen, rechtstreeks deelnemen aan de vergadering of wachten in de lobby, ongeacht de instelling Personen automatisch toelaten.</span><span class="sxs-lookup"><span data-stu-id="15c35-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="15c35-117">Organisatoren toestaan lobby-instellingen te overschrijven [(binnenkort](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **beschikbaar)** is een beleid per organisator dat bepaalt of de organisator van de vergadering de lobbyinstellingen kan overschrijven die door een beheerder **zijn** ingesteld in Automatisch personen toestaan en inbelgebruikers toestaan de **lobby** te omzeilen wanneer ze een nieuwe vergadering plannen.</span><span class="sxs-lookup"><span data-stu-id="15c35-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="15c35-118">**Opmerking:** Lees [Vergaderbeleid beheren in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van het vergaderbeleid van Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="15c35-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
