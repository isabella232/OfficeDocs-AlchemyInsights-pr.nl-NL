---
title: Zoeken in SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059247"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="df246-102">Zoeken in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="df246-102">Search in SharePoint Online</span></span>

<span data-ttu-id="df246-103">Inhoud moet worden verkend en toegevoegd aan de zoekindex kunnen vinden wat ze zoekt in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="df246-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="df246-104">Inhoud wordt automatisch verkend op basis van een vooraf gedefinieerde verkenningsschema (de planning voor verkenning kan niet worden gewijzigd).</span><span class="sxs-lookup"><span data-stu-id="df246-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="df246-105">Inhoud die is gewijzigd sinds de laatste verkenning en werkt de index hervat de crawler.</span><span class="sxs-lookup"><span data-stu-id="df246-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="df246-106">Houd rekening met de volgende inhoud wordt verkend en de index wordt bijgewerkt, zodat:</span><span class="sxs-lookup"><span data-stu-id="df246-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="df246-107">Zorg ervoor dat de inhoud kan worden gevonden door [doorzoekbare inhoud van de site](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="df246-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="df246-108">Wanneer u een beheerde eigenschap hebt gewijzigd, of wanneer u de toewijzing van hebt gewijzigd verkend en beheerde moet eigenschappen voor de site opnieuw verkende voordat uw wijzigingen worden weergegeven in de zoekindex.</span><span class="sxs-lookup"><span data-stu-id="df246-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="df246-109">Omdat uw wijzigingen worden aangebracht in het zoekschema en niet op de werkelijke locatie, wordt de crawler niet automatisch opnieuw indexeren de site.</span><span class="sxs-lookup"><span data-stu-id="df246-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="df246-110">Zie [handmatig verkennen en opnieuw indexeren van een site, een bibliotheek of een lijst met aanvragen](https://docs.microsoft.com/sharepoint/crawl-site-conten)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="df246-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="df246-111">Wacht ten minste 24 uur na het handmatig starten van een verkenning en volledig opnieuw indexeren bekijken als u steeds een probleem ondervindt.</span><span class="sxs-lookup"><span data-stu-id="df246-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="df246-112">Als u meer dan 24 uur zijn verstreken sinds u de verkenning en volledig opnieuw indexeren gestart, meld u een aanvraag voor ondersteuning.</span><span class="sxs-lookup"><span data-stu-id="df246-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="df246-113">In veel gevallen hebben werkt we aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="df246-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="df246-114">Geef ons ten minste 24 uur om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="df246-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Belangrijk!]<span data-ttu-id="df246-115">: als een site, een document (bibliotheek) of een lijst verwijderd en nog steeds wordt getoond in de zoekresultaten is, moeten ontvangen gebruikers een **Foutbericht 404 bestand niet gevonden** wanneer u probeert toegang te krijgen tot deze.</span><span class="sxs-lookup"><span data-stu-id="df246-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="df246-116">Dit probleem moet zijn aangemeld als een aanvraag voor ondersteuning voor verder onderzoek.</span><span class="sxs-lookup"><span data-stu-id="df246-116">This issue should be logged as a support case for further investigation.</span></span> 



