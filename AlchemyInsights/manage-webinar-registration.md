---
title: Webinarregistratie beheren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793710"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="96a1f-102">Webinarregistratie beheren</span><span class="sxs-lookup"><span data-stu-id="96a1f-102">Manage webinar registration</span></span>

<span data-ttu-id="96a1f-103">U beheert wie zich kan registreren voor Teams webinars met behulp Teams PowerShell-opdrachten.</span><span class="sxs-lookup"><span data-stu-id="96a1f-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="96a1f-104">Als u Teams Powershell wilt installeren, [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="96a1f-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="96a1f-105">*WhoCanRegister* is standaard ingeschakeld en ingesteld op **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="96a1f-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="96a1f-106">Als u wilt dat iedereen, inclusief anonieme gebruikers, zich kan registreren, moet u het vergaderingsbeleid instellen op **Iedereen** met de powershell-opdracht:</span><span class="sxs-lookup"><span data-stu-id="96a1f-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="96a1f-107">**Opmerking:** Als anoniem deelnemen is uitgeschakeld in vergaderingsinstellingen, kunnen anonieme gebruikers niet deelnemen aan webinars.</span><span class="sxs-lookup"><span data-stu-id="96a1f-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="96a1f-108">Zie Vergaderingsinstellingen beheren in Microsoft Teams voor meer informatie en deze [instelling in Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="96a1f-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="96a1f-109">Als u de registratie van vergaderingen wilt uitschakelen, stelt *u AllowMeetingRegistration in* op **Onwaar.**</span><span class="sxs-lookup"><span data-stu-id="96a1f-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="96a1f-110">Zie Configureren wie zich kan registreren voor webinars voor meer informatie over het configureren van wie zich kan [registreren voor webinars.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="96a1f-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="96a1f-111">Zie Besturingselementinstellingen voor Microsoft-lijsten voor meer informatie over instellingen voor [Microsoft-lijsten.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="96a1f-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
