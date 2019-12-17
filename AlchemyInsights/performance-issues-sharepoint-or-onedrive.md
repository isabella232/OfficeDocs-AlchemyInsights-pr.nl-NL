---
title: Prestatieproblemen-SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068392"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="9972f-102">SharePoint of OneDrive traag, ontoegankelijk of niet beschikbaar voor meerdere gebruikers</span><span class="sxs-lookup"><span data-stu-id="9972f-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="9972f-103">SharePoint of OneDrive is mogelijk traag, ontoegankelijk of niet beschikbaar of kan om verschillende redenen service niet beschikbaar of 503 fouten weergeven:</span><span class="sxs-lookup"><span data-stu-id="9972f-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="9972f-104">Als uw SharePoint-of OneDrive-site traag of vertraagd is voor meerdere gebruikers, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers onregelmatige vertragingen of Navigatiefouten ondervinden bij het openen van SharePoint-sites of OneDrive-inhoud.</span><span class="sxs-lookup"><span data-stu-id="9972f-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="9972f-105">Controleer de [service status dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of uw organisatie wordt beïnvloed.</span><span class="sxs-lookup"><span data-stu-id="9972f-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="9972f-106">Gebruikers kunnen een *503 Server is bezet* fout wanneer u probeert te navigeren naar SharePoint of OneDrive-sites ontvangen.</span><span class="sxs-lookup"><span data-stu-id="9972f-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="9972f-107">Deze fout kan worden veroorzaakt door beperking binnen de SharePoint-service.</span><span class="sxs-lookup"><span data-stu-id="9972f-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="9972f-108">SharePoint Online gebruikt beperking om optimale prestaties en betrouwbaarheid van de SharePoint Online-service te behouden.</span><span class="sxs-lookup"><span data-stu-id="9972f-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="9972f-109">Beperking beperkt het aantal gebruikersacties of gelijktijdige aanroepen (per script of code) om overmatig gebruik van resources te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="9972f-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="9972f-110">Voor meer informatie over bandbreedtebeperking Zie, [Vermijd het krijgen van beperkingen of geblokkeerd in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="9972f-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="9972f-111">Als u trage prestaties met een **klassieke** of **moderne** SharePoint-site of pagina ondervindt, maakt u gebruik van de [pagina diagnostisch hulpprogramma](https://aka.ms/perftool) voor het analyseren van de pagina's.</span><span class="sxs-lookup"><span data-stu-id="9972f-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="9972f-112">Als u nog steeds algemene trage prestaties ondervindt, raadpleegt u de resources aan de onderkant van dit artikel: [Inleiding tot prestatieafstemming Voorsharepoint online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="9972f-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  