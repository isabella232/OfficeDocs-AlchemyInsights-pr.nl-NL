---
title: Fouten bij het maken van livegebeurtenissen in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825510"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="02e12-102">Fouten bij het maken van livegebeurtenissen in Yammer</span><span class="sxs-lookup"><span data-stu-id="02e12-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="02e12-103">**Yammer-livegebeurtenissen maken**</span><span class="sxs-lookup"><span data-stu-id="02e12-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="02e12-104">De optie voor het maken van een livegebeurtenis, wanneer dan ook, wordt door Yammer getoond.</span><span class="sxs-lookup"><span data-stu-id="02e12-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="02e12-105">In sommige gevallen is het mogelijk dat een gebruiker niet voldoet aan de vereisten voor het maken van een livegebeurtenis en dat er een foutbericht wordt weergegeven wanneer hiertoe een poging wordt gedaan.</span><span class="sxs-lookup"><span data-stu-id="02e12-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="02e12-106">De onderstaande punten beschrijven gangbare redenen voor dit probleem en bieden manieren om dit probleem voor gebruikers op te lossen.</span><span class="sxs-lookup"><span data-stu-id="02e12-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="02e12-107">**Wie kunnen livegebeurtenissen maken?**</span><span class="sxs-lookup"><span data-stu-id="02e12-107">**Who can create live events**</span></span>
- <span data-ttu-id="02e12-108">Een Office 365 Enterprise E1-, E3- of E5-licentie of een Office 365 A3- of A5-licentie.</span><span class="sxs-lookup"><span data-stu-id="02e12-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="02e12-109">Toestemming om livegebeurtenissen te maken in het Microsoft Teams-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="02e12-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="02e12-110">Toestemming om livegebeurtenissen te maken in Microsoft Stream (voor gebeurtenissen die zijn geproduceerd met een externe uitzend-app of -apparaat).</span><span class="sxs-lookup"><span data-stu-id="02e12-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="02e12-111">Volledig teamlidmaatschap in de organisatie (geen gasten of personen van een andere organisatie).</span><span class="sxs-lookup"><span data-stu-id="02e12-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="02e12-112">Planning van privévergaderingen, scherm delen en delen van IP-video's, ingeschakeld in het beleid voor teamvergaderingen.</span><span class="sxs-lookup"><span data-stu-id="02e12-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="02e12-113">**Beleid voor het maken van livegebeurtenissen**</span><span class="sxs-lookup"><span data-stu-id="02e12-113">**Live event creation policies**</span></span>

<span data-ttu-id="02e12-114">Yammer volgt de beleidsregels voor livegebeurtenissen die zijn ingesteld in uw Office 365-tenant voor stream.</span><span class="sxs-lookup"><span data-stu-id="02e12-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="02e12-115">Standaard kan iedereen in uw organisatie een livegebeurtenis maken.</span><span class="sxs-lookup"><span data-stu-id="02e12-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="02e12-116">Beheerders kunnen [wijzigingen aanbrengen aan deze instelling, waardoor gebruikers mogelijk geen livegebeurtenis kunnen maken](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="02e12-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="02e12-117">Het is belangrijk om te controleren of gebruikers toestemming hebben voor het maken van livegebeurtenissen als ze een beleidsfout ontvangen.</span><span class="sxs-lookup"><span data-stu-id="02e12-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
