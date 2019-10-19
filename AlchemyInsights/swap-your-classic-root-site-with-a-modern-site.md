---
title: Ruil je klassieke root site met een moderne site
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749255"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="06cd1-102">Ruil je klassieke root site met een moderne site</span><span class="sxs-lookup"><span data-stu-id="06cd1-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="06cd1-103">Als uw omgeving is ingesteld vóór 2019 april, u uw hoofdsite wijzigen naar een moderne site met behulp van Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="06cd1-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="06cd1-104">Als u een andere site die u wilt gebruiken als uw hoofdsite hebt, u vervangen [(wisselen) de hoofdsite](https://docs.microsoft.com/sharepoint/modern-root-site) met deze.</span><span class="sxs-lookup"><span data-stu-id="06cd1-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="06cd1-105">Gebruik [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) om de locatie van een site met een andere site te wisselen tijdens het archiveren van de oorspronkelijke site.</span><span class="sxs-lookup"><span data-stu-id="06cd1-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="06cd1-106">Beschikbaar voor beide team sites (niet verbonden met een groep) en een communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="06cd1-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="06cd1-107">Er zullen binnenkort extra mogelijkheden worden geïntroduceerd waarmee u de inhoud op de site blijven gebruiken, maar de bestaande site naar een communicatiesite moet converteren.</span><span class="sxs-lookup"><span data-stu-id="06cd1-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="06cd1-108">Deze mogelijkheden zullen geleidelijk worden uitgerold.</span><span class="sxs-lookup"><span data-stu-id="06cd1-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="06cd1-109">Ga door met het controleren van het Office 365-berichtencentrum voor updates.</span><span class="sxs-lookup"><span data-stu-id="06cd1-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="06cd1-110">Bekende problemen met het uitwisselen van sites</span><span class="sxs-lookup"><span data-stu-id="06cd1-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="06cd1-111">De doelsite kan een fout ' niet gevonden ' (HTTP 404) retourneren voor een korte periode.</span><span class="sxs-lookup"><span data-stu-id="06cd1-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="06cd1-112">De inhoud moet opnieuw worden verkend om de zoekindex bij te werken.</span><span class="sxs-lookup"><span data-stu-id="06cd1-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="06cd1-113">Er is geen handmatige stap vereist-dit wordt automatisch gedaan.</span><span class="sxs-lookup"><span data-stu-id="06cd1-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="06cd1-114">Alles wat afhankelijk is van ' statische ' koppelingen (zoals bestandssynchronisatie en OneNote-bestanden) moet handmatig worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="06cd1-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="06cd1-115">Als de bronsite een nieuwssite voor de organisatie was, werkt u de URL bij.</span><span class="sxs-lookup"><span data-stu-id="06cd1-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="06cd1-116">Krijg een lijst van alle organisatorische nieuwssites.</span><span class="sxs-lookup"><span data-stu-id="06cd1-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="06cd1-117">Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat ze nog steeds correct zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="06cd1-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





