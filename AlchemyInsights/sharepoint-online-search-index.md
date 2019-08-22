---
title: Zoeken in SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507626"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="a10b1-102">Inhoud doorzoeken en te indexeren in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a10b1-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="a10b1-103">Inhoud moet worden verkend en toegevoegd aan de zoekindex kunnen vinden wat ze zoekt in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="a10b1-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="a10b1-104">Inhoud wordt automatisch verkend op basis van een vooraf gedefinieerde verkenningsschema (de planning voor verkenning kan niet worden gewijzigd).</span><span class="sxs-lookup"><span data-stu-id="a10b1-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="a10b1-105">Inhoud die is gewijzigd sinds de laatste verkenning en werkt de index hervat de crawler.</span><span class="sxs-lookup"><span data-stu-id="a10b1-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="a10b1-106">Houd rekening met de volgende inhoud wordt verkend en de index wordt bijgewerkt, zodat:</span><span class="sxs-lookup"><span data-stu-id="a10b1-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="a10b1-107">Zorg ervoor dat de inhoud kan worden gevonden door [doorzoekbare inhoud van de site](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="a10b1-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="a10b1-108">Wanneer u een beheerde eigenschap hebt gewijzigd, of wanneer u de toewijzing van hebt gewijzigd verkend en beheerde moet eigenschappen voor de site opnieuw verkende voordat uw wijzigingen worden weergegeven in de zoekindex.</span><span class="sxs-lookup"><span data-stu-id="a10b1-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="a10b1-109">Omdat uw wijzigingen worden aangebracht in het zoekschema en niet op de werkelijke locatie, wordt de crawler niet automatisch opnieuw indexeren de site.</span><span class="sxs-lookup"><span data-stu-id="a10b1-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="a10b1-110">Zie [handmatig verkennen en opnieuw indexeren van een site, een bibliotheek of een lijst met aanvragen](https://docs.microsoft.com/sharepoint/crawl-site-conten)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="a10b1-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="a10b1-111">Wacht ten minste 24 uur na het handmatig starten van een verkenning en volledig opnieuw indexeren bekijken als u steeds een probleem ondervindt.</span><span class="sxs-lookup"><span data-stu-id="a10b1-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="a10b1-112">Als u meer dan 24 uur zijn verstreken sinds u de verkenning en volledig opnieuw indexeren gestart, meld u een aanvraag voor ondersteuning.</span><span class="sxs-lookup"><span data-stu-id="a10b1-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="a10b1-113">In veel gevallen hebben werkt we aan een oplossing.</span><span class="sxs-lookup"><span data-stu-id="a10b1-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a10b1-114">Geef ons ten minste 24 uur om een oplossing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="a10b1-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a10b1-115">Als een site document (bibliotheek) of een lijst is verwijderd en wordt nog steeds weergegeven in de zoekresultaten moeten ontvangen gebruikers een **Foutbericht 404 bestand niet gevonden** wanneer u probeert te openen.</span><span class="sxs-lookup"><span data-stu-id="a10b1-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="a10b1-116">Dit probleem moet zijn aangemeld als een aanvraag voor ondersteuning voor verder onderzoek.</span><span class="sxs-lookup"><span data-stu-id="a10b1-116">This issue should be logged as a support case for further investigation.</span></span> 



