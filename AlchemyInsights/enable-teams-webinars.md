---
title: Webinars Teams inschakelen
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793652"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="3480d-102">Webinars Teams inschakelen</span><span class="sxs-lookup"><span data-stu-id="3480d-102">Enable Teams Webinars</span></span>

<span data-ttu-id="3480d-103">Webinars zijn standaard ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="3480d-103">Webinars are enabled by default.</span></span> <span data-ttu-id="3480d-104">U kunt beheren wie webinars kan plannen en Teams met behulp van Teams PowerShell-opdrachten.</span><span class="sxs-lookup"><span data-stu-id="3480d-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="3480d-105">Alle gebruikers die een vergadering kunnen maken, kunnen ook een webinarvergadering maken.</span><span class="sxs-lookup"><span data-stu-id="3480d-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="3480d-106">Als u wilt beheren wie de webinars Teams plannen, gebruikt *u AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="3480d-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="3480d-107">*WhoCanRegister* is standaard ingeschakeld en ingesteld op **Iedereen.**</span><span class="sxs-lookup"><span data-stu-id="3480d-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="3480d-108">Als u de registratie van vergaderingen wilt uitschakelen, stelt *u AllowMeetingRegistration in* op **Onwaar.**</span><span class="sxs-lookup"><span data-stu-id="3480d-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="3480d-109">Als u deze instellingen wilt wijzigen, moet u Teams [PowerShell installeren.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="3480d-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="3480d-110">Vergaderbeleid wordt ook afgedwongen op Teams webinars.</span><span class="sxs-lookup"><span data-stu-id="3480d-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="3480d-111">Als anonieme join bijvoorbeeld is uitgeschakeld in vergaderingsinstellingen, kunnen anonieme gebruikers niet deelnemen aan webinars.</span><span class="sxs-lookup"><span data-stu-id="3480d-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="3480d-112">Zie Configureren wie zich kan registreren voor webinars voor meer informatie over het configureren van wie zich kan [registreren voor webinars.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="3480d-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="3480d-113">Zie Besturingselementinstellingen voor Microsoft-lijsten voor meer informatie over instellingen voor [Microsoft-lijsten.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="3480d-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>