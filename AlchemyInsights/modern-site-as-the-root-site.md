---
title: Moderne site als basis site
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666865"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="51efb-102">Moderne site als basis site</span><span class="sxs-lookup"><span data-stu-id="51efb-102">Modern site as root site</span></span>

<span data-ttu-id="51efb-103">We zijn begonnen met het implementeren van een nieuwe functie waarmee u [uw klassieke site-site met een moderne site kunt uitwisselen](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="51efb-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="51efb-104">Met [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kunt u de locatie van een site met een andere site wisselen tijdens het archiveren van de oorspronkelijke site.</span><span class="sxs-lookup"><span data-stu-id="51efb-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="51efb-105">Beschikbaar voor beide team sites (niet verbonden met een groep) en communicatie site.</span><span class="sxs-lookup"><span data-stu-id="51efb-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="51efb-106">Verwijder uw klassieke basis site niet voor het maken van een moderne communicatiesite.</span><span class="sxs-lookup"><span data-stu-id="51efb-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="51efb-107">Dit wordt niet ondersteund door Microsoft.</span><span class="sxs-lookup"><span data-stu-id="51efb-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="51efb-108">Als u de hoofdsite verwijdert, worden alle SharePoint-sites in uw organisatie niet toegankelijk voor alle gebruikers totdat u de site terugzet of een nieuwe site maakt met dezelfde URL.</span><span class="sxs-lookup"><span data-stu-id="51efb-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="51efb-109">We communiceren deze functie via het berichtencentrum.</span><span class="sxs-lookup"><span data-stu-id="51efb-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="51efb-110">Normaalgesproken moet de functie in uw Tenant worden ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="51efb-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="51efb-111">Bekende problemen met het verwisselen van sites</span><span class="sxs-lookup"><span data-stu-id="51efb-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="51efb-112">De doelsite kan een "niet gevonden" (HTTP 404)-fout retourneren gedurende een korte periode.</span><span class="sxs-lookup"><span data-stu-id="51efb-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="51efb-113">Inhoud moet worden verkend om de zoekindex bij te werken.</span><span class="sxs-lookup"><span data-stu-id="51efb-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="51efb-114">U hoeft hier geen handmatige stap te vinden, dit is automatisch gebeurd.</span><span class="sxs-lookup"><span data-stu-id="51efb-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="51efb-115">Items die afhankelijk zijn van statische koppelingen (zoals bestandssynchronisatie en OneNote-bestanden), moeten handmatig worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="51efb-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="51efb-116">Project Server-sites moeten mogelijk worden gevalideerd om ervoor te zorgen dat deze correct worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="51efb-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
