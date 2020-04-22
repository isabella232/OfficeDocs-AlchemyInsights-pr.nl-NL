---
title: Moderne site als hoofdsite
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713786"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="37c85-102">Moderne site als hoofdsite</span><span class="sxs-lookup"><span data-stu-id="37c85-102">Modern site as root site</span></span>

<span data-ttu-id="37c85-103">We zijn begonnen met de uitrol van een nieuwe functie waarmee u uw klassieke site root site te [ruilen met een moderne site.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="37c85-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="37c85-104">Gebruik [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site te ruilen met een andere site terwijl u de oorspronkelijke site archiveert.</span><span class="sxs-lookup"><span data-stu-id="37c85-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="37c85-105">Beschikbaar voor zowel teamsite (niet verbonden met een groep) als voor communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="37c85-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="37c85-106">Verwijder uw klassieke hoofdsite niet om een moderne communicatiesite te maken.</span><span class="sxs-lookup"><span data-stu-id="37c85-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="37c85-107">Dit wordt niet ondersteund door Microsoft.</span><span class="sxs-lookup"><span data-stu-id="37c85-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="37c85-108">Als u de hoofdsite verwijderde, worden alle SharePoint-sites in uw organisatie ontoegankelijk voor alle gebruikers, totdat u de site herstelt of een nieuwe site met dezelfde URL maakt.</span><span class="sxs-lookup"><span data-stu-id="37c85-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="37c85-109">We communiceren deze functie via het berichtencentrum.</span><span class="sxs-lookup"><span data-stu-id="37c85-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="37c85-110">U mag verwachten dat de functie binnenkort in uw tenant wordt ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="37c85-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="37c85-111">Bekende problemen met het verwisselen van sites</span><span class="sxs-lookup"><span data-stu-id="37c85-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="37c85-112">De doelsite kan een fout 'niet gevonden' (HTTP 404) voor een korte periode retourneren.</span><span class="sxs-lookup"><span data-stu-id="37c85-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="37c85-113">Inhoud moet opnieuw worden gecrawld om de zoekindex bij te werken.</span><span class="sxs-lookup"><span data-stu-id="37c85-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="37c85-114">Er is hier geen handmatige stap vereist, dit gebeurt automatisch.</span><span class="sxs-lookup"><span data-stu-id="37c85-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="37c85-115">Alles wat afhankelijk is van 'statische' koppelingen (zoals Bestandssynchronisatie en OneNote-bestanden) moet handmatig worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="37c85-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="37c85-116">Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="37c85-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
