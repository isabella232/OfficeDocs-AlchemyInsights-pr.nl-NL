---
title: Zoeken in SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044038"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="b885c-102">Inhoud crawlen en indexeren in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b885c-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="b885c-103">Inhoud moet worden verkend en toegevoegd aan de zoekindex voor gebruikers om te vinden waarnaar ze zoeken in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b885c-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="b885c-104">De inhoud wordt automatisch gecrawld op basis van een vooraf gedefinieerd verkennings schema (het verkennings schema kan niet worden gewijzigd).</span><span class="sxs-lookup"><span data-stu-id="b885c-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="b885c-105">De crawler haalt inhoud op die sinds de laatste verkenning is gewijzigd en werkt de index bij.</span><span class="sxs-lookup"><span data-stu-id="b885c-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="b885c-106">Let op het volgende om ervoor te zorgen dat de inhoud wordt verkend en de index wordt bijgewerkt:</span><span class="sxs-lookup"><span data-stu-id="b885c-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="b885c-107">Zorg ervoor dat inhoud kan worden gevonden door [site-inhoud doorzoekbaar te maken](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b885c-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="b885c-108">Wanneer u een beheerde eigenschap hebt gewijzigd of als u de toewijzing van verkende en beheerde eigenschappen hebt gewijzigd, moet de site opnieuw worden verkend voordat de wijzigingen worden doorgevoerd in de zoekindex.</span><span class="sxs-lookup"><span data-stu-id="b885c-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="b885c-109">Omdat uw wijzigingen worden aangebracht in het zoekschema en niet op de werkelijke site, wordt de site niet automatisch opnieuw geïndexeerd door de crawler.</span><span class="sxs-lookup"><span data-stu-id="b885c-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="b885c-110">Zie voor meer informatie [handmatig crawlen en opnieuw indexeren van een site, een bibliotheek of een lijst aanvragen](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="b885c-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="b885c-111">Wacht ten minste 24 uur na het handmatig aanvragen van een crawl en volledige re-index om te zien of u nog steeds een probleem ondervindt.</span><span class="sxs-lookup"><span data-stu-id="b885c-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="b885c-112">Als er meer dan 24 uur zijn verstreken sinds u de verkenning en volledige re-index hebt gestart, meldt u een ondersteuningsaanvraag.</span><span class="sxs-lookup"><span data-stu-id="b885c-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="b885c-113">In veel gevallen werken we nu al aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="b885c-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b885c-114">Gelieve ons ten minste 24 uur te geven om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="b885c-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b885c-115">Als een site, document (bibliotheek) of een lijst is verwijderd en nog steeds wordt weergegeven in de zoekresultaten, moeten gebruikers een **fout 404-bestand** ontvangen dat niet is gevonden wanneer u toegang probeert te krijgen.</span><span class="sxs-lookup"><span data-stu-id="b885c-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="b885c-116">Dit probleem moet worden vastgelegd als een ondersteuningsaanvraag voor verder onderzoek.</span><span class="sxs-lookup"><span data-stu-id="b885c-116">This issue should be logged as a support case for further investigation.</span></span> 



