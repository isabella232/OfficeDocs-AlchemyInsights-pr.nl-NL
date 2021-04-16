---
title: Aan de slag met live evenementen van Teams
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
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811955"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="f30d7-102">Aan de slag met live evenementen van Teams</span><span class="sxs-lookup"><span data-stu-id="f30d7-102">Getting started with Teams live events</span></span>

<span data-ttu-id="f30d7-103">Live-evenementen van Microsoft Teams zijn een uitbreiding van Teams-vergaderingen waarmee u evenementen kunt plannen en produceren die naar een groot online publiek kunnen worden gestreamd.</span><span class="sxs-lookup"><span data-stu-id="f30d7-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="f30d7-104">Om een live evenement te maken, heb je het volgende nodig:</span><span class="sxs-lookup"><span data-stu-id="f30d7-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="f30d7-105">Bevestig eerst dat Teams Live Evenementen [beschikbaar is in uw land en regio](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Eventementen worden in sommige landen/regio's nog niet ondersteund.</span><span class="sxs-lookup"><span data-stu-id="f30d7-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="f30d7-106">Als u licenties toegewezen heeft en een beleid heeft ingesteld, en u kunt nog steeds geen Teams Live Eventementen maken, dan is Live Evenementen waarschijnlijk nog niet beschikbaar in uw land of regio.</span><span class="sxs-lookup"><span data-stu-id="f30d7-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="f30d7-107">Een [ Office 365 Enterprise E1-, E3- of E5-licentie of een Office 365 A3- of A5-licentie ](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="f30d7-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="f30d7-108">**Let op**: vanwege een recente toename van het Teams-gebruik, kan het ongeveer 24 uur duren voordat u een Teams-licentie aan een gebruiker toewijst voordat deze volledig is ingesteld.</span><span class="sxs-lookup"><span data-stu-id="f30d7-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="f30d7-109">Tot die tijd kunt u hen geen Teams-beleid toewijzen en hebben ze mogelijk geen toegang tot bepaalde Teams-functies zoals bellen en audioconferenties.</span><span class="sxs-lookup"><span data-stu-id="f30d7-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="f30d7-110">Toestemming om [ live evenementen te maken in het Microsoft Teams-beheercentrum ](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="f30d7-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="f30d7-111">Toestemming om [ live-evenementen te maken in Microsoft Stream ](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (voor evenementen die zijn geproduceerd met een externe uitzendapp of apparaat).</span><span class="sxs-lookup"><span data-stu-id="f30d7-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="f30d7-112">Volledig teamlidmaatschap in de organisatie (kan geen gast zijn of van een andere organisatie).</span><span class="sxs-lookup"><span data-stu-id="f30d7-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="f30d7-113">Planning van privévergaderingen, screensharing en delen van IP-video's is ingeschakeld in het beleid voor teamvergaderingen.</span><span class="sxs-lookup"><span data-stu-id="f30d7-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="f30d7-114">[Aanbevolen procedures](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) voor teams en kanalen.</span><span class="sxs-lookup"><span data-stu-id="f30d7-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="f30d7-115">Zie [ Aan de slag met live-evenementen van Microsoft Teams ](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f30d7-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>