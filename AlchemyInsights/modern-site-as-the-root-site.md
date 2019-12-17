---
title: Moderne site als de hoofdsite
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054697"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="588d1-102">Moderne site als hoofdsite</span><span class="sxs-lookup"><span data-stu-id="588d1-102">Modern site as root site</span></span>

<span data-ttu-id="588d1-103">We zijn begonnen met de uitrol van een nieuwe functie waarmee u [uw klassieke site hoofdsite met een moderne site verwisselen](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="588d1-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="588d1-104">Gebruik [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site met een andere site te wisselen tijdens het archiveren van de oorspronkelijke site.</span><span class="sxs-lookup"><span data-stu-id="588d1-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="588d1-105">Beschikbaar voor beide team sites (niet verbonden met een groep) en een communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="588d1-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="588d1-106">Verwijder uw klassieke hoofdsite niet om een moderne communicatiesite te maken.</span><span class="sxs-lookup"><span data-stu-id="588d1-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="588d1-107">Dit wordt niet ondersteund door Microsoft.</span><span class="sxs-lookup"><span data-stu-id="588d1-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="588d1-108">Als u de hoofdsite verwijdert, worden alle SharePoint-sites in uw organisatie ontoegankelijk voor alle gebruikers, totdat u de site herstelt of een nieuwe site maakt op dezelfde URL.</span><span class="sxs-lookup"><span data-stu-id="588d1-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="588d1-109">We communiceren deze functie via het berichtencentrum.</span><span class="sxs-lookup"><span data-stu-id="588d1-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="588d1-110">U moet verwachten dat de functie moet worden ingeschakeld in uw Tenant binnenkort.</span><span class="sxs-lookup"><span data-stu-id="588d1-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="588d1-111">Bekende problemen met het uitwisselen van sites</span><span class="sxs-lookup"><span data-stu-id="588d1-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="588d1-112">De doelsite kan een fout ' niet gevonden ' (HTTP 404) retourneren voor een korte periode.</span><span class="sxs-lookup"><span data-stu-id="588d1-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="588d1-113">De inhoud moet opnieuw worden verkend om de zoekindex bij te werken.</span><span class="sxs-lookup"><span data-stu-id="588d1-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="588d1-114">Er is hier geen handmatige stap vereist, dit wordt automatisch gedaan.</span><span class="sxs-lookup"><span data-stu-id="588d1-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="588d1-115">Alles wat afhankelijk is van ' statische ' koppelingen (zoals bestandssynchronisatie en OneNote-bestanden) moet handmatig worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="588d1-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="588d1-116">Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="588d1-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
