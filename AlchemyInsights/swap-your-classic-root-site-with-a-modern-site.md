---
title: Uw klassieke basis site met een moderne site uitwisselen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691174"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="b5bf9-102">Uw klassieke basis site met een moderne site uitwisselen</span><span class="sxs-lookup"><span data-stu-id="b5bf9-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="b5bf9-103">Als uw omgeving vóór april 2019 is geconfigureerd, kunt u uw hoofdsite wijzigen in een moderne site met behulp van Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b5bf9-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="b5bf9-104">Als u een andere site hebt die u wilt gebruiken als basis site, kunt u [de hoofdsite vervangen (verwisselen)](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="b5bf9-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="b5bf9-105">Met [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kunt u de locatie van een site met een andere site wisselen tijdens het archiveren van de oorspronkelijke site.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b5bf9-106">Beschikbaar voor beide team sites (niet verbonden met een groep) en communicatie site.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="b5bf9-107">Er worden binnenkort extra functies geïntroduceerd waarmee u de inhoud op de site kunt blijven gebruiken, maar de bestaande site moet converteren naar een communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="b5bf9-108">Deze mogelijkheden worden geleidelijk uitgerold.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="b5bf9-109">Ga verder naar het berichtencentrum controleren op updates.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b5bf9-110">Bekende problemen met het verwisselen van sites</span><span class="sxs-lookup"><span data-stu-id="b5bf9-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="b5bf9-111">De doelsite kan een "niet gevonden" (HTTP 404)-fout retourneren gedurende een korte periode.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b5bf9-112">Inhoud moet worden verkend om de zoekindex bij te werken.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b5bf9-113">U hoeft dit niet handmatig te doen, dit wordt automatisch uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="b5bf9-114">Items die afhankelijk zijn van statische koppelingen (zoals bestandssynchronisatie en OneNote-bestanden), moeten handmatig worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b5bf9-115">Als de bronsite een nieuwssite van een organisatie was, moet u de URL bijwerken.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="b5bf9-116">U ontvangt een lijst met alle nieuwssites van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="b5bf9-117">Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat deze correct worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="b5bf9-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
