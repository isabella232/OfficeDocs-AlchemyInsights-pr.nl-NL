---
title: Moderne site als de hoofdsite
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620754"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="6268e-102">Moderne site als hoofdsite</span><span class="sxs-lookup"><span data-stu-id="6268e-102">Modern site as root site</span></span>

<span data-ttu-id="6268e-103">We begonnen te implementatie een nieuwe functie waarmee u uw hoofdsite klassieke site met een moderne site wisselen.</span><span class="sxs-lookup"><span data-stu-id="6268e-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="6268e-104">Gebruik [Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) te verwisselen van de locatie van een site met een andere site bij het archiveren van de oorspronkelijke site.</span><span class="sxs-lookup"><span data-stu-id="6268e-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="6268e-105">Beschikbaar voor zowel Team Site (niet verbonden aan een groep) en communicatie-Site.</span><span class="sxs-lookup"><span data-stu-id="6268e-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="6268e-106">Verwijder niet de klassieke hoofdsite om een moderne communicatie-Site te maken.</span><span class="sxs-lookup"><span data-stu-id="6268e-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="6268e-107">Dit wordt niet ondersteund door Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6268e-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="6268e-108">Verwijderen van de hoofdsite brengt alle SharePoint-sites in uw organisatie niet toegankelijk voor alle gebruikers, totdat u de site terugzetten of maak een nieuwe site op dezelfde URL.</span><span class="sxs-lookup"><span data-stu-id="6268e-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="6268e-109">We zullen deze functie via het berichtencentrum communiceren.</span><span class="sxs-lookup"><span data-stu-id="6268e-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="6268e-110">U kunt de functie moet worden ingeschakeld in uw huurder binnenkort verwachten.</span><span class="sxs-lookup"><span data-stu-id="6268e-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="6268e-111">Bekende problemen bij het wisselen van sites</span><span class="sxs-lookup"><span data-stu-id="6268e-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="6268e-112">De doelsite retourneert gedurende korte tijd een "niet gevonden" (HTTP 404)-fout.</span><span class="sxs-lookup"><span data-stu-id="6268e-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="6268e-113">Inhoud moet opnieuw worden verkend om het bijwerken van de zoekindex.</span><span class="sxs-lookup"><span data-stu-id="6268e-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="6268e-114">Er is geen handmatige stap hier nodig is, wordt dit automatisch gedaan.</span><span class="sxs-lookup"><span data-stu-id="6268e-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="6268e-115">Alles wat afhankelijk is van een 'static' koppelingen (zoals bestand synchroniseren als OneNote-bestanden) moeten handmatig worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="6268e-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="6268e-116">Project Server-sites mogelijk moet worden gevalideerd om ervoor te zorgen dat ze nog steeds gekoppeld correct worden.</span><span class="sxs-lookup"><span data-stu-id="6268e-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
