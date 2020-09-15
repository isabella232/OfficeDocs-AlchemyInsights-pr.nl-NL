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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="c9726-102">De lobby-instellingen en het niveau van deelname aan teams beheren</span><span class="sxs-lookup"><span data-stu-id="c9726-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="c9726-103">Als u iedereen wilt toestaan, waaronder inbelverbindingen, externe gebruikers en anonieme gebruikers, kunt u dit voor **komen door Power**shell te gebruiken om deze taak uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="c9726-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="c9726-104">Hier ziet u een voorbeeld van het wijzigen van het globale beleid voor vergaderingen voor uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="c9726-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="c9726-105">Voor deze cmdlet is momenteel het gebruik van de Skype voor bedrijven PowerShell-module vereist.</span><span class="sxs-lookup"><span data-stu-id="c9726-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="c9726-106">Als u deze cmdlet wilt instellen voor het gebruik van deze cmdlet, raadpleegt u [beleid beheren via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="c9726-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="c9726-107">Wanneer u de beleidsregels hebt ingesteld, moet u deze op gebruikers toepassen. Als u het globale beleid hebt gewijzigd, wordt dit automatisch op gebruikers toegepast.</span><span class="sxs-lookup"><span data-stu-id="c9726-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="c9726-108">Voor elke beleidswijziging moet u minimaal **4 uur tot 24 uur** lang wachten voordat de beleidsregels van kracht worden.</span><span class="sxs-lookup"><span data-stu-id="c9726-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="c9726-109">Lees de onderstaande documentatie voordat u deze wijzigingen aanbrengt in de onderstaande documentatie voordat u ze precies begrijpt wat dit toestaat.</span><span class="sxs-lookup"><span data-stu-id="c9726-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="c9726-110">Meer informatie over de besturingselementen van het team van de teamvergadering</span><span class="sxs-lookup"><span data-stu-id="c9726-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="c9726-111">Met deze instellingen wordt bepaald welke deelnemers aan de vergadering wachten voordat ze worden toegelaten tot de vergadering en het niveau van deelname aan een vergadering.</span><span class="sxs-lookup"><span data-stu-id="c9726-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="c9726-112">U kunt PowerShell gebruiken voor het bijwerken van de beleidsinstellingen voor vergaderingen die nog niet zijn geïmplementeerd (met het label ' binnenkort beschikbaar ') in het Beheercentrum van teams.</span><span class="sxs-lookup"><span data-stu-id="c9726-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="c9726-113">Zie hieronder voor een voorbeeld van een PowerShell-cmdlet waarmee alle gebruikers de lobby kunnen overslaan.</span><span class="sxs-lookup"><span data-stu-id="c9726-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="c9726-114">[Personen automatisch toelaten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is een beleid per beheerder waarmee wordt bepaald of personen rechtstreeks deelnemen aan een vergadering of in de lobby wachten totdat ze worden toegelaten door een geverifieerde gebruiker.</span><span class="sxs-lookup"><span data-stu-id="c9726-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="c9726-115">[Anonieme personen toestaan een vergadering te starten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is een beleid op basis van een beheerder waarmee wordt bepaald of anonieme gebruikers, waaronder B2B en federatieve gebruikers, kunnen deelnemen aan de vergadering van de gebruiker zonder geverifieerde gebruiker van de organisatie in aanwezigheid.</span><span class="sxs-lookup"><span data-stu-id="c9726-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="c9726-116">[Toestaan dat inbelgebruikers de lobby overslaan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**binnenkort**beschikbaar) is een beleidsregels van een beheerder waarmee wordt bepaald of personen die per telefoon inbellen bij de vergadering rechtstreeks of in de lobby wachten, ongeacht de instelling **personen automatisch toelaten** .</span><span class="sxs-lookup"><span data-stu-id="c9726-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="c9726-117">Organisatoren [toestaan de lobby-instellingen te negeren](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**binnenkort**beschikbaar) is een beleidsregels van een beheerder waarmee wordt bepaald of de organisator van de vergadering de instellingen voor de lobby kan overschrijven die een beheerder heeft ingesteld in het **automatisch toelaten** van gebruikers en **toestaan dat inbelgebruikers de lobby overslaan** wanneer ze een nieuwe vergadering plannen.</span><span class="sxs-lookup"><span data-stu-id="c9726-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="c9726-118">**Opmerking:** Lees [beleidsregels voor vergadering beheren in teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) voor een volledig overzicht van de Vergader regels van Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="c9726-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
