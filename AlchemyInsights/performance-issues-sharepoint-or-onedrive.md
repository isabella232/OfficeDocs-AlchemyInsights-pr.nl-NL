---
title: Prestatieproblemen-SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771896"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="c70fb-102">SharePoint of OneDrive traag, niet toegankelijk of niet beschikbaar voor meerdere gebruikers</span><span class="sxs-lookup"><span data-stu-id="c70fb-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="c70fb-103">Het is mogelijk dat SharePoint of OneDrive traag, niet toegankelijk of niet beschikbaar is, of dat de service niet beschikbaar is en de fouten in 503, om een aantal redenen:</span><span class="sxs-lookup"><span data-stu-id="c70fb-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="c70fb-104">Als uw SharePoint-of OneDrive-site traag of vertraagd is voor meerdere gebruikers, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers een tijdelijke vertraging of navigatie fouten bij het openen van SharePoint-sites of OneDrive-inhoud kunnen vinden.</span><span class="sxs-lookup"><span data-stu-id="c70fb-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="c70fb-105">Controleer het [Dashboard service status](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of uw organisatie van invloed is.</span><span class="sxs-lookup"><span data-stu-id="c70fb-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="c70fb-106">Gebruikers kunnen een fout bij een *503-Server* ontvangen bij het navigeren naar SharePoint-of OneDrive-sites.</span><span class="sxs-lookup"><span data-stu-id="c70fb-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="c70fb-107">Deze fout kan worden veroorzaakt door de beperking binnen de SharePoint-service.</span><span class="sxs-lookup"><span data-stu-id="c70fb-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c70fb-108">SharePoint Online gebruikt beperking om optimale prestaties en betrouwbaarheid van de SharePoint Online-service te behouden.</span><span class="sxs-lookup"><span data-stu-id="c70fb-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c70fb-109">Dit beperkt het aantal gebruikersacties of gelijktijdige oproepen (via script of code) om overmatig gebruik van bronnen te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="c70fb-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="c70fb-110">Voor meer informatie over het beperken van beperking raadpleegt u [voorkomen dat u vertraagt of blokkeert in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c70fb-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="c70fb-111">Als u traag presteert met een **klassieke** of **moderne** SharePoint-site of-pagina, gebruikt u het [hulpprogramma](https://aka.ms/perftool) voor het maken van pagina's om de pagina's te analyseren.</span><span class="sxs-lookup"><span data-stu-id="c70fb-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="c70fb-112">Als u nog steeds veel vertragingen onderneemt, raadpleegt u de bronnen onder aan dit artikel: [Inleiding tot het optimaliseren van de prestaties voor SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="c70fb-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  