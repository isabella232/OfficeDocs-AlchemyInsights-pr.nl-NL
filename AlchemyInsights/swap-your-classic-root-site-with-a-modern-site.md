---
title: Uw klassieke hoofdsite ruilen met een moderne site
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741539"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="af693-102">Uw klassieke hoofdsite ruilen met een moderne site</span><span class="sxs-lookup"><span data-stu-id="af693-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="af693-103">Als uw omgeving vóór april 2019 is ingesteld, u uw hoofdsite wijzigen in een moderne site met Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="af693-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="af693-104">Als u een andere site hebt die u als hoofdsite wilt gebruiken, u [de hoofdsite erdoor vervangen (ruilen).](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="af693-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="af693-105">Gebruik [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site te ruilen met een andere site terwijl u de oorspronkelijke site archiveert.</span><span class="sxs-lookup"><span data-stu-id="af693-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="af693-106">Beschikbaar voor zowel teamsite (niet verbonden met een groep) als voor communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="af693-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="af693-107">Er worden binnenkort extra mogelijkheden geïntroduceerd waarmee u de inhoud op de site blijven gebruiken, maar de bestaande site converteren naar een communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="af693-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="af693-108">Deze mogelijkheden zullen geleidelijk worden uitgerold.</span><span class="sxs-lookup"><span data-stu-id="af693-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="af693-109">Blijf het Berichtencentrum controleren op updates.</span><span class="sxs-lookup"><span data-stu-id="af693-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="af693-110">Bekende problemen met het verwisselen van sites</span><span class="sxs-lookup"><span data-stu-id="af693-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="af693-111">De doelsite kan een fout 'niet gevonden' (HTTP 404) voor een korte periode retourneren.</span><span class="sxs-lookup"><span data-stu-id="af693-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="af693-112">Inhoud moet opnieuw worden gecrawld om de zoekindex bij te werken.</span><span class="sxs-lookup"><span data-stu-id="af693-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="af693-113">Er is geen handmatige stap vereist - dit wordt automatisch gedaan.</span><span class="sxs-lookup"><span data-stu-id="af693-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="af693-114">Alles wat afhankelijk is van 'statische' koppelingen (zoals Bestandssynchronisatie en OneNote-bestanden) moet handmatig worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="af693-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="af693-115">Als de bronsite een nieuwssite van de organisatie was, werkt u de URL bij.</span><span class="sxs-lookup"><span data-stu-id="af693-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="af693-116">Ontvang een lijst met alle nieuwssites van de organisatie.</span><span class="sxs-lookup"><span data-stu-id="af693-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="af693-117">Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="af693-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
