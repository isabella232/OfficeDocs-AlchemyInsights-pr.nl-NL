---
title: De hoofdsite is klassiek met een moderne site wisselen
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
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270739"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="e77bd-102">De hoofdsite is klassiek met een moderne site wisselen</span><span class="sxs-lookup"><span data-stu-id="e77bd-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="e77bd-103">Als uw omgeving vóór April 2019 is ingesteld, kunt u uw hoofdsite met een moderne site met Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e77bd-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="e77bd-104">Als u een andere site die u wilt gebruiken als uw hoofdsite hebt, kunt u (swap) de hoofdmap van de site kunt vervangen door deze.</span><span class="sxs-lookup"><span data-stu-id="e77bd-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="e77bd-105">Gebruik [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) te verwisselen van de locatie van een site met een andere site bij het archiveren van de oorspronkelijke site.</span><span class="sxs-lookup"><span data-stu-id="e77bd-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e77bd-106">Beschikbaar voor zowel Team Site (niet verbonden aan een groep) en communicatie-Site.</span><span class="sxs-lookup"><span data-stu-id="e77bd-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="e77bd-107">Extra functies geïntroduceerd spoedig waarmee u te houden met de inhoud op de site, maar de bestaande site converteren naar een communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="e77bd-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="e77bd-108">Deze mogelijkheden zullen geleidelijk worden uitgerold.</span><span class="sxs-lookup"><span data-stu-id="e77bd-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="e77bd-109">Houd het berichtencentrum van Office 365 voor updates.</span><span class="sxs-lookup"><span data-stu-id="e77bd-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e77bd-110">Bekende problemen bij het wisselen van sites</span><span class="sxs-lookup"><span data-stu-id="e77bd-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="e77bd-111">De doelsite retourneert gedurende korte tijd een "niet gevonden" (HTTP 404)-fout.</span><span class="sxs-lookup"><span data-stu-id="e77bd-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e77bd-112">Inhoud moet opnieuw worden verkend om het bijwerken van de zoekindex.</span><span class="sxs-lookup"><span data-stu-id="e77bd-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e77bd-113">Er is geen handmatige stap vereist - dit wordt automatisch gedaan.</span><span class="sxs-lookup"><span data-stu-id="e77bd-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="e77bd-114">Alles wat afhankelijk is van een 'static' koppelingen (zoals bestand synchroniseren als OneNote-bestanden) moeten handmatig worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="e77bd-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e77bd-115">Als de bronsite een organisatie-nieuwssite is, werken de URL.</span><span class="sxs-lookup"><span data-stu-id="e77bd-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="e77bd-116">Een lijst van alle organisatie-nieuwssites opvragen.</span><span class="sxs-lookup"><span data-stu-id="e77bd-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="e77bd-117">Project Server-sites mogelijk moet worden gevalideerd om ervoor te zorgen dat ze nog steeds gekoppeld correct worden.</span><span class="sxs-lookup"><span data-stu-id="e77bd-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





